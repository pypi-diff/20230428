# Comparing `tmp/tarvis-exchange-woo-0.9.3.tar.gz` & `tmp/tarvis-exchange-woo-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-woo-0.9.3.tar", last modified: Fri Apr 28 08:03:00 2023, max compression
+gzip compressed data, was "tarvis-exchange-woo-0.9.4.tar", last modified: Fri Apr 28 10:08:03 2023, max compression
```

## Comparing `tarvis-exchange-woo-0.9.3.tar` & `tarvis-exchange-woo-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      767 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.453954 tarvis-exchange-woo-0.9.3/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.453954 tarvis-exchange-woo-0.9.3/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.453954 tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/
--rw-r--r--   0 root         (0) root         (0)    10910 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11285 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/wooclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/test/
--rw-r--r--   0 root         (0) root         (0)    11990 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/test/test_exchange_woo_margin.py
--rw-r--r--   0 root         (0) root         (0)    11996 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/test/test_exchange_woo_perpetual.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/test/test_exchange_woo_spot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      767 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.485413 tarvis-exchange-woo-0.9.4/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.485413 tarvis-exchange-woo-0.9.4/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/
+-rw-r--r--   0 root         (0) root         (0)    10910 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11285 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/wooclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/test/
+-rw-r--r--   0 root         (0) root         (0)    11990 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/test/test_exchange_woo_margin.py
+-rw-r--r--   0 root         (0) root         (0)    11996 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/test/test_exchange_woo_perpetual.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/test/test_exchange_woo_spot.py
```

### Comparing `tarvis-exchange-woo-0.9.3/LICENSE.txt` & `tarvis-exchange-woo-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.3/setup.py` & `tarvis-exchange-woo-0.9.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-woo",
-    version="0.9.3",
+    version="0.9.4",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for Woo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/__init__.py` & `tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/wooclient.py` & `tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/wooclient.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.3/test/test_exchange_woo_margin.py` & `tarvis-exchange-woo-0.9.4/test/test_exchange_woo_margin.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.3/test/test_exchange_woo_perpetual.py` & `tarvis-exchange-woo-0.9.4/test/test_exchange_woo_perpetual.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.3/test/test_exchange_woo_spot.py` & `tarvis-exchange-woo-0.9.4/test/test_exchange_woo_spot.py`

 * *Files identical despite different names*

