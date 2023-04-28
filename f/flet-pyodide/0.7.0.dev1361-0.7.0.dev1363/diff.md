# Comparing `tmp/flet_pyodide-0.7.0.dev1361.tar.gz` & `tmp/flet_pyodide-0.7.0.dev1363.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.7.0.dev1361.tar", max compression
+gzip compressed data, was "flet_pyodide-0.7.0.dev1363.tar", max compression
```

## Comparing `flet_pyodide-0.7.0.dev1361.tar` & `flet_pyodide-0.7.0.dev1363.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/README.md
--rw-r--r--   0        0        0      644 2023-04-27 19:40:13.174880 flet_pyodide-0.7.0.dev1361/pyproject.toml
--rw-r--r--   0        0        0      101 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2377 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3851 2023-04-27 19:39:37.842739 flet_pyodide-0.7.0.dev1361/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-04-27 19:40:12.634914 flet_pyodide-0.7.0.dev1361/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.7.0.dev1361/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/README.md
+-rw-r--r--   0        0        0      644 2023-04-28 20:29:32.966289 flet_pyodide-0.7.0.dev1363/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2377 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-04-28 20:28:56.245654 flet_pyodide-0.7.0.dev1363/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-04-28 20:29:31.570257 flet_pyodide-0.7.0.dev1363/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.7.0.dev1363/PKG-INFO
```

### Comparing `flet_pyodide-0.7.0.dev1361/README.md` & `flet_pyodide-0.7.0.dev1363/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.7.0.dev1361/pyproject.toml` & `flet_pyodide-0.7.0.dev1363/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.7.0.dev1361"
+version = "0.7.0.dev1363"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.7.0.dev1361"
+flet-core = "0.7.0.dev1363"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.7.0.dev1361/src/flet/flet.py` & `flet_pyodide-0.7.0.dev1363/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.7.0.dev1361/src/flet/pyodide_connection.py` & `flet_pyodide-0.7.0.dev1363/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.7.0.dev1361/PKG-INFO` & `flet_pyodide-0.7.0.dev1363/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.7.0.dev1361
+Version: 0.7.0.dev1363
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.7.0.dev1361)
+Requires-Dist: flet-core (==0.7.0.dev1363)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

