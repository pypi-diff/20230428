# Comparing `tmp/flirimageextractor-1.4.1.tar.gz` & `tmp/flirimageextractor-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flirimageextractor-1.4.1.tar", max compression
+gzip compressed data, was "flirimageextractor-1.5.0.tar", max compression
```

## Comparing `flirimageextractor-1.4.1.tar` & `flirimageextractor-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-04-27 11:01:17.379121 flirimageextractor-1.4.1/LICENSE
--rw-r--r--   0        0        0     3450 2023-04-27 11:01:17.379121 flirimageextractor-1.4.1/README.md
--rw-r--r--   0        0        0      100 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/__init__.py
--rw-r--r--   0        0        0     3604 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/__main__.py
--rw-r--r--   0        0        0     2135 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/dialogs.py
--rw-r--r--   0        0        0    16918 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/flir_image_extractor.py
--rw-r--r--   0        0        0     9492 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/flyr_unpack.py
--rw-r--r--   0        0        0     4140 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/processing.py
--rw-r--r--   0        0        0    42181 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/thermal_base.py
--rw-r--r--   0        0        0     9341 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/utils.py
--rw-r--r--   0        0        0     1568 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 flirimageextractor-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 11:05:51.081444 flirimageextractor-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3450 2023-04-27 11:05:51.081444 flirimageextractor-1.5.0/README.md
+-rw-r--r--   0        0        0      100 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/__init__.py
+-rw-r--r--   0        0        0     3604 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/__main__.py
+-rw-r--r--   0        0        0     2135 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/dialogs.py
+-rw-r--r--   0        0        0    16918 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/flir_image_extractor.py
+-rw-r--r--   0        0        0     9492 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/flyr_unpack.py
+-rw-r--r--   0        0        0     4140 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/processing.py
+-rw-r--r--   0        0        0    42181 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/thermal_base.py
+-rw-r--r--   0        0        0     9341 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/flirimageextractor/utils.py
+-rw-r--r--   0        0        0     1568 2023-04-27 11:05:51.101444 flirimageextractor-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 flirimageextractor-1.5.0/PKG-INFO
```

### Comparing `flirimageextractor-1.4.1/LICENSE` & `flirimageextractor-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/README.md` & `flirimageextractor-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/__main__.py` & `flirimageextractor-1.5.0/flirimageextractor/__main__.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/dialogs.py` & `flirimageextractor-1.5.0/flirimageextractor/dialogs.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/flir_image_extractor.py` & `flirimageextractor-1.5.0/flirimageextractor/flir_image_extractor.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/flyr_unpack.py` & `flirimageextractor-1.5.0/flirimageextractor/flyr_unpack.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/processing.py` & `flirimageextractor-1.5.0/flirimageextractor/processing.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/thermal_base.py` & `flirimageextractor-1.5.0/flirimageextractor/thermal_base.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/flirimageextractor/utils.py` & `flirimageextractor-1.5.0/flirimageextractor/utils.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.4.1/pyproject.toml` & `flirimageextractor-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flirimageextractor"
-version = "1.4.1"
+version = "1.5.0"
 description = "A small tool/lib to read temperatures and original photos from FLIR® thermal camera images."
 authors = [
     "National Drones <development@nationaldrones.com>",
     "olawale williams <olawalewilliams9438@gmail.com>",
 ]
 readme = "README.md"
 maintainers = [
```

### Comparing `flirimageextractor-1.4.1/PKG-INFO` & `flirimageextractor-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flirimageextractor
-Version: 1.4.1
+Version: 1.5.0
 Summary: A small tool/lib to read temperatures and original photos from FLIR® thermal camera images.
 Home-page: https://github.com/nationaldronesau/FlirImageExtractor
 License: MIT
 Keywords: extract-images,flir,thermal,flirtools
 Author: National Drones
 Author-email: development@nationaldrones.com
 Maintainer: olawale williams
```

