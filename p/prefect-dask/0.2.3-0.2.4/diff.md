# Comparing `tmp/prefect-dask-0.2.3.tar.gz` & `tmp/prefect-dask-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-dask/prefect-dask/dist/.tmp-i6rj8k1z/prefect-dask-0.2.3.tar", last modified: Tue Feb 21 18:53:36 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-dask/prefect-dask/dist/.tmp-od9h887k/prefect-dask-0.2.4.tar", last modified: Fri Apr 28 13:31:05 2023, max compression
```

## Comparing `prefect-dask-0.2.3.tar` & `prefect-dask-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/prefect_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/prefect_dask/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/prefect_dask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/prefect_dask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:53:36.000000 prefect-dask-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-02-21 18:51:41.000000 prefect-dask-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/prefect_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/prefect_dask/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/prefect_dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/prefect_dask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:31:05.000000 prefect-dask-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-28 13:29:19.000000 prefect-dask-0.2.4/versioneer.py
```

### Comparing `prefect-dask-0.2.3/LICENSE` & `prefect-dask-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-dask-0.2.3/PKG-INFO` & `prefect-dask-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations with the Dask execution framework.
 Home-page: https://github.com/PrefectHQ/prefect-dask
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-dask-0.2.3/README.md` & `prefect-dask-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect-dask-0.2.3/prefect_dask/task_runners.py` & `prefect-dask-0.2.4/prefect_dask/task_runners.py`

 * *Files 7% similar despite different names*

```diff
@@ -206,14 +206,41 @@
     def concurrency_type(self) -> TaskConcurrencyType:
         return (
             TaskConcurrencyType.PARALLEL
             if self.cluster_kwargs.get("processes")
             else TaskConcurrencyType.CONCURRENT
         )
 
+    def duplicate(self):
+        """
+        Create a new instance of the task runner with the same settings.
+        """
+        return type(self)(
+            address=self.address,
+            cluster_class=self.cluster_class,
+            cluster_kwargs=self.cluster_kwargs,
+            adapt_kwargs=self.adapt_kwargs,
+            client_kwargs=self.client_kwargs,
+        )
+
+    def __eq__(self, other: object) -> bool:
+        """
+        Check if an instance has the same settings as this task runner.
+        """
+        if type(self) == type(other):
+            return (
+                self.address == other.address
+                and self.cluster_class == other.cluster_class
+                and self.cluster_kwargs == other.cluster_kwargs
+                and self.adapt_kwargs == other.adapt_kwargs
+                and self.client_kwargs == other.client_kwargs
+            )
+        else:
+            return NotImplemented
+
     async def submit(
         self,
         key: UUID,
         call: Callable[..., Awaitable[State[R]]],
     ) -> None:
         if not self._started:
             raise RuntimeError(
```

### Comparing `prefect-dask-0.2.3/prefect_dask/utils.py` & `prefect-dask-0.2.4/prefect_dask/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         # because this allows us to set asynchronous based on user's task
         input_client_kwargs = {}
         address = get_client().scheduler.address
         asynchronous = task_run_context.task.isasync
     elif flow_run_context:
         task_runner = flow_run_context.task_runner
         input_client_kwargs = task_runner.client_kwargs
-        address = task_runner._connect_to
+        address = task_runner._client.scheduler_info()["address"]
         asynchronous = flow_run_context.flow.isasync
     else:
         # this else clause allows users to debug or test
         # without much change to code
         input_client_kwargs = {}
         address = None
         asynchronous = async_client
```

### Comparing `prefect-dask-0.2.3/prefect_dask.egg-info/PKG-INFO` & `prefect-dask-0.2.4/prefect_dask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.3
+Version: 0.2.4
 Summary: Prefect integrations with the Dask execution framework.
 Home-page: https://github.com/PrefectHQ/prefect-dask
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-dask-0.2.3/setup.cfg` & `prefect-dask-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-dask-0.2.3/setup.py` & `prefect-dask-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-dask-0.2.3/tests/test_block_standards.py` & `prefect-dask-0.2.4/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-dask-0.2.3/tests/test_task_runners.py` & `prefect-dask-0.2.4/tests/test_task_runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 from distributed import LocalCluster
 from distributed.scheduler import KilledWorker
 from prefect import flow, get_run_logger, task
 from prefect.client.schemas import TaskRun
 from prefect.server.schemas.states import StateType
 from prefect.states import State
 from prefect.task_runners import TaskConcurrencyType
-from prefect.testing.fixtures import hosted_orion_api, use_hosted_orion  # noqa: F401
+from prefect.testing.fixtures import (  # noqa: F401
+    hosted_api_server,
+    use_hosted_api_server,
+)
 from prefect.testing.standard_test_suites import TaskRunnerStandardTestSuite
 from prefect.testing.utilities import exceptions_equal
 
 from prefect_dask import DaskTaskRunner
 
 
 @pytest.fixture(scope="session")
@@ -58,15 +61,15 @@
 
     # Workaround for failures in pytest_asyncio 0.17;
     # see https://github.com/pytest-dev/pytest-asyncio/issues/257
     policy.set_event_loop(loop)
 
 
 @pytest.fixture
-def dask_task_runner_with_existing_cluster(use_hosted_orion):  # noqa
+def dask_task_runner_with_existing_cluster(use_hosted_api_server):  # noqa
     """
     Generate a dask task runner that's connected to a local cluster
     """
     with distributed.LocalCluster(n_workers=2) as cluster:
         with distributed.Client(cluster) as client:
             address = client.scheduler.address
             yield DaskTaskRunner(address=address)
```

### Comparing `prefect-dask-0.2.3/tests/test_utils.py` & `prefect-dask-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `prefect-dask-0.2.3/versioneer.py` & `prefect-dask-0.2.4/versioneer.py`

 * *Files identical despite different names*

