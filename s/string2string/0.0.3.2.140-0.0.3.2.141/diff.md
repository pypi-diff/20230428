# Comparing `tmp/string2string-0.0.3.2.140.tar.gz` & `tmp/string2string-0.0.3.2.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string2string-0.0.3.2.140.tar", last modified: Tue Mar 21 07:26:19 2023, max compression
+gzip compressed data, was "string2string-0.0.3.2.141.tar", last modified: Tue Mar 21 07:29:21 2023, max compression
```

## Comparing `string2string-0.0.3.2.140.tar` & `string2string-0.0.3.2.141.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.819616 string2string-0.0.3.2.140/
--rw-r--r--   0 machine    (501) staff       (20)     1055 2022-07-17 23:18:45.000000 string2string-0.0.3.2.140/LICENSE.txt
--rw-r--r--   0 machine    (501) staff       (20)      869 2023-03-21 07:26:19.819401 string2string-0.0.3.2.140/PKG-INFO
--rw-r--r--   0 machine    (501) staff       (20)     2290 2023-03-21 05:43:43.000000 string2string-0.0.3.2.140/README.md
--rw-r--r--   0 machine    (501) staff       (20)       38 2023-03-21 07:26:19.819675 string2string-0.0.3.2.140/setup.cfg
--rw-r--r--   0 machine    (501) staff       (20)     1320 2023-03-21 07:26:11.000000 string2string-0.0.3.2.140/setup.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.808473 string2string-0.0.3.2.140/string2string/
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-26 19:59:48.000000 string2string-0.0.3.2.140/string2string/__init__.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.809456 string2string-0.0.3.2.140/string2string/alignment/
--rw-r--r--   0 machine    (501) staff       (20)      262 2023-03-19 23:42:10.000000 string2string-0.0.3.2.140/string2string/alignment/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)    56008 2023-03-21 05:54:31.000000 string2string-0.0.3.2.140/string2string/alignment/classical.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.810670 string2string-0.0.3.2.140/string2string/compression/
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:24:13.000000 string2string-0.0.3.2.140/string2string/compression/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:29:22.000000 string2string-0.0.3.2.140/string2string/compression/arithmetic_encoding.py
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:25:14.000000 string2string-0.0.3.2.140/string2string/compression/bpe.py
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:27:16.000000 string2string-0.0.3.2.140/string2string/compression/burrows_wheeler_transform.py
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:28:08.000000 string2string-0.0.3.2.140/string2string/compression/huffman_coding.py
--rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:25:12.000000 string2string-0.0.3.2.140/string2string/compression/lempel_ziv.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.811076 string2string-0.0.3.2.140/string2string/distance/
--rw-r--r--   0 machine    (501) staff       (20)      231 2023-03-20 16:30:22.000000 string2string-0.0.3.2.140/string2string/distance/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)    21428 2023-03-21 05:51:18.000000 string2string-0.0.3.2.140/string2string/distance/classical.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.812443 string2string-0.0.3.2.140/string2string/metrics/
--rw-r--r--   0 machine    (501) staff       (20)      177 2023-03-19 06:26:11.000000 string2string-0.0.3.2.140/string2string/metrics/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)     1693 2023-03-19 06:35:15.000000 string2string-0.0.3.2.140/string2string/metrics/exact_match.py
--rw-r--r--   0 machine    (501) staff       (20)     4997 2023-03-21 05:51:11.000000 string2string-0.0.3.2.140/string2string/metrics/rouge.py
--rw-r--r--   0 machine    (501) staff       (20)     4282 2023-03-19 23:42:11.000000 string2string-0.0.3.2.140/string2string/metrics/sbleu.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.814694 string2string-0.0.3.2.140/string2string/misc/
--rw-r--r--   0 machine    (501) staff       (20)      301 2023-03-20 20:18:31.000000 string2string-0.0.3.2.140/string2string/misc/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)     1095 2023-03-21 05:51:23.000000 string2string-0.0.3.2.140/string2string/misc/basic_functions.py
--rw-r--r--   0 machine    (501) staff       (20)     1189 2023-03-20 07:14:14.000000 string2string-0.0.3.2.140/string2string/misc/default_tokenizer.py
--rw-r--r--   0 machine    (501) staff       (20)     3425 2023-03-19 06:34:50.000000 string2string-0.0.3.2.140/string2string/misc/hash_functions.py
--rw-r--r--   0 machine    (501) staff       (20)     4394 2023-03-21 06:40:36.000000 string2string-0.0.3.2.140/string2string/misc/model_embeddings.py
--rw-r--r--   0 machine    (501) staff       (20)    10447 2023-03-20 04:28:45.000000 string2string-0.0.3.2.140/string2string/misc/plotting_functions.py
--rw-r--r--   0 machine    (501) staff       (20)    18031 2023-03-19 23:42:27.000000 string2string-0.0.3.2.140/string2string/misc/word_embeddings.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.817181 string2string-0.0.3.2.140/string2string/search/
--rw-r--r--   0 machine    (501) staff       (20)      247 2023-03-20 20:43:34.000000 string2string-0.0.3.2.140/string2string/search/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)    19203 2023-03-20 20:52:02.000000 string2string-0.0.3.2.140/string2string/search/classical.py
--rw-r--r--   0 machine    (501) staff       (20)    11337 2023-03-21 06:40:53.000000 string2string-0.0.3.2.140/string2string/search/faiss_search.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.819027 string2string-0.0.3.2.140/string2string/similarity/
--rw-r--r--   0 machine    (501) staff       (20)      257 2023-03-20 07:37:50.000000 string2string-0.0.3.2.140/string2string/similarity/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)    10528 2023-03-20 19:19:52.000000 string2string-0.0.3.2.140/string2string/similarity/bartscore.py
--rw-r--r--   0 machine    (501) staff       (20)    11218 2023-03-21 05:51:36.000000 string2string-0.0.3.2.140/string2string/similarity/bertscore.py
--rw-r--r--   0 machine    (501) staff       (20)     5072 2023-03-21 05:47:22.000000 string2string-0.0.3.2.140/string2string/similarity/classical.py
--rw-r--r--   0 machine    (501) staff       (20)     6724 2023-03-20 16:59:16.000000 string2string-0.0.3.2.140/string2string/similarity/cosine_similarity.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:26:19.809102 string2string-0.0.3.2.140/string2string.egg-info/
--rw-r--r--   0 machine    (501) staff       (20)      869 2023-03-21 07:26:19.000000 string2string-0.0.3.2.140/string2string.egg-info/PKG-INFO
--rw-r--r--   0 machine    (501) staff       (20)     1341 2023-03-21 07:26:19.000000 string2string-0.0.3.2.140/string2string.egg-info/SOURCES.txt
--rw-r--r--   0 machine    (501) staff       (20)        1 2023-03-21 07:26:19.000000 string2string-0.0.3.2.140/string2string.egg-info/dependency_links.txt
--rw-r--r--   0 machine    (501) staff       (20)       74 2023-03-21 07:26:19.000000 string2string-0.0.3.2.140/string2string.egg-info/requires.txt
--rw-r--r--   0 machine    (501) staff       (20)       14 2023-03-21 07:26:19.000000 string2string-0.0.3.2.140/string2string.egg-info/top_level.txt
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.428949 string2string-0.0.3.2.141/
+-rw-r--r--   0 machine    (501) staff       (20)     1055 2022-07-17 23:18:45.000000 string2string-0.0.3.2.141/LICENSE.txt
+-rw-r--r--   0 machine    (501) staff       (20)      869 2023-03-21 07:29:21.428758 string2string-0.0.3.2.141/PKG-INFO
+-rw-r--r--   0 machine    (501) staff       (20)     2290 2023-03-21 05:43:43.000000 string2string-0.0.3.2.141/README.md
+-rw-r--r--   0 machine    (501) staff       (20)       38 2023-03-21 07:29:21.429007 string2string-0.0.3.2.141/setup.cfg
+-rw-r--r--   0 machine    (501) staff       (20)     1324 2023-03-21 07:29:10.000000 string2string-0.0.3.2.141/setup.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.419016 string2string-0.0.3.2.141/string2string/
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-26 19:59:48.000000 string2string-0.0.3.2.141/string2string/__init__.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.420153 string2string-0.0.3.2.141/string2string/alignment/
+-rw-r--r--   0 machine    (501) staff       (20)      262 2023-03-19 23:42:10.000000 string2string-0.0.3.2.141/string2string/alignment/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)    56008 2023-03-21 05:54:31.000000 string2string-0.0.3.2.141/string2string/alignment/classical.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.421296 string2string-0.0.3.2.141/string2string/compression/
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:24:13.000000 string2string-0.0.3.2.141/string2string/compression/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:29:22.000000 string2string-0.0.3.2.141/string2string/compression/arithmetic_encoding.py
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:25:14.000000 string2string-0.0.3.2.141/string2string/compression/bpe.py
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:27:16.000000 string2string-0.0.3.2.141/string2string/compression/burrows_wheeler_transform.py
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:28:08.000000 string2string-0.0.3.2.141/string2string/compression/huffman_coding.py
+-rw-r--r--   0 machine    (501) staff       (20)        0 2023-02-27 06:25:12.000000 string2string-0.0.3.2.141/string2string/compression/lempel_ziv.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.421767 string2string-0.0.3.2.141/string2string/distance/
+-rw-r--r--   0 machine    (501) staff       (20)      231 2023-03-20 16:30:22.000000 string2string-0.0.3.2.141/string2string/distance/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)    21428 2023-03-21 05:51:18.000000 string2string-0.0.3.2.141/string2string/distance/classical.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.423125 string2string-0.0.3.2.141/string2string/metrics/
+-rw-r--r--   0 machine    (501) staff       (20)      177 2023-03-19 06:26:11.000000 string2string-0.0.3.2.141/string2string/metrics/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)     1693 2023-03-19 06:35:15.000000 string2string-0.0.3.2.141/string2string/metrics/exact_match.py
+-rw-r--r--   0 machine    (501) staff       (20)     4997 2023-03-21 05:51:11.000000 string2string-0.0.3.2.141/string2string/metrics/rouge.py
+-rw-r--r--   0 machine    (501) staff       (20)     4282 2023-03-19 23:42:11.000000 string2string-0.0.3.2.141/string2string/metrics/sbleu.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.425392 string2string-0.0.3.2.141/string2string/misc/
+-rw-r--r--   0 machine    (501) staff       (20)      301 2023-03-20 20:18:31.000000 string2string-0.0.3.2.141/string2string/misc/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)     1095 2023-03-21 05:51:23.000000 string2string-0.0.3.2.141/string2string/misc/basic_functions.py
+-rw-r--r--   0 machine    (501) staff       (20)     1189 2023-03-20 07:14:14.000000 string2string-0.0.3.2.141/string2string/misc/default_tokenizer.py
+-rw-r--r--   0 machine    (501) staff       (20)     3425 2023-03-19 06:34:50.000000 string2string-0.0.3.2.141/string2string/misc/hash_functions.py
+-rw-r--r--   0 machine    (501) staff       (20)     4394 2023-03-21 06:40:36.000000 string2string-0.0.3.2.141/string2string/misc/model_embeddings.py
+-rw-r--r--   0 machine    (501) staff       (20)    10447 2023-03-20 04:28:45.000000 string2string-0.0.3.2.141/string2string/misc/plotting_functions.py
+-rw-r--r--   0 machine    (501) staff       (20)    18031 2023-03-19 23:42:27.000000 string2string-0.0.3.2.141/string2string/misc/word_embeddings.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.426691 string2string-0.0.3.2.141/string2string/search/
+-rw-r--r--   0 machine    (501) staff       (20)      247 2023-03-20 20:43:34.000000 string2string-0.0.3.2.141/string2string/search/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)    19203 2023-03-20 20:52:02.000000 string2string-0.0.3.2.141/string2string/search/classical.py
+-rw-r--r--   0 machine    (501) staff       (20)    11337 2023-03-21 06:40:53.000000 string2string-0.0.3.2.141/string2string/search/faiss_search.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.428324 string2string-0.0.3.2.141/string2string/similarity/
+-rw-r--r--   0 machine    (501) staff       (20)      257 2023-03-20 07:37:50.000000 string2string-0.0.3.2.141/string2string/similarity/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)    10528 2023-03-20 19:19:52.000000 string2string-0.0.3.2.141/string2string/similarity/bartscore.py
+-rw-r--r--   0 machine    (501) staff       (20)    11218 2023-03-21 05:51:36.000000 string2string-0.0.3.2.141/string2string/similarity/bertscore.py
+-rw-r--r--   0 machine    (501) staff       (20)     5072 2023-03-21 05:47:22.000000 string2string-0.0.3.2.141/string2string/similarity/classical.py
+-rw-r--r--   0 machine    (501) staff       (20)     6724 2023-03-20 16:59:16.000000 string2string-0.0.3.2.141/string2string/similarity/cosine_similarity.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-03-21 07:29:21.419717 string2string-0.0.3.2.141/string2string.egg-info/
+-rw-r--r--   0 machine    (501) staff       (20)      869 2023-03-21 07:29:21.000000 string2string-0.0.3.2.141/string2string.egg-info/PKG-INFO
+-rw-r--r--   0 machine    (501) staff       (20)     1341 2023-03-21 07:29:21.000000 string2string-0.0.3.2.141/string2string.egg-info/SOURCES.txt
+-rw-r--r--   0 machine    (501) staff       (20)        1 2023-03-21 07:29:21.000000 string2string-0.0.3.2.141/string2string.egg-info/dependency_links.txt
+-rw-r--r--   0 machine    (501) staff       (20)       78 2023-03-21 07:29:21.000000 string2string-0.0.3.2.141/string2string.egg-info/requires.txt
+-rw-r--r--   0 machine    (501) staff       (20)       14 2023-03-21 07:29:21.000000 string2string-0.0.3.2.141/string2string.egg-info/top_level.txt
```

### Comparing `string2string-0.0.3.2.140/LICENSE.txt` & `string2string-0.0.3.2.141/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/PKG-INFO` & `string2string-0.0.3.2.141/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string2string
-Version: 0.0.3.2.140
+Version: 0.0.3.2.141
 Summary: String-to-String Algorithms for Natural Language Processing
 Home-page: https://github.com/suzgunmirac/string2string
 Author: Mirac Suzgun
 Author-email: msuzgun@cs.stanford.edu
 License: MIT
 Keywords: string matching,pattern matching,edit distance,string to string correction,string to string matching,Levenshtein edit distance,Hamming distance,Damerau-Levenshtein distance,Jaro-Winkler distance,longest common subsequence,longest common substring,dynamic programming,approximate string matching
 Platform: UNKNOWN
```

### Comparing `string2string-0.0.3.2.140/README.md` & `string2string-0.0.3.2.141/README.md`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/setup.py` & `string2string-0.0.3.2.141/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
     name="string2string",
-    version="0.0.3.2.140",
+    version="0.0.3.2.141",
     description="String-to-String Algorithms for Natural Language Processing",
     url="https://github.com/suzgunmirac/string2string",
     author="Mirac Suzgun",
     author_email="msuzgun@cs.stanford.edu",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "torch",
         "numpy",
         "transformers",
         "datasets",
-        "faiss==1.7.3",
+        "faiss-cpu==1.7.3",
         "bert_score",
         "fasttext",
         "pandas",
     ],
     tests_require=["pytest"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
```

### Comparing `string2string-0.0.3.2.140/string2string/alignment/classical.py` & `string2string-0.0.3.2.141/string2string/alignment/classical.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/distance/classical.py` & `string2string-0.0.3.2.141/string2string/distance/classical.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/metrics/exact_match.py` & `string2string-0.0.3.2.141/string2string/metrics/exact_match.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/metrics/rouge.py` & `string2string-0.0.3.2.141/string2string/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/metrics/sbleu.py` & `string2string-0.0.3.2.141/string2string/metrics/sbleu.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/misc/basic_functions.py` & `string2string-0.0.3.2.141/string2string/misc/basic_functions.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/misc/default_tokenizer.py` & `string2string-0.0.3.2.141/string2string/misc/default_tokenizer.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/misc/hash_functions.py` & `string2string-0.0.3.2.141/string2string/misc/hash_functions.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/misc/model_embeddings.py` & `string2string-0.0.3.2.141/string2string/misc/model_embeddings.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/misc/plotting_functions.py` & `string2string-0.0.3.2.141/string2string/misc/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/misc/word_embeddings.py` & `string2string-0.0.3.2.141/string2string/misc/word_embeddings.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/search/classical.py` & `string2string-0.0.3.2.141/string2string/search/classical.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/search/faiss_search.py` & `string2string-0.0.3.2.141/string2string/search/faiss_search.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/similarity/bartscore.py` & `string2string-0.0.3.2.141/string2string/similarity/bartscore.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/similarity/bertscore.py` & `string2string-0.0.3.2.141/string2string/similarity/bertscore.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/similarity/classical.py` & `string2string-0.0.3.2.141/string2string/similarity/classical.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string/similarity/cosine_similarity.py` & `string2string-0.0.3.2.141/string2string/similarity/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `string2string-0.0.3.2.140/string2string.egg-info/PKG-INFO` & `string2string-0.0.3.2.141/string2string.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string2string
-Version: 0.0.3.2.140
+Version: 0.0.3.2.141
 Summary: String-to-String Algorithms for Natural Language Processing
 Home-page: https://github.com/suzgunmirac/string2string
 Author: Mirac Suzgun
 Author-email: msuzgun@cs.stanford.edu
 License: MIT
 Keywords: string matching,pattern matching,edit distance,string to string correction,string to string matching,Levenshtein edit distance,Hamming distance,Damerau-Levenshtein distance,Jaro-Winkler distance,longest common subsequence,longest common substring,dynamic programming,approximate string matching
 Platform: UNKNOWN
```

### Comparing `string2string-0.0.3.2.140/string2string.egg-info/SOURCES.txt` & `string2string-0.0.3.2.141/string2string.egg-info/SOURCES.txt`

 * *Files identical despite different names*

