# Comparing `tmp/fhnw_nlp_utils-0.6.7-py3-none-any.whl.zip` & `tmp/fhnw_nlp_utils-0.6.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 23949 bytes, number of entries: 18
+Zip file size: 23950 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/nlp/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/__init__.py
 -rw-r--r--  2.0 unx      144 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/colab.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Aug-14 09:43 fhnw/nlp/utils/defaults.py
--rw-r--r--  2.0 unx     6880 b- defN 22-Aug-14 09:42 fhnw/nlp/utils/normalize.py
+-rw-r--r--  2.0 unx     6900 b- defN 23-Apr-26 17:08 fhnw/nlp/utils/normalize.py
 -rw-r--r--  2.0 unx    37887 b- defN 23-Mar-12 20:31 fhnw/nlp/utils/params.py
 -rw-r--r--  2.0 unx     9537 b- defN 22-Dec-12 20:18 fhnw/nlp/utils/ploting.py
 -rw-r--r--  2.0 unx     2262 b- defN 22-Aug-25 17:41 fhnw/nlp/utils/preprocess.py
 -rw-r--r--  2.0 unx    10048 b- defN 21-Nov-14 18:34 fhnw/nlp/utils/processing.py
 -rw-r--r--  2.0 unx     6838 b- defN 21-Nov-03 20:09 fhnw/nlp/utils/storage.py
 -rw-r--r--  2.0 unx     3346 b- defN 22-Oct-05 05:11 fhnw/nlp/utils/system.py
 -rw-r--r--  2.0 unx     3212 b- defN 22-Aug-10 15:41 fhnw/nlp/utils/text.py
 -rw-r--r--  2.0 unx     7656 b- defN 23-Apr-19 05:05 fhnw/nlp/utils/transformers.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1459 b- defN 23-Apr-19 05:21 fhnw_nlp_utils-0.6.7.dist-info/RECORD
-18 files, 92918 bytes uncompressed, 21559 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx     1298 b- defN 23-Apr-28 04:28 fhnw_nlp_utils-0.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 04:28 fhnw_nlp_utils-0.6.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-28 04:28 fhnw_nlp_utils-0.6.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1459 b- defN 23-Apr-28 04:28 fhnw_nlp_utils-0.6.8.dist-info/RECORD
+18 files, 92938 bytes uncompressed, 21560 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: fhnw/nlp/utils/text.py
 Comment: 
 
 Filename: fhnw/nlp/utils/transformers.py
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.7.dist-info/METADATA
+Filename: fhnw_nlp_utils-0.6.8.dist-info/METADATA
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.7.dist-info/WHEEL
+Filename: fhnw_nlp_utils-0.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.7.dist-info/top_level.txt
+Filename: fhnw_nlp_utils-0.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.7.dist-info/RECORD
+Filename: fhnw_nlp_utils-0.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fhnw/nlp/utils/normalize.py

```diff
@@ -62,20 +62,20 @@
     elif is_iterable(text):
         word_tokens = text
     else:
         raise TypeError("Only string or iterable (e.g. list) is supported. Received a "+ str(type(text)))
 
     if word_splitter is not None:
         # with python 3.8
-        #return [stemmer(lower) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if (lower := split.lower()) not in stopwords]
-        return [stemmer(split.lower()) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if split.lower() not in stopwords]
+        #return [stemmer.stem(lower) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if (lower := split.lower()) not in stopwords]
+        return [stemmer.stem(split.lower()) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if split.lower() not in stopwords]
     else:
         # with python 3.8
-        #return [stemmer(lower) for word in word_tokens if (lower := word.lower()) not in stopwords]
-        return [stemmer(word.lower()) for word in word_tokens if word.lower() not in stopwords]
+        #return [stemmer.stem(lower) for word in word_tokens if (lower := word.lower()) not in stopwords]
+        return [stemmer.stem(word.lower()) for word in word_tokens if word.lower() not in stopwords]
 
 
 def tokenize_lemma(text, stopwords, lemmanizer, keep_ners=False):
     """Tokenizes, lowercases and lemmatizes a text and removes stopwords
 
     Parameters
     ----------
```

## Comparing `fhnw_nlp_utils-0.6.7.dist-info/METADATA` & `fhnw_nlp_utils-0.6.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhnw-nlp-utils
-Version: 0.6.7
+Version: 0.6.8
 Summary: Utilities for NLP courses taught at FHNW.
 Home-page: http://github.com/markif/fhnw-nlp-utils
 Author: Fabian
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

## Comparing `fhnw_nlp_utils-0.6.7.dist-info/RECORD` & `fhnw_nlp_utils-0.6.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 fhnw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fhnw/nlp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fhnw/nlp/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fhnw/nlp/utils/colab.py,sha256=5XiWtCz9R_MTtGC76BJgCNhdJPp2eGNYinv5C5NAK4A,144
 fhnw/nlp/utils/defaults.py,sha256=H6IpvtUWZ2GLFyQkFBGO-gcbYhTzzLdZd772ecg5_nk,2254
-fhnw/nlp/utils/normalize.py,sha256=HZKBG8NUu2PjfHTQODuOh2omozVvekYciV3xsN17sdo,6880
+fhnw/nlp/utils/normalize.py,sha256=2ianou8ZSnKotS5oKFZgdgm1cWKIQKTpdpQbq6ZxZg4,6900
 fhnw/nlp/utils/params.py,sha256=xavHoG_CMmygKGp3lwHqPbZUpfnrjdLjZPII2fiZPjE,37887
 fhnw/nlp/utils/ploting.py,sha256=8ya50BauVgWfRh7X7V9urU5SCvd7RSF7INhCgKHdzzc,9537
 fhnw/nlp/utils/preprocess.py,sha256=FDy6HAYS3OjKue9kVigh7Cg84gc3rju5Zu0WuOLVoq0,2262
 fhnw/nlp/utils/processing.py,sha256=73R2Vy4tMzXpbjSbck7xZFDigaA3cjuLxbe-ZXxs_uc,10048
 fhnw/nlp/utils/storage.py,sha256=F3C19qp9x2cGHnE0mdLVQxLLqBzgtFUCWZSGtzmk_yw,6838
 fhnw/nlp/utils/system.py,sha256=yRphzlhw34C8qyl-sgUSbz56_Ckr8G-tsRJkko-pv-U,3346
 fhnw/nlp/utils/text.py,sha256=ElaWYdl_7YkHc_IHJyEUZPvKgcADTcbEBEL1FO5emME,3212
 fhnw/nlp/utils/transformers.py,sha256=Jge66cuppFN3llTo38FSKvjuuqbHtAZXnfgeGj6qWe4,7656
-fhnw_nlp_utils-0.6.7.dist-info/METADATA,sha256=Qd31vHy-smo76PieXLtyJ2rbTCYeS1OlOHwcOYvIPBo,1298
-fhnw_nlp_utils-0.6.7.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-fhnw_nlp_utils-0.6.7.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
-fhnw_nlp_utils-0.6.7.dist-info/RECORD,,
+fhnw_nlp_utils-0.6.8.dist-info/METADATA,sha256=-IDJU2TsA_omFKbUqtlJhaDU-qJHNVc4_FAoQ6dbg0U,1298
+fhnw_nlp_utils-0.6.8.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+fhnw_nlp_utils-0.6.8.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
+fhnw_nlp_utils-0.6.8.dist-info/RECORD,,
```

