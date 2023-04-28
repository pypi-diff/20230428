# Comparing `tmp/cmem_plugin_kaggle-1.0.0.tar.gz` & `tmp/cmem_plugin_kaggle-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kaggle-1.0.0.tar", max compression
+gzip compressed data, was "cmem_plugin_kaggle-1.0.0rc1.tar", max compression
```

## Comparing `cmem_plugin_kaggle-1.0.0.tar` & `cmem_plugin_kaggle-1.0.0rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      401 2023-03-10 10:01:55.717603 cmem_plugin_kaggle-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    11334 2023-03-10 10:01:55.717603 cmem_plugin_kaggle-1.0.0/LICENSE
--rw-r--r--   0        0        0      359 2023-03-10 10:01:55.717603 cmem_plugin_kaggle-1.0.0/README-public.md
--rw-r--r--   0        0        0        0 2023-03-10 10:01:55.717603 cmem_plugin_kaggle-1.0.0/cmem_plugin_kaggle/__init__.py
--rw-r--r--   0        0        0    12669 2023-03-10 10:01:55.717603 cmem_plugin_kaggle-1.0.0/cmem_plugin_kaggle/kaggle_import.py
--rw-r--r--   0        0        0     1763 2023-03-10 10:02:22.761562 cmem_plugin_kaggle-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 cmem_plugin_kaggle-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-03-10 09:12:33.891759 cmem_plugin_kaggle-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    11334 2023-03-10 09:12:33.891759 cmem_plugin_kaggle-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      332 2023-03-10 09:12:33.891759 cmem_plugin_kaggle-1.0.0rc1/README-public.md
+-rw-r--r--   0        0        0        0 2023-03-10 09:12:33.891759 cmem_plugin_kaggle-1.0.0rc1/cmem_plugin_kaggle/__init__.py
+-rw-r--r--   0        0        0    12669 2023-03-10 09:12:33.891759 cmem_plugin_kaggle-1.0.0rc1/cmem_plugin_kaggle/kaggle_import.py
+-rw-r--r--   0        0        0     1766 2023-03-10 09:13:03.643999 cmem_plugin_kaggle-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cmem_plugin_kaggle-1.0.0rc1/PKG-INFO
```

### Comparing `cmem_plugin_kaggle-1.0.0/LICENSE` & `cmem_plugin_kaggle-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kaggle-1.0.0/cmem_plugin_kaggle/kaggle_import.py` & `cmem_plugin_kaggle-1.0.0rc1/cmem_plugin_kaggle/kaggle_import.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kaggle-1.0.0/pyproject.toml` & `cmem_plugin_kaggle-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kaggle"
-version = "1.0.0"
+version = "1.0.0rc1"
 license = "Apache-2.0"
 description = "Import dataset resources from Kaggle."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `cmem_plugin_kaggle-1.0.0/PKG-INFO` & `cmem_plugin_kaggle-1.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kaggle
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Import dataset resources from Kaggle.
 Home-page: https://github.com/eccenca/cmem-plugin-kaggle
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kaggle,dataset
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -19,15 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cmem-plugin-base (>=3.0.0,<4.0.0)
 Requires-Dist: kaggle (>=1.5.13,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-kaggle
 
-Import dataset resources from [Kaggle](https://www.kaggle.com/).
+Import dataset resources from Kaggle.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
 
 You can install it with the [cmemc](https://eccenca.com/go/cmemc) command line
 clients like this:
 
 ```
```

