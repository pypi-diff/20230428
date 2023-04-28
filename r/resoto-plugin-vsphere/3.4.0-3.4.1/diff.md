# Comparing `tmp/resoto-plugin-vsphere-3.4.0.tar.gz` & `tmp/resoto-plugin-vsphere-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-vsphere-3.4.0.tar", last modified: Thu Apr 27 11:22:00 2023, max compression
+gzip compressed data, was "resoto-plugin-vsphere-3.4.1.tar", last modified: Fri Apr 28 15:18:07 2023, max compression
```

## Comparing `resoto-plugin-vsphere-3.4.0.tar` & `resoto-plugin-vsphere-3.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.263695 resoto-plugin-vsphere-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 11:22:00.263695 resoto-plugin-vsphere-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.263695 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.263695 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 11:22:00.000000 resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:22:00.263695 resoto-plugin-vsphere-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.263695 resoto-plugin-vsphere-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 11:19:59.000000 resoto-plugin-vsphere-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:18:07.157611 resoto-plugin-vsphere-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 15:18:07.161611 resoto-plugin-vsphere-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:18:07.157611 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:18:07.157611 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:18:07.000000 resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:18:07.161611 resoto-plugin-vsphere-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:18:07.157611 resoto-plugin-vsphere-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 15:15:27.000000 resoto-plugin-vsphere-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-vsphere-3.4.0/PKG-INFO` & `resoto-plugin-vsphere-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto VSphere Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/vsphere
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/__init__.py` & `resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/config.py` & `resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/resources.py` & `resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere/vsphere_client.py` & `resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/PKG-INFO` & `resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto VSphere Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/vsphere
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-vsphere-3.4.0/resoto_plugin_vsphere.egg-info/SOURCES.txt` & `resoto-plugin-vsphere-3.4.1/resoto_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.4.0/setup.py` & `resoto-plugin-vsphere-3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-vsphere",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto VSphere Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["vsphere = resoto_plugin_vsphere:VSphereCollectorPlugin"]},
     include_package_data=True,
```

