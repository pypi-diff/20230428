# Comparing `tmp/pychd-0.1.5.tar.gz` & `tmp/pychd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychd-0.1.5.tar", max compression
+gzip compressed data, was "pychd-0.1.6.tar", max compression
```

## Comparing `pychd-0.1.5.tar` & `pychd-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.5/LICENSE
--rw-r--r--   0        0        0    19426 2023-04-27 21:22:50.145836 pychd-0.1.5/README.md
--rw-r--r--   0        0        0      773 2023-04-27 22:49:25.140258 pychd-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.5/src/pychd/__init__.py
--rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.5/src/pychd/compile.py
--rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.5/src/pychd/decompile.py
--rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.5/src/pychd/logging.conf.template
--rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.5/src/pychd/main.py
--rw-r--r--   0        0        0    20202 1970-01-01 00:00:00.000000 pychd-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-27 23:02:38.813170 pychd-0.1.6/LICENSE
+-rw-r--r--   0        0        0    19426 2023-04-27 23:02:38.813170 pychd-0.1.6/README.md
+-rw-r--r--   0        0        0      773 2023-04-27 23:02:38.817170 pychd-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 23:02:38.817170 pychd-0.1.6/src/pychd/__init__.py
+-rw-r--r--   0        0        0      685 2023-04-27 23:02:38.817170 pychd-0.1.6/src/pychd/compile.py
+-rw-r--r--   0        0        0     3091 2023-04-27 23:02:38.817170 pychd-0.1.6/src/pychd/decompile.py
+-rw-r--r--   0        0        0      439 2023-04-27 23:02:38.817170 pychd-0.1.6/src/pychd/logging.conf.template
+-rw-r--r--   0        0        0     1709 2023-04-27 23:02:38.817170 pychd-0.1.6/src/pychd/main.py
+-rw-r--r--   0        0        0    20202 1970-01-01 00:00:00.000000 pychd-0.1.6/PKG-INFO
```

### Comparing `pychd-0.1.5/LICENSE` & `pychd-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pychd-0.1.5/README.md` & `pychd-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pychd-0.1.5/pyproject.toml` & `pychd-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities"
 keywords = ["decompiler", "python", "poetry", "bytecode"]
 license = "MIT"
 name = "pychd"
 packages = [{include = "src/pychd"}]
 readme = "README.md"
 repository = "https://github.com/diohabara/pychd"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 openai = "^0.27.4"
 python = ">=3.8, <3.11"
 pytype = "^2023.4.18"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `pychd-0.1.5/src/pychd/compile.py` & `pychd-0.1.6/src/pychd/compile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.5/src/pychd/decompile.py` & `pychd-0.1.6/src/pychd/decompile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.5/src/pychd/main.py` & `pychd-0.1.6/src/pychd/main.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.5/PKG-INFO` & `pychd-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychd
-Version: 0.1.5
+Version: 0.1.6
 Summary: The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 Home-page: https://github.com/diohabara/pychd
 License: MIT
 Keywords: decompiler,python,poetry,bytecode
 Author: 卍diohabara卍
 Author-email: diohabara@gmail.com
 Requires-Python: >=3.8,<3.11
```

