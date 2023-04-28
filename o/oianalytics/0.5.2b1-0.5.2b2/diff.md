# Comparing `tmp/oianalytics-0.5.2b1.tar.gz` & `tmp/oianalytics-0.5.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oianalytics-0.5.2b1.tar", max compression
+gzip compressed data, was "oianalytics-0.5.2b2.tar", max compression
```

## Comparing `oianalytics-0.5.2b1.tar` & `oianalytics-0.5.2b2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.2b1/LICENSE
--rw-r--r--   0        0        0       94 2023-04-19 09:25:30.486603 oianalytics-0.5.2b1/oianalytics/__init__.py
--rw-r--r--   0        0        0       99 2023-03-15 14:01:49.113825 oianalytics-0.5.2b1/oianalytics/api/__init__.py
--rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.2b1/oianalytics/api/_credentials.py
--rw-r--r--   0        0        0     1342 2023-04-18 12:32:43.993044 oianalytics-0.5.2b1/oianalytics/api/_dataframes/__init__.py
--rw-r--r--   0        0        0     7272 2023-04-18 12:32:43.960505 oianalytics-0.5.2b1/oianalytics/api/_dataframes/assets.py
--rw-r--r--   0        0        0    40776 2023-04-18 12:32:43.993542 oianalytics-0.5.2b1/oianalytics/api/_dataframes/batches.py
--rw-r--r--   0        0        0    41468 2023-04-18 12:32:43.986986 oianalytics-0.5.2b1/oianalytics/api/_dataframes/data.py
--rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.2b1/oianalytics/api/_dataframes/events.py
--rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.2b1/oianalytics/api/_dataframes/files.py
--rw-r--r--   0        0        0     4250 2023-03-15 14:01:49.114990 oianalytics-0.5.2b1/oianalytics/api/_dataframes/users.py
--rw-r--r--   0        0        0      123 2023-04-18 12:32:43.960591 oianalytics-0.5.2b1/oianalytics/api/endpoints/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-18 12:32:43.960652 oianalytics-0.5.2b1/oianalytics/api/endpoints/assets.py
--rw-r--r--   0        0        0     8316 2023-04-18 12:32:43.993820 oianalytics-0.5.2b1/oianalytics/api/endpoints/batches.py
--rw-r--r--   0        0        0    13020 2023-04-18 12:32:43.987317 oianalytics-0.5.2b1/oianalytics/api/endpoints/data.py
--rw-r--r--   0        0        0     2600 2023-03-15 14:01:49.115412 oianalytics-0.5.2b1/oianalytics/api/endpoints/events.py
--rw-r--r--   0        0        0     3159 2023-04-19 09:24:50.987573 oianalytics-0.5.2b1/oianalytics/api/endpoints/files.py
--rw-r--r--   0        0        0     1199 2023-03-15 14:01:49.115585 oianalytics-0.5.2b1/oianalytics/api/endpoints/users.py
--rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.2b1/oianalytics/api/utils.py
--rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.2b1/oianalytics/models/__init__.py
--rw-r--r--   0        0        0    39198 2023-04-18 12:32:44.003683 oianalytics-0.5.2b1/oianalytics/models/_dtos.py
--rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.2b1/oianalytics/models/_queries/__init__.py
--rw-r--r--   0        0        0     1943 2023-04-19 09:25:06.769232 oianalytics-0.5.2b1/oianalytics/models/_queries/files.py
--rw-r--r--   0        0        0      711 2023-03-15 14:01:49.116301 oianalytics-0.5.2b1/oianalytics/models/_queries/instances.py
--rw-r--r--   0        0        0    10106 2023-03-15 14:01:49.116403 oianalytics-0.5.2b1/oianalytics/models/_queries/single_observation.py
--rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.2b1/oianalytics/models/_template_resources/__init__.py
--rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.2b1/oianalytics/models/_template_resources/file_processing_template.py
--rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.2b1/oianalytics/models/_template_resources/free_from_api_template.py
--rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.2b1/oianalytics/models/_template_resources/single_observation_template.py
--rw-r--r--   0        0        0    30641 2023-04-18 12:32:43.976382 oianalytics-0.5.2b1/oianalytics/models/outputs.py
--rw-r--r--   0        0        0      992 2023-03-15 14:01:49.117047 oianalytics-0.5.2b1/oianalytics/models/templates.py
--rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.2b1/oianalytics/models/testing/__init__.py
--rw-r--r--   0        0        0    31789 2023-03-15 14:01:49.117353 oianalytics-0.5.2b1/oianalytics/models/testing/_mocking.py
--rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.2b1/oianalytics/models/testing/_tests_setup.py
--rw-r--r--   0        0        0     2791 2023-03-15 14:01:49.117545 oianalytics-0.5.2b1/oianalytics/models/testing/file_processing.py
--rw-r--r--   0        0        0     2645 2023-03-15 14:01:49.117632 oianalytics-0.5.2b1/oianalytics/models/testing/free_from_api.py
--rw-r--r--   0        0        0     6985 2023-03-15 14:01:49.117720 oianalytics-0.5.2b1/oianalytics/models/testing/single_observation.py
--rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.2b1/oianalytics/models/utils.py
--rw-r--r--   0        0        0      471 2023-04-19 09:25:35.141034 oianalytics-0.5.2b1/pyproject.toml
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 oianalytics-0.5.2b1/PKG-INFO
+-rw-r--r--   0        0        0    13799 2023-03-15 14:01:49.113528 oianalytics-0.5.2b2/LICENSE
+-rw-r--r--   0        0        0       94 2023-04-24 14:20:16.835364 oianalytics-0.5.2b2/oianalytics/__init__.py
+-rw-r--r--   0        0        0       99 2023-03-15 14:01:49.113825 oianalytics-0.5.2b2/oianalytics/api/__init__.py
+-rw-r--r--   0        0        0     2373 2023-03-15 14:01:49.113932 oianalytics-0.5.2b2/oianalytics/api/_credentials.py
+-rw-r--r--   0        0        0     1422 2023-04-28 14:52:23.621476 oianalytics-0.5.2b2/oianalytics/api/_dataframes/__init__.py
+-rw-r--r--   0        0        0     8623 2023-04-28 14:52:23.617751 oianalytics-0.5.2b2/oianalytics/api/_dataframes/assets.py
+-rw-r--r--   0        0        0    40776 2023-04-18 12:32:43.993542 oianalytics-0.5.2b2/oianalytics/api/_dataframes/batches.py
+-rw-r--r--   0        0        0    41468 2023-04-18 12:32:43.986986 oianalytics-0.5.2b2/oianalytics/api/_dataframes/data.py
+-rw-r--r--   0        0        0     9979 2023-03-15 14:01:49.114785 oianalytics-0.5.2b2/oianalytics/api/_dataframes/events.py
+-rw-r--r--   0        0        0     4631 2023-03-15 14:01:49.114887 oianalytics-0.5.2b2/oianalytics/api/_dataframes/files.py
+-rw-r--r--   0        0        0     4250 2023-03-15 14:01:49.114990 oianalytics-0.5.2b2/oianalytics/api/_dataframes/users.py
+-rw-r--r--   0        0        0      123 2023-04-18 12:32:43.960591 oianalytics-0.5.2b2/oianalytics/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     2605 2023-04-28 14:52:23.624696 oianalytics-0.5.2b2/oianalytics/api/endpoints/assets.py
+-rw-r--r--   0        0        0     8316 2023-04-18 12:32:43.993820 oianalytics-0.5.2b2/oianalytics/api/endpoints/batches.py
+-rw-r--r--   0        0        0    13020 2023-04-18 12:32:43.987317 oianalytics-0.5.2b2/oianalytics/api/endpoints/data.py
+-rw-r--r--   0        0        0     2600 2023-03-15 14:01:49.115412 oianalytics-0.5.2b2/oianalytics/api/endpoints/events.py
+-rw-r--r--   0        0        0     3159 2023-04-19 09:24:50.987573 oianalytics-0.5.2b2/oianalytics/api/endpoints/files.py
+-rw-r--r--   0        0        0     1199 2023-03-15 14:01:49.115585 oianalytics-0.5.2b2/oianalytics/api/endpoints/users.py
+-rw-r--r--   0        0        0     5881 2023-04-18 12:32:43.955607 oianalytics-0.5.2b2/oianalytics/api/utils.py
+-rw-r--r--   0        0        0      133 2023-03-15 14:01:49.115833 oianalytics-0.5.2b2/oianalytics/models/__init__.py
+-rw-r--r--   0        0        0    39198 2023-04-18 12:32:44.003683 oianalytics-0.5.2b2/oianalytics/models/_dtos.py
+-rw-r--r--   0        0        0      346 2023-04-18 12:32:43.955722 oianalytics-0.5.2b2/oianalytics/models/_queries/__init__.py
+-rw-r--r--   0        0        0     1943 2023-04-21 14:44:50.564896 oianalytics-0.5.2b2/oianalytics/models/_queries/files.py
+-rw-r--r--   0        0        0      711 2023-03-15 14:01:49.116301 oianalytics-0.5.2b2/oianalytics/models/_queries/instances.py
+-rw-r--r--   0        0        0    10106 2023-03-15 14:01:49.116403 oianalytics-0.5.2b2/oianalytics/models/_queries/single_observation.py
+-rw-r--r--   0        0        0        0 2023-03-15 14:01:49.116471 oianalytics-0.5.2b2/oianalytics/models/_template_resources/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-18 12:32:43.955950 oianalytics-0.5.2b2/oianalytics/models/_template_resources/file_processing_template.py
+-rw-r--r--   0        0        0     3841 2023-03-15 14:01:49.116690 oianalytics-0.5.2b2/oianalytics/models/_template_resources/free_from_api_template.py
+-rw-r--r--   0        0        0     2078 2023-03-15 14:01:49.116764 oianalytics-0.5.2b2/oianalytics/models/_template_resources/single_observation_template.py
+-rw-r--r--   0        0        0    30641 2023-04-18 12:32:43.976382 oianalytics-0.5.2b2/oianalytics/models/outputs.py
+-rw-r--r--   0        0        0      992 2023-03-15 14:01:49.117047 oianalytics-0.5.2b2/oianalytics/models/templates.py
+-rw-r--r--   0        0        0      117 2023-03-15 14:01:49.117158 oianalytics-0.5.2b2/oianalytics/models/testing/__init__.py
+-rw-r--r--   0        0        0    31789 2023-03-15 14:01:49.117353 oianalytics-0.5.2b2/oianalytics/models/testing/_mocking.py
+-rw-r--r--   0        0        0     1067 2023-03-15 14:01:49.117460 oianalytics-0.5.2b2/oianalytics/models/testing/_tests_setup.py
+-rw-r--r--   0        0        0     2791 2023-03-15 14:01:49.117545 oianalytics-0.5.2b2/oianalytics/models/testing/file_processing.py
+-rw-r--r--   0        0        0     2645 2023-03-15 14:01:49.117632 oianalytics-0.5.2b2/oianalytics/models/testing/free_from_api.py
+-rw-r--r--   0        0        0     6985 2023-03-15 14:01:49.117720 oianalytics-0.5.2b2/oianalytics/models/testing/single_observation.py
+-rw-r--r--   0        0        0      256 2023-03-15 14:01:49.117791 oianalytics-0.5.2b2/oianalytics/models/utils.py
+-rw-r--r--   0        0        0      471 2023-04-24 14:20:16.831112 oianalytics-0.5.2b2/pyproject.toml
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 oianalytics-0.5.2b2/PKG-INFO
```

### Comparing `oianalytics-0.5.2b1/LICENSE` & `oianalytics-0.5.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_credentials.py` & `oianalytics-0.5.2b2/oianalytics/api/_credentials.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/__init__.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     get_multiple_data_values,
     insert_time_values,
     insert_vector_time_values,
 )
 from .events import get_event_types, get_events
 from .files import get_file_uploads, read_file_from_file_upload
 from .users import get_users
-from .assets import get_asset_types, get_assets
+from .assets import get_asset_types, get_assets, update_single_asset_tags_and_values
 
 __all__ = [
     "get_batch_types",
     "get_batch_type_details",
     "get_single_batch",
     "get_batches",
     "update_batch_values",
@@ -45,8 +45,9 @@
     "get_event_types",
     "get_events",
     "get_file_uploads",
     "read_file_from_file_upload",
     "get_users",
     "get_asset_types",
     "get_assets",
+    "update_single_asset_tags_and_values",
 ]
```

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/assets.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/assets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional, List
+from typing import Optional, List, Dict
 
 import pandas as pd
 
 from .. import _credentials
 from .. import endpoints
 from .. import utils
 
-__all__ = ["get_asset_types", "get_assets"]
+__all__ = ["get_asset_types", "get_assets", "update_single_asset_tags_and_values"]
 
 
 def get_asset_types(
     page: Optional[int] = None,
     name: Optional[int] = None,
     get_all_pages: bool = True,
     multithread_pages: bool = True,
@@ -215,7 +215,48 @@
         )
 
     if expand_staticdatavalues is True and extract_from_staticdatavalues is not None:
         df = utils.expand_dataframe_column(df, "staticDataValues", add_prefix=False)
 
     # Output
     return df
+
+
+def update_single_asset_tags_and_values(
+    asset_id: str,
+    tag_values: Optional[Dict] = None,
+    static_data_values: Optional[Dict] = None,
+    static_data_units: Optional[Dict] = None,
+    api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
+):
+    # Init
+    if tag_values is None:
+        tag_values = {}
+
+    if static_data_values is None:
+        static_data_values = {}
+
+    if static_data_units is None:
+        static_data_units = {}
+
+    # Build payload
+    tag_commands = []
+    for tagkey_id, tagvalue in tag_values.items():
+        tag_commands.append({"tagKeyId": tagkey_id, "id": None, "value": tagvalue})
+
+    value_commands = []
+    for data_id, value in static_data_values.items():
+        value_commands.append(
+            {
+                "assetTypeStaticDataId": data_id,
+                "value": value,
+                "unitId": static_data_units.get(data_id),
+            }
+        )
+
+    # Query endpoint
+    response = endpoints.assets.update_single_asset_tags_and_values(asset_id=asset_id, tag_commands=tag_commands,
+                                                                    value_commands=value_commands,
+                                                                    api_credentials=api_credentials)
+
+    # Output
+    return response
```

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/batches.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/data.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/events.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/files.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/_dataframes/users.py` & `oianalytics-0.5.2b2/oianalytics/api/_dataframes/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/endpoints/assets.py` & `oianalytics-0.5.2b2/oianalytics/api/endpoints/files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,110 @@
-from typing import Optional, List
+from typing import Optional, List, Union
+from datetime import datetime
+import io
 
 import requests
 
 from .. import _credentials
+from .. import utils
 
-__all__ = ["get_asset_types", "get_assets"]
+__all__ = [
+    "get_file_uploads",
+    "get_file_upload_details",
+    "get_file_from_file_upload",
+    "upload_file",
+]
 
 
-def get_asset_types(
+def get_file_uploads(
+    start_date: Union[str, datetime],
+    end_date: Union[str, datetime],
+    filename: Optional[str] = None,
+    statuses: Optional[Union[str, List[str]]] = None,
     page: Optional[int] = None,
-    name: Optional[int] = None,
+    page_size: Optional[int] = None,
     api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
 ):
     # Get credentials from environment if not provided
     if api_credentials is None:
         api_credentials = _credentials.get_default_oianalytics_credentials()
 
+    # Format dates
+    start_date_iso = utils.get_zulu_isoformat(start_date)
+    end_date_iso = utils.get_zulu_isoformat(end_date)
+
     # Query endpoint
-    url = f"{api_credentials.base_url}/api/oianalytics/asset-types"
+    url = f"{api_credentials.base_url}/api/oianalytics/file-uploads"
     response = requests.get(
-        url=url, params={"page": page, "name": name}, **api_credentials.auth_kwargs,
+        url=url,
+        params={
+            "filename": filename,
+            "statuses": statuses,
+            "from": start_date_iso,
+            "to": end_date_iso,
+            "page": page,
+            "size": page_size,
+        },
+        **api_credentials.auth_kwargs,
     )
 
     # Output
     response.raise_for_status()
     return response.json()
 
 
-def get_assets(
-    asset_type_id: str,
-    tag_value_id: Optional[List[str]] = None,
-    query: Optional[int] = None,
-    page: Optional[int] = None,
+def get_file_upload_details(
+    file_upload_id: str,
     api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
 ):
     # Get credentials from environment if not provided
     if api_credentials is None:
         api_credentials = _credentials.get_default_oianalytics_credentials()
 
     # Query endpoint
-    url = f"{api_credentials.base_url}/api/oianalytics/assets"
-    response = requests.get(
+    url = f"{api_credentials.base_url}/api/oianalytics/file-uploads/{file_upload_id}"
+    response = requests.get(url=url, **api_credentials.auth_kwargs,)
+
+    # Output
+    response.raise_for_status()
+    return response.json()
+
+
+def get_file_from_file_upload(
+    file_upload_id: str,
+    api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
+):
+    # Get credentials from environment if not provided
+    if api_credentials is None:
+        api_credentials = _credentials.get_default_oianalytics_credentials()
+
+    # Query endpoint
+    url = (
+        f"{api_credentials.base_url}/api/oianalytics/file-uploads/{file_upload_id}/file"
+    )
+    response = requests.get(url=url, **api_credentials.auth_kwargs,)
+
+    # Output
+    response.raise_for_status()
+    return io.BytesIO(response.content)
+
+
+def upload_file(
+    file_content: Union[io.StringIO, io.BytesIO],
+    file_name: str,
+    api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
+):
+    # Get credentials from environment if not provided
+    if api_credentials is None:
+        api_credentials = _credentials.get_default_oianalytics_credentials()
+
+    # Query endpoint
+    url = f"{api_credentials.base_url}/api/oianalytics/file-uploads"
+    response = requests.post(
         url=url,
-        params={
-            "page": page,
-            "query": query,
-            "assetTypeId": asset_type_id,
-            "tagValueIds": tag_value_id,
-        },
+        files={"file": (file_name, file_content)},
         **api_credentials.auth_kwargs,
     )
 
     # Output
     response.raise_for_status()
     return response.json()
```

### Comparing `oianalytics-0.5.2b1/oianalytics/api/endpoints/batches.py` & `oianalytics-0.5.2b2/oianalytics/api/endpoints/batches.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/endpoints/data.py` & `oianalytics-0.5.2b2/oianalytics/api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/endpoints/events.py` & `oianalytics-0.5.2b2/oianalytics/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/endpoints/files.py` & `oianalytics-0.5.2b2/oianalytics/api/endpoints/assets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,93 @@
-from typing import Optional, List, Union
-from datetime import datetime
-import io
+from typing import Optional, List, Dict
 
 import requests
 
 from .. import _credentials
-from .. import utils
 
-__all__ = [
-    "get_file_uploads",
-    "get_file_upload_details",
-    "get_file_from_file_upload",
-    "upload_file",
-]
+__all__ = ["get_asset_types", "get_assets", "update_single_asset_tags_and_values"]
 
 
-def get_file_uploads(
-    start_date: Union[str, datetime],
-    end_date: Union[str, datetime],
-    filename: Optional[str] = None,
-    statuses: Optional[Union[str, List[str]]] = None,
+def get_asset_types(
     page: Optional[int] = None,
-    page_size: Optional[int] = None,
+    name: Optional[int] = None,
     api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
 ):
     # Get credentials from environment if not provided
     if api_credentials is None:
         api_credentials = _credentials.get_default_oianalytics_credentials()
 
-    # Format dates
-    start_date_iso = utils.get_zulu_isoformat(start_date)
-    end_date_iso = utils.get_zulu_isoformat(end_date)
-
     # Query endpoint
-    url = f"{api_credentials.base_url}/api/oianalytics/file-uploads"
+    url = f"{api_credentials.base_url}/api/oianalytics/asset-types"
     response = requests.get(
         url=url,
-        params={
-            "filename": filename,
-            "statuses": statuses,
-            "from": start_date_iso,
-            "to": end_date_iso,
-            "page": page,
-            "size": page_size,
-        },
+        params={"page": page, "name": name},
         **api_credentials.auth_kwargs,
     )
 
     # Output
     response.raise_for_status()
     return response.json()
 
 
-def get_file_upload_details(
-    file_upload_id: str,
+def get_assets(
+    asset_type_id: str,
+    tag_value_id: Optional[List[str]] = None,
+    query: Optional[int] = None,
+    page: Optional[int] = None,
     api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
 ):
     # Get credentials from environment if not provided
     if api_credentials is None:
         api_credentials = _credentials.get_default_oianalytics_credentials()
 
     # Query endpoint
-    url = f"{api_credentials.base_url}/api/oianalytics/file-uploads/{file_upload_id}"
-    response = requests.get(url=url, **api_credentials.auth_kwargs,)
+    url = f"{api_credentials.base_url}/api/oianalytics/assets"
+    response = requests.get(
+        url=url,
+        params={
+            "page": page,
+            "query": query,
+            "assetTypeId": asset_type_id,
+            "tagValueIds": tag_value_id,
+        },
+        **api_credentials.auth_kwargs,
+    )
 
     # Output
     response.raise_for_status()
     return response.json()
 
 
-def get_file_from_file_upload(
-    file_upload_id: str,
+def update_single_asset_tags_and_values(
+    asset_id: str,
+    tag_commands: Optional[List[Dict]] = None,
+    value_commands: Optional[List[Dict]] = None,
     api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
 ):
     # Get credentials from environment if not provided
     if api_credentials is None:
         api_credentials = _credentials.get_default_oianalytics_credentials()
 
-    # Query endpoint
-    url = (
-        f"{api_credentials.base_url}/api/oianalytics/file-uploads/{file_upload_id}/file"
-    )
-    response = requests.get(url=url, **api_credentials.auth_kwargs,)
-
-    # Output
-    response.raise_for_status()
-    return io.BytesIO(response.content)
-
-
-def upload_file(
-    file_content: Union[io.StringIO, io.BytesIO],
-    file_name: str,
-    api_credentials: Optional[_credentials.OIAnalyticsAPICredentials] = None,
-):
-    # Get credentials from environment if not provided
-    if api_credentials is None:
-        api_credentials = _credentials.get_default_oianalytics_credentials()
+    # Init commands
+    if tag_commands is None:
+        tag_commands = []
+
+    if value_commands is None:
+        value_commands = []
+
+    # Build payload
+    payload = [
+        {
+            "assetId": asset_id,
+            "tagCommands": tag_commands,
+            "staticDataValueCommands": value_commands,
+        }
+    ]
 
     # Query endpoint
-    url = f"{api_credentials.base_url}/api/oianalytics/file-uploads"
-    response = requests.post(
-        url=url,
-        files={"file": (file_name, file_content)},
-        **api_credentials.auth_kwargs,
-    )
+    url = f"{api_credentials.base_url}/api/oianalytics/assets/tags-and-values"
+    response = requests.put(url=url, json=payload, **api_credentials.auth_kwargs)
 
     # Output
     response.raise_for_status()
-    return response.json()
+    return response.status_code
```

### Comparing `oianalytics-0.5.2b1/oianalytics/api/endpoints/users.py` & `oianalytics-0.5.2b2/oianalytics/api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/api/utils.py` & `oianalytics-0.5.2b2/oianalytics/api/utils.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_dtos.py` & `oianalytics-0.5.2b2/oianalytics/models/_dtos.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_queries/files.py` & `oianalytics-0.5.2b2/oianalytics/models/_queries/files.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_queries/instances.py` & `oianalytics-0.5.2b2/oianalytics/models/_queries/instances.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_queries/single_observation.py` & `oianalytics-0.5.2b2/oianalytics/models/_queries/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_template_resources/file_processing_template.py` & `oianalytics-0.5.2b2/oianalytics/models/_template_resources/file_processing_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_template_resources/free_from_api_template.py` & `oianalytics-0.5.2b2/oianalytics/models/_template_resources/free_from_api_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/_template_resources/single_observation_template.py` & `oianalytics-0.5.2b2/oianalytics/models/_template_resources/single_observation_template.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/outputs.py` & `oianalytics-0.5.2b2/oianalytics/models/outputs.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/templates.py` & `oianalytics-0.5.2b2/oianalytics/models/templates.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/testing/_mocking.py` & `oianalytics-0.5.2b2/oianalytics/models/testing/_mocking.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/testing/_tests_setup.py` & `oianalytics-0.5.2b2/oianalytics/models/testing/_tests_setup.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/testing/file_processing.py` & `oianalytics-0.5.2b2/oianalytics/models/testing/file_processing.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/testing/free_from_api.py` & `oianalytics-0.5.2b2/oianalytics/models/testing/free_from_api.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/oianalytics/models/testing/single_observation.py` & `oianalytics-0.5.2b2/oianalytics/models/testing/single_observation.py`

 * *Files identical despite different names*

### Comparing `oianalytics-0.5.2b1/PKG-INFO` & `oianalytics-0.5.2b2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oianalytics
-Version: 0.5.2b1
+Version: 0.5.2b2
 Summary: Python tools for working with OIAnalytics
 License: EUPL-1.2
 Author: Optimistik SAS
 Author-email: arthur.martel@optimistik.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

