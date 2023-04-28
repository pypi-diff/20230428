# Comparing `tmp/docts-0.2.2.tar.gz` & `tmp/docts-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docts-0.2.2.tar", last modified: Thu Apr 27 09:39:55 2023, max compression
+gzip compressed data, was "docts-0.2.3.tar", last modified: Fri Apr 28 01:37:57 2023, max compression
```

## Comparing `docts-0.2.2.tar` & `docts-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 09:39:47.000000 docts-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:39:47.000000 docts-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 09:39:55.387328 docts-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 09:39:47.000000 docts-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 09:39:47.000000 docts-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:39:47.000000 docts-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:39:55.387328 docts-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/src/docts/
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-04-27 09:39:54.000000 docts-0.2.2/src/docts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 09:39:47.000000 docts-0.2.2/src/docts/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:55.387328 docts-0.2.2/src/docts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:39:55.000000 docts-0.2.2/src/docts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:37:57.573939 docts-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 01:37:49.000000 docts-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 01:37:49.000000 docts-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-28 01:37:57.573939 docts-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 01:37:49.000000 docts-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 01:37:49.000000 docts-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 01:37:49.000000 docts-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:37:57.573939 docts-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:37:57.569939 docts-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:37:57.573939 docts-0.2.3/src/docts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-28 01:37:56.000000 docts-0.2.3/src/docts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 01:37:49.000000 docts-0.2.3/src/docts/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:37:57.573939 docts-0.2.3/src/docts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-28 01:37:57.000000 docts-0.2.3/src/docts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 01:37:57.000000 docts-0.2.3/src/docts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:37:57.000000 docts-0.2.3/src/docts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 01:37:57.000000 docts-0.2.3/src/docts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 01:37:57.000000 docts-0.2.3/src/docts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 01:37:57.000000 docts-0.2.3/src/docts.egg-info/top_level.txt
```

### Comparing `docts-0.2.2/LICENSE` & `docts-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docts-0.2.2/PKG-INFO` & `docts-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docts
-Version: 0.2.2
+Version: 0.2.3
 Summary: python package docts
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/docts
 Project-URL: Homepage, https://github.com/foyoux/docts
 Project-URL: Bug Tracker, https://github.com/foyoux/docts/issues
 Keywords: docts
 Classifier: Programming Language :: Python
```

### Comparing `docts-0.2.2/README.md` & `docts-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `docts-0.2.2/pyproject.toml` & `docts-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docts-0.2.2/src/docts/__init__.py` & `docts-0.2.3/src/docts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 __title__ = 'docts'
 __author__ = 'foyoux'
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 __description__ = 'document translate, read & translate & write'
 __url__ = 'https://github.com/foyoux/docts'
 __author_email__ = 'yimi.0822@qq.com'
 __license__ = 'GPL-3.0'
 __copyright__ = f'Copyright 2021-2023 {__author__}'
 __ide__ = 'PyCharm - https://www.jetbrains.com/pycharm/'
 
 import argparse
 import html
+import logging
 import re
 from itertools import islice
 from typing import Callable, Pattern, AnyStr, List
 
 from pygtrans import Translate, Null
 
+log = logging.getLogger('docts')
+_handler = logging.StreamHandler()
+_handler.setFormatter(
+    logging.Formatter(
+        fmt=f'%(asctime)s datclass.%(levelname)s %(message)s',
+        datefmt='%Y-%m-%d %H:%M:%S'
+    )
+)
+log.addHandler(_handler)
+log.setLevel(logging.INFO)
+
 # filter start
 
 UPPER_CHAR = re.compile(r'[A-Z]')
 SPACE_SPLIT = re.compile('[ \t]+')
 
 
 def filter_not_str(word: str) -> bool:
@@ -66,42 +78,36 @@
 def parse_xlf(xlf_path: str) -> List[str]:
     """
     解析xlf文件, 获取原文字符串
     :param xlf_path:
     :return:
     """
     if not xlf_path.endswith('.xlf'):
-        print(f'不是xlf文件: {xlf_path}')
-        raise
+        raise ValueError(f'所给文件 {xlf_path} 不是 xlf 文件')
 
     # newline='', 换行符原样读入
     with open(xlf_path, encoding='utf-8', newline='') as f:
-        txt = f.read()
-        origen_words = re.findall(r'<source[^>]*>(.*?)</source>', txt, re.DOTALL)
-        del txt
+        origen_words = re.findall(r'<source[^>]*>(.*?)</source>', f.read(), re.DOTALL)
 
     i: str
-    # words = [html.unescape(i.replace('[]\n', '\r\n')) for i in set(origen_words) if i != '']
     words = [html.unescape(i) for i in set(origen_words) if i != '']
-
-    print(f'过滤重复或空文本 parse_xlf: {len(origen_words) - len(words)}')
-
+    log.info('过滤重复或空文本 %d 条', len(origen_words) - len(words))
     return words
 
 
 def write_xlf(xlf_path: str, origins: List[str], client: Translate, trans: List[str] = None, limit=5000):
     # 翻译
     if trans is None:
         trans = []
         for lst in [list(islice(origins, i, i + limit)) for i in range(0, len(origins), limit)]:
             tl = client.translate(lst)
             if isinstance(tl, Null):
-                print(tl.msg)
-                raise trans
+                raise Exception(tl.msg)
             trans.extend(tl)
+            log.info(f'翻译完成: %d/%d', len(trans), len(origins))
         trans = [i.translatedText for i in trans]
 
     # 写入文件
     with open(xlf_path, 'w', encoding='utf-8', newline='') as f:
         f.write(
             '<?xml version="1.0" encoding="utf-8"?>\n'
             '<xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" '
@@ -145,15 +151,15 @@
         """
         words = []
         for word in self.words:
             if _filter(word):
                 self.ignores.append(word)
                 continue
             words.append(word)
-        print(f'过滤文本 {_filter.__name__}: {len(self.words) - len(words)}')
+        log.info('过滤器 %s 过滤文本 %d 条', _filter.__name__, len(self.words) - len(words))
         self.words = words
         return self
 
     def add_contain_filter(self, contain: Pattern[AnyStr]):
         """
         支持正则表达式
         :param contain:
@@ -161,43 +167,43 @@
         """
         words = []
         for word in self.words:
             if re.search(contain, word):
                 self.ignores.append(word)
                 continue
             words.append(word)
-        print(f'过滤文本 add_contain_filter({contain}): {len(self.words) - len(words)}')
+        log.info('过滤器 add_contain_filter(%s) 过滤文本 %d 条', contain, len(self.words) - len(words))
         self.words = words
         return self
 
     def add_start_filter(self, start: str, strip: str = None):
         words = []
         word: str
         for word in self.words:
             if strip:
                 word = word.lstrip(strip)
             if word.startswith(start):
                 self.ignores.append(word)
                 continue
             words.append(word)
-        print(f'过滤文本 add_start_filter({start}): {len(self.words) - len(words)}')
+        log.info(f'过滤器 add_start_filter(%s) 过滤文本 %d 条', start, len(self.words) - len(words))
         self.words = words
         return self
 
     def add_end_filter(self, end: str, strip: str = None):
         words = []
         word: str
         for word in self.words:
             if strip:
                 word = word.rstrip(strip)
             if word.endswith(end):
                 self.ignores.append(word)
                 continue
             words.append(word)
-        print(f'过滤文本 add_end_filter({end}): {len(self.words) - len(words)}')
+        log.info(f'过滤器 add_end_filter(%s) 过滤文本 %d 条', end, len(self.words) - len(words))
         self.words = words
         return self
 
     def add_map(self, _map: Callable[[str], str]):
         """
         添加自定义映射器, 参考 def map_symbol_dot
         :param _map:
```

### Comparing `docts-0.2.2/src/docts.egg-info/PKG-INFO` & `docts-0.2.3/src/docts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docts
-Version: 0.2.2
+Version: 0.2.3
 Summary: python package docts
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/docts
 Project-URL: Homepage, https://github.com/foyoux/docts
 Project-URL: Bug Tracker, https://github.com/foyoux/docts/issues
 Keywords: docts
 Classifier: Programming Language :: Python
```

