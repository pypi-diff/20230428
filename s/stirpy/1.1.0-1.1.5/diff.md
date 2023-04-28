# Comparing `tmp/stirpy-1.1.0.tar.gz` & `tmp/stirpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\stirpy-1.1.0.tar", last modified: Fri Apr 28 16:41:08 2023, max compression
+gzip compressed data, was "dist\stirpy-1.1.5.tar", last modified: Fri Apr 28 16:43:39 2023, max compression
```

## Comparing `stirpy-1.1.0.tar` & `stirpy-1.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 16:41:08.242678 stirpy-1.1.0/
--rw-rw-rw-   0        0        0      821 2023-04-28 16:41:08.240678 stirpy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 16:41:08.242678 stirpy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-04-28 16:40:54.000000 stirpy-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:41:08.236678 stirpy-1.1.0/stirpy.egg-info/
--rw-rw-rw-   0        0        0      821 2023-04-28 16:41:08.000000 stirpy-1.1.0/stirpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-28 16:41:08.000000 stirpy-1.1.0/stirpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 16:41:08.000000 stirpy-1.1.0/stirpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-28 16:41:08.000000 stirpy-1.1.0/stirpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 16:41:08.000000 stirpy-1.1.0/stirpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 16:43:39.837275 stirpy-1.1.5/
+-rw-rw-rw-   0        0        0      821 2023-04-28 16:43:39.835275 stirpy-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 16:43:39.838276 stirpy-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1019 2023-04-28 16:43:25.000000 stirpy-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:43:39.832275 stirpy-1.1.5/stirpy.egg-info/
+-rw-rw-rw-   0        0        0      821 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/top_level.txt
```

### Comparing `stirpy-1.1.0/PKG-INFO` & `stirpy-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: stirpy
-Version: 1.1.0
+Version: 1.1.5
 Summary: A Powerful scientific strings-processing library called stipy
 Home-page: UNKNOWN
 Author: KhalidWalidAghrini
 Author-email: kwaaghrini@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `stirpy-1.1.0/setup.py` & `stirpy-1.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("stripy.py", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='stirpy',
-    version='1.1.0',
+    version='1.1.5',
     author='KhalidWalidAghrini',
     author_email='kwaaghrini@gmail.com',
     description='A Powerful scientific strings-processing library called stipy',
     packages=find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
@@ -22,12 +22,10 @@
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'nltk',
-        'afinn',
-        're',
-        'os'
+        'afinn'
     ],
 )
```

### Comparing `stirpy-1.1.0/stirpy.egg-info/PKG-INFO` & `stirpy-1.1.5/stirpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: stirpy
-Version: 1.1.0
+Version: 1.1.5
 Summary: A Powerful scientific strings-processing library called stipy
 Home-page: UNKNOWN
 Author: KhalidWalidAghrini
 Author-email: kwaaghrini@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

