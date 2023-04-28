# Comparing `tmp/schoolware_api-1.0.4.tar.gz` & `tmp/schoolware_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.0.4.tar", last modified: Fri Apr 28 09:55:08 2023, max compression
+gzip compressed data, was "schoolware_api-1.0.5.tar", last modified: Fri Apr 28 10:03:09 2023, max compression
```

## Comparing `schoolware_api-1.0.4.tar` & `schoolware_api-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:55:08.096667 schoolware_api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 09:55:08.096667 schoolware_api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 09:54:56.000000 schoolware_api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 09:54:56.000000 schoolware_api-1.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:55:08.092667 schoolware_api-1.0.4/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-28 09:54:56.000000 schoolware_api-1.0.4/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-04-28 09:54:56.000000 schoolware_api-1.0.4/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:55:08.096667 schoolware_api-1.0.4/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 09:55:08.000000 schoolware_api-1.0.4/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 09:55:08.000000 schoolware_api-1.0.4/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:55:08.000000 schoolware_api-1.0.4/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 09:55:08.000000 schoolware_api-1.0.4/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:55:08.000000 schoolware_api-1.0.4/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:55:08.096667 schoolware_api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 09:54:56.000000 schoolware_api-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:03:09.462896 schoolware_api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 10:03:09.462896 schoolware_api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 10:02:58.000000 schoolware_api-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 10:02:58.000000 schoolware_api-1.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:03:09.462896 schoolware_api-1.0.5/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-28 10:02:58.000000 schoolware_api-1.0.5/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-04-28 10:02:58.000000 schoolware_api-1.0.5/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:03:09.462896 schoolware_api-1.0.5/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 10:03:09.000000 schoolware_api-1.0.5/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 10:03:09.000000 schoolware_api-1.0.5/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:03:09.000000 schoolware_api-1.0.5/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 10:03:09.000000 schoolware_api-1.0.5/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 10:03:09.000000 schoolware_api-1.0.5/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:03:09.462896 schoolware_api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 10:02:58.000000 schoolware_api-1.0.5/setup.py
```

### Comparing `schoolware_api-1.0.4/PKG-INFO` & `schoolware_api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.0.4/README.md` & `schoolware_api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.0.4/pyproject.toml` & `schoolware_api-1.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.0.4/schoolware_api/schoolware_api.py` & `schoolware_api-1.0.5/schoolware_api/schoolware_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-
-
 import requests
 from datetime import date, datetime, timedelta
 from playwright.sync_api import sync_playwright
 import time
 from termcolor import colored
 import threading
-
-
-
-
 class schoolware:
 
     def __init__(self, config) -> None:
         """Pass config file to init class
 
         Args:
             config (dict): The config file docs at https://github.com/Maarten-buelens/schoolware_api
```

### Comparing `schoolware_api-1.0.4/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.0.5/schoolware_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

