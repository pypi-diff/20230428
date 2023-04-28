# Comparing `tmp/resoto-plugin-example-collector-3.4.0.tar.gz` & `tmp/resoto-plugin-example-collector-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-example-collector-3.4.0.tar", last modified: Thu Apr 27 11:21:37 2023, max compression
+gzip compressed data, was "resoto-plugin-example-collector-3.4.1.tar", last modified: Fri Apr 28 15:16:04 2023, max compression
```

## Comparing `resoto-plugin-example-collector-3.4.0.tar` & `resoto-plugin-example-collector-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:37.890806 resoto-plugin-example-collector-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 11:21:37.890806 resoto-plugin-example-collector-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:37.890806 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector/
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:37.890806 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 11:21:37.000000 resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:21:37.894806 resoto-plugin-example-collector-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:37.890806 resoto-plugin-example-collector-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 11:19:53.000000 resoto-plugin-example-collector-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:04.213754 resoto-plugin-example-collector-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 15:16:04.213754 resoto-plugin-example-collector-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:04.209754 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:04.213754 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 15:16:04.000000 resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:16:04.213754 resoto-plugin-example-collector-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:04.213754 resoto-plugin-example-collector-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 15:14:03.000000 resoto-plugin-example-collector-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-example-collector-3.4.0/PKG-INFO` & `resoto-plugin-example-collector-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Example Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector/__init__.py` & `resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/PKG-INFO` & `resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Example Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-example-collector-3.4.0/resoto_plugin_example_collector.egg-info/SOURCES.txt` & `resoto-plugin-example-collector-3.4.1/resoto_plugin_example_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-example-collector-3.4.0/setup.py` & `resoto-plugin-example-collector-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-example-collector",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto Example Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["example_collector = resoto_plugin_example_collector:ExampleCollectorPlugin"]},
     include_package_data=True,
```

