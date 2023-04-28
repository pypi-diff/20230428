# Comparing `tmp/shrike-1.9.4.tar.gz` & `tmp/shrike-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrike-1.9.4.tar", last modified: Thu Aug  5 18:04:48 2021, max compression
+gzip compressed data, was "shrike-1.9.5.tar", last modified: Wed Aug 11 15:45:43 2021, max compression
```

## Comparing `shrike-1.9.4.tar` & `shrike-1.9.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.624832 shrike-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-08-05 18:03:12.000000 shrike-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)   627957 2021-08-05 18:03:12.000000 shrike-1.9.4/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-08-05 18:04:48.620832 shrike-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2021-08-05 18:03:12.000000 shrike-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-05 18:04:48.624832 shrike-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2021-08-05 18:03:12.000000 shrike-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.616832 shrike-1.9.4/shrike/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/build/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/build/commands/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40962 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/commands/prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     7142 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/commands/register.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/build/core/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12518 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/core/command_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     7594 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/core/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/build/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5526 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/build/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/compliant_logging/
--rw-r--r--   0 runner    (1001) docker     (121)      932 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    10327 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13617 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    37911 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4875 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/stack_trace_extractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/compliant_logging/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (121)     7143 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/canary_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13162 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    63121 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/pipeline_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/telemetry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/pipeline/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24363 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/testing/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/testing/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/testing/module_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     7855 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/pipeline/testing/pipeline_class_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.620832 shrike-1.9.4/shrike/spark/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2021-08-05 18:03:12.000000 shrike-1.9.4/shrike/spark/spark_net.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 18:04:48.616832 shrike-1.9.4/shrike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-08-05 18:04:48.000000 shrike-1.9.4/shrike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-08-05 18:04:48.000000 shrike-1.9.4/shrike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 18:04:48.000000 shrike-1.9.4/shrike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-08-05 18:04:48.000000 shrike-1.9.4/shrike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-05 18:04:48.000000 shrike-1.9.4/shrike.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-08-11 15:43:54.000000 shrike-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)   627957 2021-08-11 15:43:54.000000 shrike-1.9.5/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-08-11 15:45:43.127162 shrike-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5637 2021-08-11 15:43:54.000000 shrike-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 15:45:43.127162 shrike-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2091 2021-08-11 15:43:54.000000 shrike-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/build/
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/build/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40962 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/commands/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7142 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/commands/register.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/build/core/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12518 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/core/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7594 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/core/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/build/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5526 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/compliant_logging/
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10327 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13617 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37911 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4875 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/stack_trace_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4900 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7143 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/canary_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13162 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3277 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63121 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/pipeline_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2685 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/telemetry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/pipeline/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24363 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/components.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/module_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7855 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/pipeline_class_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/spark/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4870 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/spark/spark_net.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/top_level.txt
```

### Comparing `shrike-1.9.4/LICENSE` & `shrike-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/NOTICE.txt` & `shrike-1.9.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/PKG-INFO` & `shrike-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 1.9.4
+Version: 1.9.5
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/azure/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: Compliant Azure ML Utilities
```

### Comparing `shrike-1.9.4/README.md` & `shrike-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/setup.py` & `shrike-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/build/commands/prepare.py` & `shrike-1.9.5/shrike/build/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/build/commands/register.py` & `shrike-1.9.5/shrike/build/commands/register.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/build/core/command_line.py` & `shrike-1.9.5/shrike/build/core/command_line.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/build/core/configuration.py` & `shrike-1.9.5/shrike/build/core/configuration.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/build/utils/utils.py` & `shrike-1.9.5/shrike/build/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/compliant_logging/__init__.py` & `shrike-1.9.5/shrike/compliant_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/compliant_logging/data_conversions.py` & `shrike-1.9.5/shrike/compliant_logging/data_conversions.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/compliant_logging/exceptions.py` & `shrike-1.9.5/shrike/compliant_logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/compliant_logging/logging.py` & `shrike-1.9.5/shrike/compliant_logging/logging.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/compliant_logging/stack_trace_extractor.py` & `shrike-1.9.5/shrike/compliant_logging/stack_trace_extractor.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/compliant_logging/system_info.py` & `shrike-1.9.5/shrike/compliant_logging/system_info.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/aml_connect.py` & `shrike-1.9.5/shrike/pipeline/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/canary_helper.py` & `shrike-1.9.5/shrike/pipeline/canary_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/module_helper.py` & `shrike-1.9.5/shrike/pipeline/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/pipeline_config.py` & `shrike-1.9.5/shrike/pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/pipeline_helper.py` & `shrike-1.9.5/shrike/pipeline/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/telemetry_utils.py` & `shrike-1.9.5/shrike/pipeline/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/testing/components.py` & `shrike-1.9.5/shrike/pipeline/testing/components.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/testing/importer.py` & `shrike-1.9.5/shrike/pipeline/testing/importer.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/testing/module_run_tests.py` & `shrike-1.9.5/shrike/pipeline/testing/module_run_tests.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/pipeline/testing/pipeline_class_test.py` & `shrike-1.9.5/shrike/pipeline/testing/pipeline_class_test.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike/spark/spark_net.py` & `shrike-1.9.5/shrike/spark/spark_net.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike.egg-info/PKG-INFO` & `shrike-1.9.5/shrike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 1.9.4
+Version: 1.9.5
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/azure/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: Compliant Azure ML Utilities
```

### Comparing `shrike-1.9.4/shrike.egg-info/SOURCES.txt` & `shrike-1.9.5/shrike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shrike-1.9.4/shrike.egg-info/requires.txt` & `shrike-1.9.5/shrike.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 pandas==1.1.5
 scikit-learn==0.24.2
 
 [pipeline]
 azureml-pipeline~=1.33.0
 azureml-sdk~=1.33.0
 azure-ml-component==0.1.0.42428082
-cryptography==3.3.2
-azure-cli-core==2.22.1
+cryptography~=3.3.2
+azure-cli-core~=2.22
 ruamel.yaml~=0.16
 gitpython~=3.1
-hydra-core==1.0.3
+hydra-core~=1.0.3
 flatten-dict~=0.4
 jsonpath_ng~=1.5
 opencensus-ext-azure==1.0.7
 pytest~=6.2
```

