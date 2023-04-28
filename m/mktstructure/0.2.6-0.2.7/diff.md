# Comparing `tmp/mktstructure-0.2.6.tar.gz` & `tmp/mktstructure-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktstructure-0.2.6.tar", last modified: Fri Apr 28 01:04:34 2023, max compression
+gzip compressed data, was "mktstructure-0.2.7.tar", last modified: Fri Apr 28 02:03:42 2023, max compression
```

## Comparing `mktstructure-0.2.6.tar` & `mktstructure-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.166175 mktstructure-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 01:04:28.000000 mktstructure-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 01:04:34.166175 mktstructure-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-28 01:04:28.000000 mktstructure-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.162175 mktstructure-0.2.6/mktstructure/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_download_mktdepth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.166175 mktstructure-0.2.6/mktstructure/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/bidask_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/effective_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/price_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/realized_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/variance_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/request_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/trth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/trth_parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.166175 mktstructure-0.2.6/mktstructure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 01:04:34.000000 mktstructure-0.2.6/mktstructure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:04:34.166175 mktstructure-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 01:04:28.000000 mktstructure-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.723733 mktstructure-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 02:03:38.000000 mktstructure-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 02:03:42.719733 mktstructure-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-28 02:03:38.000000 mktstructure-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.719733 mktstructure-0.2.7/mktstructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_download_mktdepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.719733 mktstructure-0.2.7/mktstructure/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/bidask_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/effective_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/price_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/realized_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/variance_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/request_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/trth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/trth_parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.719733 mktstructure-0.2.7/mktstructure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:03:42.723733 mktstructure-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 02:03:38.000000 mktstructure-0.2.7/setup.py
```

### Comparing `mktstructure-0.2.6/LICENSE` & `mktstructure-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/PKG-INFO` & `mktstructure-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktstructure
-Version: 0.2.6
+Version: 0.2.7
 Summary: Download data from Refinitiv Tick History and compute some market microstructure measures.
 Home-page: https://github.com/mgao6767/mktstructure
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Description: # mktstructure
```

### Comparing `mktstructure-0.2.6/README.md` & `mktstructure-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/cmd_classify.py` & `mktstructure-0.2.7/mktstructure/cmd_classify.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/cmd_clean.py` & `mktstructure-0.2.7/mktstructure/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/cmd_compute.py` & `mktstructure-0.2.7/mktstructure/cmd_compute.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/cmd_download.py` & `mktstructure-0.2.7/mktstructure/cmd_download.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/cmd_download_mktdepth.py` & `mktstructure-0.2.7/mktstructure/cmd_download_mktdepth.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         args.ric.extend(
             extract_index_components_ric(
                 trth.get_index_components([SP500_RIC], start_date, end_date),
                 mkt_index=[SP500_RIC],
             )
         )
 
-    data = trth.get_table(args.ric, start_date, end_date)
+    data = trth.get_table_mktdepth(args.ric, start_date, end_date)
 
     print(f"Saving data to {args.o}...")
 
     trth.save_results(data, args.o)
 
     print("Downloading finished.")
```

### Comparing `mktstructure-0.2.6/mktstructure/main.py` & `mktstructure-0.2.7/mktstructure/main.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/measures/bidask_spread.py` & `mktstructure-0.2.7/mktstructure/measures/bidask_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/measures/effective_spread.py` & `mktstructure-0.2.7/mktstructure/measures/effective_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/measures/price_impact.py` & `mktstructure-0.2.7/mktstructure/measures/price_impact.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/measures/realized_spread.py` & `mktstructure-0.2.7/mktstructure/measures/realized_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/measures/variance_ratio.py` & `mktstructure-0.2.7/mktstructure/measures/variance_ratio.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/request_templates.py` & `mktstructure-0.2.7/mktstructure/request_templates.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/trth.py` & `mktstructure-0.2.7/mktstructure/trth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import requests
 import time
 
-from .utils import make_request_index_components, make_request_tick_history
+from .utils import (
+    make_request_index_components,
+    make_request_tick_history,
+    make_request_tick_history_market_depth,
+)
 
 # URL_BASE = "https://hosted.datascopeapi.reuters.com/RestApi/v1"
 URL_BASE = "https://selectapi.datascope.refinitiv.com/RestApi/v1"
 
 AUTH_URL = f"{URL_BASE}/Authentication/RequestToken"
 SEARCH_HIST_CHAIN_URL = f"{URL_BASE}/Search/HistoricalChainResolution"
 EXTRACT_RAW_URL = f"{URL_BASE}/Extractions/ExtractRaw"
@@ -41,14 +45,18 @@
         resp = self.session.post(SEARCH_HIST_CHAIN_URL, payload)
         return resp.json()
 
     def get_table(self, rics, start_date, end_date):
         req = make_request_tick_history(rics, start_date, end_date)
         return self.extract_raw(req)
 
+    def get_table_mktdepth(self, rics, start_date, end_date):
+        req = make_request_tick_history_market_depth(rics, start_date, end_date)
+        return self.extract_raw(req)
+
     def _getAccessToken(self) -> str:
         """Return the access Token"""
         _data = {
             "Credentials": {
                 "Username": self._username,
                 "Password": self._password,
             }
```

### Comparing `mktstructure-0.2.6/mktstructure/trth_parser.c` & `mktstructure-0.2.7/mktstructure/trth_parser.c`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure/utils.py` & `mktstructure-0.2.7/mktstructure/utils.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/mktstructure.egg-info/PKG-INFO` & `mktstructure-0.2.7/mktstructure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktstructure
-Version: 0.2.6
+Version: 0.2.7
 Summary: Download data from Refinitiv Tick History and compute some market microstructure measures.
 Home-page: https://github.com/mgao6767/mktstructure
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Description: # mktstructure
```

### Comparing `mktstructure-0.2.6/mktstructure.egg-info/SOURCES.txt` & `mktstructure-0.2.7/mktstructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.6/setup.py` & `mktstructure-0.2.7/setup.py`

 * *Files identical despite different names*

