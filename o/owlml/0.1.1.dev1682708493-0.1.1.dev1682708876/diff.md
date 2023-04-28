# Comparing `tmp/owlml-0.1.1.dev1682708493.tar.gz` & `tmp/owlml-0.1.1.dev1682708876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.1.dev1682708493.tar", last modified: Fri Apr 28 19:01:44 2023, max compression
+gzip compressed data, was "owlml-0.1.1.dev1682708876.tar", last modified: Fri Apr 28 19:08:10 2023, max compression
```

## Comparing `owlml-0.1.1.dev1682708493.tar` & `owlml-0.1.1.dev1682708876.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/owlml/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/auth/cvat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:08:10.091710 owlml-0.1.1.dev1682708876/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:08:10.091710 owlml-0.1.1.dev1682708876/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:08:10.091710 owlml-0.1.1.dev1682708876/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/owlml/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:08:10.091710 owlml-0.1.1.dev1682708876/owlml/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/owlml/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/owlml/auth/cvat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:08:10.091710 owlml-0.1.1.dev1682708876/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:08:10.000000 owlml-0.1.1.dev1682708876/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 19:08:10.000000 owlml-0.1.1.dev1682708876/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:08:10.000000 owlml-0.1.1.dev1682708876/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:08:10.000000 owlml-0.1.1.dev1682708876/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 19:08:10.000000 owlml-0.1.1.dev1682708876/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 19:08:10.000000 owlml-0.1.1.dev1682708876/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 19:08:10.091710 owlml-0.1.1.dev1682708876/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:07:16.000000 owlml-0.1.1.dev1682708876/setup.py
```

### Comparing `owlml-0.1.1.dev1682708493/README.md` & `owlml-0.1.1.dev1682708876/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.1.dev1682708493/owlml/auth/cvat.py` & `owlml-0.1.1.dev1682708876/owlml/auth/cvat.py`

 * *Files identical despite different names*

