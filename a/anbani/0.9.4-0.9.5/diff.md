# Comparing `tmp/anbani-0.9.4.tar.gz` & `tmp/anbani-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anbani-0.9.4.tar", last modified: Fri Apr 28 05:30:35 2023, max compression
+gzip compressed data, was "anbani-0.9.5.tar", last modified: Fri Apr 28 05:56:41 2023, max compression
```

## Comparing `anbani-0.9.4.tar` & `anbani-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.044230 anbani-0.9.4/
--rw-r--r--   0 george    (1000) george    (1000)    35149 2022-07-12 06:28:39.000000 anbani-0.9.4/LICENSE
--rw-r--r--   0 george    (1000) george    (1000)       21 2022-07-12 06:28:39.000000 anbani-0.9.4/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)     3271 2023-04-28 05:30:35.044230 anbani-0.9.4/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     2738 2023-04-28 05:21:14.000000 anbani-0.9.4/README.md
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.030230 anbani-0.9.4/anbani/
--rw-r--r--   0 george    (1000) george    (1000)       66 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/__init__.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.032230 anbani-0.9.4/anbani/core/
--rw-r--r--   0 george    (1000) george    (1000)        0 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/core/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     3581 2022-07-12 06:35:34.000000 anbani-0.9.4/anbani/core/converter.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.036230 anbani-0.9.4/anbani/data/
--rw-r--r--   0 george    (1000) george    (1000)  2459360 2023-04-27 13:32:54.000000 anbani-0.9.4/anbani/data/ambigram_nc1_len10.csv
--rw-r--r--   0 george    (1000) george    (1000)   416348 2023-04-27 13:32:54.000000 anbani-0.9.4/anbani/data/ambigram_nc5_len7.csv
--rw-r--r--   0 george    (1000) george    (1000)    16939 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/data/georgian_contractions.csv
--rw-r--r--   0 george    (1000) george    (1000)    11296 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/data/letters.js
--rw-r--r--   0 george    (1000) george    (1000)  5781776 2023-04-27 13:33:08.000000 anbani-0.9.4/anbani/data/wordlist.csv
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.043230 anbani-0.9.4/anbani/nlp/
--rw-r--r--   0 george    (1000) george    (1000)       16 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)      770 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/contractions.py
--rw-r--r--   0 george    (1000) george    (1000)     5068 2023-04-28 05:27:48.000000 anbani-0.9.4/anbani/nlp/georgianisation.py
--rw-r--r--   0 george    (1000) george    (1000)     1681 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/preprocessing.py
--rw-r--r--   0 george    (1000) george    (1000)     1306 2022-07-12 06:28:39.000000 anbani-0.9.4/anbani/nlp/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:30:35.031230 anbani-0.9.4/anbani.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)     3271 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)      548 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)       32 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-28 05:30:34.000000 anbani-0.9.4/anbani.egg-info/top_level.txt
--rw-r--r--   0 george    (1000) george    (1000)      103 2023-04-28 05:30:35.044230 anbani-0.9.4/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      879 2023-04-28 05:28:52.000000 anbani-0.9.4/setup.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:56:41.590501 anbani-0.9.5/
+-rw-r--r--   0 george    (1000) george    (1000)    35149 2022-07-12 06:28:39.000000 anbani-0.9.5/LICENSE
+-rw-r--r--   0 george    (1000) george    (1000)       21 2022-07-12 06:28:39.000000 anbani-0.9.5/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)     3271 2023-04-28 05:56:41.590501 anbani-0.9.5/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)     2738 2023-04-28 05:21:14.000000 anbani-0.9.5/README.md
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:56:41.574501 anbani-0.9.5/anbani/
+-rw-r--r--   0 george    (1000) george    (1000)       66 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/__init__.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:56:41.575501 anbani-0.9.5/anbani/core/
+-rw-r--r--   0 george    (1000) george    (1000)        0 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/core/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     3581 2022-07-12 06:35:34.000000 anbani-0.9.5/anbani/core/converter.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:56:41.581501 anbani-0.9.5/anbani/data/
+-rw-r--r--   0 george    (1000) george    (1000)  2459360 2023-04-27 13:32:54.000000 anbani-0.9.5/anbani/data/ambigram_nc1_len10.csv
+-rw-r--r--   0 george    (1000) george    (1000)   416348 2023-04-27 13:32:54.000000 anbani-0.9.5/anbani/data/ambigram_nc5_len7.csv
+-rw-r--r--   0 george    (1000) george    (1000)    16939 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/data/georgian_contractions.csv
+-rw-r--r--   0 george    (1000) george    (1000)    11296 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/data/letters.js
+-rw-r--r--   0 george    (1000) george    (1000)  5781776 2023-04-27 13:33:08.000000 anbani-0.9.5/anbani/data/wordlist.csv
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:56:41.590501 anbani-0.9.5/anbani/nlp/
+-rw-r--r--   0 george    (1000) george    (1000)       16 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/nlp/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)      770 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/nlp/contractions.py
+-rw-r--r--   0 george    (1000) george    (1000)     5653 2023-04-28 05:53:18.000000 anbani-0.9.5/anbani/nlp/georgianisation.py
+-rw-r--r--   0 george    (1000) george    (1000)     1681 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/nlp/preprocessing.py
+-rw-r--r--   0 george    (1000) george    (1000)     1306 2022-07-12 06:28:39.000000 anbani-0.9.5/anbani/nlp/utils.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:56:41.575501 anbani-0.9.5/anbani.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)     3271 2023-04-28 05:56:40.000000 anbani-0.9.5/anbani.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)      548 2023-04-28 05:56:41.000000 anbani-0.9.5/anbani.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-28 05:56:40.000000 anbani-0.9.5/anbani.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)       32 2023-04-28 05:56:41.000000 anbani-0.9.5/anbani.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-28 05:56:41.000000 anbani-0.9.5/anbani.egg-info/top_level.txt
+-rw-r--r--   0 george    (1000) george    (1000)      103 2023-04-28 05:56:41.591502 anbani-0.9.5/setup.cfg
+-rw-r--r--   0 george    (1000) george    (1000)      879 2023-04-28 05:55:28.000000 anbani-0.9.5/setup.py
```

### Comparing `anbani-0.9.4/LICENSE` & `anbani-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/PKG-INFO` & `anbani-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anbani
-Version: 0.9.4
+Version: 0.9.5
 Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.
 Home-page: https://github.com/anbani/anbani.py
 Author: George Gach
 Author-email: georgegach@outlook.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anbani-0.9.4/README.md` & `anbani-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/core/converter.py` & `anbani-0.9.5/anbani/core/converter.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/data/ambigram_nc1_len10.csv` & `anbani-0.9.5/anbani/data/ambigram_nc1_len10.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/data/ambigram_nc5_len7.csv` & `anbani-0.9.5/anbani/data/ambigram_nc5_len7.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/data/georgian_contractions.csv` & `anbani-0.9.5/anbani/data/georgian_contractions.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/data/letters.js` & `anbani-0.9.5/anbani/data/letters.js`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/data/wordlist.csv` & `anbani-0.9.5/anbani/data/wordlist.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/nlp/contractions.py` & `anbani-0.9.5/anbani/nlp/contractions.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/nlp/georgianisation.py` & `anbani-0.9.5/anbani/nlp/georgianisation.py`

 * *Files 18% similar despite different names*

```diff
@@ -90,14 +90,31 @@
     ('y', 'ყ'),
     ('Y', 'ყ'),
     ('z', 'ზ'),
     ('Z', 'ძ')
 ]
 
 
+def _decapitalise(text):
+    sentences = re.split(r'([.!?]\s*)', text)
+    
+    def lowercase_first_word(sentence):
+        words = sentence.split(" ", 1)
+        words[0] = words[0].lower()
+        return " ".join(words)
+    
+    processed_sentences = [lowercase_first_word(sentence) for sentence in sentences[::2]]
+    result = ''.join([
+        processed_sentences[i] + (sentences[i * 2 + 1] if i * 2 + 1 < len(sentences) else '')
+        for i in range(len(processed_sentences))
+    ])
+
+    return result
+
+
 def _transliterate_diphthongs(sentence):
     for dfrom, dto in diphthong_mapping:
         sentence = sentence.replace(dfrom, dto)
 
     return sentence
 
 
@@ -141,28 +158,30 @@
 
 
 def georgianise_balanced(sentence):
     """
     Smarter than fastest, faster than Smartest. Uses 10K tokens.
     """
     
+    sentence = _decapitalise(sentence)
     sentence = _chevron_wrap(sentence)
     sentence = _transliterate_diphthongs(sentence)
     sentence = _transliterate_letters(sentence, even_ambiguous=False)
     sentence = _transliterate_ngrams(sentence, ambigrams=ambigrams_balanced)
     sentence = _chevron_unwrap(sentence)
 
     return sentence    
 
 
 def georgianise_accurate(sentence):
     """
     Most accurate implementation of Georgianisation without applying comprehensive million row wordlist in brute force. Uses 50K tokens.
     """
-    
+
+    sentence = _decapitalise(sentence)
     sentence = _chevron_wrap(sentence)
     sentence = _transliterate_diphthongs(sentence)
     sentence = _transliterate_letters(sentence, even_ambiguous=False)
     sentence = _transliterate_ngrams(sentence, ambigrams=ambigrams_accurate)
     sentence = _chevron_unwrap(sentence)
 
     return sentence
```

### Comparing `anbani-0.9.4/anbani/nlp/preprocessing.py` & `anbani-0.9.5/anbani/nlp/preprocessing.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani/nlp/utils.py` & `anbani-0.9.5/anbani/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/anbani.egg-info/PKG-INFO` & `anbani-0.9.5/anbani.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anbani
-Version: 0.9.4
+Version: 0.9.5
 Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.
 Home-page: https://github.com/anbani/anbani.py
 Author: George Gach
 Author-email: georgegach@outlook.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anbani-0.9.4/anbani.egg-info/SOURCES.txt` & `anbani-0.9.5/anbani.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anbani-0.9.4/setup.py` & `anbani-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='anbani',
-    version='0.9.4',
+    version='0.9.5',
     author="George Gach",
     author_email="georgegach@outlook.com",
     description="Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.",
     license='GPL',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anbani/anbani.py",
```

