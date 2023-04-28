# Comparing `tmp/tarvis-btb-0.9.2.tar.gz` & `tmp/tarvis-btb-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-btb-0.9.2.tar", last modified: Tue Apr 25 23:42:27 2023, max compression
+gzip compressed data, was "tarvis-btb-0.9.3.tar", last modified: Fri Apr 28 07:59:36 2023, max compression
```

## Comparing `tarvis-btb-0.9.2.tar` & `tarvis-btb-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:42:27.395428 tarvis-btb-0.9.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-25 23:42:27.395428 tarvis-btb-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 23:42:27.395428 tarvis-btb-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:42:27.391427 tarvis-btb-0.9.2/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:42:27.395428 tarvis-btb-0.9.2/tarvis/btb/
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/tarvis/btb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24425 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/tarvis/btb/basictradingbot.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/tarvis/btb/btbs.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/tarvis/btb/exchangeaccount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:42:27.395428 tarvis-btb-0.9.2/tarvis_btb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-25 23:42:27.000000 tarvis-btb-0.9.2/tarvis_btb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-25 23:42:27.000000 tarvis-btb-0.9.2/tarvis_btb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 23:42:27.000000 tarvis-btb-0.9.2/tarvis_btb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 23:42:27.000000 tarvis-btb-0.9.2/tarvis_btb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 23:42:27.000000 tarvis-btb-0.9.2/tarvis_btb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:42:27.395428 tarvis-btb-0.9.2/test/
--rw-r--r--   0 root         (0) root         (0)     3152 2023-04-25 23:42:17.000000 tarvis-btb-0.9.2/test/test_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/tarvis/btb/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/tarvis/btb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24425 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/tarvis/btb/basictradingbot.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/tarvis/btb/btbs.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/tarvis/btb/exchangeaccount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/tarvis_btb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-28 07:59:36.000000 tarvis-btb-0.9.3/tarvis_btb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-28 07:59:36.000000 tarvis-btb-0.9.3/tarvis_btb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:59:36.000000 tarvis-btb-0.9.3/tarvis_btb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 07:59:36.000000 tarvis-btb-0.9.3/tarvis_btb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 07:59:36.000000 tarvis-btb-0.9.3/tarvis_btb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:59:36.103313 tarvis-btb-0.9.3/test/
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-04-28 07:59:26.000000 tarvis-btb-0.9.3/test/test_all.py
```

### Comparing `tarvis-btb-0.9.2/LICENSE.txt` & `tarvis-btb-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.2/setup.py` & `tarvis-btb-0.9.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-btb",
-    version="0.9.2",
+    version="0.9.3",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-btb-0.9.2/tarvis/btb/basictradingbot.py` & `tarvis-btb-0.9.3/tarvis/btb/basictradingbot.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.2/tarvis/btb/btbs.py` & `tarvis-btb-0.9.3/tarvis/btb/btbs.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.2/tarvis/btb/exchangeaccount.py` & `tarvis-btb-0.9.3/tarvis/btb/exchangeaccount.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.2/test/test_all.py` & `tarvis-btb-0.9.3/test/test_all.py`

 * *Files identical despite different names*

