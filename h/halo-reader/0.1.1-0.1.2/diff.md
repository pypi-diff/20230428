# Comparing `tmp/halo-reader-0.1.1.tar.gz` & `tmp/halo-reader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halo-reader-0.1.1.tar", last modified: Tue Apr 25 10:17:28 2023, max compression
+gzip compressed data, was "halo-reader-0.1.2.tar", last modified: Fri Apr 28 11:22:56 2023, max compression
```

## Comparing `halo-reader-0.1.1.tar` & `halo-reader-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 10:17:06.000000 halo-reader-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-25 10:17:06.000000 halo-reader-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 10:17:28.286955 halo-reader-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-25 10:17:06.000000 halo-reader-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 10:17:06.000000 halo-reader-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:17:28.286955 halo-reader-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 10:17:06.000000 halo-reader-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/halo_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:17:27.000000 halo-reader-0.1.1/src/halo_reader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/haloboard/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/haloboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/haloboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/halodata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/halodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/halodata/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/src/haloreader/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/attenuated_backscatter_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/background_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/src/haloreader/background_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-25 10:17:26.000000 halo-reader-0.1.1/src/haloreader/background_reader/background_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/background_reader/background_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/src/haloreader/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-25 10:17:27.000000 halo-reader-0.1.1/src/haloreader/data_reader/data_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/data_reader/data_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/grammar_header.lark
--rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/halo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/type_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-25 10:17:06.000000 halo-reader-0.1.1/tests/test_halo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.929269 halo-reader-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 11:22:29.000000 halo-reader-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-28 11:22:29.000000 halo-reader-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-28 11:22:56.929269 halo-reader-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-28 11:22:29.000000 halo-reader-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-28 11:22:29.000000 halo-reader-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:22:56.929269 halo-reader-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-28 11:22:29.000000 halo-reader-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.913269 halo-reader-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.917269 halo-reader-0.1.2/src/halo_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 11:22:56.000000 halo-reader-0.1.2/src/halo_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.917269 halo-reader-0.1.2/src/haloboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.921269 halo-reader-0.1.2/src/haloboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.921269 halo-reader-0.1.2/src/haloboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloboard/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.921269 halo-reader-0.1.2/src/halodata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/halodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/halodata/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.925269 halo-reader-0.1.2/src/haloreader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/attenuated_backscatter_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/background_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.925269 halo-reader-0.1.2/src/haloreader/background_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-28 11:22:54.000000 halo-reader-0.1.2/src/haloreader/background_reader/background_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/background_reader/background_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.929269 halo-reader-0.1.2/src/haloreader/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-28 11:22:55.000000 halo-reader-0.1.2/src/haloreader/data_reader/data_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/data_reader/data_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/grammar_header.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/halo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/type_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 11:22:29.000000 halo-reader-0.1.2/src/haloreader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:22:56.929269 halo-reader-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-28 11:22:29.000000 halo-reader-0.1.2/tests/test_halo_reader.py
```

### Comparing `halo-reader-0.1.1/LICENSE` & `halo-reader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/PKG-INFO` & `halo-reader-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.1.1
+Version: 0.1.2
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.1.1/README.md` & `halo-reader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/pyproject.toml` & `halo-reader-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/setup.py` & `halo-reader-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/halo_reader.egg-info/PKG-INFO` & `halo-reader-0.1.2/src/halo_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.1.1
+Version: 0.1.2
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.1.1/src/halo_reader.egg-info/SOURCES.txt` & `halo-reader-0.1.2/src/halo_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloboard/app.py` & `halo-reader-0.1.2/src/haloboard/app.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloboard/static/favicon.ico` & `halo-reader-0.1.2/src/haloboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloboard/static/style.css` & `halo-reader-0.1.2/src/haloboard/static/style.css`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloboard/templates/index.html` & `halo-reader-0.1.2/src/haloboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/halodata/datasets.py` & `halo-reader-0.1.2/src/halodata/datasets.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/attenuated_backscatter_coefficient.py` & `halo-reader-0.1.2/src/haloreader/attenuated_backscatter_coefficient.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/attribute.py` & `halo-reader-0.1.2/src/haloreader/attribute.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/background_correction.py` & `halo-reader-0.1.2/src/haloreader/background_correction.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/background_reader/background_reader.c` & `halo-reader-0.1.2/src/haloreader/background_reader/background_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/background_reader/background_reader.pyx` & `halo-reader-0.1.2/src/haloreader/background_reader/background_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/cli.py` & `halo-reader-0.1.2/src/haloreader/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,25 @@
     log.info("Create netCDF")
     nc_buff = halo.to_nc()
     with open(f"halo_{args.site}_{args.date}.nc", "wb") as f:
         f.write(nc_buff)
     if args.plot:
         log.info("Create plots")
         writer = Writer()
-        fig, ax = plt.subplots(3, 1, figsize=(24, 16))
+        fig, ax = plt.subplots(nplots := 6, 1, figsize=(24, nplots * 6))
         halo.intensity_raw.plot(ax[0])
         halo.doppler_velocity.plot(ax[1])
         if halo.intensity is not None:
             halo.intensity.plot(ax[2])
+        if halo.beta is not None:
+            halo.beta.plot(ax[3])
+        if halo.beta_screened is not None:
+            halo.beta_screened.plot(ax[4])
+        if halo.doppler_velocity_screened is not None:
+            halo.doppler_velocity_screened.plot(ax[5])
 
         writer.add_figure(f"halo_{args.site}_{args.date}", fig)
 
 
 def _from_raw(args: argparse.Namespace) -> None:
     halo_src = [src for src in args.src if src.name.endswith(".hpl")]
     bg_src = [
```

### Comparing `halo-reader-0.1.1/src/haloreader/data_reader/data_reader.c` & `halo-reader-0.1.2/src/haloreader/data_reader/data_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/data_reader/data_reader.pyx` & `halo-reader-0.1.2/src/haloreader/data_reader/data_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/grammar_header.lark` & `halo-reader-0.1.2/src/haloreader/grammar_header.lark`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/halo.py` & `halo-reader-0.1.2/src/haloreader/halo.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/metadata.py` & `halo-reader-0.1.2/src/haloreader/metadata.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/read.py` & `halo-reader-0.1.2/src/haloreader/read.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 from haloreader.data_reader import read_data
 from haloreader.exceptions import BackgroundReadError
 from haloreader.halo import Halo, HaloBg
 from haloreader.metadata import Metadata
 from haloreader.utils import UNIX_TIME_UNIT
 from haloreader.variable import Variable
 
-from .exceptions import FileEmpty, HeaderNotFound, UnexpectedDataTokens
+from .exceptions import (
+    FileEmpty,
+    HeaderNotFound,
+    InconsistentRangeError,
+    UnexpectedDataTokens,
+)
 from .transformer import HeaderTransformer
 
 log = logging.getLogger(__name__)
 
 grammar_header = pkgutil.get_data("haloreader", "grammar_header.lark")
 if not isinstance(grammar_header, bytes):
     raise FileNotFoundError("Header grammar file not found")
@@ -39,36 +44,52 @@
     )
     log.info("Reading data from %s", metadata.filename.value)
     data_bytes = _read_data(src, header_end)
     if not isinstance(metadata.ngates.data, int):
         raise TypeError
     read_data(data_bytes, metadata.ngates.data, time_vars, time_range_vars)
     vars_ = {var.name: var for var in time_vars + time_range_vars}
+    if not _range_consistent(vars_["range"]):
+        raise InconsistentRangeError
     vars_["time"] = _decimaltime2timestamp(vars_["time"], metadata)
     vars_["range"] = range_func(vars_["range"], metadata.gate_range)
     return Halo(metadata=metadata, **vars_)
 
 
 def read(src_files: Sequence[Path | BytesIO]) -> Halo | None:
     halos = []
     for src in src_files:
         try:
             halos.append(_read_single(src))
         except (
             FileEmpty,
             HeaderNotFound,
+            InconsistentRangeError,
             UnicodeDecodeError,
             UnexpectedInput,
             UnexpectedDataTokens,
         ) as err:
             log.warning("Skipping file", exc_info=err)
     log.info("Merging files")
     return Halo.merge(halos)
 
 
+def _range_consistent(range_var: Variable) -> bool:
+    if not isinstance(range_var.dimensions, tuple):
+        raise TypeError
+    if not isinstance(range_var.data, np.ndarray):
+        raise TypeError
+    if len(range_var.dimensions) != 2 or range_var.dimensions[1] != "range":
+        return False
+    expected_range = np.arange(range_var.data.shape[1], dtype=range_var.data.dtype)
+    if all(np.allclose(expected_range, r) for r in range_var.data):
+        return True
+    return False
+
+
 def read_bg(
     src_files: Sequence[Path | BytesIO], filenames: list[str] | None = None
 ) -> HaloBg | None:
     halobgs = []
     for src, fname in _bg_src_fname_list(src_files, filenames):
         bg_bytes = _read_background(src)
         background = read_background(bg_bytes)
```

### Comparing `halo-reader-0.1.1/src/haloreader/scantype.py` & `halo-reader-0.1.2/src/haloreader/scantype.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/screen.py` & `halo-reader-0.1.2/src/haloreader/screen.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,15 @@
     # visually checking the output
     intensity_mean_mask = uniform_filter(intensity.data, size=(21, 3)) > 1.0025
     velocity_abs_mean_mask = (
         uniform_filter(np.abs(doppler_velocity.data), size=(21, 3)) < 2
     )
     bad_gates = np.zeros_like(intensity.data, dtype=bool)
     bad_gates[:, :3] = True
+    below_one = intensity.data < 1
     return Variable(
         name="noise_screen",
         dimensions=intensity.dimensions,
-        data=np.logical_not(intensity_mean_mask | velocity_abs_mean_mask) | bad_gates,
+        data=np.logical_not(intensity_mean_mask | velocity_abs_mean_mask)
+        | bad_gates
+        | below_one,
     )
```

### Comparing `halo-reader-0.1.1/src/haloreader/transformer.py` & `halo-reader-0.1.2/src/haloreader/transformer.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/type_guards.py` & `halo-reader-0.1.2/src/haloreader/type_guards.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/utils.py` & `halo-reader-0.1.2/src/haloreader/utils.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.1/src/haloreader/variable.py` & `halo-reader-0.1.2/src/haloreader/variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,14 +118,16 @@
     def plot(self, ax: Axes) -> None:  # type: ignore[no-any-unimported]
         if "intensity" in self.name:
             _plot_intensity(self, ax)
         elif "background" in self.name:
             _plot_background(self, ax)
         elif "doppler_velocity" in self.name:
             _plot_doppler_velocity(self, ax)
+        elif "beta" in self.name:
+            _plot_beta(self, ax)
         else:
             raise NotImplementedError(
                 f"Plotting not implemented for variable {self.name}"
             )
 
 
 @runtime_checkable
@@ -148,20 +150,35 @@
         vmax=vmax,
         aspect="auto",
         interpolation="none",
     )
     ax.set_title(var.name)
 
 
+def _plot_beta(var: Variable, ax: Axes) -> None:  # type: ignore[no-any-unimported]
+    if not isinstance(var.data, np.ndarray):
+        raise TypeError
+    vmin, vmax = (1e-7, 1e-4)
+    ax.imshow(
+        var.data.T,
+        origin="lower",
+        aspect="auto",
+        interpolation="none",
+        vmin=vmin,
+        vmax=vmax,
+    )
+    ax.set_title(var.name)
+
+
 def _plot_doppler_velocity(  # type: ignore[no-any-unimported]
     var: Variable, ax: Axes
 ) -> None:
     if not isinstance(var.data, np.ndarray):
         raise TypeError
-    vdelta = 10
+    vdelta = 4
     vmin, vmax = (-vdelta, vdelta)
     ax.imshow(
         var.data.T,
         origin="lower",
         aspect="auto",
         cmap="bwr",
         vmin=vmin,
```

### Comparing `halo-reader-0.1.1/tests/test_halo_reader.py` & `halo-reader-0.1.2/tests/test_halo_reader.py`

 * *Files identical despite different names*

