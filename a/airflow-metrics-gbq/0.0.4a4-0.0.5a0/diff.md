# Comparing `tmp/airflow_metrics_gbq-0.0.4a4.tar.gz` & `tmp/airflow_metrics_gbq-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.4a4.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.5a0.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.4a4.tar` & `airflow_metrics_gbq-0.0.5a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/LICENSE
--rw-r--r--   0        0        0     2549 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/README.md
--rw-r--r--   0        0        0        0 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0       94 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/exceptions.py
--rw-r--r--   0        0        0    10649 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1320 2023-04-26 22:08:04.323238 airflow_metrics_gbq-0.0.4a4/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a4/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/LICENSE
+-rw-r--r--   0        0        0     2487 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/exceptions.py
+-rw-r--r--   0        0        0    10737 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1320 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/pyproject.toml
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.5a0/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.4a4/LICENSE` & `airflow_metrics_gbq-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a4/README.md` & `airflow_metrics_gbq-0.0.5a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -58,12 +58,11 @@
 ```bash
 python monitor.py &
 ```
 9. The logs can be viewed in the GCP console under the `airflow_monitoring` app_name in Google Cloud Logging.
 
 
 **Future releases**
-- [ ] Add a buffer (pyzmq or mp queue)
-- [ ] Run sending metrics to GBQ in another process
+- [ ] Increase test coverage
 - [ ] Add proper typing and mypy support and checks
 - [ ] Provide more configurable options
 - [ ] Provide better documentation
```

### Comparing `airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return PointWithType(point, mtype)
 
 
 # pylint: disable=too-many-instance-attributes
 class AirflowMonitor:
     """Main class to ship metrics to GBQ"""
 
-    CAPACITY: t.Final = 500
+    CAPACITY: t.Final = 1000
     BATCH_TIME: t.Final = 5
 
     def __init__(
         self,
         host: str,
         port: int,
         gcp_credentials: str,
@@ -191,28 +191,30 @@
             self.logger.debug(f"Flushing out {len(metrics)} metrics to BigQuery")
             self.send_metrics(metrics)
             self._last_flush = time.time()
 
     @retry(
         retry=(retry_if_exception_type(queue.Full) | retry_if_exception_type(NoMetricFoundException)),
         wait=wait_fixed(2) + wait_random(0, 2),
-        stop=stop_after_attempt(5),
+        stop=stop_after_attempt(10),
+        reraise=True,
     )
     def _fetch(self):
         """Fetch metrics from Airflow"""
         while True:
             measure: str = self._sock.recv(1024).decode("utf-8")
 
             if measure == "":
                 raise NoMetricFoundException("No metrics detected!")
 
             try:
                 # non blocking
                 self._buffer.put_nowait(PointWithType.from_record(measure))
             except queue.Full as e:
+                self.logger.debug(self._fetch.retry.statistics)
                 self.logger.error("Queue is full")
                 raise e
 
     def _get_dfs(self, metrics: t.List[PointWithType]) -> (pd.DataFrame, pd.DataFrame, pd.DataFrame):
         """Get dataframes to upload"""
         measure_dict = self._part_types(metrics)
```

### Comparing `airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a4/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.4a4/pyproject.toml` & `airflow_metrics_gbq-0.0.5a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.4a4"
+version = "0.0.5a0"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
```

### Comparing `airflow_metrics_gbq-0.0.4a4/PKG-INFO` & `airflow_metrics_gbq-0.0.5a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.4a4
+Version: 0.0.5a0
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -87,13 +87,12 @@
 ```bash
 python monitor.py &
 ```
 9. The logs can be viewed in the GCP console under the `airflow_monitoring` app_name in Google Cloud Logging.
 
 
 **Future releases**
-- [ ] Add a buffer (pyzmq or mp queue)
-- [ ] Run sending metrics to GBQ in another process
+- [ ] Increase test coverage
 - [ ] Add proper typing and mypy support and checks
 - [ ] Provide more configurable options
 - [ ] Provide better documentation
```

