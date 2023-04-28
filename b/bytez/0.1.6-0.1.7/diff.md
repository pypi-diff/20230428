# Comparing `tmp/bytez-0.1.6.tar.gz` & `tmp/bytez-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytez-0.1.6.tar", last modified: Tue Mar 28 20:32:34 2023, max compression
+gzip compressed data, was "bytez-0.1.7.tar", last modified: Fri Apr 28 00:55:24 2023, max compression
```

## Comparing `bytez-0.1.6.tar` & `bytez-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-03-28 20:32:34.918890 bytez-0.1.6/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      353 2023-03-28 20:32:34.918890 bytez-0.1.6/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.6/README.md
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-03-28 20:32:34.918890 bytez-0.1.6/bytez/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       32 2023-03-26 06:56:40.000000 bytez-0.1.6/bytez/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)    79093 2023-03-28 20:09:16.000000 bytez-0.1.6/bytez/main.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1319 2023-03-28 20:04:36.000000 bytez-0.1.6/bytez/pipeline.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-03-28 20:32:34.918890 bytez-0.1.6/bytez.egg-info/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      353 2023-03-28 20:32:34.000000 bytez-0.1.6/bytez.egg-info/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      212 2023-03-28 20:32:34.000000 bytez-0.1.6/bytez.egg-info/SOURCES.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-03-28 20:32:34.000000 bytez-0.1.6/bytez.egg-info/dependency_links.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-03-28 20:32:34.000000 bytez-0.1.6/bytez.egg-info/requires.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-03-28 20:32:34.000000 bytez-0.1.6/bytez.egg-info/top_level.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-03-28 20:32:34.918890 bytez-0.1.6/setup.cfg
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      662 2023-03-28 20:32:27.000000 bytez-0.1.6/setup.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 00:55:24.011245 bytez-0.1.7/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 00:55:24.011245 bytez-0.1.7/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.7/README.md
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 00:55:24.011245 bytez-0.1.7/bytez/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       32 2023-03-26 06:56:40.000000 bytez-0.1.7/bytez/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)    79093 2023-03-28 20:09:16.000000 bytez-0.1.7/bytez/main.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      929 2023-04-27 23:53:25.000000 bytez-0.1.7/bytez/pipeline.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 00:55:24.011245 bytez-0.1.7/bytez.egg-info/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 00:55:23.000000 bytez-0.1.7/bytez.egg-info/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      212 2023-04-28 00:55:23.000000 bytez-0.1.7/bytez.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-04-28 00:55:23.000000 bytez-0.1.7/bytez.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-04-28 00:55:23.000000 bytez-0.1.7/bytez.egg-info/requires.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-04-28 00:55:23.000000 bytez-0.1.7/bytez.egg-info/top_level.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-04-28 00:55:24.011245 bytez-0.1.7/setup.cfg
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      662 2023-04-28 00:55:23.000000 bytez-0.1.7/setup.py
```

### Comparing `bytez-0.1.6/bytez/main.py` & `bytez-0.1.7/bytez/main.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.6/bytez/pipeline.py` & `bytez-0.1.7/bytez/pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,14 @@
+import json
 from typing import BinaryIO, Literal, get_args
 from dataclasses import dataclass
 import requests
 
-
-# this will get more sophisticated as far as configuration goes, we'll want to abtract these into classes and leverage inheritance for various config options
-tasks = {
-    "style-transfer": {
-        "fast-style-transfer": "https://fast-style-transfer-tfhmsoxnpq-uc.a.run.app",
-        "cmd_styletransfer": "https://cmd-styletransfer-tfhmsoxnpq-uc.a.run.app",
-        "tensorflow-fast-style-transfer": "https://tensorflow-fast-style-transfer-tfhmsoxnpq-uc.a.run.app"
-    }
-}
+with open('tasks.json', 'r') as file:
+    tasks = json.loads(file.read())
 
 
 @dataclass
 class Handler:
     url: str
 
     def inference(self, input_img: BinaryIO) -> bytes:
```

### Comparing `bytez-0.1.6/setup.py` & `bytez-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 packages = find_packages()
 
 
 setup(
     name='bytez',
-    version='0.1.6',
+    version='0.1.7',
     packages=packages,
     install_requires=[
         'charset-normalizer==3.1.0',
         'idna==3.4',
         'requests==2.28.2',
         'urllib3==1.26.15',
     ],
```

