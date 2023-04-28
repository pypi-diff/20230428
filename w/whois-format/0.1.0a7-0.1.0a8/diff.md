# Comparing `tmp/whois-format-0.1.0a7.tar.gz` & `tmp/whois-format-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois-format-0.1.0a7.tar", last modified: Tue Apr 18 05:55:28 2023, max compression
+gzip compressed data, was "whois-format-0.1.0a8.tar", last modified: Fri Apr 28 05:02:57 2023, max compression
```

## Comparing `whois-format-0.1.0a7.tar` & `whois-format-0.1.0a8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/
--rw-r--r--   0 dspruell  (1000) dspruell  (1000)      729 2023-03-25 10:06:17.000000 whois-format-0.1.0a7/LICENSE
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/PKG-INFO
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3126 2023-03-29 04:24:46.000000 whois-format-0.1.0a7/README.md
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      561 2023-04-18 05:55:09.000000 whois-format-0.1.0a7/pyproject.toml
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       38 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/setup.cfg
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/tests/
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       92 2023-03-27 06:34:02.000000 whois-format-0.1.0a7/tests/test_nop.py
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/whois_format.egg-info/
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/PKG-INFO
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      284 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/SOURCES.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)        1 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/dependency_links.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       50 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/entry_points.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       22 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/requires.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       13 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/top_level.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3640 2023-04-18 05:55:09.000000 whois-format-0.1.0a7/whois_format.py
+drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-28 05:02:57.460113 whois-format-0.1.0a8/
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)      729 2023-03-25 10:06:17.000000 whois-format-0.1.0a8/LICENSE
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-04-28 05:02:57.460113 whois-format-0.1.0a8/PKG-INFO
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3126 2023-03-29 04:24:46.000000 whois-format-0.1.0a8/README.md
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      561 2023-04-28 04:51:38.000000 whois-format-0.1.0a8/pyproject.toml
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       38 2023-04-28 05:02:57.460113 whois-format-0.1.0a8/setup.cfg
+drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-28 05:02:57.460113 whois-format-0.1.0a8/tests/
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       92 2023-03-27 06:34:02.000000 whois-format-0.1.0a8/tests/test_nop.py
+drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-28 05:02:57.460113 whois-format-0.1.0a8/whois_format.egg-info/
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-04-28 05:02:57.000000 whois-format-0.1.0a8/whois_format.egg-info/PKG-INFO
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      284 2023-04-28 05:02:57.000000 whois-format-0.1.0a8/whois_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)        1 2023-04-28 05:02:57.000000 whois-format-0.1.0a8/whois_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       50 2023-04-28 05:02:57.000000 whois-format-0.1.0a8/whois_format.egg-info/entry_points.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       22 2023-04-28 05:02:57.000000 whois-format-0.1.0a8/whois_format.egg-info/requires.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       13 2023-04-28 05:02:57.000000 whois-format-0.1.0a8/whois_format.egg-info/top_level.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3627 2023-04-28 04:51:27.000000 whois-format-0.1.0a8/whois_format.py
```

### Comparing `whois-format-0.1.0a7/LICENSE` & `whois-format-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-format-0.1.0a7/PKG-INFO` & `whois-format-0.1.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-format
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Whois client wrapper producing a terse, single-line format.
 Author-email: Darren Spruell <phatbuckett@gmail.com>
 Project-URL: Homepage, https://github.com/dspruell/whois-format/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whois-format-0.1.0a7/README.md` & `whois-format-0.1.0a8/README.md`

 * *Files identical despite different names*

### Comparing `whois-format-0.1.0a7/pyproject.toml` & `whois-format-0.1.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whois-format"
-version = "0.1.0-alpha.7"
+version = "0.1.0-alpha.8"
 authors = [
     { name="Darren Spruell", email="phatbuckett@gmail.com" },
 ]
 description = "Whois client wrapper producing a terse, single-line format."
 readme = "README.md"
 dependencies = [
     "python-whois",
```

### Comparing `whois-format-0.1.0a7/whois_format.egg-info/PKG-INFO` & `whois-format-0.1.0a8/whois_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-format
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Whois client wrapper producing a terse, single-line format.
 Author-email: Darren Spruell <phatbuckett@gmail.com>
 Project-URL: Homepage, https://github.com/dspruell/whois-format/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whois-format-0.1.0a7/whois_format.py` & `whois-format-0.1.0a8/whois_format.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Whois client wrapper producing a terse, single-line format."""
 
 import datetime
 import logging
 from argparse import ArgumentParser, FileType
 from time import sleep
 
-import pkg_resources
+from importlib.metadata import version
 from tabulate import tabulate
 from whois import whois  # type: ignore
 
 
 __application_name__ = "whois-format"
-__version__ = pkg_resources.get_distribution(__application_name__).version
+__version__ = version(__application_name__)
 __full_version__ = f"{__application_name__} {__version__}"
 
 logging.basicConfig(level=logging.INFO, format="[%(levelname)s] %(message)s")
 
 DEFAULT_STR = "-"
 NUM_SLEEP_SECONDS = 15
```

