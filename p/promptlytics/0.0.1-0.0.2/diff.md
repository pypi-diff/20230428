# Comparing `tmp/promptlytics-0.0.1.tar.gz` & `tmp/promptlytics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlytics-0.0.1.tar", last modified: Fri Apr 28 01:28:21 2023, max compression
+gzip compressed data, was "promptlytics-0.0.2.tar", last modified: Fri Apr 28 20:01:24 2023, max compression
```

## Comparing `promptlytics-0.0.1.tar` & `promptlytics-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 scott      (501) staff       (20)        0 2023-04-28 01:28:21.642893 promptlytics-0.0.1/
--rw-r--r--   0 scott      (501) staff       (20)      528 2023-04-28 00:37:28.000000 promptlytics-0.0.1/LICENSE
--rw-r--r--   0 scott      (501) staff       (20)     1078 2023-04-28 01:28:21.642778 promptlytics-0.0.1/PKG-INFO
--rw-r--r--   0 scott      (501) staff       (20)      768 2023-04-28 01:24:50.000000 promptlytics-0.0.1/README.md
-drwxr-xr-x   0 scott      (501) staff       (20)        0 2023-04-28 01:28:21.641951 promptlytics-0.0.1/promptlytics/
--rw-r--r--   0 scott      (501) staff       (20)       37 2023-04-28 00:15:27.000000 promptlytics-0.0.1/promptlytics/__init__.py
--rw-r--r--   0 scott      (501) staff       (20)     2966 2023-04-26 20:48:28.000000 promptlytics-0.0.1/promptlytics/promptlytics.py
-drwxr-xr-x   0 scott      (501) staff       (20)        0 2023-04-28 01:28:21.642639 promptlytics-0.0.1/promptlytics.egg-info/
--rw-r--r--   0 scott      (501) staff       (20)     1078 2023-04-28 01:28:21.000000 promptlytics-0.0.1/promptlytics.egg-info/PKG-INFO
--rw-r--r--   0 scott      (501) staff       (20)      259 2023-04-28 01:28:21.000000 promptlytics-0.0.1/promptlytics.egg-info/SOURCES.txt
--rw-r--r--   0 scott      (501) staff       (20)        1 2023-04-28 01:28:21.000000 promptlytics-0.0.1/promptlytics.egg-info/dependency_links.txt
--rw-r--r--   0 scott      (501) staff       (20)        9 2023-04-28 01:28:21.000000 promptlytics-0.0.1/promptlytics.egg-info/requires.txt
--rw-r--r--   0 scott      (501) staff       (20)       13 2023-04-28 01:28:21.000000 promptlytics-0.0.1/promptlytics.egg-info/top_level.txt
--rw-r--r--   0 scott      (501) staff       (20)       38 2023-04-28 01:28:21.642934 promptlytics-0.0.1/setup.cfg
--rw-r--r--   0 scott      (501) staff       (20)      761 2023-04-28 00:32:55.000000 promptlytics-0.0.1/setup.py
+drwxr-xr-x   0 scott      (501) staff       (20)        0 2023-04-28 20:01:24.265070 promptlytics-0.0.2/
+-rw-r--r--   0 scott      (501) staff       (20)      528 2023-04-28 00:37:28.000000 promptlytics-0.0.2/LICENSE
+-rw-r--r--   0 scott      (501) staff       (20)     1078 2023-04-28 20:01:24.264948 promptlytics-0.0.2/PKG-INFO
+-rw-r--r--   0 scott      (501) staff       (20)      768 2023-04-28 01:24:50.000000 promptlytics-0.0.2/README.md
+drwxr-xr-x   0 scott      (501) staff       (20)        0 2023-04-28 20:01:24.264155 promptlytics-0.0.2/promptlytics/
+-rw-r--r--   0 scott      (501) staff       (20)       38 2023-04-28 19:53:45.000000 promptlytics-0.0.2/promptlytics/__init__.py
+-rw-r--r--   0 scott      (501) staff       (20)     2966 2023-04-26 20:48:28.000000 promptlytics-0.0.2/promptlytics/promptlytics.py
+drwxr-xr-x   0 scott      (501) staff       (20)        0 2023-04-28 20:01:24.264800 promptlytics-0.0.2/promptlytics.egg-info/
+-rw-r--r--   0 scott      (501) staff       (20)     1078 2023-04-28 20:01:24.000000 promptlytics-0.0.2/promptlytics.egg-info/PKG-INFO
+-rw-r--r--   0 scott      (501) staff       (20)      259 2023-04-28 20:01:24.000000 promptlytics-0.0.2/promptlytics.egg-info/SOURCES.txt
+-rw-r--r--   0 scott      (501) staff       (20)        1 2023-04-28 20:01:24.000000 promptlytics-0.0.2/promptlytics.egg-info/dependency_links.txt
+-rw-r--r--   0 scott      (501) staff       (20)        9 2023-04-28 20:01:24.000000 promptlytics-0.0.2/promptlytics.egg-info/requires.txt
+-rw-r--r--   0 scott      (501) staff       (20)       13 2023-04-28 20:01:24.000000 promptlytics-0.0.2/promptlytics.egg-info/top_level.txt
+-rw-r--r--   0 scott      (501) staff       (20)       38 2023-04-28 20:01:24.265168 promptlytics-0.0.2/setup.cfg
+-rw-r--r--   0 scott      (501) staff       (20)      761 2023-04-28 19:58:53.000000 promptlytics-0.0.2/setup.py
```

### Comparing `promptlytics-0.0.1/LICENSE` & `promptlytics-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlytics-0.0.1/PKG-INFO` & `promptlytics-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlytics
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for Promptlytics
 Home-page: https://www.promptlytics.co
 Author: Promptlytics (Scott Cilento)
 Author-email: scott@promptlytics.co
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `promptlytics-0.0.1/README.md` & `promptlytics-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `promptlytics-0.0.1/promptlytics/promptlytics.py` & `promptlytics-0.0.2/promptlytics/promptlytics.py`

 * *Files identical despite different names*

### Comparing `promptlytics-0.0.1/promptlytics.egg-info/PKG-INFO` & `promptlytics-0.0.2/promptlytics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlytics
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for Promptlytics
 Home-page: https://www.promptlytics.co
 Author: Promptlytics (Scott Cilento)
 Author-email: scott@promptlytics.co
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `promptlytics-0.0.1/setup.py` & `promptlytics-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python wrapper for Promptlytics'
 LONG_DESCRIPTION = 'Promptlytics helps you find the best prompts for your use case'
 
 # Setting up
 setup(
     name="promptlytics",
     version=VERSION,
```

