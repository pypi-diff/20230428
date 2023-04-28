# Comparing `tmp/edx-proctoring-proctortrack-1.1.1.tar.gz` & `tmp/edx-proctoring-proctortrack-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-proctoring-proctortrack-1.1.1.tar", last modified: Mon Apr  4 08:50:24 2022, max compression
+gzip compressed data, was "edx-proctoring-proctortrack-1.2.1.tar", last modified: Fri Apr 28 12:33:39 2023, max compression
```

## Comparing `edx-proctoring-proctortrack-1.1.1.tar` & `edx-proctoring-proctortrack-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anup      (1000) anup      (1000)        0 2022-04-04 08:50:24.423154 edx-proctoring-proctortrack-1.1.1/
--rw-r--r--   0 anup      (1000) anup      (1000)      140 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/AUTHORS
--rw-r--r--   0 anup      (1000) anup      (1000)      145 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/MANIFEST.in
--rw-r--r--   0 anup      (1000) anup      (1000)      851 2022-04-04 08:50:24.423154 edx-proctoring-proctortrack-1.1.1/PKG-INFO
--rw-r--r--   0 anup      (1000) anup      (1000)       95 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/README.md
-drwxr-xr-x   0 anup      (1000) anup      (1000)        0 2022-04-04 08:50:24.413154 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/
--rw-r--r--   0 anup      (1000) anup      (1000)        0 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/__init__.py
-drwxr-xr-x   0 anup      (1000) anup      (1000)        0 2022-04-04 08:50:24.423154 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/backends/
--rw-r--r--   0 anup      (1000) anup      (1000)        0 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/backends/__init__.py
--rw-r--r--   0 anup      (1000) anup      (1000)     1848 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/backends/proctortrack_rest.py
-drwxr-xr-x   0 anup      (1000) anup      (1000)        0 2022-04-04 08:50:24.423154 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/static/
--rw-r--r--   0 anup      (1000) anup      (1000)     2941 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/static/proctortrack_custom.js
-drwxr-xr-x   0 anup      (1000) anup      (1000)        0 2022-04-04 08:50:24.423154 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/
--rw-r--r--   0 anup      (1000) anup      (1000)      851 2022-04-04 08:50:24.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/PKG-INFO
--rw-r--r--   0 anup      (1000) anup      (1000)      551 2022-04-04 08:50:24.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/SOURCES.txt
--rw-r--r--   0 anup      (1000) anup      (1000)        1 2022-04-04 08:50:24.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/dependency_links.txt
--rw-r--r--   0 anup      (1000) anup      (1000)      120 2022-04-04 08:50:24.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/entry_points.txt
--rw-r--r--   0 anup      (1000) anup      (1000)       15 2022-04-04 08:50:24.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/requires.txt
--rw-r--r--   0 anup      (1000) anup      (1000)       28 2022-04-04 08:50:24.000000 edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/top_level.txt
--rw-r--r--   0 anup      (1000) anup      (1000)       38 2022-04-04 08:50:24.423154 edx-proctoring-proctortrack-1.1.1/setup.cfg
--rw-r--r--   0 anup      (1000) anup      (1000)     1368 2022-04-04 08:45:42.000000 edx-proctoring-proctortrack-1.1.1/setup.py
+drwxrwxr-x   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 12:33:39.242070 edx-proctoring-proctortrack-1.2.1/
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)      140 2023-04-28 10:31:49.000000 edx-proctoring-proctortrack-1.2.1/AUTHORS
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)      145 2023-04-28 10:31:49.000000 edx-proctoring-proctortrack-1.2.1/MANIFEST.in
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)      851 2023-04-28 12:33:39.242070 edx-proctoring-proctortrack-1.2.1/PKG-INFO
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)       95 2023-04-28 10:31:49.000000 edx-proctoring-proctortrack-1.2.1/README.md
+drwxrwxr-x   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 12:33:39.238070 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 10:31:49.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/__init__.py
+drwxrwxr-x   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 12:33:39.242070 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/backends/
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 10:31:49.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/backends/__init__.py
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)     1848 2023-04-28 10:31:49.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/backends/proctortrack_rest.py
+drwxrwxr-x   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 12:33:39.242070 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/static/
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)     6361 2023-04-28 12:00:03.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/static/proctortrack_custom.js
+drwxrwxr-x   0 khushbu   (1000) khushbu   (1000)        0 2023-04-28 12:33:39.242070 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)      851 2023-04-28 12:33:39.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/PKG-INFO
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)      551 2023-04-28 12:33:39.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)        1 2023-04-28 12:33:39.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)      120 2023-04-28 12:33:39.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/entry_points.txt
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)       15 2023-04-28 12:33:39.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/requires.txt
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)       28 2023-04-28 12:33:39.000000 edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/top_level.txt
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)       38 2023-04-28 12:33:39.242070 edx-proctoring-proctortrack-1.2.1/setup.cfg
+-rw-rw-r--   0 khushbu   (1000) khushbu   (1000)     1368 2023-04-28 12:13:35.000000 edx-proctoring-proctortrack-1.2.1/setup.py
```

### Comparing `edx-proctoring-proctortrack-1.1.1/PKG-INFO` & `edx-proctoring-proctortrack-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-proctoring-proctortrack
-Version: 1.1.1
+Version: 1.2.1
 Summary: Proctoring subsystem for edX-proctoring
 Home-page: https://github.com/joshivj/edx-proctoring-proctortrack
 Author: Verificient
 Author-email: vivek@verificient.com
 License: Apache-2.0
 Description: # edx-proctoring-proctortrack
```

### Comparing `edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack/backends/proctortrack_rest.py` & `edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack/backends/proctortrack_rest.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/PKG-INFO` & `edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-proctoring-proctortrack
-Version: 1.1.1
+Version: 1.2.1
 Summary: Proctoring subsystem for edX-proctoring
 Home-page: https://github.com/joshivj/edx-proctoring-proctortrack
 Author: Verificient
 Author-email: vivek@verificient.com
 License: Apache-2.0
 Description: # edx-proctoring-proctortrack
```

### Comparing `edx-proctoring-proctortrack-1.1.1/edx_proctoring_proctortrack.egg-info/SOURCES.txt` & `edx-proctoring-proctortrack-1.2.1/edx_proctoring_proctortrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-proctoring-proctortrack-1.1.1/setup.py` & `edx-proctoring-proctortrack-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     description='Proctoring subsystem for edX-proctoring',
     long_description=README,
     author='Verificient',
     author_email='vivek@verificient.com',
     url='https://github.com/joshivj/edx-proctoring-proctortrack',
     license="Apache-2.0",
     keywords='Proctortrack edx',
-    version='1.1.1',
+    version='1.2.1',
     packages=[
         'edx_proctoring_proctortrack',
     ],
     include_package_data=True,
     install_requires=[
         'edx_proctoring',
     ],
```

