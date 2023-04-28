# Comparing `tmp/ingester3-1.8.6.tar.gz` & `tmp/ingester3-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingester3-1.8.6.tar", max compression
+gzip compressed data, was "ingester3-1.9.0.tar", max compression
```

## Comparing `ingester3-1.8.6.tar` & `ingester3-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-01-31 13:47:20.549829 ingester3-1.8.6/README.md
--rw-r--r--   0        0        0     7037 2023-01-31 13:47:20.549829 ingester3-1.8.6/ingester3/Country.py
--rw-r--r--   0        0        0    23517 2023-01-31 13:47:20.549829 ingester3-1.8.6/ingester3/DBWriter.py
--rw-r--r--   0        0        0     2197 2023-01-31 13:47:20.549829 ingester3-1.8.6/ingester3/FuzzyCountry.py
--rw-r--r--   0        0        0     6007 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/Priogrid.py
--rw-r--r--   0        0        0     2090 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/ViewsMonth.py
--rw-r--r--   0        0        0        0 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/__init__.py
--rw-r--r--   0        0        0     2661 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/config.py
--rw-r--r--   0        0        0    46660 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/extensions.py
--rw-r--r--   0        0        0     2857 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/log.py
--rw-r--r--   0        0        0    12202 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/scratch.py
--rw-r--r--   0        0        0       10 2023-01-31 13:47:20.553829 ingester3-1.8.6/ingester3/timestamp.cache
--rw-r--r--   0        0        0      600 2023-01-31 13:47:20.553829 ingester3-1.8.6/pyproject.toml
--rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 ingester3-1.8.6/setup.py
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 ingester3-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-28 14:03:06.786599 ingester3-1.9.0/README.md
+-rw-r--r--   0        0        0     7037 2023-04-28 14:03:06.786599 ingester3-1.9.0/ingester3/Country.py
+-rw-r--r--   0        0        0    23517 2023-04-28 14:03:06.786599 ingester3-1.9.0/ingester3/DBWriter.py
+-rw-r--r--   0        0        0     2197 2023-04-28 14:03:06.786599 ingester3-1.9.0/ingester3/FuzzyCountry.py
+-rw-r--r--   0        0        0     6007 2023-04-28 14:03:06.786599 ingester3-1.9.0/ingester3/Priogrid.py
+-rw-r--r--   0        0        0     2478 2023-04-28 14:03:06.786599 ingester3-1.9.0/ingester3/ViewsMonth.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:03:06.786599 ingester3-1.9.0/ingester3/__init__.py
+-rw-r--r--   0        0        0     2661 2023-04-28 14:03:06.790599 ingester3-1.9.0/ingester3/config.py
+-rw-r--r--   0        0        0    46660 2023-04-28 14:03:06.790599 ingester3-1.9.0/ingester3/extensions.py
+-rw-r--r--   0        0        0     2857 2023-04-28 14:03:06.790599 ingester3-1.9.0/ingester3/log.py
+-rw-r--r--   0        0        0    12202 2023-04-28 14:03:06.790599 ingester3-1.9.0/ingester3/scratch.py
+-rw-r--r--   0        0        0       10 2023-04-28 14:03:06.790599 ingester3-1.9.0/ingester3/timestamp.cache
+-rw-r--r--   0        0        0      600 2023-04-28 14:03:06.790599 ingester3-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 ingester3-1.9.0/PKG-INFO
```

### Comparing `ingester3-1.8.6/README.md` & `ingester3-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/Country.py` & `ingester3-1.9.0/ingester3/Country.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/DBWriter.py` & `ingester3-1.9.0/ingester3/DBWriter.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/FuzzyCountry.py` & `ingester3-1.9.0/ingester3/FuzzyCountry.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/Priogrid.py` & `ingester3-1.9.0/ingester3/Priogrid.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/config.py` & `ingester3-1.9.0/ingester3/config.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/extensions.py` & `ingester3-1.9.0/ingester3/extensions.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/log.py` & `ingester3-1.9.0/ingester3/log.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/ingester3/scratch.py` & `ingester3-1.9.0/ingester3/scratch.py`

 * *Files identical despite different names*

### Comparing `ingester3-1.8.6/pyproject.toml` & `ingester3-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ingester3"
-version = "1.8.6"
+version = "1.9.0"
 description = "Data ingester for ViEWS3."
 authors = ["Mihai Croicu <mihai.croicu@pcr.uu.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/UppsalaConflictDataProgram/ingester3>"
 
 [tool.poetry.dependencies]
```

### Comparing `ingester3-1.8.6/PKG-INFO` & `ingester3-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingester3
-Version: 1.8.6
+Version: 1.9.0
 Summary: Data ingester for ViEWS3.
 Home-page: https://github.com/UppsalaConflictDataProgram/ingester3>
 License: MIT
 Author: Mihai Croicu
 Author-email: mihai.croicu@pcr.uu.se
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

