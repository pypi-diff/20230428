# Comparing `tmp/tarvis-tradingbot-0.9.2.tar.gz` & `tmp/tarvis-tradingbot-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-tradingbot-0.9.2.tar", last modified: Thu Apr 27 02:10:17 2023, max compression
+gzip compressed data, was "tarvis-tradingbot-0.9.3.tar", last modified: Fri Apr 28 09:58:13 2023, max compression
```

## Comparing `tarvis-tradingbot-0.9.2.tar` & `tarvis-tradingbot-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 02:10:17.092916 tarvis-tradingbot-0.9.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-27 02:10:07.000000 tarvis-tradingbot-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-27 02:10:17.088916 tarvis-tradingbot-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-27 02:10:07.000000 tarvis-tradingbot-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 02:10:17.092916 tarvis-tradingbot-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-27 02:10:07.000000 tarvis-tradingbot-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 02:10:17.088916 tarvis-tradingbot-0.9.2/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 02:10:17.088916 tarvis-tradingbot-0.9.2/tarvis/tradingbot/
--rw-r--r--   0 root         (0) root         (0)      526 2023-04-27 02:10:07.000000 tarvis-tradingbot-0.9.2/tarvis/tradingbot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 02:10:17.088916 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-27 02:10:17.000000 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-27 02:10:17.000000 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 02:10:17.000000 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-27 02:10:17.000000 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-27 02:10:17.000000 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 02:10:17.000000 tarvis-tradingbot-0.9.2/tarvis_tradingbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:58:13.189347 tarvis-tradingbot-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 09:58:02.000000 tarvis-tradingbot-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-28 09:58:13.189347 tarvis-tradingbot-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-28 09:58:02.000000 tarvis-tradingbot-0.9.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 09:58:13.189347 tarvis-tradingbot-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-28 09:58:02.000000 tarvis-tradingbot-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:58:13.185346 tarvis-tradingbot-0.9.3/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:58:13.185346 tarvis-tradingbot-0.9.3/tarvis/tradingbot/
+-rw-r--r--   0 root         (0) root         (0)      526 2023-04-28 09:58:02.000000 tarvis-tradingbot-0.9.3/tarvis/tradingbot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:58:13.189347 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-28 09:58:13.000000 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-28 09:58:13.000000 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:58:13.000000 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-28 09:58:13.000000 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-28 09:58:13.000000 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 09:58:13.000000 tarvis-tradingbot-0.9.3/tarvis_tradingbot.egg-info/top_level.txt
```

### Comparing `tarvis-tradingbot-0.9.2/LICENSE.txt` & `tarvis-tradingbot-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-tradingbot-0.9.2/setup.py` & `tarvis-tradingbot-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-tradingbot",
-    version="0.9.2",
+    version="0.9.3",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-tradingbot-0.9.2/tarvis/tradingbot/__init__.py` & `tarvis-tradingbot-0.9.3/tarvis/tradingbot/__init__.py`

 * *Files identical despite different names*

