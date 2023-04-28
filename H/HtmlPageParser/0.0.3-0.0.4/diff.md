# Comparing `tmp/HtmlPageParser-0.0.3.tar.gz` & `tmp/HtmlPageParser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HtmlPageParser-0.0.3.tar", last modified: Wed Apr 26 09:02:08 2023, max compression
+gzip compressed data, was "HtmlPageParser-0.0.4.tar", last modified: Fri Apr 28 04:46:41 2023, max compression
```

## Comparing `HtmlPageParser-0.0.3.tar` & `HtmlPageParser-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     1069 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/LICENSE
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7371 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/PKG-INFO
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      515 2023-04-26 09:01:01.000000 HtmlPageParser-0.0.3/pyproject.toml
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     6937 2023-04-26 09:00:30.000000 HtmlPageParser-0.0.3/readme.md
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       38 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/setup.cfg
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/src/
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7371 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/PKG-INFO
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      317 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        1 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       40 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/top_level.txt
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/src/__init__.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     8726 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/src/htmllabel.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3636 2023-04-26 06:54:35.000000 HtmlPageParser-0.0.3/src/json2markdown.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3435 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/src/parser.py
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/tests/
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      466 2023-04-26 06:49:33.000000 HtmlPageParser-0.0.3/tests/test_json2markdown.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      918 2023-04-26 06:50:28.000000 HtmlPageParser-0.0.3/tests/test_parser.py
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-28 04:46:41.599054 HtmlPageParser-0.0.4/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     1069 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.4/LICENSE
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7365 2023-04-28 04:46:41.599054 HtmlPageParser-0.0.4/PKG-INFO
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      509 2023-04-28 04:46:04.000000 HtmlPageParser-0.0.4/pyproject.toml
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     6937 2023-04-26 09:00:30.000000 HtmlPageParser-0.0.4/readme.md
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       38 2023-04-28 04:46:41.599054 HtmlPageParser-0.0.4/setup.cfg
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-28 04:46:41.591055 HtmlPageParser-0.0.4/src/
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-28 04:46:41.595054 HtmlPageParser-0.0.4/src/HtmlPageParser.egg-info/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7365 2023-04-28 04:46:41.000000 HtmlPageParser-0.0.4/src/HtmlPageParser.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      317 2023-04-28 04:46:41.000000 HtmlPageParser-0.0.4/src/HtmlPageParser.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        1 2023-04-28 04:46:41.000000 HtmlPageParser-0.0.4/src/HtmlPageParser.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       40 2023-04-28 04:46:41.000000 HtmlPageParser-0.0.4/src/HtmlPageParser.egg-info/top_level.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.4/src/__init__.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     8726 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.4/src/htmllabel.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3636 2023-04-26 06:54:35.000000 HtmlPageParser-0.0.4/src/json2markdown.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3435 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.4/src/parser.py
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-28 04:46:41.595054 HtmlPageParser-0.0.4/tests/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      466 2023-04-26 06:49:33.000000 HtmlPageParser-0.0.4/tests/test_json2markdown.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      918 2023-04-26 06:50:28.000000 HtmlPageParser-0.0.4/tests/test_parser.py
```

### Comparing `HtmlPageParser-0.0.3/LICENSE` & `HtmlPageParser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.3/PKG-INFO` & `HtmlPageParser-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: HtmlPageParser
-Version: 0.0.3
+Version: 0.0.4
 Summary: A generic HTML page parser
-Author-email: Jeffrey Yang <snjyor@163.com>
+Author-email: snjyor <snjyor@163.com>
 Project-URL: Homepage, https://github.com/snjyor/HtmlPageParser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `HtmlPageParser-0.0.3/readme.md` & `HtmlPageParser-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/PKG-INFO` & `HtmlPageParser-0.0.4/src/HtmlPageParser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: HtmlPageParser
-Version: 0.0.3
+Version: 0.0.4
 Summary: A generic HTML page parser
-Author-email: Jeffrey Yang <snjyor@163.com>
+Author-email: snjyor <snjyor@163.com>
 Project-URL: Homepage, https://github.com/snjyor/HtmlPageParser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `HtmlPageParser-0.0.3/src/htmllabel.py` & `HtmlPageParser-0.0.4/src/htmllabel.py`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.3/src/json2markdown.py` & `HtmlPageParser-0.0.4/src/json2markdown.py`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.3/src/parser.py` & `HtmlPageParser-0.0.4/src/parser.py`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.3/tests/test_parser.py` & `HtmlPageParser-0.0.4/tests/test_parser.py`

 * *Files identical despite different names*

