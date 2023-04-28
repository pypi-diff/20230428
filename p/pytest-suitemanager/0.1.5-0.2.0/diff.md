# Comparing `tmp/pytest-suitemanager-0.1.5.tar.gz` & `tmp/pytest-suitemanager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-suitemanager-0.1.5.tar", last modified: Fri Apr 28 08:06:09 2023, max compression
+gzip compressed data, was "pytest-suitemanager-0.2.0.tar", last modified: Fri Apr 28 09:56:01 2023, max compression
```

## Comparing `pytest-suitemanager-0.1.5.tar` & `pytest-suitemanager-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:06:09.872193 pytest-suitemanager-0.1.5/
--rw-rw-rw-   0        0        0     1486 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       97 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3309 2023-04-28 08:06:09.871193 pytest-suitemanager-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 08:06:09.870193 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/
--rw-rw-rw-   0        0        0     3309 2023-04-28 08:06:09.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-04-28 08:06:09.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:06:09.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-28 08:06:09.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 08:06:09.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 08:06:09.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-04-28 08:05:10.000000 pytest-suitemanager-0.1.5/pytest_suitemanager.py
--rw-rw-rw-   0        0        0       42 2023-04-28 08:06:09.872193 pytest-suitemanager-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-04-28 08:06:06.000000 pytest-suitemanager-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:56:01.823460 pytest-suitemanager-0.2.0/
+-rw-rw-rw-   0        0        0     1486 2023-04-27 09:52:46.000000 pytest-suitemanager-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       97 2023-04-27 09:52:46.000000 pytest-suitemanager-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3309 2023-04-28 09:56:01.822468 pytest-suitemanager-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-04-27 09:52:46.000000 pytest-suitemanager-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 09:56:01.820452 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/
+-rw-rw-rw-   0        0        0     3309 2023-04-28 09:56:01.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-28 09:56:01.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:56:01.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-28 09:56:01.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 09:56:01.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 09:56:01.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3525 2023-04-28 09:30:39.000000 pytest-suitemanager-0.2.0/pytest_suitemanager.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:56:01.823460 pytest-suitemanager-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-04-28 09:55:54.000000 pytest-suitemanager-0.2.0/setup.py
```

### Comparing `pytest-suitemanager-0.1.5/LICENSE` & `pytest-suitemanager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-suitemanager-0.1.5/PKG-INFO` & `pytest-suitemanager-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-suitemanager
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/mf.liang/pytest-suitemanager
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Maintainer: mf.liang
 Maintainer-email: mf.liang@outlook.com
 License: BSD-3
```

### Comparing `pytest-suitemanager-0.1.5/README.rst` & `pytest-suitemanager-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-suitemanager-0.1.5/pytest_suitemanager.egg-info/PKG-INFO` & `pytest-suitemanager-0.2.0/pytest_suitemanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-suitemanager
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/mf.liang/pytest-suitemanager
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Maintainer: mf.liang
 Maintainer-email: mf.liang@outlook.com
 License: BSD-3
```

### Comparing `pytest-suitemanager-0.1.5/setup.py` & `pytest-suitemanager-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-suitemanager',
-    version='0.1.5',
+    version='0.2.0',
     author='mf.liang',
     author_email='mf.liang@outlook.com',
     maintainer='mf.liang',
     maintainer_email='mf.liang@outlook.com',
     license='BSD-3',
     url='https://github.com/mf.liang/pytest-suitemanager',
     description='A simple plugin to use with pytest',
```

