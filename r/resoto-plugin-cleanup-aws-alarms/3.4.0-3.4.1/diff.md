# Comparing `tmp/resoto-plugin-cleanup-aws-alarms-3.4.0.tar.gz` & `tmp/resoto-plugin-cleanup-aws-alarms-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-alarms-3.4.0.tar", last modified: Thu Apr 27 11:25:34 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-alarms-3.4.1.tar", last modified: Fri Apr 28 15:16:10 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0.tar` & `resoto-plugin-cleanup-aws-alarms-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:34.096356 resoto-plugin-cleanup-aws-alarms-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-27 11:25:34.096356 resoto-plugin-cleanup-aws-alarms-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:34.092356 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:34.096356 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 11:25:34.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:25:34.100356 resoto-plugin-cleanup-aws-alarms-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:34.096356 resoto-plugin-cleanup-aws-alarms-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-27 11:22:46.000000 resoto-plugin-cleanup-aws-alarms-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:10.101931 resoto-plugin-cleanup-aws-alarms-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 15:16:10.101931 resoto-plugin-cleanup-aws-alarms-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:10.097931 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:10.101931 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 15:16:10.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:16:10.101931 resoto-plugin-cleanup-aws-alarms-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:10.101931 resoto-plugin-cleanup-aws-alarms-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 15:13:47.000000 resoto-plugin-cleanup-aws-alarms-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/PKG-INFO` & `resoto-plugin-cleanup-aws-alarms-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-alarms
-Version: 3.4.0
+Version: 3.4.1
 Summary: AWS Cloudwatch Alarms Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/README.md` & `resoto-plugin-cleanup-aws-alarms-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms/__init__.py` & `resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms/config.py` & `resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-alarms
-Version: 3.4.0
+Version: 3.4.1
 Summary: AWS Cloudwatch Alarms Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-alarms-3.4.1/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.4.0/setup.py` & `resoto-plugin-cleanup-aws-alarms-3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-aws-alarms",
-    version="3.4.0",
+    version="3.4.1",
     description="AWS Cloudwatch Alarms Cleaner Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["cleanup_aws_alarms = resoto_plugin_cleanup_aws_alarms:CleanupAWSAlarmsPlugin"]},
     include_package_data=True,
```

