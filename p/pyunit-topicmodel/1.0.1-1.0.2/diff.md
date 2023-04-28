# Comparing `tmp/pyunit-topicmodel-1.0.1.tar.gz` & `tmp/pyunit-topicmodel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunit-topicmodel-1.0.1.tar", last modified: Tue Mar 21 03:19:38 2023, max compression
+gzip compressed data, was "pyunit-topicmodel-1.0.2.tar", last modified: Fri Apr 28 01:46:08 2023, max compression
```

## Comparing `pyunit-topicmodel-1.0.1.tar` & `pyunit-topicmodel-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:19:38.974171 pyunit-topicmodel-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-21 03:19:38.974171 pyunit-topicmodel-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:19:38.970171 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 03:19:38.000000 pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 03:19:38.974171 pyunit-topicmodel-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:19:38.970171 pyunit-topicmodel-1.0.1/topicModel/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/stopwords.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-03-21 03:19:04.000000 pyunit-topicmodel-1.0.1/topicModel/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:46:08.715609 pyunit-topicmodel-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-28 01:46:08.715609 pyunit-topicmodel-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:46:08.711609 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 01:46:08.000000 pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:46:08.715609 pyunit-topicmodel-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:46:08.715609 pyunit-topicmodel-1.0.2/topicModel/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/stopwords.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-28 01:45:25.000000 pyunit-topicmodel-1.0.2/topicModel/tool.py
```

### Comparing `pyunit-topicmodel-1.0.1/LICENSE` & `pyunit-topicmodel-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunit-topicmodel-1.0.1/PKG-INFO` & `pyunit-topicmodel-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunit-topicmodel
-Version: 1.0.1
+Version: 1.0.2
 Summary: 主题识别模型
 Home-page: https://github.com/pyunits/pyunits-topicmodel
 Author: 张伟
 Author-email: jtyoui@qq.com
 License: MIT Licence
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyunit-topicmodel-1.0.1/README.md` & `pyunit-topicmodel-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyunit-topicmodel-1.0.1/pyunit_topicmodel.egg-info/PKG-INFO` & `pyunit-topicmodel-1.0.2/pyunit_topicmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunit-topicmodel
-Version: 1.0.1
+Version: 1.0.2
 Summary: 主题识别模型
 Home-page: https://github.com/pyunits/pyunits-topicmodel
 Author: 张伟
 Author-email: jtyoui@qq.com
 License: MIT Licence
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyunit-topicmodel-1.0.1/setup.py` & `pyunit-topicmodel-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_text = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     install_requires = f.read().strip().splitlines()
 
 setup(
     name="pyUnit-topicModel".lower(),
-    version="1.0.1",
+    version="1.0.2",
     description="主题识别模型",
     long_description=long_text,
     long_description_content_type="text/markdown",
     url="https://github.com/pyunits/pyunits-topicmodel",
     author="张伟",
     author_email="jtyoui@qq.com",
     license='MIT Licence',
```

### Comparing `pyunit-topicmodel-1.0.1/topicModel/cli.py` & `pyunit-topicmodel-1.0.2/topicModel/cli.py`

 * *Files identical despite different names*

### Comparing `pyunit-topicmodel-1.0.1/topicModel/config.py` & `pyunit-topicmodel-1.0.2/topicModel/config.py`

 * *Files identical despite different names*

### Comparing `pyunit-topicmodel-1.0.1/topicModel/model.py` & `pyunit-topicmodel-1.0.2/topicModel/model.py`

 * *Files identical despite different names*

### Comparing `pyunit-topicmodel-1.0.1/topicModel/preprocess.py` & `pyunit-topicmodel-1.0.2/topicModel/preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # @Time  : 2022/8/31 15:21
 # @Email: jtyoui@qq.com
 import json
+from typing import List
 import pandas as pd
 from collections import Counter
 from .tool import word_cut
 from .config import Config
 
 
 def read_title_abstract(config: Config) -> list:
@@ -37,26 +38,36 @@
     m = {}
     with open(stop_path, encoding="utf-8") as fp:
         for line in fp:
             m[line.strip()] = False
     return m
 
 
-def save_word_count(word_path: str, word_count: dict):
+def save_word_count(word_path: str, word_count: List[tuple]):
     """ 保存词频信息,保存成Excel，[index,单词,词频]
 
     :param word_path: 词频文本保存路径
     :param word_count: 词频信息
     """
     ls = []
 
-    for index, (key, value) in enumerate(word_count.items()):
-        ls.append({"id": index, "单词": key, "词频": value})
+    for index, (key, value) in enumerate(word_count):
+        ls.append({"单词": key, "词频": value})
 
-    pd.DataFrame(ls).to_excel(word_path, index=False)
+    df = pd.DataFrame(ls)
+    # 如果df为空，就不保存
+    if df.empty:
+        return
+
+    # 当df的大小超过 65535 时，就保存65535行
+    row = 65535
+    if df.shape[0] > row:
+        df = df.loc[:row, :]
+
+    df.to_excel(word_path, index=False)
 
 
 def preprocess_func(config: Config, stop_num: int = 3) -> list:
     """ 预处理文本函数
     :param stop_num: 停用词个数,默认是3
     :param config: 配置文件
     :return: 切词
@@ -68,15 +79,15 @@
     count = Counter(words)
     preprocess = []
 
     for key, value in count.items():
         if value < stop_num and m.get(key, True):
             m[key] = False
 
-    save_word_count(config.WordPath, count)
+    save_word_count(config.WordPath, count.most_common())
 
     for content in cut:
         values = [value for value in content["text"] if m.get(value, True)]
         preprocess.append({"text": values, "id": content["id"]})
 
     with open(config.PreprocessPath, "w", encoding="utf-8") as wp:
         json.dump(preprocess, wp, ensure_ascii=False, indent="\t")
```

### Comparing `pyunit-topicmodel-1.0.1/topicModel/stopwords.txt` & `pyunit-topicmodel-1.0.2/topicModel/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pyunit-topicmodel-1.0.1/topicModel/tool.py` & `pyunit-topicmodel-1.0.2/topicModel/tool.py`

 * *Files identical despite different names*

