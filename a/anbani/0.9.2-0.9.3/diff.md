# Comparing `tmp/anbani-0.9.2.tar.gz` & `tmp/anbani-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anbani-0.9.2.tar", last modified: Tue Jul 12 06:39:26 2022, max compression
+gzip compressed data, was "anbani-0.9.3.tar", last modified: Fri Apr 28 05:18:19 2023, max compression
```

## Comparing `anbani-0.9.2.tar` & `anbani-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2022-07-12 06:39:26.240837 anbani-0.9.2/
--rw-r--r--   0 george    (1000) george    (1000)    35149 2022-07-12 06:28:39.000000 anbani-0.9.2/LICENSE
--rw-r--r--   0 george    (1000) george    (1000)       21 2022-07-12 06:28:39.000000 anbani-0.9.2/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)     2968 2022-07-12 06:39:26.240837 anbani-0.9.2/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     2434 2022-07-12 06:28:39.000000 anbani-0.9.2/README.md
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2022-07-12 06:39:26.214836 anbani-0.9.2/anbani/
--rw-r--r--   0 george    (1000) george    (1000)       66 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/__init__.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2022-07-12 06:39:26.232837 anbani-0.9.2/anbani/core/
--rw-r--r--   0 george    (1000) george    (1000)        0 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/core/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     3581 2022-07-12 06:35:34.000000 anbani-0.9.2/anbani/core/converter.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2022-07-12 06:39:26.236837 anbani-0.9.2/anbani/data/
--rw-r--r--   0 george    (1000) george    (1000)    16939 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/data/georgian_contractions.csv
--rw-r--r--   0 george    (1000) george    (1000)    11296 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/data/letters.js
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2022-07-12 06:39:26.240837 anbani-0.9.2/anbani/nlp/
--rw-r--r--   0 george    (1000) george    (1000)       16 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/nlp/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)      770 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/nlp/contractions.py
--rw-r--r--   0 george    (1000) george    (1000)     1681 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/nlp/preprocessing.py
--rw-r--r--   0 george    (1000) george    (1000)     1306 2022-07-12 06:28:39.000000 anbani-0.9.2/anbani/nlp/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2022-07-12 06:39:26.227837 anbani-0.9.2/anbani.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)     2968 2022-07-12 06:39:25.000000 anbani-0.9.2/anbani.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)      424 2022-07-12 06:39:26.000000 anbani-0.9.2/anbani.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2022-07-12 06:39:25.000000 anbani-0.9.2/anbani.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)       32 2022-07-12 06:39:25.000000 anbani-0.9.2/anbani.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2022-07-12 06:39:25.000000 anbani-0.9.2/anbani.egg-info/top_level.txt
--rw-r--r--   0 george    (1000) george    (1000)      103 2022-07-12 06:39:26.241837 anbani-0.9.2/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      880 2022-07-12 06:37:39.000000 anbani-0.9.2/setup.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.566458 anbani-0.9.3/
+-rw-r--r--   0 george    (1000) george    (1000)    35149 2022-07-12 06:28:39.000000 anbani-0.9.3/LICENSE
+-rw-r--r--   0 george    (1000) george    (1000)       21 2022-07-12 06:28:39.000000 anbani-0.9.3/MANIFEST.in
+-rw-r--r--   0 george    (1000) george    (1000)     2967 2023-04-28 05:18:19.566458 anbani-0.9.3/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)     2434 2022-07-12 06:28:39.000000 anbani-0.9.3/README.md
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.552457 anbani-0.9.3/anbani/
+-rw-r--r--   0 george    (1000) george    (1000)       66 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/__init__.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.553457 anbani-0.9.3/anbani/core/
+-rw-r--r--   0 george    (1000) george    (1000)        0 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/core/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     3581 2022-07-12 06:35:34.000000 anbani-0.9.3/anbani/core/converter.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.558458 anbani-0.9.3/anbani/data/
+-rw-r--r--   0 george    (1000) george    (1000)  2459360 2023-04-27 13:32:54.000000 anbani-0.9.3/anbani/data/ambigram_nc1_len10.csv
+-rw-r--r--   0 george    (1000) george    (1000)   416348 2023-04-27 13:32:54.000000 anbani-0.9.3/anbani/data/ambigram_nc5_len7.csv
+-rw-r--r--   0 george    (1000) george    (1000)    16939 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/data/georgian_contractions.csv
+-rw-r--r--   0 george    (1000) george    (1000)    11296 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/data/letters.js
+-rw-r--r--   0 george    (1000) george    (1000)  5781776 2023-04-27 13:33:08.000000 anbani-0.9.3/anbani/data/wordlist.csv
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.566458 anbani-0.9.3/anbani/nlp/
+-rw-r--r--   0 george    (1000) george    (1000)       16 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)      770 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/contractions.py
+-rw-r--r--   0 george    (1000) george    (1000)     4924 2023-04-28 04:44:57.000000 anbani-0.9.3/anbani/nlp/georgianisation.py
+-rw-r--r--   0 george    (1000) george    (1000)     1681 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/preprocessing.py
+-rw-r--r--   0 george    (1000) george    (1000)     1306 2022-07-12 06:28:39.000000 anbani-0.9.3/anbani/nlp/utils.py
+drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-28 05:18:19.552457 anbani-0.9.3/anbani.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)     2967 2023-04-28 05:18:18.000000 anbani-0.9.3/anbani.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)      548 2023-04-28 05:18:19.000000 anbani-0.9.3/anbani.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-28 05:18:18.000000 anbani-0.9.3/anbani.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)       32 2023-04-28 05:18:19.000000 anbani-0.9.3/anbani.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-28 05:18:19.000000 anbani-0.9.3/anbani.egg-info/top_level.txt
+-rw-r--r--   0 george    (1000) george    (1000)      103 2023-04-28 05:18:19.567458 anbani-0.9.3/setup.cfg
+-rw-r--r--   0 george    (1000) george    (1000)      879 2023-04-28 05:17:54.000000 anbani-0.9.3/setup.py
```

### Comparing `anbani-0.9.2/LICENSE` & `anbani-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/PKG-INFO` & `anbani-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: anbani
-Version: 0.9.2
-Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion  and more.
+Version: 0.9.3
+Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.
 Home-page: https://github.com/anbani/anbani.py
 Author: George Gach
 Author-email: georgegach@outlook.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `anbani-0.9.2/README.md` & `anbani-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani/core/converter.py` & `anbani-0.9.3/anbani/core/converter.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani/data/georgian_contractions.csv` & `anbani-0.9.3/anbani/data/georgian_contractions.csv`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani/data/letters.js` & `anbani-0.9.3/anbani/data/letters.js`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani/nlp/contractions.py` & `anbani-0.9.3/anbani/nlp/contractions.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani/nlp/preprocessing.py` & `anbani-0.9.3/anbani/nlp/preprocessing.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani/nlp/utils.py` & `anbani-0.9.3/anbani/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `anbani-0.9.2/anbani.egg-info/PKG-INFO` & `anbani-0.9.3/anbani.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: anbani
-Version: 0.9.2
-Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion  and more.
+Version: 0.9.3
+Summary: Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.
 Home-page: https://github.com/anbani/anbani.py
 Author: George Gach
 Author-email: georgegach@outlook.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `anbani-0.9.2/setup.py` & `anbani-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='anbani',
-    version='0.9.2',
+    version='0.9.3',
     author="George Gach",
     author_email="georgegach@outlook.com",
-    description="Georgian alphabet and language utilities for Natural Language Processing, script conversion  and more.",
+    description="Georgian alphabet and language utilities for Natural Language Processing, script conversion and more.",
     license='GPL',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anbani/anbani.py",
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
```

