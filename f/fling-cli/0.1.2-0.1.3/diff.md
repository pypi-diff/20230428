# Comparing `tmp/fling_cli-0.1.2.tar.gz` & `tmp/fling_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_cli-0.1.2.tar", max compression
+gzip compressed data, was "fling_cli-0.1.3.tar", max compression
```

## Comparing `fling_cli-0.1.2.tar` & `fling_cli-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-04-13 01:17:37.262832 fling_cli-0.1.2/fling_cli/__init__.py
--rw-r--r--   0        0        0     2040 2023-04-13 01:15:50.829929 fling_cli-0.1.2/fling_cli/auth.py
--rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.2/fling_cli/bin/__init__.py
--rw-r--r--   0        0        0     6870 2023-04-12 19:37:24.854872 fling_cli-0.1.2/fling_cli/bin/fling.py
--rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.2/fling_cli/logo-hc.txt
--rw-r--r--   0        0        0      861 2023-04-13 01:17:37.257680 fling_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 fling_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-04-27 22:06:05.211556 fling_cli-0.1.3/fling_cli/__init__.py
+-rw-r--r--   0        0        0     2040 2023-04-13 01:15:50.829929 fling_cli-0.1.3/fling_cli/auth.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.3/fling_cli/bin/__init__.py
+-rw-r--r--   0        0        0     6849 2023-04-27 22:05:56.105344 fling_cli-0.1.3/fling_cli/bin/fling.py
+-rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.3/fling_cli/logo-hc.txt
+-rw-r--r--   0        0        0      861 2023-04-27 22:06:13.497372 fling_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 fling_cli-0.1.3/PKG-INFO
```

### Comparing `fling_cli-0.1.2/README.md` & `fling_cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.2/fling_cli/auth.py` & `fling_cli-0.1.3/fling_cli/auth.py`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.2/fling_cli/bin/fling.py` & `fling_cli-0.1.3/fling_cli/bin/fling.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from fling_core import settings
 import gitinfo
 from git import Repo
 from giturlparse import parse
 
 
 def get_fling_client(require_auth=False):
-    username = settings.username or "system-default"
+    username = "system-default"
     token = keyring.get_password("fling-github-token", username)
     if not token and require_auth:
         raise UsageError("No token found, please run ```fling auth``` first.")
     headers = {"gh-token": token or "none"}
     fling_client = Client(
         settings.api_server,
         headers=headers,
```

### Comparing `fling_cli-0.1.2/fling_cli/logo-hc.txt` & `fling_cli-0.1.3/fling_cli/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.2/pyproject.toml` & `fling_cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fling-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "Side Project Management from the command line"
 authors = ["Joshua McKenty <jmckenty@gmail.com>", "Anouk Ruhaak <anoukruhaak@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fling_cli"}]
 
 [tool.poetry.dependencies]
 click = "*"
```

### Comparing `fling_cli-0.1.2/PKG-INFO` & `fling_cli-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

