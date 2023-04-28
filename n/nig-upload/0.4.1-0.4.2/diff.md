# Comparing `tmp/nig-upload-0.4.1.tar.gz` & `tmp/nig-upload-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nig-upload-0.4.1.tar", last modified: Mon Nov 21 11:51:05 2022, max compression
+gzip compressed data, was "nig-upload-0.4.2.tar", last modified: Fri Apr 28 13:46:35 2023, max compression
```

## Comparing `nig-upload-0.4.1.tar` & `nig-upload-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-21 11:51:05.262076 nig-upload-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-11-21 11:51:05.262076 nig-upload-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       43 2022-11-21 11:51:04.000000 nig-upload-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-21 11:51:05.262076 nig-upload-0.4.1/nig/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-21 11:51:04.000000 nig-upload-0.4.1/nig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      102 2022-11-21 11:51:04.000000 nig-upload-0.4.1/nig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    35506 2022-11-21 11:51:04.000000 nig-upload-0.4.1/nig/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-21 11:51:05.262076 nig-upload-0.4.1/nig_upload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-11-21 11:51:05.000000 nig-upload-0.4.1/nig_upload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      270 2022-11-21 11:51:05.000000 nig-upload-0.4.1/nig_upload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-21 11:51:05.000000 nig-upload-0.4.1/nig_upload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       50 2022-11-21 11:51:05.000000 nig-upload-0.4.1/nig_upload.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2022-11-21 11:51:05.000000 nig-upload-0.4.1/nig_upload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2022-11-21 11:51:05.000000 nig-upload-0.4.1/nig_upload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-21 11:51:05.262076 nig-upload-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1042 2022-11-21 11:51:04.000000 nig-upload-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:46:35.623951 nig-upload-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 13:46:35.623951 nig-upload-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 13:46:34.000000 nig-upload-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:46:35.619951 nig-upload-0.4.2/nig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:46:34.000000 nig-upload-0.4.2/nig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 13:46:34.000000 nig-upload-0.4.2/nig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-28 13:46:34.000000 nig-upload-0.4.2/nig/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:46:35.623951 nig-upload-0.4.2/nig_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 13:46:35.000000 nig-upload-0.4.2/nig_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-28 13:46:35.000000 nig-upload-0.4.2/nig_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:46:35.000000 nig-upload-0.4.2/nig_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 13:46:35.000000 nig-upload-0.4.2/nig_upload.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 13:46:35.000000 nig-upload-0.4.2/nig_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 13:46:35.000000 nig-upload-0.4.2/nig_upload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:46:35.623951 nig-upload-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-28 13:46:34.000000 nig-upload-0.4.2/setup.py
```

### Comparing `nig-upload-0.4.1/PKG-INFO` & `nig-upload-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nig-upload
-Version: 0.4.1
+Version: 0.4.2
 Summary: CLI script for automated uploads of NIG studies
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nig-upload-0.4.1/nig/upload.py` & `nig-upload-0.4.2/nig/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 import tempfile
+import time
 import urllib.request
 from contextlib import contextmanager
 from datetime import datetime
 from mimetypes import MimeTypes
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Tuple, Union
 
@@ -167,50 +168,88 @@
     method: str,
     url: str,
     certfile: Path,
     certpwd: str,
     data: Union[bytes, Dict[str, Any]],
     headers: Optional[Dict[str, Any]] = None,
 ) -> requests.Response:
+    MAX_RETRIES = 3
+    SLEEP_TIME = 10
 
     with pfx_to_pem(certfile, certpwd) as cert:
         if method == POST:
-            return requests.post(
-                url,
-                data=data,
-                headers=headers,
-                timeout=15,
-                cert=cert,
-            )
+            for i in range(MAX_RETRIES):
+                try:
+                    r = requests.post(
+                        url,
+                        data=data,
+                        headers=headers,
+                        timeout=15,
+                        cert=cert,
+                    )
+                    return r
+                except Exception as e:
+                    error(f"The request raised the following error {e}")
+                    if i < MAX_RETRIES:
+                        debug(f"Retry n.{i + 1} will be done in {SLEEP_TIME} seconds")
+                    time.sleep(SLEEP_TIME)
+                    continue
 
         if method == PUT:
-            return requests.put(
-                url,
-                data=data,
-                headers=headers,
-                timeout=15,
-                cert=cert,
-            )
+            for i in range(MAX_RETRIES):
+                try:
+                    r = requests.put(
+                        url,
+                        data=data,
+                        headers=headers,
+                        timeout=15,
+                        cert=cert,
+                    )
+                    return r
+                except Exception as e:
+                    error(f"The request raised the following error {e}")
+                    if i < MAX_RETRIES:
+                        debug(f"Retry n.{i + 1} will be done in {SLEEP_TIME} seconds")
+                    time.sleep(SLEEP_TIME)
+                    continue
 
         if method == PATCH:
-            return requests.patch(
-                url,
-                data=data,
-                headers=headers,
-                timeout=15,
-                cert=cert,
-            )
+            for i in range(MAX_RETRIES):
+                try:
+                    r = requests.patch(
+                        url,
+                        data=data,
+                        headers=headers,
+                        timeout=15,
+                        cert=cert,
+                    )
+                    return r
+                except Exception as e:
+                    error(f"The request raised the following error {e}")
+                    if i < MAX_RETRIES:
+                        debug(f"Retry n.{i + 1} will be done in {SLEEP_TIME} seconds")
+                    time.sleep(SLEEP_TIME)
+                    continue
 
         if method == GET:
-            return requests.get(
-                url,
-                headers=headers,
-                timeout=15,
-                cert=cert,
-            )
+            for i in range(MAX_RETRIES):
+                try:
+                    r = requests.get(
+                        url,
+                        headers=headers,
+                        timeout=15,
+                        cert=cert,
+                    )
+                    return r
+                except Exception as e:
+                    error(f"The request raised the following error {e}")
+                    if i < MAX_RETRIES:
+                        debug(f"Retry n.{i + 1} will be done in {SLEEP_TIME} seconds")
+                    time.sleep(SLEEP_TIME)
+                    continue
 
         # if hasn't returned yet is because the method is unknown
         raise RequestMethodError(f"method {method} not allowed")
 
 
 def error(text: str, r: Optional[requests.Response] = None) -> None:
     if r is not None:
@@ -225,14 +264,19 @@
 
 
 def success(text: str) -> None:
     typer.secho(text, fg=typer.colors.GREEN)
     return None
 
 
+def debug(text: str) -> None:
+    typer.secho(text, fg=typer.colors.BLUE)
+    return None
+
+
 def get_response(r: requests.Response) -> Any:
     if r.text:
         return r.text
     return r.json()
 
 
 def get_value(key: str, header: List[str], line: List[str]) -> Optional[str]:
@@ -548,23 +592,31 @@
                 if (
                     dat.is_file()
                     and dat.name.endswith(".fastq.gz")
                     and dat.stat().st_size >= 1
                 ):
                     study_tree["datasets"].setdefault(d.name, [])
                     study_tree["datasets"][d.name].append(dat)
+                else:
+                    warning(f"File {dat} skipped")
+                    debug(
+                        f"DEBUG : skipped because is not a file? { not dat.is_file()}, skipped because is empty? {dat.stat().st_size < 1}, has the correct file extension (.fastq.gz)? {dat.name.endswith('.fastq.gz')}"
+                    )
             if (
                 study_tree["datasets"].get(d.name)
                 and len(study_tree["datasets"][d.name]) > 2
             ):
                 # the dataset is invalid because contains too many fastq
                 warning(
                     f"Upload of {study.name} skipped: Dataset {d.name} contains too many fastq files: max allowed files are 2 per dataset"
                 )
                 return None
+        else:
+            if d.name != "technical.txt" and d.name != "pedigree.txt":
+                warning(f"{d} is not a directory")
 
     if not study_tree["datasets"]:
         warning(
             f"Upload of {study.name} skipped: No files found for upload in: {study}"
         )
         return None
```

### Comparing `nig-upload-0.4.1/nig_upload.egg-info/PKG-INFO` & `nig-upload-0.4.2/nig_upload.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nig-upload
-Version: 0.4.1
+Version: 0.4.2
 Summary: CLI script for automated uploads of NIG studies
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nig-upload-0.4.1/setup.py` & `nig-upload-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-version = "0.4.1"
+version = "0.4.2"
 
 setup(
     name="nig-upload",
     version=version,
     description="CLI script for automated uploads of NIG studies",
     url="",
     license="MIT",
```

