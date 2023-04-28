# Comparing `tmp/CharacterAPI-0.1.1.tar.gz` & `tmp/CharacterAPI-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CharacterAPI-0.1.1.tar", last modified: Fri Apr 28 18:35:57 2023, max compression
+gzip compressed data, was "dist\CharacterAPI-0.1.3.tar", last modified: Fri Apr 28 18:59:04 2023, max compression
```

## Comparing `CharacterAPI-0.1.1.tar` & `CharacterAPI-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:35:57.827737 CharacterAPI-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-28 18:35:57.711878 CharacterAPI-0.1.1/CharacterAPI/
--rw-rw-rw-   0        0        0     4457 2023-04-28 17:13:01.000000 CharacterAPI-0.1.1/CharacterAPI/CharacterAI.py
--rw-rw-rw-   0        0        0     4850 2023-04-28 17:25:33.000000 CharacterAPI-0.1.1/CharacterAPI/CharacterAI_async.py
--rw-rw-rw-   0        0        0       66 2023-04-28 17:03:21.000000 CharacterAPI-0.1.1/CharacterAPI/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-27 15:21:32.000000 CharacterAPI-0.1.1/CharacterAPI/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:35:57.811732 CharacterAPI-0.1.1/CharacterAPI.egg-info/
--rw-rw-rw-   0        0        0      457 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 CharacterAPI-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      457 2023-04-28 18:35:57.819735 CharacterAPI-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 CharacterAPI-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 18:35:57.827737 CharacterAPI-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-04-28 18:35:17.000000 CharacterAPI-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:59:04.076184 CharacterAPI-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-04-28 18:59:03.990506 CharacterAPI-0.1.3/CharacterAPI/
+-rw-rw-rw-   0        0        0     4468 2023-04-28 18:58:01.000000 CharacterAPI-0.1.3/CharacterAPI/CharacterAI.py
+-rw-rw-rw-   0        0        0     4861 2023-04-28 18:58:06.000000 CharacterAPI-0.1.3/CharacterAPI/CharacterAI_async.py
+-rw-rw-rw-   0        0        0       65 2023-04-28 18:57:56.000000 CharacterAPI-0.1.3/CharacterAPI/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-27 15:21:32.000000 CharacterAPI-0.1.3/CharacterAPI/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:59:04.068194 CharacterAPI-0.1.3/CharacterAPI.egg-info/
+-rw-rw-rw-   0        0        0      457 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 CharacterAPI-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      457 2023-04-28 18:59:04.076184 CharacterAPI-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 CharacterAPI-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:59:04.076184 CharacterAPI-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-28 18:59:00.000000 CharacterAPI-0.1.3/setup.py
```

### Comparing `CharacterAPI-0.1.1/CharacterAPI/CharacterAI.py` & `CharacterAPI-0.1.3/CharacterAPI/CharacterAI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 import json
 import time
 
 from playwright.sync_api import sync_playwright
 
-from errors import *
+from CharacterAPI import errors
 
 __all__ = ['pyCAI']
 
 text = []
 page = None
 
 class pyCAI:
```

### Comparing `CharacterAPI-0.1.1/CharacterAPI/CharacterAI_async.py` & `CharacterAPI-0.1.3/CharacterAPI/CharacterAI_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 import asyncio
 import json
 import time
 
 from playwright.async_api import async_playwright
 
-from errors import *
+from CharacterAPI import errors
 
 __all__ = ['pyCAI']
 
 text = []
 page = None
 
 class pyCAI:
```

### Comparing `CharacterAPI-0.1.1/LICENSE` & `CharacterAPI-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CharacterAPI-0.1.1/setup.py` & `CharacterAPI-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='CharacterAPI',
-    version='0.1.1',
+    version='0.1.3',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/CharacterAPI',
     packages=find_packages(),
     install_requires=["playwright==1.32.1"],
```

