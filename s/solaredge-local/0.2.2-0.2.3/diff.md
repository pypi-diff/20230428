# Comparing `tmp/solaredge_local-0.2.2.tar.gz` & `tmp/solaredge_local-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaredge_local-0.2.2.tar", last modified: Wed Apr 26 22:36:05 2023, max compression
+gzip compressed data, was "solaredge_local-0.2.3.tar", last modified: Fri Apr 28 13:44:35 2023, max compression
```

## Comparing `solaredge_local-0.2.2.tar` & `solaredge_local-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/
--rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/PKG-INFO
--rw-rw-r--   0 drob      (1000) drob      (1000)     8375 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/README.md
--rw-rw-r--   0 drob      (1000) drob      (1000)       38 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/setup.cfg
--rw-rw-r--   0 drob      (1000) drob      (1000)     1371 2023-04-26 22:33:58.000000 solaredge_local-0.2.2/setup.py
-drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/solaredge_local/
--rw-rw-r--   0 drob      (1000) drob      (1000)       49 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/__init__.py
--rw-rw-r--   0 drob      (1000) drob      (1000)     2240 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/information_pb2.py
--rw-rw-r--   0 drob      (1000) drob      (1000)     5145 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/maintenance_pb2.py
--rw-rw-r--   0 drob      (1000) drob      (1000)    12142 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/powercontrol_pb2.py
--rw-rw-r--   0 drob      (1000) drob      (1000)      664 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/solaredge.py
--rw-rw-r--   0 drob      (1000) drob      (1000)     6161 2023-04-26 14:20:16.000000 solaredge_local-0.2.2/solaredge_local/status_pb2.py
-drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 22:36:05.649291 solaredge_local-0.2.2/solaredge_local.egg-info/
--rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/PKG-INFO
--rw-rw-r--   0 drob      (1000) drob      (1000)      405 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/SOURCES.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)        1 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/dependency_links.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)       37 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/requires.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)       16 2023-04-26 22:36:05.000000 solaredge_local-0.2.2/solaredge_local.egg-info/top_level.txt
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-28 13:44:35.886469 solaredge_local-0.2.3/
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-28 13:44:35.886469 solaredge_local-0.2.3/PKG-INFO
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8375 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/README.md
+-rw-rw-r--   0 drob      (1000) drob      (1000)       38 2023-04-28 13:44:35.886469 solaredge_local-0.2.3/setup.cfg
+-rw-rw-r--   0 drob      (1000) drob      (1000)     1307 2023-04-28 13:42:35.000000 solaredge_local-0.2.3/setup.py
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-28 13:44:35.886469 solaredge_local-0.2.3/solaredge_local/
+-rw-rw-r--   0 drob      (1000) drob      (1000)       49 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/solaredge_local/__init__.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     2240 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/solaredge_local/information_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     5145 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/solaredge_local/maintenance_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)    12142 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/solaredge_local/powercontrol_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)      664 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/solaredge_local/solaredge.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     6161 2023-04-26 14:20:16.000000 solaredge_local-0.2.3/solaredge_local/status_pb2.py
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-28 13:44:35.886469 solaredge_local-0.2.3/solaredge_local.egg-info/
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-28 13:44:35.000000 solaredge_local-0.2.3/solaredge_local.egg-info/PKG-INFO
+-rw-rw-r--   0 drob      (1000) drob      (1000)      405 2023-04-28 13:44:35.000000 solaredge_local-0.2.3/solaredge_local.egg-info/SOURCES.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)        1 2023-04-28 13:44:35.000000 solaredge_local-0.2.3/solaredge_local.egg-info/dependency_links.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)       37 2023-04-28 13:44:35.000000 solaredge_local-0.2.3/solaredge_local.egg-info/requires.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)       16 2023-04-28 13:44:35.000000 solaredge_local-0.2.3/solaredge_local.egg-info/top_level.txt
```

### Comparing `solaredge_local-0.2.2/PKG-INFO` & `solaredge_local-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge_local
-Version: 0.2.2
+Version: 0.2.3
 Summary: API wrapper to communicate locally with SolarEdge Inverters
 Home-page: https://github.com/drobtravels/solaredge-local
 Author: David Roberts
 Author-email: 
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solaredge_local-0.2.2/README.md` & `solaredge_local-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.2/setup.py` & `solaredge_local-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from __future__ import print_function
-from setuptools import setup, find_packages
+from setuptools import setup
 import io
-import codecs
 import os
-import sys
-
-import solaredge_local
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 def read(*filenames, **kwargs):
     encoding = kwargs.get('encoding', 'utf-8')
     sep = kwargs.get('sep', '\n')
     buf = []
@@ -18,15 +14,15 @@
             buf.append(f.read())
     return sep.join(buf)
 
 long_description = read('README.md')
 
 setup(
     name='solaredge_local',
-    version="0.2.2",
+    version="0.2.3",
     url='https://github.com/drobtravels/solaredge-local',
     license='MIT License',
     author='David Roberts',
     author_email="",
     description='API wrapper to communicate locally with SolarEdge Inverters',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `solaredge_local-0.2.2/solaredge_local/information_pb2.py` & `solaredge_local-0.2.3/solaredge_local/information_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.2/solaredge_local/maintenance_pb2.py` & `solaredge_local-0.2.3/solaredge_local/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.2/solaredge_local/powercontrol_pb2.py` & `solaredge_local-0.2.3/solaredge_local/powercontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.2/solaredge_local/solaredge.py` & `solaredge_local-0.2.3/solaredge_local/solaredge.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.2/solaredge_local/status_pb2.py` & `solaredge_local-0.2.3/solaredge_local/status_pb2.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.2/solaredge_local.egg-info/PKG-INFO` & `solaredge_local-0.2.3/solaredge_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge-local
-Version: 0.2.2
+Version: 0.2.3
 Summary: API wrapper to communicate locally with SolarEdge Inverters
 Home-page: https://github.com/drobtravels/solaredge-local
 Author: David Roberts
 Author-email: 
 License: MIT License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

