# Comparing `tmp/plotarchive-0.0.5.tar.gz` & `tmp/plotarchive-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plotarchive-0.0.5.tar", last modified: Tue Sep 15 23:20:39 2020, max compression
+gzip compressed data, was "dist/plotarchive-0.0.6.tar", last modified: Tue Sep 15 23:31:29 2020, max compression
```

## Comparing `plotarchive-0.0.5.tar` & `plotarchive-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:20:39.956298 plotarchive-0.0.5/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1555 2020-09-15 23:20:39.956298 plotarchive-0.0.5/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      824 2020-08-13 23:47:44.000000 plotarchive-0.0.5/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:20:39.956298 plotarchive-0.0.5/plotarchive/
--rw-rw-r--   0 chris     (1000) chris     (1000)       68 2020-08-13 22:52:29.000000 plotarchive-0.0.5/plotarchive/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:20:39.956298 plotarchive-0.0.5/plotarchive/src/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-08-13 19:40:12.000000 plotarchive-0.0.5/plotarchive/src/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1307 2020-09-15 23:18:04.000000 plotarchive-0.0.5/plotarchive/src/archive.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1182 2020-08-13 20:45:52.000000 plotarchive-0.0.5/plotarchive/src/files.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      337 2020-08-13 22:52:29.000000 plotarchive-0.0.5/plotarchive/src/unarchive.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:20:39.956298 plotarchive-0.0.5/plotarchive.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1555 2020-09-15 23:20:39.000000 plotarchive-0.0.5/plotarchive.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2020-09-15 23:20:39.000000 plotarchive-0.0.5/plotarchive.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2020-09-15 23:20:39.000000 plotarchive-0.0.5/plotarchive.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       12 2020-09-15 23:20:39.000000 plotarchive-0.0.5/plotarchive.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2020-09-15 23:20:39.956298 plotarchive-0.0.5/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      721 2020-09-15 23:19:25.000000 plotarchive-0.0.5/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:31:29.144407 plotarchive-0.0.6/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1555 2020-09-15 23:31:29.140407 plotarchive-0.0.6/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      824 2020-08-13 23:47:44.000000 plotarchive-0.0.6/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:31:29.140407 plotarchive-0.0.6/plotarchive/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       68 2020-08-13 22:52:29.000000 plotarchive-0.0.6/plotarchive/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:31:29.140407 plotarchive-0.0.6/plotarchive/src/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-08-13 19:40:12.000000 plotarchive-0.0.6/plotarchive/src/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1306 2020-09-15 23:30:08.000000 plotarchive-0.0.6/plotarchive/src/archive.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1182 2020-08-13 20:45:52.000000 plotarchive-0.0.6/plotarchive/src/files.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      337 2020-08-13 22:52:29.000000 plotarchive-0.0.6/plotarchive/src/unarchive.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-09-15 23:31:29.140407 plotarchive-0.0.6/plotarchive.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1555 2020-09-15 23:31:29.000000 plotarchive-0.0.6/plotarchive.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2020-09-15 23:31:29.000000 plotarchive-0.0.6/plotarchive.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2020-09-15 23:31:29.000000 plotarchive-0.0.6/plotarchive.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       12 2020-09-15 23:31:29.000000 plotarchive-0.0.6/plotarchive.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2020-09-15 23:31:29.144407 plotarchive-0.0.6/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      721 2020-09-15 23:31:17.000000 plotarchive-0.0.6/setup.py
```

### Comparing `plotarchive-0.0.5/PKG-INFO` & `plotarchive-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotarchive
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy method to save code and data that generates scientific plots.
 Home-page: https://github.com/buswinka/plotarchive
 Author: Chris Buswinka
 Author-email: buswinka@gmail.com
 License: UNKNOWN
 Description: # plotarchive
         Plotarchive is a simple package which aims to assist plotters remeber what code created which figure.
```

### Comparing `plotarchive-0.0.5/README.md` & `plotarchive-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `plotarchive-0.0.5/plotarchive/src/archive.py` & `plotarchive-0.0.6/plotarchive/src/archive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from numpy import ndarray
-import torch.tensor
+from torch import Tensor
 import dill
 import inspect
 
 from . import files
 
 
 """
@@ -32,15 +32,15 @@
 
             python_files = files.create_file_dict()
 
             args_name = inspect.getfullargspec(func)[0]
             args_dict = dict(zip(args_name, args))
 
             for i, arg in enumerate(args):
-                if not isinstance(arg, (int, float, bool, bytes, str, list, tuple, dict, ndarray, torch.tensor)):
+                if not isinstance(arg, (int, float, bool, bytes, str, list, tuple, dict, ndarray, Tensor)):
                     raise TypeError(f'Unrecognized argument type for {args_name[i]}:{type(arg)}')
 
             data = {'args': args_dict, 'files': python_files, 'func': func}
             dill.dump(data, open(self.filename, 'wb'))
 
             return func(*args, **kwargs)
         return wrapper
```

### Comparing `plotarchive-0.0.5/plotarchive/src/files.py` & `plotarchive-0.0.6/plotarchive/src/files.py`

 * *Files identical despite different names*

### Comparing `plotarchive-0.0.5/plotarchive.egg-info/PKG-INFO` & `plotarchive-0.0.6/plotarchive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotarchive
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy method to save code and data that generates scientific plots.
 Home-page: https://github.com/buswinka/plotarchive
 Author: Chris Buswinka
 Author-email: buswinka@gmail.com
 License: UNKNOWN
 Description: # plotarchive
         Plotarchive is a simple package which aims to assist plotters remeber what code created which figure.
```

### Comparing `plotarchive-0.0.5/setup.py` & `plotarchive-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotarchive", # Replace with your own username
-    version="0.0.5",
+    version="0.0.6",
     author="Chris Buswinka",
     author_email="buswinka@gmail.com",
     description="An easy method to save code and data that generates scientific plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/buswinka/plotarchive",
     packages=setuptools.find_packages(),
```

