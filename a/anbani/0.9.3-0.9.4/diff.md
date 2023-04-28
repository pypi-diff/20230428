# Comparing `tmp/anbani-0.9.3.tar.gz` & `tmp/anbani-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anbani-0.9.3.tar", last modified: Fri Apr 28 05:18:19 2023, max compression
+gzip compressed data, was "anbani-0.9.4.tar", last modified: Fri Apr 28 05:30:35 2023, max compression
```

## Comparing `anbani-0.9.3.tar` & `anbani-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.566458 anbani-0.9.3/
--rw-r--r--   0 george    (1000) george    (1000)    35149 2022-07-12 06:28:39.000000 anbani-0.9.3/LICENSE
--rw-r--r--   0 george    (1000) george    (1000)       21 2022-07-12 06:28:39.000000 anbani-0.9.3/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)     2967 2023-04-28 05:18:19.566458 anbani-0.9.3/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     2434 2022-07-12 06:28:39.000000 anbani-0.9.3/README.md
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.552457 anbani-0.9.3/anbani/
--rw-r--r--   0 george    (1000) george    (1000)       66 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/__init__.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.553457 anbani-0.9.3/anbani/core/
--rw-r--r--   0 george    (1000) george    (1000)        0 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/core/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     3581 2022-07-12 06:35:34.000000 anbani-0.9.3/anbani/core/converter.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.558458 anbani-0.9.3/anbani/data/
--rw-r--r--   0 george    (1000) george    (1000)  2459360 2023-04-27 13:32:54.000000 anbani-0.9.3/anbani/data/ambigram_nc1_len10.csv
--rw-r--r--   0 george    (1000) george    (1000)   416348 2023-04-27 13:32:54.000000 anbani-0.9.3/anbani/data/ambigram_nc5_len7.csv
--rw-r--r--   0 george    (1000) george    (1000)    16939 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/data/georgian_contractions.csv
--rw-r--r--   0 george    (1000) george    (1000)    11296 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/data/letters.js
--rw-r--r--   0 george    (1000) george    (1000)  5781776 2023-04-27 13:33:08.000000 anbani-0.9.3/anbani/data/wordlist.csv
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.566458 anbani-0.9.3/anbani/nlp/
--rw-r--r--   0 george    (1000) george    (1000)       16 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)      770 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/contractions.py
--rw-r--r--   0 george    (1000) george    (1000)     4924 2023-04-28 04:44:57.000000 anbani-0.9.3/anbani/nlp/georgianisation.py
--rw-r--r--   0 george    (1000) george    (1000)     1681 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/preprocessing.py
--rw-r--r--   0 george    (1000) george    (1000)     1306 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.552457 anbani-0.9.3/anbani.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)     2967 2023-04-28 05:18:18.000000 anbani-0.9.3/anbani.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)      548 2023-04-28 05:18:19.000000 anbani-0.9.3/anbani.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-28 05:18:18.000000 anbani-0.9.3/anbani.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)       32 2023-04-28 05:18:19.000000 anbani-0.9.3/anbani.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-28 05:18:19.000000 anbani-0.9.3/anbani.egg-info/top_level.txt
--rw-r--r--   0 george    (1000) george    (1000)      103 2023-04-28 05:18:19.567458 anbani-0.9.3/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      879 2023-04-28 05:17:54.000000 anbani-0.9.3/setup.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.044230 anbani-0.9.4/
+-rw-r--r--   0 george    (1000) george    (1000)    35149 2022-07-12 06:28:39.000000 anbani-0.9.4/LICENSE
+-rw-r--r--   0 george    (1000) george    (1000)       21 2022-07-12 06:28:39.000000 anbani-0.9.4/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)     3271 2023-04-28 05:30:35.044230 anbani-0.9.4/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)     2738 2023-04-28 05:21:14.000000 anbani-0.9.4/README.md
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.030230 anbani-0.9.4/anbani/
+-rw-r--r--   0 george    (1000) george    (1000)       66 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/__init__.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.032230 anbani-0.9.4/anbani/core/
+-rw-r--r--   0 george    (1000) george    (1000)        0 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/core/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     3581 2022-07-12 06:35:34.000000 anbani-0.9.4/anbani/core/converter.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.036230 anbani-0.9.4/anbani/data/
+-rw-r--r--   0 george    (1000) george    (1000)  2459360 2023-04-27 13:32:54.000000 anbani-0.9.4/anbani/data/ambigram_nc1_len10.csv
+-rw-r--r--   0 george    (1000) george    (1000)   416348 2023-04-27 13:32:54.000000 anbani-0.9.4/anbani/data/ambigram_nc5_len7.csv
+-rw-r--r--   0 george    (1000) george    (1000)    16939 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/data/georgian_contractions.csv
+-rw-r--r--   0 george    (1000) george    (1000)    11296 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/data/letters.js
+-rw-r--r--   0 george    (1000) george    (1000)  5781776 2023-04-27 13:33:08.000000 anbani-0.9.4/anbani/data/wordlist.csv
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.043230 anbani-0.9.4/anbani/nlp/
+-rw-r--r--   0 george    (1000) george    (1000)       16 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)      770 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/contractions.py
+-rw-r--r--   0 george    (1000) george    (1000)     5068 2023-04-28 05:27:48.000000 anbani-0.9.4/anbani/nlp/georgianisation.py
+-rw-r--r--   0 george    (1000) george    (1000)     1681 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/preprocessing.py
+-rw-r--r--   0 george    (1000) george    (1000)     1306 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/utils.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.031230 anbani-0.9.4/anbani.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)     3271 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)      548 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)       32 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/top_level.txt
+-rw-r--r--   0 george    (1000) george    (1000)      103 2023-04-28 05:30:35.044230 anbani-0.9.4/setup.cfg
+-rw-r--r--   0 george    (1000) george    (1000)      879 2023-04-28 05:28:52.000000 anbani-0.9.4/setup.py
```

### Comparing `anbani-0.9.3/LICENSE` & `anbani-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/PKG-INFO` & `anbani-0.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anbani
-Version: 0.9.3
+Version: 0.9.4
 Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.
 Home-page: https://github.com/anbani/anbani.py
 Author: George Gach
 Author-email: georgegach@outlook.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,25 @@
 from anbani.core.converter import convert, interpret
 
 interpret("გამარჯობა", "asomtavruli")
 
 # 'ႢႠႫႠႰႿႭႡႠ'
 ```
 
+Georgianisation example:
+
+```python
+from anbani.nlp.georgianisation import georgianise
+
+georgianise("gamarjoba - rogor xar - rasa iqm - kaia kata - kai erti")
+
+# 'გამარჯობა - როგორ ხარ - რასა იქმ - კაია კატა - კაი ერთი'
+```
+
+
 Convert ebooks with qwerty encoding to unicode Mkhedruli:
 
 ```python
 from anbani.nlp.utils import ebook2text
 from anbani.core.converter import classify_text
 from anbani.core.converter import convert
```

### Comparing `anbani-0.9.3/README.md` & `anbani-0.9.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 from anbani.core.converter import convert, interpret
 
 interpret("გამარჯობა", "asomtavruli")
 
 # 'ႢႠႫႠႰႿႭႡႠ'
 ```
 
+Georgianisation example:
+
+```python
+from anbani.nlp.georgianisation import georgianise
+
+georgianise("gamarjoba - rogor xar - rasa iqm - kaia kata - kai erti")
+
+# 'გამარჯობა - როგორ ხარ - რასა იქმ - კაია კატა - კაი ერთი'
+```
+
+
 Convert ebooks with qwerty encoding to unicode Mkhedruli:
 
 ```python
 from anbani.nlp.utils import ebook2text
 from anbani.core.converter import classify_text
 from anbani.core.converter import convert
```

### Comparing `anbani-0.9.3/anbani/core/converter.py` & `anbani-0.9.4/anbani/core/converter.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/data/ambigram_nc1_len10.csv` & `anbani-0.9.4/anbani/data/ambigram_nc1_len10.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/data/ambigram_nc5_len7.csv` & `anbani-0.9.4/anbani/data/ambigram_nc5_len7.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/data/georgian_contractions.csv` & `anbani-0.9.4/anbani/data/georgian_contractions.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/data/letters.js` & `anbani-0.9.4/anbani/data/letters.js`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/data/wordlist.csv` & `anbani-0.9.4/anbani/data/wordlist.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/nlp/contractions.py` & `anbani-0.9.4/anbani/nlp/contractions.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/nlp/georgianisation.py` & `anbani-0.9.4/anbani/nlp/georgianisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import pandas as pd
 import re
+import os
+from pathlib import Path
+module_path = Path(__file__).parent.parent.absolute()
 
-AMBIGRAM_BALANCED_PATH = "data/ambigram_nc5_len7.csv"
-AMBIGRAM_ACCURATE_PATH = "data/ambigram_nc1_len10.csv"
+
+AMBIGRAM_BALANCED_PATH = os.path.join(module_path, "data/ambigram_nc5_len7.csv")
+AMBIGRAM_ACCURATE_PATH = os.path.join(module_path, "data/ambigram_nc1_len10.csv")
 
 extract_mapping = lambda df: df[~df.REDUNDANT][["MASKED", "NGRAM"]].values
 
 ambigrams_balanced = extract_mapping(pd.read_csv(AMBIGRAM_BALANCED_PATH))
 ambigrams_accurate = extract_mapping(pd.read_csv(AMBIGRAM_ACCURATE_PATH))
```

### Comparing `anbani-0.9.3/anbani/nlp/preprocessing.py` & `anbani-0.9.4/anbani/nlp/preprocessing.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani/nlp/utils.py` & `anbani-0.9.4/anbani/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/anbani.egg-info/PKG-INFO` & `anbani-0.9.4/anbani.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anbani
-Version: 0.9.3
+Version: 0.9.4
 Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.
 Home-page: https://github.com/anbani/anbani.py
 Author: George Gach
 Author-email: georgegach@outlook.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,25 @@
 from anbani.core.converter import convert, interpret
 
 interpret("გამარჯობა", "asomtavruli")
 
 # 'ႢႠႫႠႰႿႭႡႠ'
 ```
 
+Georgianisation example:
+
+```python
+from anbani.nlp.georgianisation import georgianise
+
+georgianise("gamarjoba - rogor xar - rasa iqm - kaia kata - kai erti")
+
+# 'გამარჯობა - როგორ ხარ - რასა იქმ - კაია კატა - კაი ერთი'
+```
+
+
 Convert ebooks with qwerty encoding to unicode Mkhedruli:
 
 ```python
 from anbani.nlp.utils import ebook2text
 from anbani.core.converter import classify_text
 from anbani.core.converter import convert
```

### Comparing `anbani-0.9.3/anbani.egg-info/SOURCES.txt` & `anbani-0.9.4/anbani.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anbani-0.9.3/setup.py` & `anbani-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='anbani',
-    version='0.9.3',
+    version='0.9.4',
     author="George Gach",
     author_email="georgegach@outlook.com",
     description="Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.",
     license='GPL',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anbani/anbani.py",
```

