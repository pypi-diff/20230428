# Comparing `tmp/pytest-suitemanager-0.1.3.tar.gz` & `tmp/pytest-suitemanager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-suitemanager-0.1.3.tar", last modified: Fri Apr 28 07:47:19 2023, max compression
+gzip compressed data, was "pytest-suitemanager-0.1.4.tar", last modified: Fri Apr 28 07:56:28 2023, max compression
```

## Comparing `pytest-suitemanager-0.1.3.tar` & `pytest-suitemanager-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:47:19.568873 pytest-suitemanager-0.1.3/
--rw-rw-rw-   0        0        0     1486 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       97 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3309 2023-04-28 07:47:19.568873 pytest-suitemanager-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 07:47:19.566765 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/
--rw-rw-rw-   0        0        0     3309 2023-04-28 07:47:19.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-04-28 07:47:19.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:47:19.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-28 07:47:19.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 07:47:19.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 07:47:19.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1107 2023-04-28 07:47:12.000000 pytest-suitemanager-0.1.3/pytest_suitemanager.py
--rw-rw-rw-   0        0        0       42 2023-04-28 07:47:19.568873 pytest-suitemanager-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-04-28 07:47:12.000000 pytest-suitemanager-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:56:28.821399 pytest-suitemanager-0.1.4/
+-rw-rw-rw-   0        0        0     1486 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       97 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3309 2023-04-28 07:56:28.821399 pytest-suitemanager-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-04-27 09:52:46.000000 pytest-suitemanager-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 07:56:28.820400 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/
+-rw-rw-rw-   0        0        0     3309 2023-04-28 07:56:28.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-28 07:56:28.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:56:28.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-28 07:56:28.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 07:56:28.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 07:56:28.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1170 2023-04-28 07:55:38.000000 pytest-suitemanager-0.1.4/pytest_suitemanager.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:56:28.821399 pytest-suitemanager-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-04-28 07:56:25.000000 pytest-suitemanager-0.1.4/setup.py
```

### Comparing `pytest-suitemanager-0.1.3/LICENSE` & `pytest-suitemanager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-suitemanager-0.1.3/PKG-INFO` & `pytest-suitemanager-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-suitemanager
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/mf.liang/pytest-suitemanager
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Maintainer: mf.liang
 Maintainer-email: mf.liang@outlook.com
 License: BSD-3
```

### Comparing `pytest-suitemanager-0.1.3/README.rst` & `pytest-suitemanager-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-suitemanager-0.1.3/pytest_suitemanager.egg-info/PKG-INFO` & `pytest-suitemanager-0.1.4/pytest_suitemanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-suitemanager
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/mf.liang/pytest-suitemanager
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Maintainer: mf.liang
 Maintainer-email: mf.liang@outlook.com
 License: BSD-3
```

### Comparing `pytest-suitemanager-0.1.3/pytest_suitemanager.py` & `pytest-suitemanager-0.1.4/pytest_suitemanager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 
+import logging
+from typing import Text, Dict
 import pytest
+import yaml
 from _pytest.main import Session
-from .utils import run_testsuites
+
+from utils import run_testsuites
 
 
 def pytest_addoption(parser):
     """
     给pytest增加 自定义 命令行解析参数
     """
     group = parser.getgroup('suitemanager')
@@ -34,12 +38,13 @@
     :param session:
     :return:
     """
     option = vars(session.config.option)
     suite_path = option.get('suite_path')
     file_or_dir = option.get('file_or_dir')
     root_path = str(session.path)
-
     # 测试用例加载
     if suite_path and not file_or_dir:
         scenario_list = run_testsuites(root_path, suite_path)
         session.config.args = scenario_list
+
+
```

### Comparing `pytest-suitemanager-0.1.3/setup.py` & `pytest-suitemanager-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import os
-import codecs
-from setuptools import setup
-
-
-def read(fname):
-    file_path = os.path.join(os.path.dirname(__file__), fname)
-    return codecs.open(file_path, encoding='utf-8').read()
-
-
-setup(
-    name='pytest-suitemanager',
-    version='0.1.3',
-    author='mf.liang',
-    author_email='mf.liang@outlook.com',
-    maintainer='mf.liang',
-    maintainer_email='mf.liang@outlook.com',
-    license='BSD-3',
-    url='https://github.com/mf.liang/pytest-suitemanager',
-    description='A simple plugin to use with pytest',
-    long_description=read('README.rst'),
-    py_modules=['pytest_suitemanager'],
-    python_requires='>=3.5',
-    install_requires=['pytest>=3.5.0'],
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Framework :: Pytest',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Testing',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Operating System :: OS Independent',
-        'License :: OSI Approved :: BSD License',
-    ],
-    entry_points={
-        'pytest11': [
-            'suitemanager = pytest_suitemanager',
-        ],
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import os
+import codecs
+from setuptools import setup
+
+
+def read(fname):
+    file_path = os.path.join(os.path.dirname(__file__), fname)
+    return codecs.open(file_path, encoding='utf-8').read()
+
+
+setup(
+    name='pytest-suitemanager',
+    version='0.1.4',
+    author='mf.liang',
+    author_email='mf.liang@outlook.com',
+    maintainer='mf.liang',
+    maintainer_email='mf.liang@outlook.com',
+    license='BSD-3',
+    url='https://github.com/mf.liang/pytest-suitemanager',
+    description='A simple plugin to use with pytest',
+    long_description=read('README.rst'),
+    py_modules=['pytest_suitemanager'],
+    python_requires='>=3.5',
+    install_requires=['pytest>=3.5.0'],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Framework :: Pytest',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Testing',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
+        'Operating System :: OS Independent',
+        'License :: OSI Approved :: BSD License',
+    ],
+    entry_points={
+        'pytest11': [
+            'suitemanager = pytest_suitemanager',
+        ],
+    },
+)
```

