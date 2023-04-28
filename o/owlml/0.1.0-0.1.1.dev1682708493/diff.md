# Comparing `tmp/owlml-0.1.0.tar.gz` & `tmp/owlml-0.1.1.dev1682708493.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.0.tar", last modified: Fri Apr 28 18:51:04 2023, max compression
+gzip compressed data, was "owlml-0.1.1.dev1682708493.tar", last modified: Fri Apr 28 19:01:44 2023, max compression
```

## Comparing `owlml-0.1.0.tar` & `owlml-0.1.1.dev1682708493.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-04-28 18:51:04.191900 owlml-0.1.0/
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)      125 2023-04-28 18:51:04.193690 owlml-0.1.0/PKG-INFO
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)     1089 2023-04-28 18:44:14.000000 owlml-0.1.0/README.md
-drwxr-xr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-04-28 18:51:04.060852 owlml-0.1.0/owlml/
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)        0 2023-04-28 18:36:39.000000 owlml-0.1.0/owlml/__init__.py
-drwxr-xr-x   0 jbencook  (1000) jbencook  (1000)        0 2023-04-28 18:51:04.177412 owlml-0.1.0/owlml.egg-info/
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)      125 2023-04-28 18:51:03.000000 owlml-0.1.0/owlml.egg-info/PKG-INFO
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)      190 2023-04-28 18:51:03.000000 owlml-0.1.0/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)        1 2023-04-28 18:51:03.000000 owlml-0.1.0/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)       63 2023-04-28 18:51:03.000000 owlml-0.1.0/owlml.egg-info/requires.txt
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)        6 2023-04-28 18:51:03.000000 owlml-0.1.0/owlml.egg-info/top_level.txt
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)      287 2023-04-28 18:51:04.203873 owlml-0.1.0/setup.cfg
--rw-r--r--   0 jbencook  (1000) jbencook  (1000)       38 2023-04-28 18:36:39.000000 owlml-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/owlml/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/owlml/auth/cvat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 19:01:44.000000 owlml-0.1.1.dev1682708493/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 19:01:44.828027 owlml-0.1.1.dev1682708493/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:01:00.000000 owlml-0.1.1.dev1682708493/setup.py
```

### Comparing `owlml-0.1.0/README.md` & `owlml-0.1.1.dev1682708493/README.md`

 * *Files identical despite different names*

