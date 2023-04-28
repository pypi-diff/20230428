# Comparing `tmp/stc-tools-1.0.8.tar.gz` & `tmp/stc-tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-tools-1.0.8.tar", last modified: Wed Apr 26 12:06:25 2023, max compression
+gzip compressed data, was "stc-tools-1.0.9.tar", last modified: Wed Apr 26 14:03:35 2023, max compression
```

## Comparing `stc-tools-1.0.8.tar` & `stc-tools-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-04-26 12:06:25.123672 stc-tools-1.0.8/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.0.8/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-04-26 12:06:25.123276 stc-tools-1.0.8/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.0.8/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      560 2023-04-26 12:06:13.000000 stc-tools-1.0.8/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       29 2023-04-26 12:04:12.000000 stc-tools-1.0.8/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-04-26 12:06:25.123849 stc-tools-1.0.8/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-04-26 12:06:25.120097 stc-tools-1.0.8/stc_tools/
--rw-r--r--   0 pasha      (501) staff       (20)     3497 2023-04-26 12:03:42.000000 stc-tools-1.0.8/stc_tools/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     1885 2023-04-26 12:05:53.000000 stc-tools-1.0.8/stc_tools/client.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-04-26 12:06:25.122703 stc-tools-1.0.8/stc_tools.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-04-26 12:06:25.000000 stc-tools-1.0.8/stc_tools.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      290 2023-04-26 12:06:25.000000 stc-tools-1.0.8/stc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-04-26 12:06:25.000000 stc-tools-1.0.8/stc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       49 2023-04-26 12:06:25.000000 stc-tools-1.0.8/stc_tools.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       30 2023-04-26 12:06:25.000000 stc-tools-1.0.8/stc_tools.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-04-26 12:06:25.000000 stc-tools-1.0.8/stc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-04-26 14:03:35.277772 stc-tools-1.0.9/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.0.9/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-04-26 14:03:35.277374 stc-tools-1.0.9/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.0.9/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      560 2023-04-26 14:03:16.000000 stc-tools-1.0.9/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       34 2023-04-26 14:03:14.000000 stc-tools-1.0.9/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-04-26 14:03:35.277918 stc-tools-1.0.9/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-04-26 14:03:35.273425 stc-tools-1.0.9/stc_tools/
+-rw-r--r--   0 pasha      (501) staff       (20)     3497 2023-04-26 12:03:42.000000 stc-tools-1.0.9/stc_tools/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1885 2023-04-26 12:05:53.000000 stc-tools-1.0.9/stc_tools/client.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-04-26 14:03:35.276743 stc-tools-1.0.9/stc_tools.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-04-26 14:03:35.000000 stc-tools-1.0.9/stc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      290 2023-04-26 14:03:35.000000 stc-tools-1.0.9/stc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-04-26 14:03:35.000000 stc-tools-1.0.9/stc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       49 2023-04-26 14:03:35.000000 stc-tools-1.0.9/stc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       35 2023-04-26 14:03:35.000000 stc-tools-1.0.9/stc_tools.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-04-26 14:03:35.000000 stc-tools-1.0.9/stc_tools.egg-info/top_level.txt
```

### Comparing `stc-tools-1.0.8/pyproject.toml` & `stc-tools-1.0.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-tools"
-version = "1.0.8"
+version = "1.0.9"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Standard Template Construct Client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-tools-1.0.8/stc_tools/cli.py` & `stc-tools-1.0.9/stc_tools/cli.py`

 * *Files identical despite different names*

### Comparing `stc-tools-1.0.8/stc_tools/client.py` & `stc-tools-1.0.9/stc_tools/client.py`

 * *Files identical despite different names*

