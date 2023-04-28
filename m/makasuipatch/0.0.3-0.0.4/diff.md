# Comparing `tmp/makasuipatch-0.0.3.tar.gz` & `tmp/makasuipatch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makasuipatch-0.0.3.tar", last modified: Fri Apr 28 08:39:15 2023, max compression
+gzip compressed data, was "makasuipatch-0.0.4.tar", last modified: Fri Apr 28 09:12:34 2023, max compression
```

## Comparing `makasuipatch-0.0.3.tar` & `makasuipatch-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 08:39:15.175450 makasuipatch-0.0.3/
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     1068 2023-04-28 07:50:18.000000 makasuipatch-0.0.3/LICENSE
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      694 2023-04-28 08:39:15.175450 makasuipatch-0.0.3/PKG-INFO
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      186 2023-04-28 08:16:23.000000 makasuipatch-0.0.3/README.md
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      617 2023-04-28 08:39:05.000000 makasuipatch-0.0.3/pyproject.toml
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)       38 2023-04-28 08:39:15.175450 makasuipatch-0.0.3/setup.cfg
-drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 08:39:15.175450 makasuipatch-0.0.3/src/
-drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 08:39:15.175450 makasuipatch-0.0.3/src/makasuipatch/
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      790 2023-04-28 07:26:15.000000 makasuipatch-0.0.3/src/makasuipatch/__init__.py
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     2503 2023-04-28 07:47:41.000000 makasuipatch-0.0.3/src/makasuipatch/apps.py
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     2801 2023-04-28 07:26:15.000000 makasuipatch-0.0.3/src/makasuipatch/decode_simplepro_file.py
-drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 08:39:15.175450 makasuipatch-0.0.3/src/makasuipatch.egg-info/
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      694 2023-04-28 08:39:15.000000 makasuipatch-0.0.3/src/makasuipatch.egg-info/PKG-INFO
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      327 2023-04-28 08:39:15.000000 makasuipatch-0.0.3/src/makasuipatch.egg-info/SOURCES.txt
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)        1 2023-04-28 08:39:15.000000 makasuipatch-0.0.3/src/makasuipatch.egg-info/dependency_links.txt
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)       10 2023-04-28 08:39:15.000000 makasuipatch-0.0.3/src/makasuipatch.egg-info/requires.txt
--rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)       13 2023-04-28 08:39:15.000000 makasuipatch-0.0.3/src/makasuipatch.egg-info/top_level.txt
+drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 09:12:34.516924 makasuipatch-0.0.4/
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     1068 2023-04-28 07:50:18.000000 makasuipatch-0.0.4/LICENSE
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     1213 2023-04-28 09:12:34.516924 makasuipatch-0.0.4/PKG-INFO
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      663 2023-04-28 09:10:55.000000 makasuipatch-0.0.4/README.md
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      659 2023-04-28 09:12:19.000000 makasuipatch-0.0.4/pyproject.toml
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)       38 2023-04-28 09:12:34.516924 makasuipatch-0.0.4/setup.cfg
+drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 09:12:34.516924 makasuipatch-0.0.4/src/
+drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 09:12:34.516924 makasuipatch-0.0.4/src/makasuipatch/
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      790 2023-04-28 07:26:15.000000 makasuipatch-0.0.4/src/makasuipatch/__init__.py
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     2503 2023-04-28 07:47:41.000000 makasuipatch-0.0.4/src/makasuipatch/apps.py
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     2801 2023-04-28 07:26:15.000000 makasuipatch-0.0.4/src/makasuipatch/decode_simplepro_file.py
+drwxr-xr-x   0 izhangxm  (1000) izhangxm  (1000)        0 2023-04-28 09:12:34.516924 makasuipatch-0.0.4/src/makasuipatch.egg-info/
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)     1213 2023-04-28 09:12:34.000000 makasuipatch-0.0.4/src/makasuipatch.egg-info/PKG-INFO
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)      327 2023-04-28 09:12:34.000000 makasuipatch-0.0.4/src/makasuipatch.egg-info/SOURCES.txt
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)        1 2023-04-28 09:12:34.000000 makasuipatch-0.0.4/src/makasuipatch.egg-info/dependency_links.txt
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)       10 2023-04-28 09:12:34.000000 makasuipatch-0.0.4/src/makasuipatch.egg-info/requires.txt
+-rw-r--r--   0 izhangxm  (1000) izhangxm  (1000)       13 2023-04-28 09:12:34.000000 makasuipatch-0.0.4/src/makasuipatch.egg-info/top_level.txt
```

### Comparing `makasuipatch-0.0.3/LICENSE` & `makasuipatch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `makasuipatch-0.0.3/pyproject.toml` & `makasuipatch-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "makasuipatch"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="makabaka", email="izhangxm@gmail.com" },
 ]
-description = "patch to simple ui pro package"
+description = "A patch to simple pro to make you activate it. Just used for learning."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "simplepro"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/izhangxm/makasuipatc"
-"Bug Tracker" = "https://github.com/izhangxm/makasuipatc/issues"
+"Homepage" = "https://github.com/izhangxm/makasuipatch"
+"Bug Tracker" = "https://github.com/izhangxm/makasuipatch/issues"
```

### Comparing `makasuipatch-0.0.3/src/makasuipatch/__init__.py` & `makasuipatch-0.0.4/src/makasuipatch/__init__.py`

 * *Files identical despite different names*

### Comparing `makasuipatch-0.0.3/src/makasuipatch/apps.py` & `makasuipatch-0.0.4/src/makasuipatch/apps.py`

 * *Files identical despite different names*

### Comparing `makasuipatch-0.0.3/src/makasuipatch/decode_simplepro_file.py` & `makasuipatch-0.0.4/src/makasuipatch/decode_simplepro_file.py`

 * *Files identical despite different names*

