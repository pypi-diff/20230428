# Comparing `tmp/dag-factory-0.9.0.tar.gz` & `tmp/dag-factory-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dag-factory-0.9.0.tar", last modified: Sun Jul 25 18:51:10 2021, max compression
+gzip compressed data, was "dist/dag-factory-0.9.1.tar", last modified: Tue Jul 27 21:48:30 2021, max compression
```

## Comparing `dag-factory-0.9.0.tar` & `dag-factory-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 aboscarino   (501) staff       (20)        0 2021-07-25 18:51:10.000000 dag-factory-0.9.0/
--rw-r--r--   0 aboscarino   (501) staff       (20)     1080 2021-07-25 17:59:57.000000 dag-factory-0.9.0/LICENSE
--rw-r--r--   0 aboscarino   (501) staff       (20)       62 2021-07-25 17:59:57.000000 dag-factory-0.9.0/MANIFEST.in
--rw-r--r--   0 aboscarino   (501) staff       (20)     4207 2021-07-25 18:51:10.000000 dag-factory-0.9.0/PKG-INFO
--rw-r--r--   0 aboscarino   (501) staff       (20)     2853 2021-07-25 17:59:57.000000 dag-factory-0.9.0/README.md
-drwxr-xr-x   0 aboscarino   (501) staff       (20)        0 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dag_factory.egg-info/
--rw-r--r--   0 aboscarino   (501) staff       (20)     4207 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dag_factory.egg-info/PKG-INFO
--rw-r--r--   0 aboscarino   (501) staff       (20)      331 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dag_factory.egg-info/SOURCES.txt
--rw-r--r--   0 aboscarino   (501) staff       (20)        1 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dag_factory.egg-info/dependency_links.txt
--rw-r--r--   0 aboscarino   (501) staff       (20)       94 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dag_factory.egg-info/requires.txt
--rw-r--r--   0 aboscarino   (501) staff       (20)       11 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dag_factory.egg-info/top_level.txt
-drwxr-xr-x   0 aboscarino   (501) staff       (20)        0 2021-07-25 18:51:10.000000 dag-factory-0.9.0/dagfactory/
--rw-r--r--   0 aboscarino   (501) staff       (20)       89 2021-07-25 17:59:57.000000 dag-factory-0.9.0/dagfactory/__init__.py
--rw-r--r--   0 aboscarino   (501) staff       (20)       71 2021-07-25 18:50:13.000000 dag-factory-0.9.0/dagfactory/__version__.py
--rw-r--r--   0 aboscarino   (501) staff       (20)    20411 2021-07-25 18:48:57.000000 dag-factory-0.9.0/dagfactory/dagbuilder.py
--rw-r--r--   0 aboscarino   (501) staff       (20)     5439 2021-07-25 18:48:57.000000 dag-factory-0.9.0/dagfactory/dagfactory.py
--rw-r--r--   0 aboscarino   (501) staff       (20)     5067 2021-07-25 18:02:01.000000 dag-factory-0.9.0/dagfactory/utils.py
--rw-r--r--   0 aboscarino   (501) staff       (20)       38 2021-07-25 18:51:10.000000 dag-factory-0.9.0/setup.cfg
--rw-r--r--   0 aboscarino   (501) staff       (20)     3091 2021-07-25 17:59:57.000000 dag-factory-0.9.0/setup.py
+drwxr-xr-x   0 aboscarino   (501) staff       (20)        0 2021-07-27 21:48:30.000000 dag-factory-0.9.1/
+-rw-r--r--   0 aboscarino   (501) staff       (20)     1080 2021-07-25 17:59:57.000000 dag-factory-0.9.1/LICENSE
+-rw-r--r--   0 aboscarino   (501) staff       (20)       62 2021-07-25 17:59:57.000000 dag-factory-0.9.1/MANIFEST.in
+-rw-r--r--   0 aboscarino   (501) staff       (20)     4207 2021-07-27 21:48:30.000000 dag-factory-0.9.1/PKG-INFO
+-rw-r--r--   0 aboscarino   (501) staff       (20)     2853 2021-07-25 17:59:57.000000 dag-factory-0.9.1/README.md
+drwxr-xr-x   0 aboscarino   (501) staff       (20)        0 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dag_factory.egg-info/
+-rw-r--r--   0 aboscarino   (501) staff       (20)     4207 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dag_factory.egg-info/PKG-INFO
+-rw-r--r--   0 aboscarino   (501) staff       (20)      331 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dag_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 aboscarino   (501) staff       (20)        1 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dag_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 aboscarino   (501) staff       (20)       94 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dag_factory.egg-info/requires.txt
+-rw-r--r--   0 aboscarino   (501) staff       (20)       11 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dag_factory.egg-info/top_level.txt
+drwxr-xr-x   0 aboscarino   (501) staff       (20)        0 2021-07-27 21:48:30.000000 dag-factory-0.9.1/dagfactory/
+-rw-r--r--   0 aboscarino   (501) staff       (20)       89 2021-07-25 17:59:57.000000 dag-factory-0.9.1/dagfactory/__init__.py
+-rw-r--r--   0 aboscarino   (501) staff       (20)       71 2021-07-27 21:47:52.000000 dag-factory-0.9.1/dagfactory/__version__.py
+-rw-r--r--   0 aboscarino   (501) staff       (20)    21114 2021-07-27 21:46:11.000000 dag-factory-0.9.1/dagfactory/dagbuilder.py
+-rw-r--r--   0 aboscarino   (501) staff       (20)     5439 2021-07-25 18:48:57.000000 dag-factory-0.9.1/dagfactory/dagfactory.py
+-rw-r--r--   0 aboscarino   (501) staff       (20)     5067 2021-07-25 18:02:01.000000 dag-factory-0.9.1/dagfactory/utils.py
+-rw-r--r--   0 aboscarino   (501) staff       (20)       38 2021-07-27 21:48:30.000000 dag-factory-0.9.1/setup.cfg
+-rw-r--r--   0 aboscarino   (501) staff       (20)     3091 2021-07-25 17:59:57.000000 dag-factory-0.9.1/setup.py
```

### Comparing `dag-factory-0.9.0/LICENSE` & `dag-factory-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dag-factory-0.9.0/PKG-INFO` & `dag-factory-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dag-factory
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dynamically build Airflow DAGs from YAML files
 Home-page: https://github.com/ajbosco/dag-factory
 Author: Adam Boscarino
 Author-email: adam@boscarino.me
 License: MIT
 Description: 
         # dag-factory
```

### Comparing `dag-factory-0.9.0/README.md` & `dag-factory-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dag-factory-0.9.0/dag_factory.egg-info/PKG-INFO` & `dag-factory-0.9.1/dag_factory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dag-factory
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dynamically build Airflow DAGs from YAML files
 Home-page: https://github.com/ajbosco/dag-factory
 Author: Adam Boscarino
 Author-email: adam@boscarino.me
 License: MIT
 Description: 
         # dag-factory
```

### Comparing `dag-factory-0.9.0/dagfactory/dagbuilder.py` & `dag-factory-0.9.1/dagfactory/dagbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from copy import deepcopy
 
 from airflow import DAG, configuration
 from airflow.models import Variable
 from airflow.contrib.operators.kubernetes_pod_operator import KubernetesPodOperator
 from airflow.models import BaseOperator
-from airflow.operators.python_operator import PythonOperator
+from airflow.operators.python_operator import PythonOperator, BranchPythonOperator
 from airflow.utils.module_loading import import_string
 from airflow import __version__ as AIRFLOW_VERSION
 
 # kubernetes operator
 try:
     from airflow.kubernetes.secret import Secret
     from airflow.kubernetes.pod import Port
@@ -105,42 +105,54 @@
         if utils.check_dict_key(dag_params["default_args"], "retry_delay_sec"):
             dag_params["default_args"]["retry_delay"]: timedelta = timedelta(
                 seconds=dag_params["default_args"]["retry_delay_sec"]
             )
             del dag_params["default_args"]["retry_delay_sec"]
 
         if utils.check_dict_key(dag_params["default_args"], "sla_miss_callback"):
-            dag_params["default_args"]["sla_miss_callback"]: Callable = import_string(
-                dag_params["default_args"]["sla_miss_callback"]
-            )
+            if isinstance(dag_params["default_args"]["sla_miss_callback"], str):
+                dag_params["default_args"][
+                    "sla_miss_callback"
+                ]: Callable = import_string(
+                    dag_params["default_args"]["sla_miss_callback"]
+                )
 
         if utils.check_dict_key(dag_params["default_args"], "on_success_callback"):
-            dag_params["default_args"]["on_success_callback"]: Callable = import_string(
-                dag_params["default_args"]["on_success_callback"]
-            )
+            if isinstance(dag_params["default_args"]["on_success_callback"], str):
+                dag_params["default_args"][
+                    "on_success_callback"
+                ]: Callable = import_string(
+                    dag_params["default_args"]["on_success_callback"]
+                )
 
         if utils.check_dict_key(dag_params["default_args"], "on_failure_callback"):
-            dag_params["default_args"]["on_failure_callback"]: Callable = import_string(
-                dag_params["default_args"]["on_failure_callback"]
-            )
+            if isinstance(dag_params["default_args"]["on_failure_callback"], str):
+                dag_params["default_args"][
+                    "on_failure_callback"
+                ]: Callable = import_string(
+                    dag_params["default_args"]["on_failure_callback"]
+                )
 
         if utils.check_dict_key(dag_params, "sla_miss_callback"):
-            dag_params["sla_miss_callback"]: Callable = import_string(
-                dag_params["sla_miss_callback"]
-            )
+            if isinstance(dag_params["sla_miss_callback"], str):
+                dag_params["sla_miss_callback"]: Callable = import_string(
+                    dag_params["sla_miss_callback"]
+                )
 
         if utils.check_dict_key(dag_params, "on_success_callback"):
-            dag_params["on_success_callback"]: Callable = import_string(
-                dag_params["on_success_callback"]
-            )
+            if isinstance(dag_params["on_success_callback"], str):
+                dag_params["on_success_callback"]: Callable = import_string(
+                    dag_params["on_success_callback"]
+                )
 
         if utils.check_dict_key(dag_params, "on_failure_callback"):
-            dag_params["on_failure_callback"]: Callable = import_string(
-                dag_params["on_failure_callback"]
-            )
+            if isinstance(dag_params["on_failure_callback"], str):
+                dag_params["on_failure_callback"]: Callable = import_string(
+                    dag_params["on_failure_callback"]
+                )
 
         if utils.check_dict_key(
             dag_params, "on_success_callback_name"
         ) and utils.check_dict_key(dag_params, "on_success_callback_file"):
             dag_params["on_success_callback"]: Callable = utils.get_python_callable(
                 dag_params["on_success_callback_name"],
                 dag_params["on_success_callback_file"],
@@ -175,21 +187,21 @@
         """
         try:
             # class is a Callable https://stackoverflow.com/a/34578836/3679900
             operator_obj: Callable[..., BaseOperator] = import_string(operator)
         except Exception as err:
             raise Exception(f"Failed to import operator: {operator}") from err
         try:
-            if operator_obj == PythonOperator:
+            if operator_obj in [PythonOperator, BranchPythonOperator]:
                 if not task_params.get("python_callable_name") and not task_params.get(
                     "python_callable_file"
                 ):
                     raise Exception(
-                        "Failed to create task. PythonOperator requires `python_callable_name` \
-                        and `python_callable_file` parameters."
+                        "Failed to create task. PythonOperator and BranchPythonOperator requires \
+                        `python_callable_name` and `python_callable_file` parameters."
                     )
                 task_params["python_callable"]: Callable = utils.get_python_callable(
                     task_params["python_callable_name"],
                     task_params["python_callable_file"],
                 )
                 # remove dag-factory specific parameters
                 # Airflow 2.0 doesn't allow these to be passed to operator
```

### Comparing `dag-factory-0.9.0/dagfactory/dagfactory.py` & `dag-factory-0.9.1/dagfactory/dagfactory.py`

 * *Files identical despite different names*

### Comparing `dag-factory-0.9.0/dagfactory/utils.py` & `dag-factory-0.9.1/dagfactory/utils.py`

 * *Files identical despite different names*

### Comparing `dag-factory-0.9.0/setup.py` & `dag-factory-0.9.1/setup.py`

 * *Files identical despite different names*

