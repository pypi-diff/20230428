# Comparing `tmp/prefect-spark-on-k8s-operator-0.1.1.tar.gz` & `tmp/prefect-spark-on-k8s-operator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-spark-on-k8s-operator/prefect-spark-on-k8s-operator/dist/.tmp-ilitp9ls/prefect-spark-on-k8s-operator-", last modified: Sun Apr  2 05:57:11 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-spark-on-k8s-operator/prefect-spark-on-k8s-operator/dist/.tmp-frcebcth/prefect-spark-on-k8s-operator-", last modified: Fri Apr 28 15:06:28 2023, max compression
```

## Comparing `prefect-spark-on-k8s-operator-0.1.1.tar` & `prefect-spark-on-k8s-operator-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/flows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 05:57:11.000000 prefect-spark-on-k8s-operator-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-02 05:55:38.000000 prefect-spark-on-k8s-operator-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/flows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:06:28.000000 prefect-spark-on-k8s-operator-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-28 15:05:06.000000 prefect-spark-on-k8s-operator-0.1.2/versioneer.py
```

### Comparing `prefect-spark-on-k8s-operator-0.1.1/LICENSE` & `prefect-spark-on-k8s-operator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/PKG-INFO` & `prefect-spark-on-k8s-operator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-spark-on-k8s-operator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prefect integrations for orchestrating and monitoring apache spark jobs on kubernetes using spark-on-k8s-operator.
 Home-page: https://github.com/tardunge/prefect-spark-on-k8s-operator
 Author: Manoj Babu Katragadda
 Author-email: manojbabuiit@gmail.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-spark-on-k8s-operator-0.1.1/README.md` & `prefect-spark-on-k8s-operator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/app.py` & `prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             " By default this is done only upon failures."
             " Logs for successful runs will be collected by setting this option to True"
         ),
     )
 
     _block_type_name = "Spark On K8s Operator"
     _block_type_slug = "spark-on-k8s-operator"
-    _logo_url = "https://images.ctfassets.net/zscdif0zqppk/35vNcprr3MmIlkrKxxCiah/1d720b4b50dfa8876198cf21730cf123/Kubernetes_logo_without_workmark.svg.png?h=250"  # noqa: E501
+    _logo_url = "https://docs.prefect.io/img/collections/spark-on-kubernetes.png?h=250"  # noqa: E501
     _documentation_url = "https://tardunge.github.io/prefect-spark-on-k8s-operator/app/#prefect_spark_on_k8s_operator.app.SparkApplication"  # noqa
     name: str = ""
 
     @sync_compatible
     async def trigger(self) -> "SparkApplicationRun":
         """Apply the spark application and return a `SparkApplicationRun` object.
 
@@ -263,18 +263,14 @@
             The application is in UNKNOWN state. This happens if the
             Kubernetes node hosting the driver pod crashes. If the
             state doesn't change for `timeout_seconds`, then the application
             is terminated.
         For more information on the spark-on-k8s-operator state-machine please
         refer [here](https://github.com/GoogleCloudPlatform/spark-on-k8s-operator/
         blob/master/pkg/controller/sparkapplication/controller.go#L485)
-
-        Raises:
-            RuntimeError: If the application fails or in unknown state
-                for timeout_seconds.
         """
         self.application_logs = {}
 
         # wait for the status to change from ""(empty string) to something.
         while True:
             status = await self._fetch_status()
             if constants.STATUS not in status:
@@ -370,31 +366,31 @@
                     container=constants.SPARK_DRIVER_CONAINER_NAME,
                     **self._spark_application.api_kwargs,
                 )
 
         if self._spark_application.delete_after_completion or self._timed_out:
             self._cleanup_status = await self._cleanup()
 
-        if self._terminal_state != constants.COMPLETED:
-            raise RuntimeError(
-                "The SparkApplication run is not in a completed state,"
-                f" last observed state was {self._terminal_state} - "
-                f"possible errors: {self._error_msg}"
-            )
-
     @sync_compatible
     async def fetch_result(self) -> Dict[str, Any]:
         """Returns the logs from driver pod when:
         `collect_driver_logs` is set to true
         or the application is not in COMPLETED state.
 
         Returns:
             A dict containing the driver pod name and its main container logs.
+
+        Raises:
+            RuntimeError: If the application fails or in unknown state
+              for timeout_seconds.
         """
-        self.logger.info(f"logs: {self.application_logs}")
+        for pod in self.application_logs:
+            self.logger.info(f"logs for pod {pod}")
+            self.logger.info(f"{self.application_logs[pod]}")
+        # self.logger.info(f"logs: {self.application_logs}")
         if self._terminal_state != constants.COMPLETED:
-            raise ValueError(
+            raise RuntimeError(
                 "The SparkApplication run is not in a completed state,"
                 f" last observed state was {self._terminal_state} - "
                 f"possible errors: {self._error_msg}"
             )
         return self.application_logs
```

### Comparing `prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/constants.py` & `prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/constants.py`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator/flows.py` & `prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/PKG-INFO` & `prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-spark-on-k8s-operator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prefect integrations for orchestrating and monitoring apache spark jobs on kubernetes using spark-on-k8s-operator.
 Home-page: https://github.com/tardunge/prefect-spark-on-k8s-operator
 Author: Manoj Babu Katragadda
 Author-email: manojbabuiit@gmail.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-spark-on-k8s-operator-0.1.1/prefect_spark_on_k8s_operator.egg-info/SOURCES.txt` & `prefect-spark-on-k8s-operator-0.1.2/prefect_spark_on_k8s_operator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/setup.cfg` & `prefect-spark-on-k8s-operator-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/setup.py` & `prefect-spark-on-k8s-operator-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/tests/test_app.py` & `prefect-spark-on-k8s-operator-0.1.2/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,22 +105,22 @@
 ):
     spark_app = SparkApplication.from_yaml_file(
         credentials=kubernetes_credentials,
         manifest_path="tests/sample_spark_jobs/sample_job.yaml",
     )
 
     app_run = await spark_app.trigger()
-    with pytest.raises(RuntimeError):
-        await app_run.wait_for_completion()
+
+    await app_run.wait_for_completion()
 
     assert app_run.application_logs.get("spark-pi-khha-driver") == "test-logs"
     assert not app_run._completed
     assert app_run._terminal_state == constants.FAILED
 
-    with pytest.raises(ValueError):
+    with pytest.raises(RuntimeError):
         await app_run.fetch_result()
 
 
 async def test_wait_for_completion_completed_with_logs(
     kubernetes_credentials,
     _mock_kubernets_api_client,
     mock_create_namespaced_custom_object,
@@ -152,22 +152,21 @@
         credentials=kubernetes_credentials,
         manifest_path="tests/sample_spark_jobs/sample_job.yaml",
         interval_seconds=0,
         timeout_seconds=0,
     )
     app_run = await spark_app.trigger()
 
-    with pytest.raises(RuntimeError):
-        await app_run.wait_for_completion()
+    await app_run.wait_for_completion()
 
     assert not app_run._completed
     assert app_run._terminal_state == constants.UNKNOWN
     assert len(app_run.application_logs) == 0
 
-    with pytest.raises(ValueError):
+    with pytest.raises(RuntimeError):
         await app_run.fetch_result()
 
 
 async def test_wait_for_completion_recovered(
     kubernetes_credentials,
     _mock_kubernets_api_client,
     mock_create_namespaced_custom_object,
```

### Comparing `prefect-spark-on-k8s-operator-0.1.1/tests/test_flows.py` & `prefect-spark-on-k8s-operator-0.1.2/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect-spark-on-k8s-operator-0.1.1/versioneer.py` & `prefect-spark-on-k8s-operator-0.1.2/versioneer.py`

 * *Files identical despite different names*

