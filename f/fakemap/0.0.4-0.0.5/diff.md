# Comparing `tmp/fakemap-0.0.4.tar.gz` & `tmp/fakemap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakemap-0.0.4.tar", last modified: Fri Apr 21 21:31:37 2023, max compression
+gzip compressed data, was "fakemap-0.0.5.tar", last modified: Fri Apr 28 00:47:50 2023, max compression
```

## Comparing `fakemap-0.0.4.tar` & `fakemap-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:31:37.613739 fakemap-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-21 21:31:27.000000 fakemap-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-21 21:31:27.000000 fakemap-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-21 21:31:37.613739 fakemap-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 21:31:27.000000 fakemap-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:31:37.609739 fakemap-0.0.4/fakemap/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-21 21:31:27.000000 fakemap-0.0.4/fakemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-21 21:31:27.000000 fakemap-0.0.4/fakemap/fakemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-21 21:31:27.000000 fakemap-0.0.4/fakemap/foliummap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:31:37.609739 fakemap-0.0.4/fakemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-21 21:31:37.000000 fakemap-0.0.4/fakemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 21:31:37.000000 fakemap-0.0.4/fakemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 21:31:37.000000 fakemap-0.0.4/fakemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:31:37.000000 fakemap-0.0.4/fakemap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 21:31:37.000000 fakemap-0.0.4/fakemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 21:31:37.000000 fakemap-0.0.4/fakemap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 21:31:27.000000 fakemap-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-21 21:31:37.613739 fakemap-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-21 21:31:27.000000 fakemap-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:50.508988 fakemap-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 00:47:39.000000 fakemap-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 00:47:39.000000 fakemap-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-28 00:47:50.508988 fakemap-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-28 00:47:39.000000 fakemap-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:50.508988 fakemap-0.0.5/fakemap/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 00:47:39.000000 fakemap-0.0.5/fakemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-28 00:47:39.000000 fakemap-0.0.5/fakemap/fakemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-28 00:47:39.000000 fakemap-0.0.5/fakemap/foliummap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:50.508988 fakemap-0.0.5/fakemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 00:47:39.000000 fakemap-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 00:47:50.508988 fakemap-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-28 00:47:39.000000 fakemap-0.0.5/setup.py
```

### Comparing `fakemap-0.0.4/LICENSE` & `fakemap-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.4/PKG-INFO` & `fakemap-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakemap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/MattAGUT/fakemap
 Author: Matthew Gerloff
 Author-email: mapache.tn@gmail.com
 License: MIT license
 Keywords: fakemap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fakemap-0.0.4/README.md` & `fakemap-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.4/fakemap/foliummap.py` & `fakemap-0.0.5/fakemap/foliummap.py`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.4/fakemap.egg-info/PKG-INFO` & `fakemap-0.0.5/fakemap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakemap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/MattAGUT/fakemap
 Author: Matthew Gerloff
 Author-email: mapache.tn@gmail.com
 License: MIT license
 Keywords: fakemap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fakemap-0.0.4/setup.py` & `fakemap-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='fakemap',
     name='fakemap',
     packages=find_packages(include=['fakemap', 'fakemap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MattAGUT/fakemap',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

