# Comparing `tmp/snapctl-0.2.0.tar.gz` & `tmp/snapctl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.2.0.tar", max compression
+gzip compressed data, was "snapctl-0.2.1.tar", max compression
```

## Comparing `snapctl-0.2.0.tar` & `snapctl-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.0/README.md
--rw-r--r--   0        0        0      399 2023-04-11 05:17:16.404291 snapctl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.0/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.0/snapctl/__main__.py
--rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.0/snapctl/commands/__init__.py
--rw-r--r--   0        0        0     7704 2023-04-11 06:02:17.804521 snapctl-0.2.0/snapctl/commands/byosnap.py
--rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.0/snapctl/main.py
--rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.0/snapctl/types/__init__.py
--rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.0/snapctl/types/definitions.py
--rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.0/snapctl/utils/__init__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.0/snapctl/utils/echo.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.1/README.md
+-rw-r--r--   0        0        0      399 2023-04-27 23:45:47.616360 snapctl-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.1/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.1/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.1/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0     8011 2023-04-27 23:45:34.185135 snapctl-0.2.1/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.1/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.1/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.1/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.1/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.1/snapctl/utils/echo.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.1/PKG-INFO
```

### Comparing `snapctl-0.2.0/snapctl/commands/byosnap.py` & `snapctl-0.2.1/snapctl/commands/byosnap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import os
 import requests
-from rich.progress import Progress, SpinnerColumn, TextColumn
 import subprocess
+from rich.progress import Progress, SpinnerColumn, TextColumn
+from sys import platform
 
 from snapctl.types.definitions import ResponseType
 from snapctl.utils.echo import error, success, info
 
 class ByoSnap:
   COMMANDS = ['build', 'push', 'upload-docs', 'publish']
 
@@ -90,17 +91,22 @@
       # Login to Snapser Registry
       with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
         progress.add_task(description=f'Logging into Snapser Image Registry...', total=None)
-        response = subprocess.run([
-          f'echo "{ecr_repo_token}" | docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
-        ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        if platform == 'win32':
+          response = subprocess.run([
+            f'echo({ecr_repo_token}| docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
+          ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        else:
+          response = subprocess.run([
+            f'echo "{ecr_repo_token}" | docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
+          ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to connect to the Snapser Container Repository. Please get the latest token from the Web app.')
           return False
       success('Login Successful')
 
       # Build your snap
       with Progress(
```

### Comparing `snapctl-0.2.0/snapctl/main.py` & `snapctl-0.2.1/snapctl/main.py`

 * *Files identical despite different names*

### Comparing `snapctl-0.2.0/PKG-INFO` & `snapctl-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapctl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Snapser CLI Tool
 Author: Ajinkya Apte
 Author-email: aj@snapser.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

