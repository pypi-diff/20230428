# Comparing `tmp/demeuk-3.9.6.tar.gz` & `tmp/demeuk-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demeuk-3.9.6.tar", last modified: Tue Jan 25 15:40:24 2022, max compression
+gzip compressed data, was "demeuk-3.9.7.tar", last modified: Thu Feb 17 11:46:06 2022, max compression
```

## Comparing `demeuk-3.9.6.tar` & `demeuk-3.9.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 15:40:24.726222 demeuk-3.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-25 15:40:04.000000 demeuk-3.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-01-25 15:40:24.726222 demeuk-3.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-01-25 15:40:04.000000 demeuk-3.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 15:40:24.722221 demeuk-3.9.6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)    42674 2022-01-25 15:40:04.000000 demeuk-3.9.6/bin/demeuk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 15:40:24.726222 demeuk-3.9.6/demeuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-01-25 15:40:24.000000 demeuk-3.9.6/demeuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-25 15:40:24.000000 demeuk-3.9.6/demeuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 15:40:24.000000 demeuk-3.9.6/demeuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-25 15:40:24.000000 demeuk-3.9.6/demeuk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 15:40:24.000000 demeuk-3.9.6/demeuk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-25 15:40:24.726222 demeuk-3.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-01-25 15:40:04.000000 demeuk-3.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:46:06.901337 demeuk-3.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-17 11:45:48.000000 demeuk-3.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-02-17 11:46:06.901337 demeuk-3.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-02-17 11:45:48.000000 demeuk-3.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:46:06.901337 demeuk-3.9.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    42836 2022-02-17 11:45:48.000000 demeuk-3.9.7/bin/demeuk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:46:06.901337 demeuk-3.9.7/demeuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 11:46:06.000000 demeuk-3.9.7/demeuk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-17 11:46:06.901337 demeuk-3.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-02-17 11:45:48.000000 demeuk-3.9.7/setup.py
```

### Comparing `demeuk-3.9.6/LICENSE` & `demeuk-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `demeuk-3.9.6/PKG-INFO` & `demeuk-3.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demeuk
-Version: 3.9.6
+Version: 3.9.7
 Summary: CLI tool to remove invalid chars from a corpus.
 Home-page: https://github.com/NetherlandsForensicInstitute/demeuk
 Author: Netherlands Forensic Institute
 Author-email: holmesnl@users.noreply.github.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `demeuk-3.9.6/README.md` & `demeuk-3.9.7/README.md`

 * *Files identical despite different names*

### Comparing `demeuk-3.9.6/bin/demeuk.py` & `demeuk-3.9.7/bin/demeuk.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,19 @@
 from ftfy.fixes import fix_latin_ligatures
 from nltk import str2tuple
 from nltk.tokenize import WhitespaceTokenizer
 from tqdm import tqdm
 from unidecode import unidecode
 
 
-version = '3.9.6'
+version = '3.9.7'
 
-HEX_REGEX = re_compile(r'\$HEX\[([0-9a-f]+)\]')
+# Search from start to finish for the string $HEX[], with block of a-f0-9 with even number
+# of hex chars. The first match group is repeated.
+HEX_REGEX = re_compile(r"^\$(?:HEX|hex)\[((?:[0-9a-fA-F]{2})+)\]$")
 EMAIL_REGEX = '.{1,64}@([a-zA-Z0-9_-]{1,63}\\.){1,3}[a-zA-Z]{2,6}'
 HASH_HEX_REGEX = '^[a-fA-F0-9]+$'
 
 # Officiale bcrypt hashes hae a bit more fixed size, but saw some weird once:
 # $2a$10$demo as example
 HASH_BCRYPT_REGEX = '^\\$2[ayb]\\$[0-9]{1,}\\$[\\w\\.\\/]{4,}$'
 # Crypt hashes can look a lot like passwords. We do two options here
```

### Comparing `demeuk-3.9.6/demeuk.egg-info/PKG-INFO` & `demeuk-3.9.7/demeuk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demeuk
-Version: 3.9.6
+Version: 3.9.7
 Summary: CLI tool to remove invalid chars from a corpus.
 Home-page: https://github.com/NetherlandsForensicInstitute/demeuk
 Author: Netherlands Forensic Institute
 Author-email: holmesnl@users.noreply.github.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `demeuk-3.9.6/setup.py` & `demeuk-3.9.7/setup.py`

 * *Files identical despite different names*

