# Comparing `tmp/tap_shiftbase-1.0.0.tar.gz` & `tmp/tap_shiftbase-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shiftbase-1.0.0.tar", max compression
+gzip compressed data, was "tap_shiftbase-1.0.1.tar", max compression
```

## Comparing `tap_shiftbase-1.0.0.tar` & `tap_shiftbase-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-1.0.0/README.md
--rw-r--r--   0        0        0     1078 2023-04-24 11:00:53.404675 tap_shiftbase-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-1.0.0/tap_shiftbase/__init__.py
--rw-r--r--   0        0        0     3440 2023-04-23 14:51:42.320155 tap_shiftbase-1.0.0/tap_shiftbase/client.py
--rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentee_options.json
--rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentees.json
--rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-1.0.0/tap_shiftbase/schemas/contract_types.json
--rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-1.0.0/tap_shiftbase/schemas/custom_fields.json
--rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-1.0.0/tap_shiftbase/schemas/departments.json
--rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-1.0.0/tap_shiftbase/schemas/docs.json
--rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-1.0.0/tap_shiftbase/schemas/locations.json
--rw-r--r--   0        0        0     5731 2023-04-24 10:57:42.043955 tap_shiftbase-1.0.0/tap_shiftbase/schemas/rosters.json
--rw-r--r--   0        0        0     3512 2023-04-24 06:41:32.883984 tap_shiftbase-1.0.0/tap_shiftbase/schemas/shifts.json
--rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-1.0.0/tap_shiftbase/schemas/teams.json
--rw-r--r--   0        0        0    13203 2023-04-24 10:59:43.238525 tap_shiftbase-1.0.0/tap_shiftbase/schemas/timesheets.json
--rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-1.0.0/tap_shiftbase/schemas/users.json
--rw-r--r--   0        0        0     2548 2023-04-24 06:55:35.086547 tap_shiftbase-1.0.0/tap_shiftbase/streams.py
--rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-1.0.0/tap_shiftbase/tap.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3110 2023-04-07 11:27:41.183945 tap_shiftbase-1.0.1/README.md
+-rw-r--r--   0        0        0     1078 2023-04-28 11:05:34.780992 tap_shiftbase-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-07 11:27:41.193691 tap_shiftbase-1.0.1/tap_shiftbase/__init__.py
+-rw-r--r--   0        0        0     3654 2023-04-28 11:05:23.809227 tap_shiftbase-1.0.1/tap_shiftbase/client.py
+-rw-r--r--   0        0        0     1193 2023-04-23 14:51:12.161977 tap_shiftbase-1.0.1/tap_shiftbase/schemas/absentee_options.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:20.335499 tap_shiftbase-1.0.1/tap_shiftbase/schemas/absentees.json
+-rw-r--r--   0        0        0     1624 2023-04-23 14:56:11.138011 tap_shiftbase-1.0.1/tap_shiftbase/schemas/contract_types.json
+-rw-r--r--   0        0        0      821 2023-04-23 14:52:30.815793 tap_shiftbase-1.0.1/tap_shiftbase/schemas/custom_fields.json
+-rw-r--r--   0        0        0     3098 2023-04-23 14:52:35.921568 tap_shiftbase-1.0.1/tap_shiftbase/schemas/departments.json
+-rw-r--r--   0        0        0  1373258 2023-04-21 13:49:20.419188 tap_shiftbase-1.0.1/tap_shiftbase/schemas/docs.json
+-rw-r--r--   0        0        0      732 2023-04-23 14:52:42.342142 tap_shiftbase-1.0.1/tap_shiftbase/schemas/locations.json
+-rw-r--r--   0        0        0     5731 2023-04-24 10:57:42.043955 tap_shiftbase-1.0.1/tap_shiftbase/schemas/rosters.json
+-rw-r--r--   0        0        0     3512 2023-04-24 06:41:32.883984 tap_shiftbase-1.0.1/tap_shiftbase/schemas/shifts.json
+-rw-r--r--   0        0        0     1129 2023-04-23 14:53:30.521959 tap_shiftbase-1.0.1/tap_shiftbase/schemas/teams.json
+-rw-r--r--   0        0        0    13203 2023-04-24 10:59:43.238525 tap_shiftbase-1.0.1/tap_shiftbase/schemas/timesheets.json
+-rw-r--r--   0        0        0     3675 2023-04-23 14:53:39.566226 tap_shiftbase-1.0.1/tap_shiftbase/schemas/users.json
+-rw-r--r--   0        0        0     2548 2023-04-24 06:55:35.086547 tap_shiftbase-1.0.1/tap_shiftbase/streams.py
+-rw-r--r--   0        0        0     1571 2023-04-21 13:29:44.823280 tap_shiftbase-1.0.1/tap_shiftbase/tap.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 tap_shiftbase-1.0.1/PKG-INFO
```

### Comparing `tap_shiftbase-1.0.0/README.md` & `tap_shiftbase-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/pyproject.toml` & `tap_shiftbase-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shiftbase"
-version = "1.0.0"
+version = "1.0.1"
 description = "`tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "shiftbase",
 ]
```

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/client.py` & `tap_shiftbase-1.0.1/tap_shiftbase/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Callable, Iterable
 
 import requests
 from singer_sdk.authenticators import APIKeyAuthenticator
 from singer_sdk.helpers.jsonpath import extract_jsonpath
 from singer_sdk.streams import RESTStream
 
-import logging
+from datetime import datetime, timedelta
 
 _Auth = Callable[[requests.PreparedRequest], requests.PreparedRequest]
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class shiftbaseStream(RESTStream):
     """shiftbase stream class."""
@@ -79,14 +79,17 @@
             context: The stream context.
             next_page_token: The next page index or value.
 
         Returns:
             A dictionary of URL query parameters.
         """
         params: dict = {}
+        if self.name == "timesheets" or self.name == "rosters":
+            min_date = datetime.today() - timedelta(weeks=2)
+            params["min_date"] = min_date.strftime("%Y-%m-%d")
         if next_page_token:
             params["page"] = next_page_token
         if self.replication_key:
             params["sort"] = "asc"
             params["order_by"] = self.replication_key
         return params
```

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentee_options.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/absentee_options.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/absentees.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/absentees.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/contract_types.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/contract_types.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/custom_fields.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/custom_fields.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/departments.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/departments.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/docs.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/docs.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/locations.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/rosters.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/rosters.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/shifts.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/shifts.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/teams.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/timesheets.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/timesheets.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/schemas/users.json` & `tap_shiftbase-1.0.1/tap_shiftbase/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/streams.py` & `tap_shiftbase-1.0.1/tap_shiftbase/streams.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/tap_shiftbase/tap.py` & `tap_shiftbase-1.0.1/tap_shiftbase/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shiftbase-1.0.0/PKG-INFO` & `tap_shiftbase-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-shiftbase
-Version: 1.0.0
+Version: 1.0.1
 Summary: `tap-shiftbase` is a Singer tap for shiftbase, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,shiftbase
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

