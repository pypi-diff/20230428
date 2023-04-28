# Comparing `tmp/tamp-1.0.0.tar.gz` & `tmp/tamp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.0.0.tar", max compression
+gzip compressed data, was "tamp-1.0.1.tar", max compression
```

## Comparing `tamp-1.0.0.tar` & `tamp-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-28 19:18:02.269358 tamp-1.0.0/LICENSE
--rw-r--r--   0        0        0    14269 2023-04-28 19:18:02.273358 tamp-1.0.0/README.rst
--rw-r--r--   0        0        0     4998 2023-04-28 19:18:19.405580 tamp-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2497 2023-04-28 19:18:19.405580 tamp-1.0.0/tamp/__init__.py
--rw-r--r--   0        0        0     1523 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/__main__.py
--rw-r--r--   0        0        0        0 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2665 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/cli/main.py
--rw-r--r--   0        0        0     8237 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/compressor.py
--rw-r--r--   0        0        0     7136 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/compressor_viper.py
--rw-r--r--   0        0        0     6530 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/decompressor.py
--rw-r--r--   0        0        0     9951 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/py.typed
--rw-r--r--   0        0        0    14888 1970-01-01 00:00:00.000000 tamp-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 19:23:23.715803 tamp-1.0.1/LICENSE
+-rw-r--r--   0        0        0    14323 2023-04-28 19:23:23.715803 tamp-1.0.1/README.rst
+-rw-r--r--   0        0        0     4998 2023-04-28 19:23:46.532631 tamp-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2497 2023-04-28 19:23:46.536632 tamp-1.0.1/tamp/__init__.py
+-rw-r--r--   0        0        0     1523 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2665 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/cli/main.py
+-rw-r--r--   0        0        0     8237 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/compressor.py
+-rw-r--r--   0        0        0     7136 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     6530 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/decompressor.py
+-rw-r--r--   0        0        0     9951 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/py.typed
+-rw-r--r--   0        0        0    14942 1970-01-01 00:00:00.000000 tamp-1.0.1/PKG-INFO
```

### Comparing `tamp-1.0.0/LICENSE` & `tamp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/README.rst` & `tamp-1.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: assets/logo_300w.png
+.. image:: https://raw.githubusercontent.com/BrianPugh/tamp/main/assets/logo_300w.png
    :alt: tamp logo
    :width: 300
    :align: center
 
 -----------------------------------------------------------------
 
 |Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|
```

### Comparing `tamp-1.0.0/pyproject.toml` & `tamp-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.0.0"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.0.1"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
```

### Comparing `tamp-1.0.0/tamp/__init__.py` & `tamp-1.0.1/tamp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
```

### Comparing `tamp-1.0.0/tamp/__init__.pyi` & `tamp-1.0.1/tamp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/tamp/cli/main.py` & `tamp-1.0.1/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/tamp/compressor.py` & `tamp-1.0.1/tamp/compressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/tamp/compressor_viper.py` & `tamp-1.0.1/tamp/compressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/tamp/decompressor.py` & `tamp-1.0.1/tamp/decompressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/tamp/decompressor_viper.py` & `tamp-1.0.1/tamp/decompressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.0/PKG-INFO` & `tamp-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typer (>=0.6.0,<0.7.0)
 Project-URL: Repository, https://github.com/BrianPugh/tamp
 Description-Content-Type: text/x-rst
 
-.. image:: assets/logo_300w.png
+.. image:: https://raw.githubusercontent.com/BrianPugh/tamp/main/assets/logo_300w.png
    :alt: tamp logo
    :width: 300
    :align: center
 
 -----------------------------------------------------------------
 
 |Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|
```

