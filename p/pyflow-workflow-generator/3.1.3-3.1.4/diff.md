# Comparing `tmp/pyflow-workflow-generator-3.1.3.tar.gz` & `tmp/pyflow-workflow-generator-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflow-workflow-generator-3.1.3.tar", last modified: Fri Apr 28 12:36:11 2023, max compression
+gzip compressed data, was "pyflow-workflow-generator-3.1.4.tar", last modified: Fri Apr 28 13:12:15 2023, max compression
```

## Comparing `pyflow-workflow-generator-3.1.3.tar` & `pyflow-workflow-generator-3.1.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:36:11.831037 pyflow-workflow-generator-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 12:36:11.831037 pyflow-workflow-generator-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:36:11.827037 pyflow-workflow-generator-3.1.3/pyflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)    33241 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/extern.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    40761 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    48368 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/script.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:36:11.827037 pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 12:36:11.000000 pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-28 12:36:11.000000 pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:36:11.000000 pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-28 12:36:11.000000 pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 12:36:11.000000 pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 12:36:11.831037 pyflow-workflow-generator-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:36:11.831037 pyflow-workflow-generator-3.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_contextmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_extern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_families.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_inlimits.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-28 12:35:59.000000 pyflow-workflow-generator-3.1.3/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:12:15.353279 pyflow-workflow-generator-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 13:12:15.353279 pyflow-workflow-generator-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:12:15.349279 pyflow-workflow-generator-3.1.4/pyflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33241 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/extern.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40761 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48368 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:12:15.349279 pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 13:12:15.000000 pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-28 13:12:15.000000 pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:12:15.000000 pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-28 13:12:15.000000 pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 13:12:15.000000 pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 13:12:15.357279 pyflow-workflow-generator-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:12:15.353279 pyflow-workflow-generator-3.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_contextmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_extern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_families.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_inlimits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-28 13:12:01.000000 pyflow-workflow-generator-3.1.4/tests/test_time.py
```

### Comparing `pyflow-workflow-generator-3.1.3/LICENSE` & `pyflow-workflow-generator-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/PKG-INFO` & `pyflow-workflow-generator-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflow-workflow-generator
-Version: 3.1.3
+Version: 3.1.4
 Summary: Create pythonic ecFlow suites
 Home-page: https://pyflow-workflow-generator.readthedocs.io/en/
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: diagrams
```

### Comparing `pyflow-workflow-generator-3.1.3/README.md` & `pyflow-workflow-generator-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/__init__.py` & `pyflow-workflow-generator-3.1.4/pyflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/adder.py` & `pyflow-workflow-generator-3.1.4/pyflow/adder.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/anchor.py` & `pyflow-workflow-generator-3.1.4/pyflow/anchor.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/attributes.py` & `pyflow-workflow-generator-3.1.4/pyflow/attributes.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/base.py` & `pyflow-workflow-generator-3.1.4/pyflow/base.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/configurator.py` & `pyflow-workflow-generator-3.1.4/pyflow/configurator.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/cron.py` & `pyflow-workflow-generator-3.1.4/pyflow/cron.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/deployment.py` & `pyflow-workflow-generator-3.1.4/pyflow/deployment.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/expressions.py` & `pyflow-workflow-generator-3.1.4/pyflow/expressions.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/extern.py` & `pyflow-workflow-generator-3.1.4/pyflow/extern.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/graph.py` & `pyflow-workflow-generator-3.1.4/pyflow/graph.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/header.py` & `pyflow-workflow-generator-3.1.4/pyflow/header.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/host.py` & `pyflow-workflow-generator-3.1.4/pyflow/host.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/html.py` & `pyflow-workflow-generator-3.1.4/pyflow/html.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/importer.py` & `pyflow-workflow-generator-3.1.4/pyflow/importer.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/multiple.py` & `pyflow-workflow-generator-3.1.4/pyflow/multiple.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/nodes.py` & `pyflow-workflow-generator-3.1.4/pyflow/nodes.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/resource.py` & `pyflow-workflow-generator-3.1.4/pyflow/resource.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/script.py` & `pyflow-workflow-generator-3.1.4/pyflow/script.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow/state.py` & `pyflow-workflow-generator-3.1.4/pyflow/state.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/PKG-INFO` & `pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflow-workflow-generator
-Version: 3.1.3
+Version: 3.1.4
 Summary: Create pythonic ecFlow suites
 Home-page: https://pyflow-workflow-generator.readthedocs.io/en/
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: diagrams
```

### Comparing `pyflow-workflow-generator-3.1.3/pyflow_workflow_generator.egg-info/SOURCES.txt` & `pyflow-workflow-generator-3.1.4/pyflow_workflow_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/setup.cfg` & `pyflow-workflow-generator-3.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_adder.py` & `pyflow-workflow-generator-3.1.4/tests/test_adder.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_attributes.py` & `pyflow-workflow-generator-3.1.4/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_contextmanager.py` & `pyflow-workflow-generator-3.1.4/tests/test_contextmanager.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_deployment.py` & `pyflow-workflow-generator-3.1.4/tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_expressions.py` & `pyflow-workflow-generator-3.1.4/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_extern.py` & `pyflow-workflow-generator-3.1.4/tests/test_extern.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_families.py` & `pyflow-workflow-generator-3.1.4/tests/test_families.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_host.py` & `pyflow-workflow-generator-3.1.4/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_script.py` & `pyflow-workflow-generator-3.1.4/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_suite.py` & `pyflow-workflow-generator-3.1.4/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_task.py` & `pyflow-workflow-generator-3.1.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pyflow-workflow-generator-3.1.3/tests/test_time.py` & `pyflow-workflow-generator-3.1.4/tests/test_time.py`

 * *Files identical despite different names*

