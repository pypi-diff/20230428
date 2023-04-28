# Comparing `tmp/NNFAL-1.7.tar.gz` & `tmp/NNFAL-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NNFAL-1.7.tar", last modified: Wed Apr 26 10:58:00 2023, max compression
+gzip compressed data, was "NNFAL-1.8.tar", last modified: Fri Apr 28 17:40:31 2023, max compression
```

## Comparing `NNFAL-1.7.tar` & `NNFAL-1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sauvik    (1000) sauvik    (1000)        0 2023-04-26 10:58:00.192504 NNFAL-1.7/
-drwxrwxr-x   0 sauvik    (1000) sauvik    (1000)        0 2023-04-26 10:58:00.192504 NNFAL-1.7/NNFAL.egg-info/
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       47 2023-04-26 10:58:00.000000 NNFAL-1.7/NNFAL.egg-info/PKG-INFO
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)      326 2023-04-26 10:58:00.000000 NNFAL-1.7/NNFAL.egg-info/SOURCES.txt
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)        1 2023-04-26 10:58:00.000000 NNFAL-1.7/NNFAL.egg-info/dependency_links.txt
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       44 2023-04-26 10:58:00.000000 NNFAL-1.7/NNFAL.egg-info/entry_points.txt
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)        7 2023-04-26 10:58:00.000000 NNFAL-1.7/NNFAL.egg-info/top_level.txt
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       47 2023-04-26 10:58:00.192504 NNFAL-1.7/PKG-INFO
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)     1838 2023-04-12 09:03:56.000000 NNFAL-1.7/README.md
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       38 2023-04-26 10:58:00.192504 NNFAL-1.7/setup.cfg
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)      320 2023-04-26 10:57:56.000000 NNFAL-1.7/setup.py
-drwxrwxr-x   0 sauvik    (1000) sauvik    (1000)        0 2023-04-26 10:58:00.192504 NNFAL-1.7/source/
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     5445 2023-04-26 10:57:48.000000 NNFAL-1.7/source/NNFAL.py
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     1130 2023-03-30 15:36:10.000000 NNFAL-1.7/source/dnnf.py
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     6118 2023-04-21 06:00:31.000000 NNFAL-1.7/source/run_matlab.py
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)    10120 2023-03-30 15:36:10.000000 NNFAL-1.7/source/run_xspeed.py
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)    11130 2023-03-30 15:36:10.000000 NNFAL-1.7/source/runscript.py
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     5337 2023-04-11 07:16:57.000000 NNFAL-1.7/source/scale.py
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)     7982 2023-04-11 07:16:57.000000 NNFAL-1.7/source/setting.py
--rw-rw-r--   0 sauvik    (1000) sauvik    (1000)      291 2023-04-26 10:19:09.000000 NNFAL-1.7/source/setup.py
--rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)      949 2023-03-30 15:36:10.000000 NNFAL-1.7/source/xspeed.py
+drwxrwxr-x   0 sauvik    (1000) sauvik    (1000)        0 2023-04-28 17:40:31.304495 NNFAL-1.8/
+drwxrwxr-x   0 sauvik    (1000) sauvik    (1000)        0 2023-04-28 17:40:31.304495 NNFAL-1.8/NNFAL.egg-info/
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       47 2023-04-28 17:40:31.000000 NNFAL-1.8/NNFAL.egg-info/PKG-INFO
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)      326 2023-04-28 17:40:31.000000 NNFAL-1.8/NNFAL.egg-info/SOURCES.txt
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)        1 2023-04-28 17:40:31.000000 NNFAL-1.8/NNFAL.egg-info/dependency_links.txt
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       44 2023-04-28 17:40:31.000000 NNFAL-1.8/NNFAL.egg-info/entry_points.txt
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)        7 2023-04-28 17:40:31.000000 NNFAL-1.8/NNFAL.egg-info/top_level.txt
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       47 2023-04-28 17:40:31.304495 NNFAL-1.8/PKG-INFO
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)     1838 2023-04-12 09:03:56.000000 NNFAL-1.8/README.md
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)       38 2023-04-28 17:40:31.304495 NNFAL-1.8/setup.cfg
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)      320 2023-04-28 17:39:04.000000 NNFAL-1.8/setup.py
+drwxrwxr-x   0 sauvik    (1000) sauvik    (1000)        0 2023-04-28 17:40:31.304495 NNFAL-1.8/source/
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     5187 2023-04-28 17:40:02.000000 NNFAL-1.8/source/NNFAL.py
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     1130 2023-03-30 15:36:10.000000 NNFAL-1.8/source/dnnf.py
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     6118 2023-04-21 06:00:31.000000 NNFAL-1.8/source/run_matlab.py
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)    10120 2023-03-30 15:36:10.000000 NNFAL-1.8/source/run_xspeed.py
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)    11130 2023-03-30 15:36:10.000000 NNFAL-1.8/source/runscript.py
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)     5337 2023-04-11 07:16:57.000000 NNFAL-1.8/source/scale.py
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)     7982 2023-04-11 07:16:57.000000 NNFAL-1.8/source/setting.py
+-rw-rw-r--   0 sauvik    (1000) sauvik    (1000)      291 2023-04-26 10:19:09.000000 NNFAL-1.8/source/setup.py
+-rwxrwxr-x   0 sauvik    (1000) sauvik    (1000)      949 2023-03-30 15:36:10.000000 NNFAL-1.8/source/xspeed.py
```

### Comparing `NNFAL-1.7/README.md` & `NNFAL-1.8/README.md`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/NNFAL.py` & `NNFAL-1.8/source/NNFAL.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 ##!/usr/bin/env python3
 
 import os
 import sys
 
-module_dir = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(module_dir, 'source'))
-
-# Set the PYTHONPATH environment variable
-os.environ['PYTHONPATH'] = os.path.join(module_dir, 'source') + ':' + os.environ.get('PYTHONPATH', '')
-
 import os
 import subprocess
 import re
 import numpy as np
 import xspeed
 import dnnf
 import time
```

### Comparing `NNFAL-1.7/source/dnnf.py` & `NNFAL-1.8/source/dnnf.py`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/run_matlab.py` & `NNFAL-1.8/source/run_matlab.py`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/run_xspeed.py` & `NNFAL-1.8/source/run_xspeed.py`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/runscript.py` & `NNFAL-1.8/source/runscript.py`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/scale.py` & `NNFAL-1.8/source/scale.py`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/setting.py` & `NNFAL-1.8/source/setting.py`

 * *Files identical despite different names*

### Comparing `NNFAL-1.7/source/xspeed.py` & `NNFAL-1.8/source/xspeed.py`

 * *Files identical despite different names*

