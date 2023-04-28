# Comparing `tmp/IPAkor-2.5.1.tar.gz` & `tmp/IPAkor-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.5.1.tar", last modified: Thu Apr 27 21:27:14 2023, max compression
+gzip compressed data, was "IPAkor-2.5.2.tar", last modified: Fri Apr 28 06:29:44 2023, max compression
```

## Comparing `IPAkor-2.5.1.tar` & `IPAkor-2.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.611902 IPAkor-2.5.1/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.609421 IPAkor-2.5.1/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.5.1/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     3969 2023-04-27 20:40:43.000000 IPAkor-2.5.1/IPAkor/border_maker.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.611272 IPAkor-2.5.1/IPAkor/static/
--rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.5.1/IPAkor/static/final_trans.csv
--rw-r--r--   0 eneminova   (501) staff       (20)    15016 2023-04-27 21:27:08.000000 IPAkor-2.5.1/IPAkor/transcription.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:27:14.611005 IPAkor-2.5.1/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 21:27:14.000000 IPAkor-2.5.1/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.5.1/MANIFEST.in
--rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 21:27:14.612030 IPAkor-2.5.1/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.5.1/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 21:27:14.612583 IPAkor-2.5.1/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      585 2023-04-27 21:25:10.000000 IPAkor-2.5.1/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:29:44.433744 IPAkor-2.5.2/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:29:44.428325 IPAkor-2.5.2/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 22:17:02.000000 IPAkor-2.5.2/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     3962 2023-04-28 06:22:19.000000 IPAkor-2.5.2/IPAkor/border_maker.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:29:44.430921 IPAkor-2.5.2/IPAkor/static/
+-rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-27 22:17:02.000000 IPAkor-2.5.2/IPAkor/static/final_trans.csv
+-rw-r--r--   0 eneminova   (501) staff       (20)    14967 2023-04-28 06:28:48.000000 IPAkor-2.5.2/IPAkor/transcription.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:29:44.430552 IPAkor-2.5.2/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-28 06:29:44.000000 IPAkor-2.5.2/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-28 06:29:44.000000 IPAkor-2.5.2/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-28 06:29:44.000000 IPAkor-2.5.2/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-28 06:29:44.000000 IPAkor-2.5.2/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-28 06:29:44.000000 IPAkor-2.5.2/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 22:17:02.000000 IPAkor-2.5.2/MANIFEST.in
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-28 06:29:44.433910 IPAkor-2.5.2/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     3633 2023-04-27 22:12:54.000000 IPAkor-2.5.2/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-28 06:29:44.434384 IPAkor-2.5.2/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      585 2023-04-28 06:29:05.000000 IPAkor-2.5.2/setup.py
```

### Comparing `IPAkor-2.5.1/IPAkor/border_maker.py` & `IPAkor-2.5.2/IPAkor/border_maker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# ЭТОТ КОД ДЕЛАЕТ РАЗНЫЕ ВИДЫ ГРАНИЦ МЕЖДУ СЛОГАМИ, КЛИТИКАМИ,
-# СЛОВАМИ И СИНТАГМАМИ
-# подробнее: https://colab.research.google.com/drive/1F6rf_Difpv1sYtp2X1PNsvUi3ARu0b07#scrollTo=KE5t4CsRGmzl
+# ЭТОТ КОД ДЕЛАЕТ РАЗНЫЕ ВИДЫ ГРАНИЦ МЕЖДУ СЛОГАМИ, КЛИТИКАМИ, СЛОВАМИ И СИНТАГМАМИ
 from konlpy.tag import Twitter
 from konlpy.tag import Kkma
 import csv
 import re
 import wget
 
 
@@ -94,7 +92,10 @@
             elif entity[1] in bad:
                 pass
 
             else:
                 good_text += self.intruser(entity[0]) + '#'
 
         return good_text.strip(' /#') + ' / '
+
+separation = BorderMaker()
+print(separation.separator('이해할수 있어요? 설악산의 높은 뭐예요?'))
```

### Comparing `IPAkor-2.5.1/IPAkor/static/final_trans.csv` & `IPAkor-2.5.2/IPAkor/static/final_trans.csv`

 * *Files identical despite different names*

### Comparing `IPAkor-2.5.1/IPAkor/transcription.py` & `IPAkor-2.5.2/IPAkor/transcription.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         # 덕분에
         given = given.replace('tʌk-pun-e', 't͈ʌk-pun-e')
         return given
 
     def palatalization(self, given):  # must be second!!
         to_pal = ['k', 'g', 'l', 'ɾ', 'm', 'p', 's', 'ŋ', 'cʰ', 'kʰ', 'tʰ', 'pʰ',
-                  't', 'n', 'h', 'k͈', 't͈', 'p͈', 's͈', 'c͈']
+                  't', 'n', 'h', 'k͈', 't͈', 'p͈', 's͈', 'c͈', 'ɦ']
 
         front_row = ['i', 'e']
 
         for tp in to_pal:
             # гласные переднего ряда
             for fr in front_row:
                 given = given.replace(tp + '-' + fr, tp + 'ʲ-' + fr)
@@ -237,15 +237,15 @@
 
                 elif chunks[i][-1] in final_sonor and chunks[i + 1][0] == 'ɾ':
                     chunks[i + 1] = 'n' + chunks[i + 1][1:]
             given = s.join(chunks)
 
         return given
 
-    def coronal_asim(self, given):
+    def coronal_assim(self, given):
         # ассимиляция переднеязычных
 
         seps = ['-', '#']
         coronals = ['t', 't͈', 'tʰ', 's', 's͈']
 
         labial = ['m', 'p', 'pʰ', 'p͈']
         post_alveolar = ['cʰ', 'c', 'c͈']
@@ -279,66 +279,68 @@
                     chunks[i] = chunks[i][:-1] + 'ŋ'
 
                 elif chunks[i][-1] in post_alveolar and chunks[i + 1][0] in velars:
                     chunks[i] = chunks[i][:-1] + 'k'
             given = s.join(chunks)
 
         return given
-
+      
+      
     def patchims(self, given):
         # чтение патчимов
         seps = ['-', '#']
         vowels = ['ɐ', 'ʌ', 'o', 'ɨ', 'u', 'i', 'ɛ', 'e', 'ɰi']
         excepted = {'nʌlb': 'nʌp', 'pɐlb': 'pɐp'}
-        first = {'ks': 'k', 'lg': 'k', 'nɟ': 'n', 'nh': 'n', 'lm': 'm', 'lb': 'l', 'ls': 'l', 'ltʰ': 'l', 'lh': 'l',
+        first = {'ks': 'k', 'lg': 'k', 'nɟ': 'n', 'nh': 'n', 'lm': 'm', 
+                 'lb': 'l', 'ls': 'l', 'ltʰ': 'l', 'lh': 'l',
                  'lpʰ': 'p', 'ps': 'p'}
         second = {'t͈': 't', 'tʰ': 't', 's': 't', 's͈': 't', 'cʰ': 't', 'c': 't', 'c͈': 't', 'h': 't'}
         # конец слога перед согласной
         for s in seps:
             chunks = given.split(s)
             for i in range(len(chunks) - 1):
+      
                 if chunks[i + 1][0] not in vowels:
                     for root in excepted.keys():  # проверка на исключения
                         if root in chunks[i]:
                             chunks[i] = excepted[root]
                     for patchim in first.keys():
-                        if patchim in chunks[i][-3:]:
+                        if chunks[i].endswith(patchim):
                             chunks[i] = chunks[i].replace(patchim, first[patchim])
                     for patchim in second.keys():
-                        if patchim in chunks[i][-2:]:
+                        if chunks[i].endswith(patchim):
                             chunks[i] = chunks[i].replace(patchim, second[patchim])
             given = s.join(chunks)
         # абсолютный конец
         for root in excepted.keys():
-            given = given.replace(root + '/', excepted[root] + '/')
+            given = given.replace(root + ' / ', excepted[root] + ' / ')
         for patchim in first.keys():
-            given = given.replace(patchim + '/', first[patchim] + '/')
+            given = given.replace(patchim + ' / ', first[patchim] + ' / ')
         for patchim in second.keys():
-            given = given.replace(patchim + '/', second[patchim] + '/')
+            given = given.replace(patchim + ' / ', second[patchim] + ' / ')
         return given
 
+
     def voicing_and_h(self, given):  # должно быть после патчимов
-        # фонетические переходы в позиции между гласными
+     # фонетические переходы в позиции между гласными
         vowels = ['ɐ', 'ʌ', 'o', 'ɨ', 'u', 'i', 'ɛ', 'e', 'ɰi']
         to_voice = {'c': 'ɟ', 'k': 'g', 't': 'd', 'p': 'b', 'h': 'ɦ',
                     'cʲ': 'ɟʲ', 'kʲ': 'gʲ', 'tʲ': 'dʲ', 'pʲ': 'bʲ'}
         for tv in to_voice.keys():
             voiced = to_voice[tv]
             for v1 in vowels:
                 for v2 in vowels:
                     given = given.replace(v1 + tv + '-' + v2, v1 + voiced + '-' + v2)
                     given = given.replace(v1 + '-' + tv + v2, v1 + '-' + voiced + v2)
-            given = given.replace('n' + '-' + tv, 'n' + '-' + voiced)
-            given = given.replace('m' + '-' + tv, 'm' + '-' + voiced)
-            given = given.replace('l' + '-' + tv, 'l' + '-' + voiced)
-            given = given.replace('ŋ' + '-' + tv, 'ŋ' + '-' + voiced)
-            given = given.replace('n' + '#' + tv, 'n' + '#' + voiced)
-            given = given.replace('m' + '#' + tv, 'm' + '#' + voiced)
-            given = given.replace('l' + '#' + tv, 'l' + '#' + voiced)
-            given = given.replace('ŋ' + '#' + tv, 'ŋ' + '#' + voiced)
+                
+                sonors = ['l', 'm', 'n', 'ŋ']         
+                if tv != 'h':
+                    for son in sonors:
+                        given = given.replace(son + '-' + tv + v1, son + '-' + voiced + v1)
+                        given = given.replace(son + '#' + tv + v1, son + '#' + voiced + v1)
 
         return given
 
     def pot(self, given):  # должно быть в самом конце
         obstr = ['k', 'p', 'c', 'cʰ', 'kʰ', 'tʰ',
                  'pʰ', 't', 'k͈', 't͈', 'p͈', 'c͈']
         for obs in obstr:
@@ -355,12 +357,16 @@
         given = self.palatalization(given)
         given = self.yi(given)
         given = self.liquids(given)
         given = self.aspiration(given)
         given = self.stop_assim(given)
         given = self.spirantization(given)
         given = self.sonor_assim(given)
-        given = self.coronal_asim(given)
+        given = self.coronal_assim(given)
         given = self.patchims(given)
         given = self.voicing_and_h(given)
         given = self.pot(given)
         return given
+
+
+separation = Transcription()
+print(separation.transcribe('아름다운 꽃과 나무를 보지 않다고 하니까 안하자'))
```

### Comparing `IPAkor-2.5.1/setup.py` & `IPAkor-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='IPAkor',
-                 version='2.5.1',
+                 version='2.5.2',
                  packages=['IPAkor'],
                  package_data={'IPAkor': ['static/final_trans.csv']},
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'Operating System :: OS Independent',
                      'Topic :: Scientific/Engineering'
                  ],
```

