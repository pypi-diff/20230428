# Comparing `tmp/interactions-restful-1.0.0.tar.gz` & `tmp/interactions-restful-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions-restful-1.0.0.tar", last modified: Wed Apr 12 17:07:47 2023, max compression
+gzip compressed data, was "interactions-restful-1.0.1.tar", last modified: Fri Apr 28 07:20:37 2023, max compression
```

## Comparing `interactions-restful-1.0.0.tar` & `interactions-restful-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:07:47.158396 interactions-restful-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-12 17:07:47.158396 interactions-restful-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:07:47.158396 interactions-restful-1.0.0/interactions_restful/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/interactions_restful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/interactions_restful/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/interactions_restful/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/interactions_restful/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:07:47.158396 interactions-restful-1.0.0/interactions_restful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-12 17:07:47.000000 interactions-restful-1.0.0/interactions_restful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 17:07:47.000000 interactions-restful-1.0.0/interactions_restful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:07:47.000000 interactions-restful-1.0.0/interactions_restful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 17:07:47.000000 interactions-restful-1.0.0/interactions_restful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 17:07:47.000000 interactions-restful-1.0.0/interactions_restful.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:07:47.158396 interactions-restful-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 17:07:37.000000 interactions-restful-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/interactions_restful/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/interactions_restful/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/backends/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/backends/flask_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/interactions_restful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/setup.py
```

### Comparing `interactions-restful-1.0.0/LICENSE` & `interactions-restful-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.0/PKG-INFO` & `interactions-restful-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions-restful
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for interactions.py allowing runtime API structures
 Home-page: https://github.com/interactions-py/restful
 Author: Damego
 Author-email: damego.dev@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `interactions-restful-1.0.0/README.md` & `interactions-restful-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.0/interactions_restful/abc.py` & `interactions-restful-1.0.1/interactions_restful/abc.py`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.0/interactions_restful/extension.py` & `interactions-restful-1.0.1/interactions_restful/extension.py`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.0/interactions_restful.egg-info/PKG-INFO` & `interactions-restful-1.0.1/interactions_restful.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions-restful
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for interactions.py allowing runtime API structures
 Home-page: https://github.com/interactions-py/restful
 Author: Damego
 Author-email: damego.dev@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `interactions-restful-1.0.0/pyproject.toml` & `interactions-restful-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 100
 
 [tool.poetry]
 name = "interactions-restful"
-version = "1.0.0"
+version = "1.0.1"
 description = "A library for interactions.py allowing runtime API structures"
 authors = ["Damego <damego.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `interactions-restful-1.0.0/setup.py` & `interactions-restful-1.0.1/setup.py`

 * *Files identical despite different names*

