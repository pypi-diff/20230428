# Comparing `tmp/airflow_metrics_gbq-0.0.5a0.tar.gz` & `tmp/airflow_metrics_gbq-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.5a0.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.5a1.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.5a0.tar` & `airflow_metrics_gbq-0.0.5a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/LICENSE
--rw-r--r--   0        0        0     2487 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0       94 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/exceptions.py
--rw-r--r--   0        0        0    10737 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1320 2023-04-27 22:45:59.145521 airflow_metrics_gbq-0.0.5a0/pyproject.toml
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/LICENSE
+-rw-r--r--   0        0        0     2487 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/exceptions.py
+-rw-r--r--   0        0        0    10738 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1320 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/pyproject.toml
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.5a1/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.5a0/LICENSE` & `airflow_metrics_gbq-0.0.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a0/README.md` & `airflow_metrics_gbq-0.0.5a1/README.md`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 
 # pylint: disable=too-many-instance-attributes
 class AirflowMonitor:
     """Main class to ship metrics to GBQ"""
 
     CAPACITY: t.Final = 1000
-    BATCH_TIME: t.Final = 5
+    BATCH_TIME: t.Final = 15
 
     def __init__(
         self,
         host: str,
         port: int,
         gcp_credentials: str,
         dataset_id: str,
```

### Comparing `airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a0/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a0/pyproject.toml` & `airflow_metrics_gbq-0.0.5a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.5a0"
+version = "0.0.5a1"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
```

### Comparing `airflow_metrics_gbq-0.0.5a0/PKG-INFO` & `airflow_metrics_gbq-0.0.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.5a0
+Version: 0.0.5a1
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

