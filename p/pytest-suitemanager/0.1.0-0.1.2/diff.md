# Comparing `tmp/pytest-suitemanager-0.1.0.tar.gz` & `tmp/pytest-suitemanager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-suitemanager-0.1.0.tar", last modified: Fri Apr 28 06:36:58 2023, max compression
+gzip compressed data, was "pytest-suitemanager-0.1.2.tar", last modified: Fri Apr 28 07:39:52 2023, max compression
```

## Comparing `pytest-suitemanager-0.1.0.tar` & `pytest-suitemanager-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 06:36:58.882386 pytest-suitemanager-0.1.0/
--rw-rw-rw-   0        0        0     1486 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       97 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3309 2023-04-28 06:36:58.882386 pytest-suitemanager-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 06:36:58.881376 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/
--rw-rw-rw-   0        0        0     3309 2023-04-28 06:36:58.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-04-28 06:36:58.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 06:36:58.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-28 06:36:58.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 06:36:58.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 06:36:58.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1210 2023-04-28 06:33:34.000000 pytest-suitemanager-0.1.0/pytest_suitemanager.py
--rw-rw-rw-   0        0        0       42 2023-04-28 06:36:58.882386 pytest-suitemanager-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:39:52.751832 pytest-suitemanager-0.1.2/
+-rw-rw-rw-   0        0        0     1486 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       97 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3309 2023-04-28 07:39:52.751832 pytest-suitemanager-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 07:39:52.750821 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/
+-rw-rw-rw-   0        0        0     3309 2023-04-28 07:39:52.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-28 07:39:52.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:39:52.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-28 07:39:52.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 07:39:52.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 07:39:52.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1211 2023-04-28 07:26:26.000000 pytest-suitemanager-0.1.2/pytest_suitemanager.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:39:52.752830 pytest-suitemanager-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-04-28 07:34:10.000000 pytest-suitemanager-0.1.2/setup.py
```

### Comparing `pytest-suitemanager-0.1.0/LICENSE` & `pytest-suitemanager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-suitemanager-0.1.0/PKG-INFO` & `pytest-suitemanager-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-suitemanager
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/mf.liang/pytest-suitemanager
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Maintainer: mf.liang
 Maintainer-email: mf.liang@outlook.com
 License: BSD-3
```

### Comparing `pytest-suitemanager-0.1.0/README.rst` & `pytest-suitemanager-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-suitemanager-0.1.0/pytest_suitemanager.egg-info/PKG-INFO` & `pytest-suitemanager-0.1.2/pytest_suitemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-suitemanager
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/mf.liang/pytest-suitemanager
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Maintainer: mf.liang
 Maintainer-email: mf.liang@outlook.com
 License: BSD-3
```

### Comparing `pytest-suitemanager-0.1.0/pytest_suitemanager.py` & `pytest-suitemanager-0.1.2/pytest_suitemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from typing import Text, Dict
 
 import pytest
 import yaml
 from _pytest.main import Session
 
-from utils import run_testsuites
+from .utils import run_testsuites
 
 
 def pytest_addoption(parser):
     """
     给pytest增加 自定义 命令行解析参数
     """
     group = parser.getgroup('suitemanager')
```

### Comparing `pytest-suitemanager-0.1.0/setup.py` & `pytest-suitemanager-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-suitemanager',
-    version='0.1.0',
+    version='0.1.2',
     author='mf.liang',
     author_email='mf.liang@outlook.com',
     maintainer='mf.liang',
     maintainer_email='mf.liang@outlook.com',
     license='BSD-3',
     url='https://github.com/mf.liang/pytest-suitemanager',
     description='A simple plugin to use with pytest',
```

