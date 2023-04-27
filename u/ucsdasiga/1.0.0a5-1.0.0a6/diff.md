# Comparing `tmp/ucsdasiga-1.0.0a5.tar.gz` & `tmp/ucsdasiga-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucsdasiga-1.0.0a5.tar", last modified: Thu Apr 27 00:20:28 2023, max compression
+gzip compressed data, was "ucsdasiga-1.0.0a6.tar", last modified: Thu Apr 27 22:42:37 2023, max compression
```

## Comparing `ucsdasiga-1.0.0a5.tar` & `ucsdasiga-1.0.0a6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 00:20:28.309195 ucsdasiga-1.0.0a5/
--rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasiga-1.0.0a5/LICENSE
--rw-rw-rw-   0        0        0     2243 2023-04-27 00:20:28.309195 ucsdasiga-1.0.0a5/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-27 00:15:43.000000 ucsdasiga-1.0.0a5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 00:20:28.295022 ucsdasiga-1.0.0a5/asiga/
--rw-rw-rw-   0        0        0     1119 2023-04-27 00:15:28.000000 ucsdasiga-1.0.0a5/asiga/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasiga-1.0.0a5/asiga/__main__.py
--rw-rw-rw-   0        0        0     2860 2023-04-26 22:40:41.000000 ucsdasiga-1.0.0a5/asiga/scraper.py
--rw-rw-rw-   0        0        0     1117 2023-04-27 00:19:34.000000 ucsdasiga-1.0.0a5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 00:20:28.309195 ucsdasiga-1.0.0a5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 00:20:28.305212 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/
--rw-rw-rw-   0        0        0     2243 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 22:42:37.881288 ucsdasiga-1.0.0a6/
+-rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasiga-1.0.0a6/LICENSE
+-rw-rw-rw-   0        0        0     8465 2023-04-27 22:42:37.880273 ucsdasiga-1.0.0a6/PKG-INFO
+-rw-rw-rw-   0        0        0     6235 2023-04-27 20:14:28.000000 ucsdasiga-1.0.0a6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 22:42:37.826640 ucsdasiga-1.0.0a6/asiga/
+-rw-rw-rw-   0        0        0     1692 2023-04-27 20:14:28.000000 ucsdasiga-1.0.0a6/asiga/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasiga-1.0.0a6/asiga/__main__.py
+-rw-rw-rw-   0        0        0     2413 2023-04-27 20:14:28.000000 ucsdasiga-1.0.0a6/asiga/scraper.py
+-rw-rw-rw-   0        0        0     1117 2023-04-27 22:40:53.000000 ucsdasiga-1.0.0a6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 22:42:37.881288 ucsdasiga-1.0.0a6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 22:42:37.878567 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/
+-rw-rw-rw-   0        0        0     8465 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/top_level.txt
```

### Comparing `ucsdasiga-1.0.0a5/LICENSE` & `ucsdasiga-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ucsdasiga-1.0.0a5/asiga/scraper.py` & `ucsdasiga-1.0.0a6/asiga/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 """
 
 import datetime
-import pathlib
 import re
 import typing
 
 import pandas as pd
 import requests
 
 
@@ -81,24 +80,7 @@
         assert len(dfs) == 1
         dataframe = dfs[0]
 
         columns = ["A", "B", "C", "D", "F", "W", "P", "NP"]
         dataframe[columns] = dataframe[columns].applymap(lambda x: float(x.strip("%")))
 
         return dataframe
-
-    def export(self, path: typing.Union[str, pathlib.Path]) -> pathlib.Path:
-        """
-
-        :param path:
-        :return:
-        """
-        path = pathlib.Path(path)
-        dataframe = self.data()
-
-        if path.suffix == ".csv":
-            dataframe.to_csv(path)
-        else:
-            with open(path, "w", encoding="utf-8") as file:
-                dataframe.to_string(file)
-
-        return path
```

### Comparing `ucsdasiga-1.0.0a5/pyproject.toml` & `ucsdasiga-1.0.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ucsdasiga"
-version = "1.0.0-a.5"
+version = "1.0.0-a.6"
 description = "A simple API wrapper and web scraper for the UCSD Associated Students (AS) instructor grade archive."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
```

