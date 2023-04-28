# Comparing `tmp/Chinese-webtext-spider-1.0.1.tar.gz` & `tmp/Chinese-webtext-spider-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chinese-webtext-spider-1.0.1.tar", last modified: Fri Apr 28 09:31:27 2023, max compression
+gzip compressed data, was "Chinese-webtext-spider-1.0.2.tar", last modified: Fri Apr 28 10:30:34 2023, max compression
```

## Comparing `Chinese-webtext-spider-1.0.1.tar` & `Chinese-webtext-spider-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:31:27.002318 Chinese-webtext-spider-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-28 09:31:26.983072 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/
--rw-rw-rw-   0        0        0      421 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 09:31:26.000000 Chinese-webtext-spider-1.0.1/Chinese_webtext_spider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-28 09:00:56.000000 Chinese-webtext-spider-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      421 2023-04-28 09:31:27.002318 Chinese-webtext-spider-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 09:31:27.003319 Chinese-webtext-spider-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-04-28 09:30:47.000000 Chinese-webtext-spider-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:31:27.001317 Chinese-webtext-spider-1.0.1/zhspider/
--rw-rw-rw-   0        0        0      165 2023-04-28 08:48:51.000000 Chinese-webtext-spider-1.0.1/zhspider/__init__.py
--rw-rw-rw-   0        0        0     1591 2023-04-28 09:21:08.000000 Chinese-webtext-spider-1.0.1/zhspider/evaluator.py
--rw-rw-rw-   0        0        0     1377 2023-04-28 08:19:59.000000 Chinese-webtext-spider-1.0.1/zhspider/extractor.py
--rw-rw-rw-   0        0        0    12663 2023-04-28 09:19:58.000000 Chinese-webtext-spider-1.0.1/zhspider/spider.py
--rw-rw-rw-   0        0        0    14009 2023-04-28 09:20:49.000000 Chinese-webtext-spider-1.0.1/zhspider/spiders.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:30:34.472515 Chinese-webtext-spider-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-28 10:30:34.443290 Chinese-webtext-spider-1.0.2/Chinese_webtext_spider.egg-info/
+-rw-rw-rw-   0        0        0      421 2023-04-28 10:30:34.000000 Chinese-webtext-spider-1.0.2/Chinese_webtext_spider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-28 10:30:34.000000 Chinese-webtext-spider-1.0.2/Chinese_webtext_spider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:30:34.000000 Chinese-webtext-spider-1.0.2/Chinese_webtext_spider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-28 10:30:34.000000 Chinese-webtext-spider-1.0.2/Chinese_webtext_spider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 10:30:34.000000 Chinese-webtext-spider-1.0.2/Chinese_webtext_spider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-28 09:00:56.000000 Chinese-webtext-spider-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      421 2023-04-28 10:30:34.468528 Chinese-webtext-spider-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 10:30:34.472515 Chinese-webtext-spider-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-04-28 10:29:30.000000 Chinese-webtext-spider-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:30:34.468528 Chinese-webtext-spider-1.0.2/zhspider/
+-rw-rw-rw-   0        0        0      165 2023-04-28 08:48:51.000000 Chinese-webtext-spider-1.0.2/zhspider/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-04-28 09:37:02.000000 Chinese-webtext-spider-1.0.2/zhspider/evaluator.py
+-rw-rw-rw-   0        0        0     1377 2023-04-28 08:19:59.000000 Chinese-webtext-spider-1.0.2/zhspider/extractor.py
+-rw-rw-rw-   0        0        0    12663 2023-04-28 09:37:27.000000 Chinese-webtext-spider-1.0.2/zhspider/spider.py
+-rw-rw-rw-   0        0        0    14009 2023-04-28 09:20:49.000000 Chinese-webtext-spider-1.0.2/zhspider/spiders.py
```

### Comparing `Chinese-webtext-spider-1.0.1/LICENSE.txt` & `Chinese-webtext-spider-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Chinese-webtext-spider-1.0.1/setup.py` & `Chinese-webtext-spider-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from io import open
 from setuptools import setup, find_packages
 setup(
     name='Chinese-webtext-spider',
-    version='1.0.1',
+    version='1.0.2',
     description='a package for crawling chinese webtext',
     long_description='一个用于爬取网络中文文本的爬虫工具',
     author='ZhaoRunSong',
     author_email='1398915234@qq.com',
     license='Apache License 2.0',
     url='https://github.com/1azybug/chinese-webtext-spider',
     download_url='https://github.com/1azybug/chinese-webtext-spider/master.zip',
```

### Comparing `Chinese-webtext-spider-1.0.1/zhspider/evaluator.py` & `Chinese-webtext-spider-1.0.2/zhspider/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.tokenizer =tokenizer
         self.model=model
         self.threshold = threshold
         if not self.tokenizer:
             self.tokenizer = BertTokenizer.from_pretrained("uer/albert-large-chinese-cluecorpussmall")
         if not self.model:
             self.model = AutoModelForSequenceClassification.from_pretrained("uer/albert-large-chinese-cluecorpussmall", num_labels=2)
-            self.model.load_state_dict(torch.load("large.pt",map_location=self.device))
+            self.model.load_state_dict(torch.load("./large.pt",map_location=self.device))
             self.model.to(self.device)
 
     def predict(self,text1,text2=None):
         self.model.eval()
         
         encoded_input = self.tokenizer(text1[-32:],text2[:32], padding=True ,return_tensors='pt').to(self.device) \
     if text2 else self.tokenizer(text1[:64], padding=True ,return_tensors='pt').to(self.device)
```

### Comparing `Chinese-webtext-spider-1.0.1/zhspider/extractor.py` & `Chinese-webtext-spider-1.0.2/zhspider/extractor.py`

 * *Files identical despite different names*

### Comparing `Chinese-webtext-spider-1.0.1/zhspider/spider.py` & `Chinese-webtext-spider-1.0.2/zhspider/spider.py`

 * *Files identical despite different names*

### Comparing `Chinese-webtext-spider-1.0.1/zhspider/spiders.py` & `Chinese-webtext-spider-1.0.2/zhspider/spiders.py`

 * *Files identical despite different names*

