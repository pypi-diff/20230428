# Comparing `tmp/cryptical-0.2.tar.gz` & `tmp/cryptical-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptical-0.2.tar", last modified: Fri Apr 28 20:52:53 2023, max compression
+gzip compressed data, was "cryptical-0.3.tar", last modified: Fri Apr 28 20:55:08 2023, max compression
```

## Comparing `cryptical-0.2.tar` & `cryptical-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:52:53.226440 cryptical-0.2/
--rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:52:53.225440 cryptical-0.2/PKG-INFO
--rw-r--r--   0 harshit   (1000) harshit   (1000)      785 2023-04-28 20:18:30.000000 cryptical-0.2/README.md
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:52:53.222440 cryptical-0.2/cryptical/
--rw-r--r--   0 harshit   (1000) harshit   (1000)     8616 2023-04-28 20:30:40.000000 cryptical-0.2/cryptical/cryptical.py
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:52:53.225440 cryptical-0.2/cryptical.egg-info/
--rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:52:53.000000 cryptical-0.2/cryptical.egg-info/PKG-INFO
--rw-r--r--   0 harshit   (1000) harshit   (1000)      241 2023-04-28 20:52:53.000000 cryptical-0.2/cryptical.egg-info/SOURCES.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-28 20:52:53.000000 cryptical-0.2/cryptical.egg-info/dependency_links.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       55 2023-04-28 20:52:53.000000 cryptical-0.2/cryptical.egg-info/entry_points.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       89 2023-04-28 20:52:53.000000 cryptical-0.2/cryptical.egg-info/requires.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       10 2023-04-28 20:52:53.000000 cryptical-0.2/cryptical.egg-info/top_level.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       38 2023-04-28 20:52:53.226440 cryptical-0.2/setup.cfg
--rw-r--r--   0 harshit   (1000) harshit   (1000)      521 2023-04-28 20:51:21.000000 cryptical-0.2/setup.py
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:55:08.252367 cryptical-0.3/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:55:08.252367 cryptical-0.3/PKG-INFO
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      785 2023-04-28 20:18:30.000000 cryptical-0.3/README.md
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:55:08.249367 cryptical-0.3/cryptical/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)     8616 2023-04-28 20:30:40.000000 cryptical-0.3/cryptical/cryptical.py
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:55:08.251367 cryptical-0.3/cryptical.egg-info/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/PKG-INFO
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      241 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/SOURCES.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/dependency_links.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       55 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/entry_points.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       75 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/requires.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       10 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/top_level.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       38 2023-04-28 20:55:08.252367 cryptical-0.3/setup.cfg
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      496 2023-04-28 20:54:58.000000 cryptical-0.3/setup.py
```

### Comparing `cryptical-0.2/README.md` & `cryptical-0.3/README.md`

 * *Files identical despite different names*

### Comparing `cryptical-0.2/cryptical/cryptical.py` & `cryptical-0.3/cryptical/cryptical.py`

 * *Files identical despite different names*

