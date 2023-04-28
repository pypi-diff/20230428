# Comparing `tmp/pyg-encoders-0.0.8.tar.gz` & `tmp/pyg-encoders-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg-encoders-0.0.8.tar", last modified: Wed Aug  3 08:31:29 2022, max compression
+gzip compressed data, was "pyg-encoders-0.0.9.tar", last modified: Wed Aug  3 09:33:02 2022, max compression
```

## Comparing `pyg-encoders-0.0.8.tar` & `pyg-encoders-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-08-03 08:31:29.076611 pyg-encoders-0.0.8/
--rw-rw-rw-   0        0        0    35803 2022-07-21 08:08:57.000000 pyg-encoders-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      591 2022-08-03 08:31:29.076611 pyg-encoders-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       19 2022-07-21 08:08:57.000000 pyg-encoders-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2022-07-21 08:08:57.000000 pyg-encoders-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      749 2022-08-03 08:31:29.080802 pyg-encoders-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-03 08:31:29.037200 pyg-encoders-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-03 08:31:29.055712 pyg-encoders-0.0.8/src/pyg_encoders/
--rw-rw-rw-   0        0        0      498 2022-08-03 06:07:16.000000 pyg-encoders-0.0.8/src/pyg_encoders/__init__.py
--rw-rw-rw-   0        0        0    11032 2022-07-21 08:08:57.000000 pyg-encoders-0.0.8/src/pyg_encoders/_encode.py
--rw-rw-rw-   0        0        0    16812 2022-08-03 08:10:08.000000 pyg-encoders-0.0.8/src/pyg_encoders/_encoders.py
--rw-rw-rw-   0        0        0     3449 2022-07-21 08:08:57.000000 pyg-encoders-0.0.8/src/pyg_encoders/_parquet.py
--rw-rw-rw-   0        0        0     2933 2022-08-03 06:23:50.000000 pyg-encoders-0.0.8/src/pyg_encoders/_writers.py
-drwxrwxrwx   0        0        0        0 2022-08-03 08:31:29.075615 pyg-encoders-0.0.8/src/pyg_encoders.egg-info/
--rw-rw-rw-   0        0        0      591 2022-08-03 08:31:29.000000 pyg-encoders-0.0.8/src/pyg_encoders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2022-08-03 08:31:29.000000 pyg-encoders-0.0.8/src/pyg_encoders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-03 08:31:29.000000 pyg-encoders-0.0.8/src/pyg_encoders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-08-03 08:31:29.000000 pyg-encoders-0.0.8/src/pyg_encoders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-08-03 08:31:29.000000 pyg-encoders-0.0.8/src/pyg_encoders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-03 09:33:02.235844 pyg-encoders-0.0.9/
+-rw-rw-rw-   0        0        0    35803 2022-07-21 08:08:57.000000 pyg-encoders-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      591 2022-08-03 09:33:02.235844 pyg-encoders-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2022-07-21 08:08:57.000000 pyg-encoders-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2022-07-21 08:08:57.000000 pyg-encoders-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      749 2022-08-03 09:33:02.238009 pyg-encoders-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-08-03 09:33:02.205746 pyg-encoders-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-03 09:33:02.223844 pyg-encoders-0.0.9/src/pyg_encoders/
+-rw-rw-rw-   0        0        0      498 2022-08-03 06:07:16.000000 pyg-encoders-0.0.9/src/pyg_encoders/__init__.py
+-rw-rw-rw-   0        0        0    11032 2022-07-21 08:08:57.000000 pyg-encoders-0.0.9/src/pyg_encoders/_encode.py
+-rw-rw-rw-   0        0        0    16812 2022-08-03 08:10:08.000000 pyg-encoders-0.0.9/src/pyg_encoders/_encoders.py
+-rw-rw-rw-   0        0        0     3449 2022-07-21 08:08:57.000000 pyg-encoders-0.0.9/src/pyg_encoders/_parquet.py
+-rw-rw-rw-   0        0        0     3202 2022-08-03 09:32:16.000000 pyg-encoders-0.0.9/src/pyg_encoders/_writers.py
+drwxrwxrwx   0        0        0        0 2022-08-03 09:33:02.234845 pyg-encoders-0.0.9/src/pyg_encoders.egg-info/
+-rw-rw-rw-   0        0        0      591 2022-08-03 09:33:02.000000 pyg-encoders-0.0.9/src/pyg_encoders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2022-08-03 09:33:02.000000 pyg-encoders-0.0.9/src/pyg_encoders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-03 09:33:02.000000 pyg-encoders-0.0.9/src/pyg_encoders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2022-08-03 09:33:02.000000 pyg-encoders-0.0.9/src/pyg_encoders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-08-03 09:33:02.000000 pyg-encoders-0.0.9/src/pyg_encoders.egg-info/top_level.txt
```

### Comparing `pyg-encoders-0.0.8/LICENSE` & `pyg-encoders-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg-encoders-0.0.8/PKG-INFO` & `pyg-encoders-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-encoders
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for encoding DataFrame/Series within a document as npy parquet or csv files
 Home-page: https://github.com/gityoav/pyg-encoders
 Author: Yoav Git
 Author-email: yoav.git@gmail.com
 Project-URL: Bug Tracker, https://github.com/gityoav/pyg-encoders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyg-encoders-0.0.8/setup.cfg` & `pyg-encoders-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7967 2d65 6e63 6f64 6572 730d   = pyg-encoders.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e38  .version = 0.0.8
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e39  .version = 0.0.9
 00000030: 0d0a 6175 7468 6f72 203d 2059 6f61 7620  ..author = Yoav 
 00000040: 4769 740d 0a61 7574 686f 725f 656d 6169  Git..author_emai
 00000050: 6c20 3d20 796f 6176 2e67 6974 4067 6d61  l = yoav.git@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5574 696c 6974 6965 7320  ion = Utilities 
 00000080: 666f 7220 656e 636f 6469 6e67 2044 6174  for encoding Dat
 00000090: 6146 7261 6d65 2f53 6572 6965 7320 7769  aFrame/Series wi
```

### Comparing `pyg-encoders-0.0.8/src/pyg_encoders/_encode.py` & `pyg-encoders-0.0.9/src/pyg_encoders/_encode.py`

 * *Files identical despite different names*

### Comparing `pyg-encoders-0.0.8/src/pyg_encoders/_encoders.py` & `pyg-encoders-0.0.9/src/pyg_encoders/_encoders.py`

 * *Files identical despite different names*

### Comparing `pyg-encoders-0.0.8/src/pyg_encoders/_parquet.py` & `pyg-encoders-0.0.9/src/pyg_encoders/_parquet.py`

 * *Files identical despite different names*

### Comparing `pyg-encoders-0.0.8/src/pyg_encoders/_writers.py` & `pyg-encoders-0.0.9/src/pyg_encoders/_writers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from pyg_encoders._encoders import csv_write, parquet_write, npy_write, pickle_write, _csv, _npy, _npa, _parquet, _pickle, root_path
 from pyg_encoders._encode import encode, decode 
-from pyg_base import passthru, is_str, as_list
+from pyg_base import passthru, is_str, as_list, get_cache
 from functools import partial
 
-WRITERS = {_csv: csv_write , 
-           _npy: partial(npy_write, append = False), 
-           _npa: partial(npy_write, append = True), 
-           _parquet: parquet_write, 
-           _pickle : pickle_write}
+
+_WRITERS = 'WRITERS'
+if _WRITERS not in get_cache():
+    get_cache()[_WRITERS] = {}
+    
+WRITERS = get_cache()[_WRITERS]
+WRITERS.update({_csv: csv_write , 
+               _npy: partial(npy_write, append = False), 
+               _npa: partial(npy_write, append = True), 
+               _parquet: parquet_write, 
+               _pickle : pickle_write})
 
 def as_reader(reader = None):
     """
         returns a list of functions that are applied to an object to turn it into a valid document
     """
     if isinstance(reader, list):
         return sum([as_reader(r) for r in reader], [])
@@ -54,19 +60,21 @@
     e = encode if unchanged is None and unchanged_keys is None else partial(encode, unchanged = unchanged, unchanged_keys = unchanged_keys)
     if writer is None or writer is True or writer == ():
         return [e]
     elif writer is False or writer == 0:
         return [passthru]
     elif is_str(writer):
         for ext, w in WRITERS.items():
-            if writer.endswith(ext):
+            if writer.lower().endswith(ext):
                 root = writer[:-len(ext)]                    
-                if root:
+                if len(root)>0:
                     if kwargs:
                         root = root_path(kwargs, root)
                     return [partial(w, root = root), e]
                 else:
                     return [w, e]
-        raise ValueError('We support only csv/npy/parquet/parquet writers and writer should look like: c:/somewhere/%name/%surname.csv or d:/archive/%country/%city/results.parquet or with .npy or .pickle')
+        err = 'Could not convert "%s" into a valid writer.\nAt the moment we support these extenstions: \n%s'%(writer, '\n'.join('%s maps to %s'%(k,v) for k,v in WRITERS.items()))
+        err += '\nWriter should look like "d:/archive/%country/%city/results.parquet"'
+        raise ValueError(err)
     else:
         return as_list(writer)
```

### Comparing `pyg-encoders-0.0.8/src/pyg_encoders.egg-info/PKG-INFO` & `pyg-encoders-0.0.9/src/pyg_encoders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-encoders
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for encoding DataFrame/Series within a document as npy parquet or csv files
 Home-page: https://github.com/gityoav/pyg-encoders
 Author: Yoav Git
 Author-email: yoav.git@gmail.com
 Project-URL: Bug Tracker, https://github.com/gityoav/pyg-encoders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

