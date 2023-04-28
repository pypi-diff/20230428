# Comparing `tmp/com_digitalruiz_shopify_http_client-0.0.8.tar.gz` & `tmp/com_digitalruiz_shopify_http_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com_digitalruiz_shopify_http_client-0.0.8.tar", last modified: Thu Jan 19 00:13:22 2023, max compression
+gzip compressed data, was "com_digitalruiz_shopify_http_client-0.0.9.tar", last modified: Thu Jan 19 23:54:18 2023, max compression
```

## Comparing `com_digitalruiz_shopify_http_client-0.0.8.tar` & `com_digitalruiz_shopify_http_client-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:13:22.008185 com_digitalruiz_shopify_http_client-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-19 00:13:08.000000 com_digitalruiz_shopify_http_client-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-19 00:13:22.008185 com_digitalruiz_shopify_http_client-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-19 00:13:08.000000 com_digitalruiz_shopify_http_client-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-19 00:13:08.000000 com_digitalruiz_shopify_http_client-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 00:13:22.008185 com_digitalruiz_shopify_http_client-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:13:22.004185 com_digitalruiz_shopify_http_client-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:13:22.004185 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 00:13:08.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-01-19 00:13:08.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client/shopify_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:13:22.008185 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-19 00:13:21.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-19 00:13:22.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 00:13:21.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-19 00:13:21.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-19 00:13:22.000000 com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 23:54:18.624908 com_digitalruiz_shopify_http_client-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-19 23:54:05.000000 com_digitalruiz_shopify_http_client-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-19 23:54:18.620908 com_digitalruiz_shopify_http_client-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-19 23:54:05.000000 com_digitalruiz_shopify_http_client-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-01-19 23:54:05.000000 com_digitalruiz_shopify_http_client-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 23:54:18.624908 com_digitalruiz_shopify_http_client-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 23:54:18.620908 com_digitalruiz_shopify_http_client-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 23:54:18.620908 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 23:54:05.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-01-19 23:54:05.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client/shopify_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 23:54:18.620908 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-19 23:54:18.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-19 23:54:18.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 23:54:18.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-19 23:54:18.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-19 23:54:18.000000 com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/top_level.txt
```

### Comparing `com_digitalruiz_shopify_http_client-0.0.8/LICENSE` & `com_digitalruiz_shopify_http_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `com_digitalruiz_shopify_http_client-0.0.8/PKG-INFO` & `com_digitalruiz_shopify_http_client-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com_digitalruiz_shopify_http_client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A custom http client for shopify
 Author-email: Reyes Ruiz <reyes@digitalruiz.com>
 Project-URL: Homepage, https://github.com/reyesruiz/shopify_http_client
 Project-URL: Bug Tracker, https://github.com/reyesruiz/shopify_http_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `com_digitalruiz_shopify_http_client-0.0.8/pyproject.toml` & `com_digitalruiz_shopify_http_client-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "com_digitalruiz_shopify_http_client"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Reyes Ruiz", email="reyes@digitalruiz.com" },
 ]
 description = "A custom http client for shopify"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   'requests',
+  'python-dotenv',
   'com-digitalruiz-my-logger',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/reyesruiz/shopify_http_client"
 "Bug Tracker" = "https://github.com/reyesruiz/shopify_http_client/issues"
```

### Comparing `com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client/shopify_http_client.py` & `com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client/shopify_http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 '''
 HTTPS client to connect to shopify:
 Copyright 2023 Reyes Ruiz
 '''
 
-from pathlib import Path
 import sys
 import os
 import time
-import json
 import requests
+from dotenv import load_dotenv, find_dotenv
 from com_digitalruiz_my_logger import my_logger
 
 LOGGER = my_logger.set_logger(module_name=sys.argv[0], loglevel='INFO')
 
 
 def __get_shopify_configs():
     '''
     Getting configs from .Shopify-Config.json locally, if it fails,
     will look it up in home directory
     '''
-    file_name = str(os.getcwd()) + '/.Shopify-Config.json'
-    if not os.path.isfile(file_name):
-        file_name = str(Path.home()) + '/.Shopify-Config.json'
-    with open(file_name, "r", encoding='utf-8') as json_file:
-        shopify_config = json.load(json_file)
+    load_dotenv(find_dotenv())
+    shopify_config = {}
+    shopify_config['shopify_store_name'] = os.environ['shopify_store_name']
+    shopify_config['shopify_admin_api_version'] = os.environ['shopify_admin_api_version']
+    shopify_config['shopify_access_token'] = os.environ['shopify_access_token']
+    shopify_config['shopify_deafult_location'] = os.environ['shopify_deafult_location']
     return shopify_config
 
 def __get_shopify_token():
     '''
     Getting shopify api access token.
     '''
     shopify_config = __get_shopify_configs()
```

### Comparing `com_digitalruiz_shopify_http_client-0.0.8/src/com_digitalruiz_shopify_http_client.egg-info/PKG-INFO` & `com_digitalruiz_shopify_http_client-0.0.9/src/com_digitalruiz_shopify_http_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com-digitalruiz-shopify-http-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A custom http client for shopify
 Author-email: Reyes Ruiz <reyes@digitalruiz.com>
 Project-URL: Homepage, https://github.com/reyesruiz/shopify_http_client
 Project-URL: Bug Tracker, https://github.com/reyesruiz/shopify_http_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

