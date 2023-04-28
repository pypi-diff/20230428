# Comparing `tmp/resoto-plugin-tagvalidator-3.4.0.tar.gz` & `tmp/resoto-plugin-tagvalidator-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-tagvalidator-3.4.0.tar", last modified: Thu Apr 27 11:25:04 2023, max compression
+gzip compressed data, was "resoto-plugin-tagvalidator-3.4.1.tar", last modified: Fri Apr 28 15:13:07 2023, max compression
```

## Comparing `resoto-plugin-tagvalidator-3.4.0.tar` & `resoto-plugin-tagvalidator-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:04.168394 resoto-plugin-tagvalidator-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-27 11:25:04.168394 resoto-plugin-tagvalidator-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:04.164394 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:04.168394 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 11:25:04.000000 resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:25:04.168394 resoto-plugin-tagvalidator-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:04.168394 resoto-plugin-tagvalidator-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-27 11:22:50.000000 resoto-plugin-tagvalidator-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:07.591026 resoto-plugin-tagvalidator-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-28 15:13:07.591026 resoto-plugin-tagvalidator-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:07.591026 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:07.591026 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 15:13:07.000000 resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:13:07.591026 resoto-plugin-tagvalidator-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:07.591026 resoto-plugin-tagvalidator-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-28 15:10:53.000000 resoto-plugin-tagvalidator-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-tagvalidator-3.4.0/PKG-INFO` & `resoto-plugin-tagvalidator-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Tag Validator Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-tagvalidator-3.4.0/README.md` & `resoto-plugin-tagvalidator-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator/__init__.py` & `resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator/config.py` & `resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.4.0/resoto_plugin_tagvalidator.egg-info/PKG-INFO` & `resoto-plugin-tagvalidator-3.4.1/resoto_plugin_tagvalidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Tag Validator Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-tagvalidator-3.4.0/setup.py` & `resoto-plugin-tagvalidator-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-tagvalidator",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto Tag Validator Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["tagvalidator = resoto_plugin_tagvalidator:TagValidatorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-tagvalidator-3.4.0/test/test_config.py` & `resoto-plugin-tagvalidator-3.4.1/test/test_config.py`

 * *Files identical despite different names*

