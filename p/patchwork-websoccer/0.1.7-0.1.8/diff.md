# Comparing `tmp/patchwork-websoccer-0.1.7.tar.gz` & `tmp/patchwork-websoccer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/patchwork-websoccer-0.1.7.tar", last modified: Wed Aug 10 12:30:00 2022, max compression
+gzip compressed data, was "dist/patchwork-websoccer-0.1.8.tar", last modified: Sat Dec  3 20:06:27 2022, max compression
```

## Comparing `patchwork-websoccer-0.1.7.tar` & `patchwork-websoccer-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1033 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/client/
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/client/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2380 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/client/websock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/court/
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/court/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3021 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/court/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/court/local.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/court/patchwork.py
--rw-rw-rw-   0 root         (0) root         (0)     2987 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/fastapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/router/
--rw-rw-rw-   0 root         (0) root         (0)       71 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/patchwork/websoccer/router/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1033 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      762 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      146 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1722 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-10 12:30:00.000000 patchwork-websoccer-0.1.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-08-10 12:29:47.000000 patchwork-websoccer-0.1.7/tests/test_usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1033 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/client/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/client/websock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/court/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/court/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3021 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/court/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/court/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/court/patchwork.py
+-rw-rw-rw-   0 root         (0) root         (0)     2987 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/fastapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/router/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/patchwork/websoccer/router/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1033 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      762 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      143 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 20:06:27.000000 patchwork-websoccer-0.1.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2022-12-03 20:06:14.000000 patchwork-websoccer-0.1.8/tests/test_usage.py
```

### Comparing `patchwork-websoccer-0.1.7/LICENSE` & `patchwork-websoccer-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/PKG-INFO` & `patchwork-websoccer-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-websoccer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Websockets integration for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/client/base.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/client/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/client/websock.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/client/websock.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/court/base.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/court/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/court/local.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/court/local.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/court/patchwork.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/court/patchwork.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/fastapi.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/fastapi.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork/websoccer/router/base.py` & `patchwork-websoccer-0.1.8/patchwork/websoccer/router/base.py`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/PKG-INFO` & `patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-websoccer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Websockets integration for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-websoccer-0.1.7/patchwork_websoccer.egg-info/SOURCES.txt` & `patchwork-websoccer-0.1.8/patchwork_websoccer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchwork-websoccer-0.1.7/setup.py` & `patchwork-websoccer-0.1.8/setup.py`

 * *Files identical despite different names*

