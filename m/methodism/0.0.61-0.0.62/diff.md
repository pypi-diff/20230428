# Comparing `tmp/methodism-0.0.61.tar.gz` & `tmp/methodism-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.0.61.tar", last modified: Fri Apr 28 10:29:21 2023, max compression
+gzip compressed data, was "methodism-0.0.62.tar", last modified: Fri Apr 28 13:17:53 2023, max compression
```

## Comparing `methodism-0.0.61.tar` & `methodism-0.0.62.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 10:29:21.338079 methodism-0.0.61/
--rw-rw-rw-   0        0        0     2917 2023-04-28 10:29:21.338079 methodism-0.0.61/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2023-04-28 10:28:06.000000 methodism-0.0.61/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 10:29:21.306810 methodism-0.0.61/methodism/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.61/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.0.61/methodism/costumizing.py
--rw-rw-rw-   0        0        0      718 2023-04-28 10:28:06.000000 methodism-0.0.61/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.61/methodism/error_messages.py
--rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.61/methodism/helper.py
--rw-rw-rw-   0        0        0     3294 2023-04-28 10:28:06.000000 methodism-0.0.61/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:29:21.322436 methodism-0.0.61/methodism.egg-info/
--rw-rw-rw-   0        0        0     2917 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      604 2023-04-28 10:28:51.000000 methodism-0.0.61/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-04-28 10:29:21.338079 methodism-0.0.61/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 13:17:53.324593 methodism-0.0.62/
+-rw-rw-rw-   0        0        0     2917 2023-04-28 13:17:53.324593 methodism-0.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2023-04-28 10:28:06.000000 methodism-0.0.62/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 13:17:53.308967 methodism-0.0.62/methodism/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.62/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.0.62/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      772 2023-04-28 13:17:15.000000 methodism-0.0.62/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.62/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.62/methodism/helper.py
+-rw-rw-rw-   0        0        0     3294 2023-04-28 10:28:06.000000 methodism-0.0.62/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:17:53.324593 methodism-0.0.62/methodism.egg-info/
+-rw-rw-rw-   0        0        0     2917 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 13:17:53.000000 methodism-0.0.62/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      604 2023-04-28 13:17:15.000000 methodism-0.0.62/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-04-28 13:17:53.324593 methodism-0.0.62/setup.cfg
```

### Comparing `methodism-0.0.61/PKG-INFO` & `methodism-0.0.62/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.61
+Version: 0.0.62
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.0.61/README.md` & `methodism-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `methodism-0.0.61/methodism/costumizing.py` & `methodism-0.0.62/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.61/methodism/error_messages.py` & `methodism-0.0.62/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.61/methodism/helper.py` & `methodism-0.0.62/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.61/methodism/main.py` & `methodism-0.0.62/methodism/main.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.61/methodism.egg-info/PKG-INFO` & `methodism-0.0.62/methodism.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.61
+Version: 0.0.62
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.0.61/pyproject.toml` & `methodism-0.0.62/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.0.61"
+version = "0.0.62"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.0.61/setup.cfg` & `methodism-0.0.62/setup.cfg`

 * *Files identical despite different names*

