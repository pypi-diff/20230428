# Comparing `tmp/mrdoxmrgt-0.0.9.tar.gz` & `tmp/mrdoxmrgt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.9.tar", last modified: Fri Apr 28 18:42:25 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.1.1.tar", last modified: Fri Apr 28 18:52:53 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.9.tar` & `mrdoxmrgt-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-04-14 09:24:50.000000 mrdoxmrgt-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      800 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-14 09:24:50.000000 mrdoxmrgt-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/
--rw-rw-rw-   0        0        0        0 2023-04-28 10:15:20.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     3792 2023-04-28 10:21:08.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/main.py
--rw-rw-rw-   0        0        0    15122 2023-04-28 10:15:42.000000 mrdoxmrgt-0.0.9/mrdoxmrgt/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      800 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 18:42:26.000000 mrdoxmrgt-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1252 2023-04-28 10:22:02.000000 mrdoxmrgt-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt/
+-rw-rw-rw-   0        0        0        0 2023-04-28 10:15:20.000000 mrdoxmrgt-0.1.1/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     3792 2023-04-28 10:21:08.000000 mrdoxmrgt-0.1.1/mrdoxmrgt/main.py
+-rw-rw-rw-   0        0        0    15122 2023-04-28 10:15:42.000000 mrdoxmrgt-0.1.1/mrdoxmrgt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:52:54.000000 mrdoxmrgt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-04-28 18:52:06.000000 mrdoxmrgt-0.1.1/setup.py
```

### Comparing `mrdoxmrgt-0.0.9/LICENSE` & `mrdoxmrgt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.9/PKG-INFO` & `mrdoxmrgt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.9
+Version: 0.1.1
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.9/mrdoxmrgt/main.py` & `mrdoxmrgt-0.1.1/mrdoxmrgt/main.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.9/mrdoxmrgt/utils.py` & `mrdoxmrgt-0.1.1/mrdoxmrgt/utils.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.9/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.1.1/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.9
+Version: 0.1.1
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.9/setup.py` & `mrdoxmrgt-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.9",
+    version="0.1.1",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/gtf',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
```

