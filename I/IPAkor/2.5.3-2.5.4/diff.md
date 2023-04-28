# Comparing `tmp/IPAkor-2.5.3.tar.gz` & `tmp/IPAkor-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.5.3.tar", last modified: Fri Apr 28 06:35:12 2023, max compression
+gzip compressed data, was "IPAkor-2.5.4.tar", last modified: Fri Apr 28 06:37:05 2023, max compression
```

## Comparing `IPAkor-2.5.3.tar` & `IPAkor-2.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:35:12.948032 IPAkor-2.5.3/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:35:12.943977 IPAkor-2.5.3/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 22:17:02.000000 IPAkor-2.5.3/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     4059 2023-04-28 06:35:03.000000 IPAkor-2.5.3/IPAkor/border_maker.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:35:12.945695 IPAkor-2.5.3/IPAkor/static/
--rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-27 22:17:02.000000 IPAkor-2.5.3/IPAkor/static/final_trans.csv
--rw-r--r--   0 eneminova   (501) staff       (20)    14967 2023-04-28 06:28:48.000000 IPAkor-2.5.3/IPAkor/transcription.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:35:12.945458 IPAkor-2.5.3/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-28 06:35:12.000000 IPAkor-2.5.3/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-28 06:35:12.000000 IPAkor-2.5.3/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-28 06:35:12.000000 IPAkor-2.5.3/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-28 06:35:12.000000 IPAkor-2.5.3/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-28 06:35:12.000000 IPAkor-2.5.3/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 22:17:02.000000 IPAkor-2.5.3/MANIFEST.in
--rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-28 06:35:12.948171 IPAkor-2.5.3/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     3633 2023-04-27 22:12:54.000000 IPAkor-2.5.3/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-28 06:35:12.948658 IPAkor-2.5.3/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      585 2023-04-28 06:35:03.000000 IPAkor-2.5.3/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:37:05.645925 IPAkor-2.5.4/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:37:05.641142 IPAkor-2.5.4/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 22:17:02.000000 IPAkor-2.5.4/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     3928 2023-04-28 06:36:55.000000 IPAkor-2.5.4/IPAkor/border_maker.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:37:05.643202 IPAkor-2.5.4/IPAkor/static/
+-rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-27 22:17:02.000000 IPAkor-2.5.4/IPAkor/static/final_trans.csv
+-rw-r--r--   0 eneminova   (501) staff       (20)    14837 2023-04-28 06:36:55.000000 IPAkor-2.5.4/IPAkor/transcription.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-28 06:37:05.642863 IPAkor-2.5.4/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-28 06:37:05.000000 IPAkor-2.5.4/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-28 06:37:05.000000 IPAkor-2.5.4/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-28 06:37:05.000000 IPAkor-2.5.4/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-28 06:37:05.000000 IPAkor-2.5.4/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-28 06:37:05.000000 IPAkor-2.5.4/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 22:17:02.000000 IPAkor-2.5.4/MANIFEST.in
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-28 06:37:05.646043 IPAkor-2.5.4/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     3633 2023-04-27 22:12:54.000000 IPAkor-2.5.4/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-28 06:37:05.646498 IPAkor-2.5.4/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      585 2023-04-28 06:36:55.000000 IPAkor-2.5.4/setup.py
```

### Comparing `IPAkor-2.5.3/IPAkor/border_maker.py` & `IPAkor-2.5.4/IPAkor/border_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,29 @@
         for char in word:
             ready_word += '-' + self.final_trans[char]
         return ready_word.strip('-')
 
     def separator(self, text: str) -> str:
         syll_dict = dict()
 
-        with open(self.filename) as csvfile:
+        with open(self.weight_path, 'r') as csvfile:
             spamreader = csv.reader(csvfile)
             sylls = list(spamreader)
             for s in sylls:
                 syll_dict[s[0]] = s[2]
 
         good_text = ' '
         twit_morph = self.twitter.pos(text, norm=True)
 
         lil_morphs = ('Josa', 'Suffix', 'Eomi', 'PreEomi')
         end_morphs = ('Exclamation', 'Conjunction', 'Eomi', 'PreEomi')
         bad = ('Foreign', 'Alpha', 'Number', 'Unknown', 'KoreanParticle',
                'Hashtag', 'ScreenName', 'Email', 'URL')
 
         for entity in twit_morph:
-            print(entity)
             if entity[1] in lil_morphs:
                 if entity[0] == '의':
                     good_text = good_text.strip(" /-#") + '-ɛ#'  # генитив
                 else:
                     good_text = good_text.strip(" /-#") + '-' + self.intruser(entity[0]) + '#'
 
             elif entity[1] in end_morphs:
@@ -94,10 +93,7 @@
             elif entity[1] in bad:
                 pass
 
             else:
                 good_text += self.intruser(entity[0]) + '#'
 
         return good_text.strip(' /#') + ' / '
-
-separation = BorderMaker()
-print(separation.separator('이해할수 있어요? 설악산의 높은 뭐예요?'))
```

### Comparing `IPAkor-2.5.3/IPAkor/static/final_trans.csv` & `IPAkor-2.5.4/IPAkor/static/final_trans.csv`

 * *Files identical despite different names*

### Comparing `IPAkor-2.5.3/IPAkor/transcription.py` & `IPAkor-2.5.4/IPAkor/transcription.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,12 +361,8 @@
         given = self.stop_assim(given)
         given = self.spirantization(given)
         given = self.sonor_assim(given)
         given = self.coronal_assim(given)
         given = self.patchims(given)
         given = self.voicing_and_h(given)
         given = self.pot(given)
-        return given
-
-
-separation = Transcription()
-print(separation.transcribe('아름다운 꽃과 나무를 보지 않다고 하니까 안하자'))
+        return given
```

### Comparing `IPAkor-2.5.3/README.md` & `IPAkor-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `IPAkor-2.5.3/setup.py` & `IPAkor-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='IPAkor',
-                 version='2.5.3',
+                 version='2.5.4',
                  packages=['IPAkor'],
                  package_data={'IPAkor': ['static/final_trans.csv']},
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'Operating System :: OS Independent',
                      'Topic :: Scientific/Engineering'
                  ],
```

