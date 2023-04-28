# Comparing `tmp/rssfixer-0.1.3.tar.gz` & `tmp/rssfixer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.1.3.tar", last modified: Wed Apr 26 18:45:41 2023, max compression
+gzip compressed data, was "rssfixer-0.1.4.tar", last modified: Thu Apr 27 12:08:03 2023, max compression
```

## Comparing `rssfixer-0.1.3.tar` & `rssfixer-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.082135 rssfixer-0.1.3/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.3/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:45:41.081919 rssfixer-0.1.3/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     8682 2023-04-26 18:07:49.000000 rssfixer-0.1.3/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-26 18:44:42.000000 rssfixer-0.1.3/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-26 18:45:41.082197 rssfixer-0.1.3/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.077840 rssfixer-0.1.3/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.079056 rssfixer-0.1.3/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.3/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)    12618 2023-04-26 18:40:18.000000 rssfixer-0.1.3/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.080498 rssfixer-0.1.3/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      371 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.081480 rssfixer-0.1.3/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 16:32:08.000000 rssfixer-0.1.3/src/tests/test_rss.py
--rw-r--r--   0 reuteras   (501) staff       (20)     4141 2023-04-26 18:16:41.000000 rssfixer-0.1.3/src/tests/test_rss_args.py
--rw-r--r--   0 reuteras   (501) staff       (20)     1980 2023-04-26 16:34:02.000000 rssfixer-0.1.3/src/tests/test_rss_main.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-27 12:08:03.904010 rssfixer-0.1.4/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-17 09:42:15.000000 rssfixer-0.1.4/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-27 12:08:03.903830 rssfixer-0.1.4/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     8682 2023-04-27 04:47:13.000000 rssfixer-0.1.4/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-27 11:57:51.000000 rssfixer-0.1.4/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-27 12:08:03.904056 rssfixer-0.1.4/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-27 12:08:03.901247 rssfixer-0.1.4/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-27 12:08:03.902045 rssfixer-0.1.4/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-24 04:52:30.000000 rssfixer-0.1.4/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)    12428 2023-04-27 11:44:54.000000 rssfixer-0.1.4/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-27 12:08:03.902962 rssfixer-0.1.4/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-27 12:08:03.000000 rssfixer-0.1.4/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      415 2023-04-27 12:08:03.000000 rssfixer-0.1.4/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-27 12:08:03.000000 rssfixer-0.1.4/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-27 12:08:03.000000 rssfixer-0.1.4/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-27 12:08:03.000000 rssfixer-0.1.4/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-27 12:08:03.000000 rssfixer-0.1.4/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-27 12:08:03.903622 rssfixer-0.1.4/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-27 04:47:13.000000 rssfixer-0.1.4/src/tests/test_rss.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     4983 2023-04-27 11:44:54.000000 rssfixer-0.1.4/src/tests/test_rss_args.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     2236 2023-04-27 11:44:54.000000 rssfixer-0.1.4/src/tests/test_rss_extract_links_release.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     1980 2023-04-27 04:47:13.000000 rssfixer-0.1.4/src/tests/test_rss_main.py
```

### Comparing `rssfixer-0.1.3/LICENSE` & `rssfixer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.3/PKG-INFO` & `rssfixer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rssfixer-0.1.3/README.md` & `rssfixer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.3/pyproject.toml` & `rssfixer-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rssfixer"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "Development Status :: 4 - Beta",
     "Environment :: Console",
 ]
 
 dependencies = [
     "beautifulsoup4==4.12.2",
     "feedgen==0.9.0",
-    "requests==2.28.2",
+    "requests==2.29.0",
 ]
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
```

### Comparing `rssfixer-0.1.3/src/rssfixer/rss.py` & `rssfixer-0.1.4/src/rssfixer/rss.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 
 import requests
 from bs4 import BeautifulSoup
 from feedgen.feed import FeedGenerator
 
 try:
-    __version__ = importlib.metadata.version(__package__ or __name__)
+    __version__ = "version " + importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = "0.0.0"
 
 
 class CheckHtmlAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if not namespace.html:
@@ -26,21 +26,14 @@
 class CheckJsonAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if not namespace.json:
             parser.error(f"{option_string} requires --json to be specified.")
         setattr(namespace, self.dest, values)
 
 
-class CheckListAction(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string=None):
-        if not namespace.list:
-            parser.error(f"{option_string} requires --list to be specified.")
-        setattr(namespace, self.dest, values)
-
-
 class CheckReleaseAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if not namespace.release:
             parser.error(f"{option_string} requires --release to be specified.")
         setattr(namespace, self.dest, values)
 
 
@@ -175,14 +168,16 @@
     links = []
     unique_titles = set()
 
     # Iterate through all the elements of type html_entries in the page
     for entry in soup.find_all(arguments.release_entries):
         try:
             title = entry.text.strip()
+            if title == "":
+                raise AttributeError
             title_bytes = title.encode("utf-8")
             title_hash = hashlib.sha256(title_bytes)
             title_sha256 = title_hash.hexdigest()
             url = arguments.release_url + "?" + title_sha256
         except (KeyError, AttributeError):
             print("ERROR: Unable to title in HTML element")
             sys.exit(1)
```

### Comparing `rssfixer-0.1.3/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.1.4/src/rssfixer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rssfixer-0.1.3/src/tests/test_rss.py` & `rssfixer-0.1.4/src/tests/test_rss.py`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.3/src/tests/test_rss_main.py` & `rssfixer-0.1.4/src/tests/test_rss_main.py`

 * *Files identical despite different names*

