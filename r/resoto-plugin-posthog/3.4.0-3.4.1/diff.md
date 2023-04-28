# Comparing `tmp/resoto-plugin-posthog-3.4.0.tar.gz` & `tmp/resoto-plugin-posthog-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-posthog-3.4.0.tar", last modified: Thu Apr 27 11:21:41 2023, max compression
+gzip compressed data, was "resoto-plugin-posthog-3.4.1.tar", last modified: Fri Apr 28 15:15:16 2023, max compression
```

## Comparing `resoto-plugin-posthog-3.4.0.tar` & `resoto-plugin-posthog-3.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:41.805725 resoto-plugin-posthog-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-27 11:21:41.805725 resoto-plugin-posthog-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:41.801725 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:41.805725 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 11:21:41.000000 resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:21:41.805725 resoto-plugin-posthog-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:41.805725 resoto-plugin-posthog-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 11:19:57.000000 resoto-plugin-posthog-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:16.913874 resoto-plugin-posthog-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 15:15:16.913874 resoto-plugin-posthog-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:16.913874 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:16.913874 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:15:16.000000 resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:15:16.913874 resoto-plugin-posthog-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:16.913874 resoto-plugin-posthog-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 15:13:23.000000 resoto-plugin-posthog-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-posthog-3.4.0/PKG-INFO` & `resoto-plugin-posthog-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Posthog Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.4.0/README.md` & `resoto-plugin-posthog-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/__init__.py` & `resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/posthog.py` & `resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.4.0/resoto_plugin_posthog/resources.py` & `resoto-plugin-posthog-3.4.1/resoto_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/PKG-INFO` & `resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Posthog Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.4.0/resoto_plugin_posthog.egg-info/SOURCES.txt` & `resoto-plugin-posthog-3.4.1/resoto_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.4.0/setup.py` & `resoto-plugin-posthog-3.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-posthog",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto Posthog Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["posthog = resoto_plugin_posthog:PosthogCollectorPlugin"]},
     include_package_data=True,
```

