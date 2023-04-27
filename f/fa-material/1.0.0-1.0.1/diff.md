# Comparing `tmp/fa_material-1.0.0.tar.gz` & `tmp/fa_material-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa_material-1.0.0.tar", max compression
+gzip compressed data, was "fa_material-1.0.1.tar", max compression
```

## Comparing `fa_material-1.0.0.tar` & `fa_material-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1091 2023-04-27 23:37:43.171786 fa_material-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     1767 2023-04-27 23:37:43.171786 fa_material-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 23:37:43.171786 fa_material-1.0.0/fa_material/__init__.py
--rw-r--r--   0        0        0     1160 2023-04-27 23:37:43.171786 fa_material-1.0.0/fa_material/plugin.py
--rw-r--r--   0        0        0      840 2023-04-27 23:37:43.171786 fa_material-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 fa_material-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-27 23:41:31.236428 fa_material-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     1767 2023-04-27 23:41:31.236428 fa_material-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 23:41:31.236428 fa_material-1.0.1/fa_material/__init__.py
+-rw-r--r--   0        0        0     1160 2023-04-27 23:41:31.236428 fa_material-1.0.1/fa_material/plugin.py
+-rw-r--r--   0        0        0      839 2023-04-27 23:41:31.240429 fa_material-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 fa_material-1.0.1/PKG-INFO
```

### Comparing `fa_material-1.0.0/LICENSE.md` & `fa_material-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fa_material-1.0.0/README.md` & `fa_material-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fa_material-1.0.0/fa_material/plugin.py` & `fa_material-1.0.1/fa_material/plugin.py`

 * *Files identical despite different names*

### Comparing `fa_material-1.0.0/pyproject.toml` & `fa_material-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "fa-material"
-version = "1.0.0"
+version = "1.0.1"
 description = "Font Awesome Pro + Material for MkDocs"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.7"
 dict-deep = "^4.1.2"
 mkdocs = "^1.4.2"
 path = "^16.6.0"
 
 [tool.poetry.group.dev.dependencies]
 doppler-env = "^0.3.1"
 mkdocs-material = "^9.1.8"
```

### Comparing `fa_material-1.0.0/PKG-INFO` & `fa_material-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: fa-material
-Version: 1.0.0
+Version: 1.0.1
 Summary: Font Awesome Pro + Material for MkDocs
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Requires-Dist: path (>=16.6.0,<17.0.0)
 Description-Content-Type: text/markdown
 
 # fa-material
```

