# Comparing `tmp/pycstruct-0.9.0.tar.gz` & `tmp/pycstruct-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycstruct-0.9.0.tar", last modified: Wed Feb 24 21:14:45 2021, max compression
+gzip compressed data, was "dist\pycstruct-0.9.1.tar", last modified: Mon Mar  1 15:43:30 2021, max compression
```

## Comparing `pycstruct-0.9.0.tar` & `pycstruct-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-02-24 21:14:45.000000 pycstruct-0.9.0/
--rw-rw-rw-   0        0        0     8121 2021-02-24 21:14:45.000000 pycstruct-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     5292 2021-02-24 21:13:50.000000 pycstruct-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2021-02-24 21:14:45.000000 pycstruct-0.9.0/pycstruct/
--rw-rw-rw-   0        0        0      663 2021-02-24 21:13:50.000000 pycstruct-0.9.0/pycstruct/__init__.py
--rw-rw-rw-   0        0        0    25788 2021-02-24 21:13:50.000000 pycstruct-0.9.0/pycstruct/cparser.py
--rw-rw-rw-   0        0        0     8311 2021-02-24 21:13:50.000000 pycstruct-0.9.0/pycstruct/instance.py
--rw-rw-rw-   0        0        0    47393 2021-02-24 21:13:50.000000 pycstruct-0.9.0/pycstruct/pycstruct.py
-drwxrwxrwx   0        0        0        0 2021-02-24 21:14:45.000000 pycstruct-0.9.0/pycstruct.egg-info/
--rw-rw-rw-   0        0        0     8121 2021-02-24 21:14:45.000000 pycstruct-0.9.0/pycstruct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2021-02-24 21:14:45.000000 pycstruct-0.9.0/pycstruct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-24 21:14:45.000000 pycstruct-0.9.0/pycstruct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-24 21:13:59.000000 pycstruct-0.9.0/pycstruct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2021-02-24 21:14:45.000000 pycstruct-0.9.0/pycstruct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-02-24 21:14:45.000000 pycstruct-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1353 2021-02-24 21:13:50.000000 pycstruct-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-01 15:43:30.000000 pycstruct-0.9.1/
+-rw-rw-rw-   0        0        0     8121 2021-03-01 15:43:30.000000 pycstruct-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5292 2021-03-01 15:42:28.000000 pycstruct-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2021-03-01 15:43:30.000000 pycstruct-0.9.1/pycstruct/
+-rw-rw-rw-   0        0        0      663 2021-03-01 15:42:28.000000 pycstruct-0.9.1/pycstruct/__init__.py
+-rw-rw-rw-   0        0        0    25788 2021-03-01 15:42:28.000000 pycstruct-0.9.1/pycstruct/cparser.py
+-rw-rw-rw-   0        0        0     8311 2021-03-01 15:42:28.000000 pycstruct-0.9.1/pycstruct/instance.py
+-rw-rw-rw-   0        0        0    47408 2021-03-01 15:42:28.000000 pycstruct-0.9.1/pycstruct/pycstruct.py
+drwxrwxrwx   0        0        0        0 2021-03-01 15:43:30.000000 pycstruct-0.9.1/pycstruct.egg-info/
+-rw-rw-rw-   0        0        0     8121 2021-03-01 15:43:30.000000 pycstruct-0.9.1/pycstruct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2021-03-01 15:43:30.000000 pycstruct-0.9.1/pycstruct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-01 15:43:30.000000 pycstruct-0.9.1/pycstruct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-03-01 15:42:38.000000 pycstruct-0.9.1/pycstruct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2021-03-01 15:43:30.000000 pycstruct-0.9.1/pycstruct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2021-03-01 15:43:30.000000 pycstruct-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1353 2021-03-01 15:42:28.000000 pycstruct-0.9.1/setup.py
```

### Comparing `pycstruct-0.9.0/PKG-INFO` & `pycstruct-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycstruct
-Version: 0.9.0
+Version: 0.9.1
 Summary: Binary data handling in Python using dictionaries
 Home-page: http://github.com/midstar/pycstruct
 Author: Joel Midstjärna
 Author-email: joel.midstjarna@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/midstar/pycstruct/issues
 Project-URL: Documentation, https://pycstruct.readthedocs.io/en/latest/
```

### Comparing `pycstruct-0.9.0/README.md` & `pycstruct-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pycstruct-0.9.0/pycstruct/__init__.py` & `pycstruct-0.9.1/pycstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `pycstruct-0.9.0/pycstruct/cparser.py` & `pycstruct-0.9.1/pycstruct/cparser.py`

 * *Files identical despite different names*

### Comparing `pycstruct-0.9.0/pycstruct/instance.py` & `pycstruct-0.9.1/pycstruct/instance.py`

 * *Files identical despite different names*

### Comparing `pycstruct-0.9.0/pycstruct/pycstruct.py` & `pycstruct-0.9.1/pycstruct/pycstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ###############################################################################
 # Global constants
 
 # Basic Types
 _TYPE = {
     "int8": {"format": "b", "bytes": 1, "dtype": "i1"},
     "uint8": {"format": "B", "bytes": 1, "dtype": "u1"},
-    "bool8": {"format": "B", "bytes": 1},
+    "bool8": {"format": "B", "bytes": 1, "dtype": "b1"},
     "int16": {"format": "h", "bytes": 2, "dtype": "i2"},
     "uint16": {"format": "H", "bytes": 2, "dtype": "u2"},
     "bool16": {"format": "H", "bytes": 2},
     "float16": {"format": "e", "bytes": 2, "dtype": "f2"},
     "int32": {"format": "i", "bytes": 4, "dtype": "i4"},
     "uint32": {"format": "I", "bytes": 4, "dtype": "u4"},
     "bool32": {"format": "I", "bytes": 4},
```

### Comparing `pycstruct-0.9.0/pycstruct.egg-info/PKG-INFO` & `pycstruct-0.9.1/pycstruct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycstruct
-Version: 0.9.0
+Version: 0.9.1
 Summary: Binary data handling in Python using dictionaries
 Home-page: http://github.com/midstar/pycstruct
 Author: Joel Midstjärna
 Author-email: joel.midstjarna@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/midstar/pycstruct/issues
 Project-URL: Documentation, https://pycstruct.readthedocs.io/en/latest/
```

### Comparing `pycstruct-0.9.0/setup.py` & `pycstruct-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except:
       long_description = ""
 
 setup(name='pycstruct',
-      version='0.9.0',
+      version='0.9.1',
       description='Binary data handling in Python using dictionaries',
       long_description=long_description,
        long_description_content_type="text/markdown",
       url='http://github.com/midstar/pycstruct',
       project_urls={
             'Bug Tracker': 'https://github.com/midstar/pycstruct/issues',
             'Documentation': 'https://pycstruct.readthedocs.io/en/latest/',
```

