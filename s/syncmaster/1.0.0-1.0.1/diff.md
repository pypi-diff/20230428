# Comparing `tmp/syncmaster-1.0.0.tar.gz` & `tmp/syncmaster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncmaster-1.0.0.tar", last modified: Mon Apr 17 17:15:22 2023, max compression
+gzip compressed data, was "syncmaster-1.0.1.tar", last modified: Fri Apr 28 10:15:46 2023, max compression
```

## Comparing `syncmaster-1.0.0.tar` & `syncmaster-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 17:15:22.672109 syncmaster-1.0.0/
--rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.0/LICENSE
--rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.0/MANIFEST.in
--rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-17 17:15:22.672109 syncmaster-1.0.0/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)     2410 2023-04-17 14:44:42.000000 syncmaster-1.0.0/README.md
--rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-04-17 17:15:06.000000 syncmaster-1.0.0/settings.ini
--rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-17 17:15:22.672109 syncmaster-1.0.0/setup.cfg
--rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.0/setup.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 17:15:22.672109 syncmaster-1.0.0/syncmaster/
--rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-04-17 17:13:49.000000 syncmaster-1.0.0/syncmaster/__init__.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     1918 2023-04-17 17:13:49.000000 syncmaster-1.0.0/syncmaster/_modidx.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2371 2023-04-17 17:13:49.000000 syncmaster-1.0.0/syncmaster/analysis.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     3529 2023-04-17 17:13:49.000000 syncmaster-1.0.0/syncmaster/device.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-17 17:15:22.672109 syncmaster-1.0.0/syncmaster.egg-info/
--rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-17 17:15:22.000000 syncmaster-1.0.0/syncmaster.egg-info/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-17 17:15:22.000000 syncmaster-1.0.0/syncmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 17:15:22.000000 syncmaster-1.0.0/syncmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-17 17:15:22.000000 syncmaster-1.0.0/syncmaster.egg-info/entry_points.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.0/syncmaster.egg-info/not-zip-safe
--rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-04-17 17:15:22.000000 syncmaster-1.0.0/syncmaster.egg-info/requires.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-17 17:15:22.000000 syncmaster-1.0.0/syncmaster.egg-info/top_level.txt
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-28 10:15:46.865980 syncmaster-1.0.1/
+-rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.1/LICENSE
+-rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.1/MANIFEST.in
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-28 10:15:46.865980 syncmaster-1.0.1/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2410 2023-04-17 17:49:29.000000 syncmaster-1.0.1/README.md
+-rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-04-28 10:14:01.000000 syncmaster-1.0.1/settings.ini
+-rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-28 10:15:46.865980 syncmaster-1.0.1/setup.cfg
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.1/setup.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-28 10:15:46.861981 syncmaster-1.0.1/syncmaster/
+-rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-04-17 17:49:26.000000 syncmaster-1.0.1/syncmaster/__init__.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     1918 2023-04-17 17:49:26.000000 syncmaster-1.0.1/syncmaster/_modidx.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2371 2023-04-17 17:49:26.000000 syncmaster-1.0.1/syncmaster/analysis.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3529 2023-04-17 17:49:26.000000 syncmaster-1.0.1/syncmaster/device.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-28 10:15:46.865980 syncmaster-1.0.1/syncmaster.egg-info/
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-28 10:15:46.000000 syncmaster-1.0.1/syncmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-28 10:15:46.000000 syncmaster-1.0.1/syncmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-28 10:15:46.000000 syncmaster-1.0.1/syncmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-28 10:15:46.000000 syncmaster-1.0.1/syncmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.1/syncmaster.egg-info/not-zip-safe
+-rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-04-28 10:15:46.000000 syncmaster-1.0.1/syncmaster.egg-info/requires.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-28 10:15:46.000000 syncmaster-1.0.1/syncmaster.egg-info/top_level.txt
```

### Comparing `syncmaster-1.0.0/LICENSE` & `syncmaster-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.0/PKG-INFO` & `syncmaster-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.0
+Version: 1.0.1
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `syncmaster-1.0.0/README.md` & `syncmaster-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.0/settings.ini` & `syncmaster-1.0.1/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = syncmaster
 lib_name = syncmaster
-version = 1.0.0
+version = 1.0.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = syncmaster
 nbs_path = nbs
 recursive = True
```

### Comparing `syncmaster-1.0.0/setup.py` & `syncmaster-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.0/syncmaster/_modidx.py` & `syncmaster-1.0.1/syncmaster/_modidx.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.0/syncmaster/analysis.py` & `syncmaster-1.0.1/syncmaster/analysis.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.0/syncmaster/device.py` & `syncmaster-1.0.1/syncmaster/device.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.0/syncmaster.egg-info/PKG-INFO` & `syncmaster-1.0.1/syncmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.0
+Version: 1.0.1
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

