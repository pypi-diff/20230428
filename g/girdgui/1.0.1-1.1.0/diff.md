# Comparing `tmp/girdgui-1.0.1.tar.gz` & `tmp/girdgui-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girdgui-1.0.1.tar", last modified: Mon Apr 24 12:17:11 2023, max compression
+gzip compressed data, was "girdgui-1.1.0.tar", last modified: Fri Apr 28 14:32:32 2023, max compression
```

## Comparing `girdgui-1.0.1.tar` & `girdgui-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.780628 girdgui-1.0.1/
--rw-rw-rw-   0        0        0     1192 2023-04-24 12:17:11.774630 girdgui-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 12:17:11.780628 girdgui-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1401 2023-04-24 12:17:06.000000 girdgui-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.736628 girdgui-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.740627 girdgui-1.0.1/src/girdgui/
--rw-rw-rw-   0        0        0      932 2023-03-25 13:38:07.000000 girdgui-1.0.1/src/girdgui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.771628 girdgui-1.0.1/src/girdgui.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:32.560595 girdgui-1.1.0/
+-rw-rw-rw-   0        0        0     1192 2023-04-28 14:32:32.560595 girdgui-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:32:32.560595 girdgui-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-04-28 14:31:15.000000 girdgui-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:32.546595 girdgui-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:32.549595 girdgui-1.1.0/src/girdgui/
+-rw-rw-rw-   0        0        0     3181 2023-04-28 14:27:17.000000 girdgui-1.1.0/src/girdgui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:32.557595 girdgui-1.1.0/src/girdgui.egg-info/
+-rw-rw-rw-   0        0        0     1192 2023-04-28 14:32:32.000000 girdgui-1.1.0/src/girdgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-28 14:32:32.000000 girdgui-1.1.0/src/girdgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:32:32.000000 girdgui-1.1.0/src/girdgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 14:32:32.000000 girdgui-1.1.0/src/girdgui.egg-info/top_level.txt
```

### Comparing `girdgui-1.0.1/PKG-INFO` & `girdgui-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girdgui
-Version: 1.0.1
+Version: 1.1.0
 Summary: 作者：李青泽
 Home-page: 
 Author: DogEgg
 Author-email: 2408311660@qq.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `girdgui-1.0.1/setup.py` & `girdgui-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from setuptools import setup, find_packages
 
 setup(
     name='girdgui',
-    version="1.0.1",
+    version="1.1.0",
     url='',
     author='DogEgg',
     author_email='2408311660@qq.com',
     description=('作者：李青泽'),
     license='BSD',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
```

### Comparing `girdgui-1.0.1/src/girdgui.egg-info/PKG-INFO` & `girdgui-1.1.0/src/girdgui.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girdgui
-Version: 1.0.1
+Version: 1.1.0
 Summary: 作者：李青泽
 Home-page: 
 Author: DogEgg
 Author-email: 2408311660@qq.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

