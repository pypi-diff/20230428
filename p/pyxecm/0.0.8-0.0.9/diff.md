# Comparing `tmp/pyxecm-0.0.8.tar.gz` & `tmp/pyxecm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.8.tar", last modified: Fri Apr 28 18:16:37 2023, max compression
+gzip compressed data, was "pyxecm-0.0.9.tar", last modified: Fri Apr 28 18:49:27 2023, max compression
```

## Comparing `pyxecm-0.0.8.tar` & `pyxecm-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:16:37.651923 pyxecm-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-04-28 18:16:20.000000 pyxecm-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-28 18:16:37.650923 pyxecm-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-28 18:16:20.000000 pyxecm-0.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-28 18:16:26.000000 pyxecm-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 18:16:37.651923 pyxecm-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:16:37.642923 pyxecm-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:16:37.648923 pyxecm-0.0.8/src/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28270 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   213612 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   115022 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10226 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   223628 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-28 18:16:20.000000 pyxecm-0.0.8/src/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:16:37.650923 pyxecm-0.0.8/src/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-28 18:16:37.000000 pyxecm-0.0.8/src/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2023-04-28 18:16:37.000000 pyxecm-0.0.8/src/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 18:16:37.000000 pyxecm-0.0.8/src/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 18:16:37.000000 pyxecm-0.0.8/src/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 18:16:37.000000 pyxecm-0.0.8/src/pyxecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:49:27.961866 pyxecm-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-04-28 18:49:08.000000 pyxecm-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-28 18:49:27.961866 pyxecm-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-28 18:49:08.000000 pyxecm-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-28 18:49:17.000000 pyxecm-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 18:49:27.961866 pyxecm-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:49:27.954866 pyxecm-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:49:27.959866 pyxecm-0.0.9/src/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28270 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   213620 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   115022 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10226 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-28 18:49:08.000000 pyxecm-0.0.9/src/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:49:27.961866 pyxecm-0.0.9/src/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-28 18:49:27.000000 pyxecm-0.0.9/src/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-28 18:49:27.000000 pyxecm-0.0.9/src/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 18:49:27.000000 pyxecm-0.0.9/src/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 18:49:27.000000 pyxecm-0.0.9/src/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 18:49:27.000000 pyxecm-0.0.9/src/pyxecm.egg-info/top_level.txt
```

### Comparing `pyxecm-0.0.8/LICENSE` & `pyxecm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/PKG-INFO` & `pyxecm-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to connect to Opentext Extended ECM
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxecm-0.0.8/pyproject.toml` & `pyxecm-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36"]
   description = "A library to connect to Opentext Extended ECM"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.8"
+  version = "0.0.9"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.8/src/pyxecm/k8s.py` & `pyxecm-0.0.9/src/pyxecm/k8s.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/src/pyxecm/otac.py` & `pyxecm-0.0.9/src/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/src/pyxecm/otcs.py` & `pyxecm-0.0.9/src/pyxecm/otcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 import os
 import logging
 import requests
 import json
 import urllib.parse
 from datetime import datetime
-import translate
+from .translate import *
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 requestJsonHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
```

### Comparing `pyxecm-0.0.8/src/pyxecm/otds.py` & `pyxecm-0.0.9/src/pyxecm/otds.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/src/pyxecm/otiv.py` & `pyxecm-0.0.9/src/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/src/pyxecm/otpd.py` & `pyxecm-0.0.9/src/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/src/pyxecm/web.py` & `pyxecm-0.0.9/src/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.8/src/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.9/src/pyxecm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to connect to Opentext Extended ECM
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

