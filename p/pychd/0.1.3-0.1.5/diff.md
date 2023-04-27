# Comparing `tmp/pychd-0.1.3.tar.gz` & `tmp/pychd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychd-0.1.3.tar", max compression
+gzip compressed data, was "pychd-0.1.5.tar", max compression
```

## Comparing `pychd-0.1.3.tar` & `pychd-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.3/LICENSE
--rw-r--r--   0        0        0    19426 2023-04-21 04:13:06.795036 pychd-0.1.3/README.md
--rw-r--r--   0        0        0      791 2023-04-21 04:14:32.525484 pychd-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.3/src/pychd/__init__.py
--rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.3/src/pychd/compile.py
--rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.3/src/pychd/decompile.py
--rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.3/src/pychd/logging.conf.template
--rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.3/src/pychd/main.py
--rw-r--r--   0        0        0    20241 1970-01-01 00:00:00.000000 pychd-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.5/LICENSE
+-rw-r--r--   0        0        0    19426 2023-04-27 21:22:50.145836 pychd-0.1.5/README.md
+-rw-r--r--   0        0        0      773 2023-04-27 22:49:25.140258 pychd-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.5/src/pychd/__init__.py
+-rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.5/src/pychd/compile.py
+-rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.5/src/pychd/decompile.py
+-rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.5/src/pychd/logging.conf.template
+-rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.5/src/pychd/main.py
+-rw-r--r--   0        0        0    20202 1970-01-01 00:00:00.000000 pychd-0.1.5/PKG-INFO
```

### Comparing `pychd-0.1.3/LICENSE` & `pychd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pychd-0.1.3/README.md` & `pychd-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pychd
+# PyChD
 
 [![CI](https://github.com/diohabara/pychd/actions/workflows/ci.yml/badge.svg)](https://github.com/diohabara/pychd/actions/workflows/ci.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/pychd.svg)](https://pypi.python.org/pypi/pychd)
 
 The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 
 ## Usage
```

### Comparing `pychd-0.1.3/pyproject.toml` & `pychd-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 description = "The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities"
 keywords = ["decompiler", "python", "poetry", "bytecode"]
 license = "MIT"
 name = "pychd"
 packages = [{include = "src/pychd"}]
 readme = "README.md"
 repository = "https://github.com/diohabara/pychd"
-version = "0.1.3"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 openai = "^0.27.4"
-pytest = "^7.3.1"
 python = ">=3.8, <3.11"
 pytype = "^2023.4.18"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
```

### Comparing `pychd-0.1.3/src/pychd/compile.py` & `pychd-0.1.5/src/pychd/compile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.3/src/pychd/decompile.py` & `pychd-0.1.5/src/pychd/decompile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.3/src/pychd/main.py` & `pychd-0.1.5/src/pychd/main.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.3/PKG-INFO` & `pychd-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pychd
-Version: 0.1.3
+Version: 0.1.5
 Summary: The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 Home-page: https://github.com/diohabara/pychd
 License: MIT
 Keywords: decompiler,python,poetry,bytecode
 Author: 卍diohabara卍
 Author-email: diohabara@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: openai (>=0.27.4,<0.28.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pytype (>=2023.4.18,<2024.0.0)
 Project-URL: Repository, https://github.com/diohabara/pychd
 Description-Content-Type: text/markdown
 
-# pychd
+# PyChD
 
 [![CI](https://github.com/diohabara/pychd/actions/workflows/ci.yml/badge.svg)](https://github.com/diohabara/pychd/actions/workflows/ci.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/pychd.svg)](https://pypi.python.org/pypi/pychd)
 
 The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 
 ## Usage
```

