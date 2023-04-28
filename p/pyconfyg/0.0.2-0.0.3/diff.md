# Comparing `tmp/pyconfyg-0.0.2.tar.gz` & `tmp/pyconfyg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyconfyg-0.0.2.tar", last modified: Fri Oct 28 09:29:51 2022, max compression
+gzip compressed data, was "dist/pyconfyg-0.0.3.tar", last modified: Fri Apr 28 11:53:25 2023, max compression
```

## Comparing `pyconfyg-0.0.2.tar` & `pyconfyg-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 gva       (1002) cv        (1001)        0 2022-10-28 09:29:51.383830 pyconfyg-0.0.2/
--rw-r--r--   0 gva       (1002) cv        (1001)      298 2022-10-28 09:29:51.383830 pyconfyg-0.0.2/PKG-INFO
--rw-r--r--   0 gva       (1002) cv        (1001)     1092 2022-10-28 09:29:25.000000 pyconfyg-0.0.2/README.md
-drwxr-xr-x   0 gva       (1002) cv        (1001)        0 2022-10-28 09:29:51.383830 pyconfyg-0.0.2/pyconfyg/
--rw-r--r--   0 gva       (1002) cv        (1001)      105 2022-03-31 07:59:11.000000 pyconfyg-0.0.2/pyconfyg/__init__.py
--rw-r--r--   0 gva       (1002) cv        (1001)     1575 2022-03-31 07:59:11.000000 pyconfyg-0.0.2/pyconfyg/ast.py
--rw-r--r--   0 gva       (1002) cv        (1001)     5172 2022-10-28 09:28:30.000000 pyconfyg-0.0.2/pyconfyg/core.py
--rw-r--r--   0 gva       (1002) cv        (1001)       99 2022-03-31 07:59:11.000000 pyconfyg-0.0.2/pyconfyg/exceptions.py
-drwxr-xr-x   0 gva       (1002) cv        (1001)        0 2022-10-28 09:29:51.383830 pyconfyg-0.0.2/pyconfyg.egg-info/
--rw-r--r--   0 gva       (1002) cv        (1001)      298 2022-10-28 09:29:51.000000 pyconfyg-0.0.2/pyconfyg.egg-info/PKG-INFO
--rw-r--r--   0 gva       (1002) cv        (1001)      254 2022-10-28 09:29:51.000000 pyconfyg-0.0.2/pyconfyg.egg-info/SOURCES.txt
--rw-r--r--   0 gva       (1002) cv        (1001)        1 2022-10-28 09:29:51.000000 pyconfyg-0.0.2/pyconfyg.egg-info/dependency_links.txt
--rw-r--r--   0 gva       (1002) cv        (1001)       11 2022-10-28 09:29:51.000000 pyconfyg-0.0.2/pyconfyg.egg-info/requires.txt
--rw-r--r--   0 gva       (1002) cv        (1001)        9 2022-10-28 09:29:51.000000 pyconfyg-0.0.2/pyconfyg.egg-info/top_level.txt
--rw-r--r--   0 gva       (1002) cv        (1001)       38 2022-10-28 09:29:51.387831 pyconfyg-0.0.2/setup.cfg
--rw-r--r--   0 gva       (1002) cv        (1001)      419 2022-10-28 09:28:54.000000 pyconfyg-0.0.2/setup.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-28 11:53:25.969483 pyconfyg-0.0.3/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       43 2023-03-29 13:43:34.000000 pyconfyg-0.0.3/.gitignore
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      298 2023-04-28 11:53:25.968484 pyconfyg-0.0.3/PKG-INFO
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1094 2023-03-29 13:43:34.000000 pyconfyg-0.0.3/README.md
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-28 11:53:25.954484 pyconfyg-0.0.3/pyconfyg/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      105 2023-03-29 13:43:34.000000 pyconfyg-0.0.3/pyconfyg/__init__.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1663 2023-03-29 13:45:12.000000 pyconfyg-0.0.3/pyconfyg/ast.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     5223 2023-04-28 09:58:49.000000 pyconfyg-0.0.3/pyconfyg/core.py
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       99 2023-03-29 13:43:34.000000 pyconfyg-0.0.3/pyconfyg/exceptions.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-28 11:53:25.964484 pyconfyg-0.0.3/pyconfyg.egg-info/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      298 2023-04-28 11:53:25.000000 pyconfyg-0.0.3/pyconfyg.egg-info/PKG-INFO
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      299 2023-04-28 11:53:25.000000 pyconfyg-0.0.3/pyconfyg.egg-info/SOURCES.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        1 2023-04-28 11:53:25.000000 pyconfyg-0.0.3/pyconfyg.egg-info/dependency_links.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       11 2023-04-28 11:53:25.000000 pyconfyg-0.0.3/pyconfyg.egg-info/requires.txt
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)        9 2023-04-28 11:53:25.000000 pyconfyg-0.0.3/pyconfyg.egg-info/top_level.txt
+-rwxr-x---   0 gvanzand (3002593) gvanzand (3002593)      346 2023-03-29 13:43:34.000000 pyconfyg-0.0.3/release.sh
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)       38 2023-04-28 11:53:25.969483 pyconfyg-0.0.3/setup.cfg
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)      419 2023-04-28 11:53:09.000000 pyconfyg-0.0.3/setup.py
+drwxr-x---   0 gvanzand (3002593) gvanzand (3002593)        0 2023-04-28 11:53:25.966483 pyconfyg-0.0.3/tests/
+-rw-r-----   0 gvanzand (3002593) gvanzand (3002593)     1166 2023-03-29 13:43:34.000000 pyconfyg-0.0.3/tests/test_pyconfyg.py
```

### Comparing `pyconfyg-0.0.2/README.md` & `pyconfyg-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 For a configuration file `cfg.py`:
 ```
 digit = 2
 key = "a"
 value = {
   "a": 12,
   "b": 42,
-}[k]
+}[key]
 ```
 
 ## Usage
 
 ### Load configuration
 Loads the configuration file as a dictionary
 ```python
```

### Comparing `pyconfyg-0.0.2/pyconfyg/ast.py` & `pyconfyg-0.0.3/pyconfyg/ast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import ast
+from functools import lru_cache
 import logging
 from typing import Dict
 
 logger = logging.getLogger(__name__)
 
+@lru_cache(None)
+def warn_once(msg):
+    logger.warning(msg)
+
 def update_ast(
     tree: ast.Module,
     overwrite: Dict = None,
     allow_double_assignation: bool = False,
     allow_tuple_assignation: bool = False,
 ):
     if not overwrite:
@@ -36,9 +41,9 @@
     for key, value in overwrite.items():
         tree.body.append(
             ast.Assign(
                 [ast.Name(id=key, ctx=ast.Store())], ast.Constant(value, kind=None)
             )
         )
     ast.fix_missing_locations(tree)
-    logging.warning(f"Unoverwritten parameters : {list(overwrite.keys())}")
+    warn_once(f"Unoverwritten parameters : {list(overwrite.keys())}")
     return overwrite
```

### Comparing `pyconfyg-0.0.2/pyconfyg/core.py` & `pyconfyg-0.0.3/pyconfyg/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,16 @@
             err.lineno
             if isinstance(err, SyntaxError)
             else traceback.extract_tb(tb)[-1][1]
         )
         traceback.print_exception(type(err), err, tb)
     else:
         return
-    raise InterpreterError(f"{error_class} at line {line_number}: {detail}\n{cmd}")
+    line = cmd.split('\n')[line_number-1]
+    raise InterpreterError(f"{error_class} at line {line_number}: {detail}\n\t'''{line}'''")
 
 
 class Confyg:
     def __init__(self, config, overwrite: Optional[Dict] = None):
         """Some documentation here
 
         :param config: ................
```

