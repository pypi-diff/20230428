# Comparing `tmp/huntflow_api_client-0.0.1.tar.gz` & `tmp/huntflow_api_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_api_client-0.0.1.tar", max compression
+gzip compressed data, was "huntflow_api_client-0.0.2.tar", max compression
```

## Comparing `huntflow_api_client-0.0.1.tar` & `huntflow_api_client-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/LICENSE
--rw-r--r--   0        0        0      488 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/README.md
--rw-r--r--   0        0        0       76 2023-04-27 14:11:29.797006 huntflow_api_client-0.0.1/huntflow_api_client/__init__.py
--rw-r--r--   0        0        0     6105 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/huntflow_api_client/api.py
--rw-r--r--   0        0        0        0 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/huntflow_api_client/entities/__init__.py
--rw-r--r--   0        0        0      955 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/huntflow_api_client/entities/base.py
--rw-r--r--   0        0        0     1483 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/huntflow_api_client/entities/tags.py
--rw-r--r--   0        0        0      134 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/huntflow_api_client/errors.py
--rw-r--r--   0        0        0        0 2023-04-27 14:11:11.685077 huntflow_api_client-0.0.1/huntflow_api_client/models/__init__.py
--rw-r--r--   0        0        0      196 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/models/common.py
--rw-r--r--   0        0        0        0 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/models/request/__init__.py
--rw-r--r--   0        0        0      298 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/models/request/tags.py
--rw-r--r--   0        0        0        0 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/models/response/__init__.py
--rw-r--r--   0        0        0      313 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/models/response/tags.py
--rw-r--r--   0        0        0       53 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/tokens/__init__.py
--rw-r--r--   0        0        0     1871 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/tokens/locker.py
--rw-r--r--   0        0        0     5186 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/tokens/proxy.py
--rw-r--r--   0        0        0      730 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/tokens/storage.py
--rw-r--r--   0        0        0      562 2023-04-27 14:11:11.689077 huntflow_api_client-0.0.1/huntflow_api_client/tokens/token.py
--rw-r--r--   0        0        0     1328 2023-04-27 14:11:29.985005 huntflow_api_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0      488 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/README.md
+-rw-r--r--   0        0        0       76 2023-04-28 13:36:59.459770 huntflow_api_client-0.0.2/huntflow_api_client/__init__.py
+-rw-r--r--   0        0        0     6250 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/api.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/entities/__init__.py
+-rw-r--r--   0        0        0      955 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/entities/base.py
+-rw-r--r--   0        0        0     1483 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/entities/tags.py
+-rw-r--r--   0        0        0      187 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/errors.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/common.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/request/__init__.py
+-rw-r--r--   0        0        0      298 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/request/tags.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/response/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/response/tags.py
+-rw-r--r--   0        0        0       53 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/__init__.py
+-rw-r--r--   0        0        0     1871 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/locker.py
+-rw-r--r--   0        0        0     5186 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/proxy.py
+-rw-r--r--   0        0        0      730 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/storage.py
+-rw-r--r--   0        0        0      562 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/token.py
+-rw-r--r--   0        0        0     1328 2023-04-28 13:36:59.463770 huntflow_api_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.2/PKG-INFO
```

### Comparing `huntflow_api_client-0.0.1/LICENSE` & `huntflow_api_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/api.py` & `huntflow_api_client-0.0.2/huntflow_api_client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 from typing import Optional
 
 import httpx
 
-from huntflow_api_client.errors import InvalidAccessTokenError, TokenExpiredError
+from huntflow_api_client.errors import (
+    InvalidAccessTokenError,
+    InvalidRefreshTokenError,
+    TokenExpiredError,
+)
 from huntflow_api_client.tokens.proxy import AbstractTokenProxy, DummyHuntflowTokenProxy
 from huntflow_api_client.tokens.token import ApiToken
 
 logger = logging.getLogger(__name__)
 
 
 class HuntflowAPI:
@@ -146,14 +150,17 @@
         try:
             refresh_data = await self._token_proxy.get_refresh_data()
             async with self.http_client as client:
                 response = await client.post(
                     "/token/refresh",
                     json=refresh_data,
                 )
+                if response.status_code == 404:
+                    raise InvalidRefreshTokenError()
+
                 response.raise_for_status()
             await self._token_proxy.update(response.json())
         finally:
             await self._token_proxy.release_lock()
 
     async def _autorefresh_token_request(self, *args: str, **kwargs: str) -> httpx.Response:
         try:
```

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/entities/base.py` & `huntflow_api_client-0.0.2/huntflow_api_client/entities/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/entities/tags.py` & `huntflow_api_client-0.0.2/huntflow_api_client/entities/tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/tokens/locker.py` & `huntflow_api_client-0.0.2/huntflow_api_client/tokens/locker.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/tokens/proxy.py` & `huntflow_api_client-0.0.2/huntflow_api_client/tokens/proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/tokens/storage.py` & `huntflow_api_client-0.0.2/huntflow_api_client/tokens/storage.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/huntflow_api_client/tokens/token.py` & `huntflow_api_client-0.0.2/huntflow_api_client/tokens/token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.1/pyproject.toml` & `huntflow_api_client-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huntflow-api-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "Public client for Huntflow API"
 authors = ["Huntflow developers <developer@huntflow.ru>"]
 readme = "README.md"
 homepage = "https://github.com/huntflow/huntflow-api-client-python"
 packages = [{include = "huntflow_api_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `huntflow_api_client-0.0.1/PKG-INFO` & `huntflow_api_client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-api-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Public client for Huntflow API
 Home-page: https://github.com/huntflow/huntflow-api-client-python
 Author: Huntflow developers
 Author-email: developer@huntflow.ru
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

