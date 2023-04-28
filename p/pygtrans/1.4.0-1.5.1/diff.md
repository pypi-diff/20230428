# Comparing `tmp/pygtrans-1.4.0.tar.gz` & `tmp/pygtrans-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygtrans-1.4.0.tar", last modified: Tue Apr 19 07:14:19 2022, max compression
+gzip compressed data, was "pygtrans-1.5.1.tar", last modified: Thu Apr 27 10:04:13 2023, max compression
```

## Comparing `pygtrans-1.4.0.tar` & `pygtrans-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 07:14:19.807459 pygtrans-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-04-19 07:14:09.000000 pygtrans-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3841 2022-04-19 07:14:19.807459 pygtrans-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-04-19 07:14:09.000000 pygtrans-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 07:14:19.807459 pygtrans-1.4.0/pygtrans/
--rw-r--r--   0 runner    (1001) docker     (121)     9404 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pygtrans/ApiKeyTranslate.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pygtrans/DetectResponse.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pygtrans/LanguageResponse.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pygtrans/Null.py
--rw-r--r--   0 runner    (1001) docker     (121)     8690 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pygtrans/Translate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pygtrans/TranslateResponse.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-04-19 07:14:12.000000 pygtrans-1.4.0/pygtrans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 07:14:19.807459 pygtrans-1.4.0/pygtrans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3841 2022-04-19 07:14:19.000000 pygtrans-1.4.0/pygtrans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-04-19 07:14:19.000000 pygtrans-1.4.0/pygtrans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 07:14:19.000000 pygtrans-1.4.0/pygtrans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-19 07:14:19.000000 pygtrans-1.4.0/pygtrans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-19 07:14:19.000000 pygtrans-1.4.0/pygtrans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-19 07:14:09.000000 pygtrans-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-04-19 07:14:19.807459 pygtrans-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:04:13.177820 pygtrans-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 10:04:04.000000 pygtrans-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:04:04.000000 pygtrans-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-27 10:04:13.177820 pygtrans-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 10:04:04.000000 pygtrans-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 10:04:04.000000 pygtrans-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 10:04:04.000000 pygtrans-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 10:04:13.177820 pygtrans-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:04:13.173820 pygtrans-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:04:13.177820 pygtrans-1.5.1/src/pygtrans/
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/ApiKeyTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/DetectResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/LanguageResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/TranslateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 10:04:12.000000 pygtrans-1.5.1/src/pygtrans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-27 10:04:04.000000 pygtrans-1.5.1/src/pygtrans/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:04:13.177820 pygtrans-1.5.1/src/pygtrans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-27 10:04:13.000000 pygtrans-1.5.1/src/pygtrans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-27 10:04:13.000000 pygtrans-1.5.1/src/pygtrans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:04:13.000000 pygtrans-1.5.1/src/pygtrans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 10:04:13.000000 pygtrans-1.5.1/src/pygtrans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 10:04:13.000000 pygtrans-1.5.1/src/pygtrans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:04:13.000000 pygtrans-1.5.1/src/pygtrans.egg-info/top_level.txt
```

### Comparing `pygtrans-1.4.0/LICENSE` & `pygtrans-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygtrans-1.4.0/PKG-INFO` & `pygtrans-1.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: pygtrans
-Version: 1.4.0
+Version: 1.5.1
 Summary: Google Translate, support APIKEY
-Home-page: https://github.com/foyoux/pygtrans
-Author: foyou
-Author-email: yimi.0822@qq.com
-License: GPL-3.0
-Project-URL: Documentation, https://pygtrans.readthedocs.io/zh_CN/latest/
+Author: foyoux
 Project-URL: Source, https://github.com/foyoux/pygtrans
+Project-URL: Homepage, https://github.com/foyoux/pygtrans
 Project-URL: Bug Tracker, https://github.com/foyoux/pygtrans/issues
-Keywords: google translate apikey text html google.cn google.com
-Platform: UNKNOWN
+Project-URL: Documentation, https://pygtrans.readthedocs.io/zh_CN/latest/
+Keywords: pygtrans,google,translate,apikey,text,html,google.cn,google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygtrans
 
 谷歌翻译, 支持 **APIKEY**
 
@@ -38,14 +35,16 @@
 
 ## 安装
 
 [![](https://img.shields.io/pypi/pyversions/pygtrans)](https://pypi.org/project/pygtrans/) 
 
 ```bash
 pip install -U pygtrans
+pip install git+ssh://git@github.com/foyoux/pygtrans.git
+pip install git+https://github.com/foyoux/pygtrans.git
 ```
 
 
 ## 基本功能
 
 - [x] 获取语言支持列表
 - [x] 自动检测语言, 支持批量
@@ -103,9 +102,7 @@
       - 从2021年9月15日开始, 需要翻墙才能使用, 具体参考 [#8](https://github.com/foyoux/pygtrans/issues/8)
    2. `ApiKeyTranslate`: 需要有效的谷歌翻译 **API KEY**，[谷歌提供免费试用](https://cloud.google.com/translate/docs/quickstarts)
 2. `Translate`的最佳实践:
    1. `http` 代理：`Translate(proxies={"https": "http://localhost:10809"})`
    2. `socks5` 代理: `Translate(proxies={"https": "socks5://localhost:10808"})`
    3. **重要**：尽量一次性多翻译，减少请求次数，参考 [#13](https://github.com/foyoux/pygtrans/issues/13)，比如一次性翻译 2000 / 5000 / 10000
 
-
-
```

### Comparing `pygtrans-1.4.0/README.md` & `pygtrans-1.5.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 ## 安装
 
 [![](https://img.shields.io/pypi/pyversions/pygtrans)](https://pypi.org/project/pygtrans/) 
 
 ```bash
 pip install -U pygtrans
+pip install git+ssh://git@github.com/foyoux/pygtrans.git
+pip install git+https://github.com/foyoux/pygtrans.git
 ```
 
 
 ## 基本功能
 
 - [x] 获取语言支持列表
 - [x] 自动检测语言, 支持批量
```

### Comparing `pygtrans-1.4.0/pygtrans/ApiKeyTranslate.py` & `pygtrans-1.5.1/src/pygtrans/ApiKeyTranslate.py`

 * *Files identical despite different names*

### Comparing `pygtrans-1.4.0/pygtrans/DetectResponse.py` & `pygtrans-1.5.1/src/pygtrans/DetectResponse.py`

 * *Files identical despite different names*

### Comparing `pygtrans-1.4.0/pygtrans/Translate.py` & `pygtrans-1.5.1/src/pygtrans/Translate.py`

 * *Files identical despite different names*

### Comparing `pygtrans-1.4.0/pygtrans/TranslateResponse.py` & `pygtrans-1.5.1/src/pygtrans/TranslateResponse.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
         :param translatedText: 翻译成目标语言的文本。
         :param detectedSourceLanguage: 如果初始请求中没有传递源语言，则自动检测初始请求的源语言。如果通过了源语言，则不会自动检测语言，并且将省略此字段。
         :param model: 翻译模型。可以是基于短语的机器翻译 (PBMT) 模型的基础，也可以是神经机器翻译 (NMT) 模型的 nmt。如果您的请求中没有包含模型参数，则该字段不会包含在响应中。
         """
         if isinstance(translatedText, list):
             self.translatedText = translatedText[0]
-            self.detectedSourceLanguage = translatedText[1]
+            if len(translatedText) > 1:
+                self.detectedSourceLanguage = translatedText[1]
         else:
             self.translatedText = translatedText
             self.detectedSourceLanguage = detectedSourceLanguage
 
         self.model = model
 
     def __repr__(self):
```

### Comparing `pygtrans-1.4.0/pygtrans/__init__.py` & `pygtrans-1.5.1/src/pygtrans/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from .Null import Null
 from .Translate import Translate
 from .TranslateResponse import TranslateResponse
 
 __title__ = 'pygtrans'
 __description__ = 'Google Translate, support APIKEY'
 __url__ = 'https://github.com/foyoux/pygtrans'
-__version__ = '1.4.0'
-__author__ = 'foyou'
+__version__ = '1.5.1'
+__author__ = 'foyoux'
 __author_email__ = 'yimi.0822@qq.com'
 __license__ = 'GPL-3.0'
 __copyright__ = f'Copyright 2021 {__author__}'
 __ide__ = 'PyCharm - https://www.jetbrains.com/pycharm/'
 
 __all__ = [
     'Translate', 'ApiKeyTranslate', 'Null', 'LanguageResponse', 'DetectResponse', 'TranslateResponse'
```

### Comparing `pygtrans-1.4.0/pygtrans.egg-info/PKG-INFO` & `pygtrans-1.5.1/src/pygtrans.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: pygtrans
-Version: 1.4.0
+Version: 1.5.1
 Summary: Google Translate, support APIKEY
-Home-page: https://github.com/foyoux/pygtrans
-Author: foyou
-Author-email: yimi.0822@qq.com
-License: GPL-3.0
-Project-URL: Documentation, https://pygtrans.readthedocs.io/zh_CN/latest/
+Author: foyoux
 Project-URL: Source, https://github.com/foyoux/pygtrans
+Project-URL: Homepage, https://github.com/foyoux/pygtrans
 Project-URL: Bug Tracker, https://github.com/foyoux/pygtrans/issues
-Keywords: google translate apikey text html google.cn google.com
-Platform: UNKNOWN
+Project-URL: Documentation, https://pygtrans.readthedocs.io/zh_CN/latest/
+Keywords: pygtrans,google,translate,apikey,text,html,google.cn,google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygtrans
 
 谷歌翻译, 支持 **APIKEY**
 
@@ -38,14 +35,16 @@
 
 ## 安装
 
 [![](https://img.shields.io/pypi/pyversions/pygtrans)](https://pypi.org/project/pygtrans/) 
 
 ```bash
 pip install -U pygtrans
+pip install git+ssh://git@github.com/foyoux/pygtrans.git
+pip install git+https://github.com/foyoux/pygtrans.git
 ```
 
 
 ## 基本功能
 
 - [x] 获取语言支持列表
 - [x] 自动检测语言, 支持批量
@@ -103,9 +102,7 @@
       - 从2021年9月15日开始, 需要翻墙才能使用, 具体参考 [#8](https://github.com/foyoux/pygtrans/issues/8)
    2. `ApiKeyTranslate`: 需要有效的谷歌翻译 **API KEY**，[谷歌提供免费试用](https://cloud.google.com/translate/docs/quickstarts)
 2. `Translate`的最佳实践:
    1. `http` 代理：`Translate(proxies={"https": "http://localhost:10809"})`
    2. `socks5` 代理: `Translate(proxies={"https": "socks5://localhost:10808"})`
    3. **重要**：尽量一次性多翻译，减少请求次数，参考 [#13](https://github.com/foyoux/pygtrans/issues/13)，比如一次性翻译 2000 / 5000 / 10000
 
-
-
```

