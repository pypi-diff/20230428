# Comparing `tmp/Chinese-webtext-spider-1.0.0.tar.gz` & `tmp/Chinese-webtext-spider-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chinese-webtext-spider-1.0.0.tar", last modified: Fri Apr 28 09:02:26 2023, max compression
+gzip compressed data, was "Chinese-webtext-spider-1.0.1.tar", last modified: Fri Apr 28 09:31:27 2023, max compression
```

## Comparing `Chinese-webtext-spider-1.0.0.tar` & `Chinese-webtext-spider-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:02:26.539898 Chinese-webtext-spider-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-28 09:02:26.535393 Chinese-webtext-spider-1.0.0/Chinese_webtext_spider.egg-info/
--rw-rw-rw-   0        0        0      421 2023-04-28 09:02:25.000000 Chinese-webtext-spider-1.0.0/Chinese_webtext_spider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-28 09:02:25.000000 Chinese-webtext-spider-1.0.0/Chinese_webtext_spider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:02:25.000000 Chinese-webtext-spider-1.0.0/Chinese_webtext_spider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-28 09:02:25.000000 Chinese-webtext-spider-1.0.0/Chinese_webtext_spider.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 09:02:25.000000 Chinese-webtext-spider-1.0.0/Chinese_webtext_spider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-28 09:00:56.000000 Chinese-webtext-spider-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      421 2023-04-28 09:02:26.539898 Chinese-webtext-spider-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 09:02:26.540436 Chinese-webtext-spider-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-04-28 08:55:38.000000 Chinese-webtext-spider-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:02:26.538915 Chinese-webtext-spider-1.0.0/zhspider/
--rw-rw-rw-   0        0        0      165 2023-04-28 08:48:51.000000 Chinese-webtext-spider-1.0.0/zhspider/__init__.py
--rw-rw-rw-   0        0        0     1591 2023-04-28 08:20:00.000000 Chinese-webtext-spider-1.0.0/zhspider/evaluator.py
--rw-rw-rw-   0        0        0     1377 2023-04-28 08:19:59.000000 Chinese-webtext-spider-1.0.0/zhspider/extractor.py
--rw-rw-rw-   0        0        0    12687 2023-04-28 08:19:58.000000 Chinese-webtext-spider-1.0.0/zhspider/spider.py
--rw-rw-rw-   0        0        0    14006 2023-04-28 08:19:57.000000 Chinese-webtext-spider-1.0.0/zhspider/spiders.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:31:27.002318 Chinese-webtext-spider-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:31:26.983072 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/
+-rw-rw-rw-   0        0        0      421 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-28 09:00:56.000000 Chinese-webtext-spider-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      421 2023-04-28 09:31:27.002318 Chinese-webtext-spider-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:31:27.003319 Chinese-webtext-spider-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-04-28 09:30:47.000000 Chinese-webtext-spider-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:31:27.001317 Chinese-webtext-spider-1.0.1/zhspider/
+-rw-rw-rw-   0        0        0      165 2023-04-28 08:48:51.000000 Chinese-webtext-spider-1.0.1/zhspider/__init__.py
+-rw-rw-rw-   0        0        0     1591 2023-04-28 09:21:08.000000 Chinese-webtext-spider-1.0.1/zhspider/evaluator.py
+-rw-rw-rw-   0        0        0     1377 2023-04-28 08:19:59.000000 Chinese-webtext-spider-1.0.1/zhspider/extractor.py
+-rw-rw-rw-   0        0        0    12663 2023-04-28 09:19:58.000000 Chinese-webtext-spider-1.0.1/zhspider/spider.py
+-rw-rw-rw-   0        0        0    14009 2023-04-28 09:20:49.000000 Chinese-webtext-spider-1.0.1/zhspider/spiders.py
```

### Comparing `Chinese-webtext-spider-1.0.0/LICENSE.txt` & `Chinese-webtext-spider-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Chinese-webtext-spider-1.0.0/setup.py` & `Chinese-webtext-spider-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from io import open
 from setuptools import setup, find_packages
 setup(
     name='Chinese-webtext-spider',
-    version='1.0.0',
+    version='1.0.1',
     description='a package for crawling chinese webtext',
     long_description='一个用于爬取网络中文文本的爬虫工具',
     author='ZhaoRunSong',
     author_email='1398915234@qq.com',
     license='Apache License 2.0',
     url='https://github.com/1azybug/chinese-webtext-spider',
     download_url='https://github.com/1azybug/chinese-webtext-spider/master.zip',
```

### Comparing `Chinese-webtext-spider-1.0.0/zhspider/evaluator.py` & `Chinese-webtext-spider-1.0.1/zhspider/evaluator.py`

 * *Files identical despite different names*

### Comparing `Chinese-webtext-spider-1.0.0/zhspider/extractor.py` & `Chinese-webtext-spider-1.0.1/zhspider/extractor.py`

 * *Files identical despite different names*

### Comparing `Chinese-webtext-spider-1.0.0/zhspider/spider.py` & `Chinese-webtext-spider-1.0.1/zhspider/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import requests
 import json
 import time
 import os
-import time
-import json
 import urllib
-from evaluator import Evaluator
-from extractor import Extractor
+from .evaluator import Evaluator
+from .extractor import Extractor
 
 
 
 class Spider:
```

### Comparing `Chinese-webtext-spider-1.0.0/zhspider/spiders.py` & `Chinese-webtext-spider-1.0.1/zhspider/spiders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from spider import Spider
+from .spider import Spider
 import re
-from evaluator import Evaluator
-from extractor import Extractor
+from .evaluator import Evaluator
+from .extractor import Extractor
 
 class BilibiliSpider(Spider):
     def __init__(self, database_path, sleep_time=15, mode="external", debug=True, load_old=False):
         super().__init__(database_path, sleep_time, mode, debug, load_old)
         
         # 构造初始url
         # https://www.bilibili.com/read/cv22990000 从2023-04-11 16:27开始往前爬
```

