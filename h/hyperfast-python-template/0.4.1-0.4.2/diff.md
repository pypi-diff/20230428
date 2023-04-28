# Comparing `tmp/hyperfast_python_template-0.4.1.tar.gz` & `tmp/hyperfast_python_template-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.4.1.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.4.2.tar", max compression
```

## Comparing `hyperfast_python_template-0.4.1.tar` & `hyperfast_python_template-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/LICENSE
--rw-r--r--   0        0        0     1991 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/README.md
--rw-r--r--   0        0        0     2968 2023-04-28 06:45:53.143121 hyperfast_python_template-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      323 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-04-28 06:45:53.091120 hyperfast_python_template-0.4.1/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-04-28 06:45:53.091120 hyperfast_python_template-0.4.1/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-04-28 06:45:37.794894 hyperfast_python_template-0.4.1/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-28 06:47:50.364501 hyperfast_python_template-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1991 2023-04-28 06:47:50.364501 hyperfast_python_template-0.4.2/README.md
+-rw-r--r--   0        0        0     2968 2023-04-28 06:48:10.449975 hyperfast_python_template-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-04-28 06:47:50.364501 hyperfast_python_template-0.4.2/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-04-28 06:47:50.368502 hyperfast_python_template-0.4.2/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-28 06:48:10.389972 hyperfast_python_template-0.4.2/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-04-28 06:48:10.389972 hyperfast_python_template-0.4.2/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-04-28 06:47:50.368502 hyperfast_python_template-0.4.2/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-04-28 06:47:50.368502 hyperfast_python_template-0.4.2/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-04-28 06:47:50.368502 hyperfast_python_template-0.4.2/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.2/PKG-INFO
```

### Comparing `hyperfast_python_template-0.4.1/LICENSE` & `hyperfast_python_template-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.1/README.md` & `hyperfast_python_template-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.1/pyproject.toml` & `hyperfast_python_template-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.4.1"
+version = "0.4.2"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.4.1/PKG-INFO` & `hyperfast_python_template-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

