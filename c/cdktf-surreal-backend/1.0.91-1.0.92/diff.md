# Comparing `tmp/cdktf-surreal-backend-1.0.91.tar.gz` & `tmp/cdktf-surreal-backend-1.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-surreal-backend-1.0.91.tar", last modified: Wed Apr 26 00:18:03 2023, max compression
+gzip compressed data, was "cdktf-surreal-backend-1.0.92.tar", last modified: Thu Apr 27 00:20:10 2023, max compression
```

## Comparing `cdktf-surreal-backend-1.0.91.tar` & `cdktf-surreal-backend-1.0.92.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:03.038934 cdktf-surreal-backend-1.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-26 00:18:03.038934 cdktf-surreal-backend-1.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:18:03.038934 cdktf-surreal-backend-1.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:03.034933 cdktf-surreal-backend-1.0.91/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:03.038934 cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:03.038934 cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.91.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:17:44.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:03.038934 cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-26 00:18:02.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 00:18:03.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:18:02.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 00:18:02.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 00:18:02.000000 cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:20:10.575227 cdktf-surreal-backend-1.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-27 00:20:10.575227 cdktf-surreal-backend-1.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:20:10.575227 cdktf-surreal-backend-1.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:20:10.571227 cdktf-surreal-backend-1.0.92/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:20:10.571227 cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:20:10.575227 cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.92.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:19:57.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:20:10.575227 cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-27 00:20:10.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-27 00:20:10.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:20:10.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 00:20:10.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 00:20:10.000000 cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/top_level.txt
```

### Comparing `cdktf-surreal-backend-1.0.91/LICENSE` & `cdktf-surreal-backend-1.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.91/PKG-INFO` & `cdktf-surreal-backend-1.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.91
+Version: 1.0.92
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-surreal-backend-1.0.91/README.md` & `cdktf-surreal-backend-1.0.92/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.91/setup.py` & `cdktf-surreal-backend-1.0.92/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-surreal-backend",
-    "version": "1.0.91",
+    "version": "1.0.92",
     "description": "A package that vends a construct to setup the surreal backend in CDKTF",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-surreal-backend.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_surreal-backend",
         "cdktf_surreal-backend._jsii"
     ],
     "package_data": {
         "cdktf_surreal-backend._jsii": [
-            "cdktf-surreal-backend@1.0.91.jsii.tgz"
+            "cdktf-surreal-backend@1.0.92.jsii.tgz"
         ],
         "cdktf_surreal-backend": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-surreal-backend-1.0.91/src/cdktf_surreal-backend/__init__.py` & `cdktf-surreal-backend-1.0.92/src/cdktf_surreal-backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.91/src/cdktf_surreal_backend.egg-info/PKG-INFO` & `cdktf-surreal-backend-1.0.92/src/cdktf_surreal_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.91
+Version: 1.0.92
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

