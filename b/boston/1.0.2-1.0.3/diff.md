# Comparing `tmp/boston-1.0.2.tar.gz` & `tmp/boston-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boston-1.0.2.tar", last modified: Thu Apr 27 15:31:01 2023, max compression
+gzip compressed data, was "boston-1.0.3.tar", last modified: Thu Apr 27 15:38:31 2023, max compression
```

## Comparing `boston-1.0.2.tar` & `boston-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:31:01.372792 boston-1.0.2/
--rw-rw-rw-   0        0        0      451 2023-04-27 15:31:01.371797 boston-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 15:31:01.335787 boston-1.0.2/boston/
--rw-rw-rw-   0        0        0      338 2023-04-27 15:30:45.000000 boston-1.0.2/boston/__init__.py
--rw-rw-rw-   0        0        0      338 2023-04-27 15:13:35.000000 boston-1.0.2/boston/boston.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:31:01.368786 boston-1.0.2/boston.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-27 15:31:01.000000 boston-1.0.2/boston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:31:01.373787 boston-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-04-27 15:30:48.000000 boston-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:38:31.470567 boston-1.0.3/
+-rw-rw-rw-   0        0        0      451 2023-04-27 15:38:31.468568 boston-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 15:38:31.436579 boston-1.0.3/boston/
+-rw-rw-rw-   0        0        0      338 2023-04-27 15:36:50.000000 boston-1.0.3/boston/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-04-27 15:37:58.000000 boston-1.0.3/boston/house.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:38:31.465564 boston-1.0.3/boston.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-27 15:38:30.000000 boston-1.0.3/boston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-27 15:38:31.000000 boston-1.0.3/boston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:38:30.000000 boston-1.0.3/boston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 15:38:30.000000 boston-1.0.3/boston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 15:38:30.000000 boston-1.0.3/boston.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 15:38:31.470567 boston-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-04-27 15:36:53.000000 boston-1.0.3/setup.py
```

### Comparing `boston-1.0.2/setup.py` & `boston-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="boston", # Replace with your own username
-    version="1.0.2",
+    version="1.0.3",
     author="julmubm",
     author_email="dltpdn@gmail.com",
     description="loading boston housing price dataset like sklearn.datasets.load_boston() style.",
     long_description_content_type="text/markdown",
     url="https://github.com/dltpdn/boston",
     install_requires=['pandas'],
     packages=setuptools.find_packages(),
```

