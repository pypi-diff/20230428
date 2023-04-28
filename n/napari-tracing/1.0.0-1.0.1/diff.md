# Comparing `tmp/napari-tracing-1.0.0.tar.gz` & `tmp/napari-tracing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tracing-1.0.0.tar", last modified: Sun Apr 23 04:47:48 2023, max compression
+gzip compressed data, was "napari-tracing-1.0.1.tar", last modified: Fri Apr 28 18:06:18 2023, max compression
```

## Comparing `napari-tracing-1.0.0.tar` & `napari-tracing-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:47:48.110237 napari-tracing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-23 04:47:48.110237 napari-tracing-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-23 04:47:48.110237 napari-tracing-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:47:48.106237 napari-tracing-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:47:48.110237 napari-tracing-1.0.0/src/napari_tracing/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_dialog_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_layer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_segment_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:47:48.110237 napari-tracing-1.0.0/src/napari_tracing/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_trace_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_trace_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    33433 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 04:47:31.000000 napari-tracing-1.0.0/src/napari_tracing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:47:48.110237 napari-tracing-1.0.0/src/napari_tracing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-23 04:47:48.000000 napari-tracing-1.0.0/src/napari_tracing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 04:47:48.000000 napari-tracing-1.0.0/src/napari_tracing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:47:48.000000 napari-tracing-1.0.0/src/napari_tracing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 04:47:48.000000 napari-tracing-1.0.0/src/napari_tracing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 04:47:48.000000 napari-tracing-1.0.0/src/napari_tracing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 04:47:48.000000 napari-tracing-1.0.0/src/napari_tracing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:06:18.800350 napari-tracing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-28 18:06:18.800350 napari-tracing-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-28 18:06:18.800350 napari-tracing-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:06:18.796350 napari-tracing-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:06:18.800350 napari-tracing-1.0.1/src/napari_tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_dialog_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_layer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_segment_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:06:18.800350 napari-tracing-1.0.1/src/napari_tracing/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_trace_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_trace_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33433 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-28 18:05:58.000000 napari-tracing-1.0.1/src/napari_tracing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:06:18.800350 napari-tracing-1.0.1/src/napari_tracing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-28 18:06:18.000000 napari-tracing-1.0.1/src/napari_tracing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-28 18:06:18.000000 napari-tracing-1.0.1/src/napari_tracing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:06:18.000000 napari-tracing-1.0.1/src/napari_tracing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 18:06:18.000000 napari-tracing-1.0.1/src/napari_tracing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 18:06:18.000000 napari-tracing-1.0.1/src/napari_tracing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 18:06:18.000000 napari-tracing-1.0.1/src/napari_tracing.egg-info/top_level.txt
```

### Comparing `napari-tracing-1.0.0/LICENSE` & `napari-tracing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/setup.cfg` & `napari-tracing-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-tracing
-version = 1.0.0
+version = 1.0.1
 description = A plugin to trace the brightest path between two points in an image
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mapmanager/napari-tracing
 author = Vasudha Jha
 author_email = reachvasudha27@gmail.com
 license = GPL-3.0-only
```

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_combobox.py` & `napari-tracing-1.0.1/src/napari_tracing/_combobox.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_dialog_widget.py` & `napari-tracing-1.0.1/src/napari_tracing/_dialog_widget.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_logger.py` & `napari-tracing-1.0.1/src/napari_tracing/_logger.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_segment_model.py` & `napari-tracing-1.0.1/src/napari_tracing/_segment_model.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_tests/test_widget.py` & `napari-tracing-1.0.1/src/napari_tracing/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_trace_loader.py` & `napari-tracing-1.0.1/src/napari_tracing/_trace_loader.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_trace_saver.py` & `napari-tracing-1.0.1/src/napari_tracing/_trace_saver.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/_widget.py` & `napari-tracing-1.0.1/src/napari_tracing/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/point.py` & `napari-tracing-1.0.1/src/napari_tracing/point.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing/utils.py` & `napari-tracing-1.0.1/src/napari_tracing/utils.py`

 * *Files identical despite different names*

### Comparing `napari-tracing-1.0.0/src/napari_tracing.egg-info/SOURCES.txt` & `napari-tracing-1.0.1/src/napari_tracing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

