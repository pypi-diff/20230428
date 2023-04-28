# Comparing `tmp/monocleaner-1.3.tar.gz` & `tmp/monocleaner-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monocleaner-1.3.tar", last modified: Wed Mar 15 13:29:54 2023, max compression
+gzip compressed data, was "monocleaner-1.4.tar", last modified: Fri Apr 28 14:17:39 2023, max compression
```

## Comparing `monocleaner-1.3.tar` & `monocleaner-1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 13:29:54.445968 monocleaner-1.3/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-03-15 13:29:44.000000 monocleaner-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6154 2023-03-15 13:29:54.445968 monocleaner-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5060 2023-03-15 13:29:44.000000 monocleaner-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-03-15 13:29:44.000000 monocleaner-1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 13:29:54.441968 monocleaner-1.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)      918 2023-03-15 13:29:44.000000 monocleaner-1.3/scripts/monocleaner-download
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-15 13:29:54.445968 monocleaner-1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 13:29:54.441968 monocleaner-1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 13:29:54.445968 monocleaner-1.3/src/monocleaner/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7703 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/hardrules.py
--rw-r--r--   0 runner    (1001) docker     (122)    13407 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/lm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/monocleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/monocleaner_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-03-15 13:29:44.000000 monocleaner-1.3/src/monocleaner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 13:29:54.445968 monocleaner-1.3/src/monocleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6154 2023-03-15 13:29:54.000000 monocleaner-1.3/src/monocleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-03-15 13:29:54.000000 monocleaner-1.3/src/monocleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 13:29:54.000000 monocleaner-1.3/src/monocleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-03-15 13:29:54.000000 monocleaner-1.3/src/monocleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-15 13:29:54.000000 monocleaner-1.3/src/monocleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-15 13:29:54.000000 monocleaner-1.3/src/monocleaner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.233454 monocleaner-1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-04-28 14:17:26.000000 monocleaner-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-04-28 14:17:39.233454 monocleaner-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-04-28 14:17:26.000000 monocleaner-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-04-28 14:17:26.000000 monocleaner-1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.229453 monocleaner-1.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      918 2023-04-28 14:17:26.000000 monocleaner-1.4/scripts/monocleaner-download
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 14:17:39.233454 monocleaner-1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.229453 monocleaner-1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.233454 monocleaner-1.4/src/monocleaner/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7703 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/hardrules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13407 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/lm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/monocleaner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/monocleaner_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.233454 monocleaner-1.4/src/monocleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/top_level.txt
```

### Comparing `monocleaner-1.3/LICENSE` & `monocleaner-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/PKG-INFO` & `monocleaner-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monocleaner
-Version: 1.3
+Version: 1.4
 Summary: Monolingual corpus fluency filter
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/bitextor/monocleaner
 Project-URL: Monocleaner on GitHub, https://github.com/bitextor/monocleaner
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
@@ -51,23 +51,23 @@
   month     = {October},
   address   = {Brussels, Belgium},
   publisher = {Association for Computational Linguistics}
 }
 ```
 
 ## Installation & Requirements
-Monocleaner uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev` and `libhunspell-dev`:
+Monocleaner uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev`:
 ```bash
-sudo apt install python-dev libhunspell-dev
+sudo apt install python-dev
 ```
 
 Monocleaner can be installed using `pip`:
 
 ```bash
-python3.7 -m pip install monocleaner
+python3 -m pip install monocleaner
 ```
 
 Monocleaner requires the [KenLM](https://github.com/kpu/kenlm) Python bindings with support for 7-gram language models. You can easily install it by running the following commands:
 
 ```bash
 git clone https://github.com/kpu/kenlm
 cd kenlm
```

### Comparing `monocleaner-1.3/README.md` & `monocleaner-1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,23 @@
   month     = {October},
   address   = {Brussels, Belgium},
   publisher = {Association for Computational Linguistics}
 }
 ```
 
 ## Installation & Requirements
-Monocleaner uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev` and `libhunspell-dev`:
+Monocleaner uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev`:
 ```bash
-sudo apt install python-dev libhunspell-dev
+sudo apt install python-dev
 ```
 
 Monocleaner can be installed using `pip`:
 
 ```bash
-python3.7 -m pip install monocleaner
+python3 -m pip install monocleaner
 ```
 
 Monocleaner requires the [KenLM](https://github.com/kpu/kenlm) Python bindings with support for 7-gram language models. You can easily install it by running the following commands:
 
 ```bash
 git clone https://github.com/kpu/kenlm
 cd kenlm
```

### Comparing `monocleaner-1.3/pyproject.toml` & `monocleaner-1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "monocleaner"
-version = "1.3"
+version = "1.4"
 requires-python = ">=3.8"
 authors = [
     { name = "Prompsit Language Engineering", email = "info@prompsit.com" },
 ]
 maintainers = [
     { name = "Jaume Zaragoza", email = "jzaragoza@prompsit.com" },
 ]
@@ -22,15 +22,15 @@
 ]
 dependencies = [
     "regex",
     "toolwrapper",
     "sacremoses",
     "numpy",
     "pyyaml",
-    "fastspell==0.8",
+    "fastspell==0.9",
 ]
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.readme]
 file = "README.md"
```

### Comparing `monocleaner-1.3/scripts/monocleaner-download` & `monocleaner-1.4/scripts/monocleaner-download`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner/hardrules.py` & `monocleaner-1.4/src/monocleaner/hardrules.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner/lm.py` & `monocleaner-1.4/src/monocleaner/lm.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner/monocleaner.py` & `monocleaner-1.4/src/monocleaner/monocleaner.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner/monocleaner_train.py` & `monocleaner-1.4/src/monocleaner/monocleaner_train.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner/tokenizer.py` & `monocleaner-1.4/src/monocleaner/tokenizer.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner/util.py` & `monocleaner-1.4/src/monocleaner/util.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.3/src/monocleaner.egg-info/PKG-INFO` & `monocleaner-1.4/src/monocleaner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monocleaner
-Version: 1.3
+Version: 1.4
 Summary: Monolingual corpus fluency filter
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/bitextor/monocleaner
 Project-URL: Monocleaner on GitHub, https://github.com/bitextor/monocleaner
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
@@ -51,23 +51,23 @@
   month     = {October},
   address   = {Brussels, Belgium},
   publisher = {Association for Computational Linguistics}
 }
 ```
 
 ## Installation & Requirements
-Monocleaner uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev` and `libhunspell-dev`:
+Monocleaner uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev`:
 ```bash
-sudo apt install python-dev libhunspell-dev
+sudo apt install python-dev
 ```
 
 Monocleaner can be installed using `pip`:
 
 ```bash
-python3.7 -m pip install monocleaner
+python3 -m pip install monocleaner
 ```
 
 Monocleaner requires the [KenLM](https://github.com/kpu/kenlm) Python bindings with support for 7-gram language models. You can easily install it by running the following commands:
 
 ```bash
 git clone https://github.com/kpu/kenlm
 cd kenlm
```

