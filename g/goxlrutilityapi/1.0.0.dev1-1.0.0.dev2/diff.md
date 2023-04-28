# Comparing `tmp/goxlrutilityapi-1.0.0.dev1.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev1.tar", last modified: Fri Apr 28 19:09:24 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev2.tar", last modified: Fri Apr 28 19:33:37 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev1.tar` & `goxlrutilityapi-1.0.0.dev2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:09:24.667273 goxlrutilityapi-1.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:09:24.667273 goxlrutilityapi-1.0.0.dev1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:09:24.663273 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 19:09:22.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:09:24.667273 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:09:24.663273 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:09:24.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 19:09:24.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:09:24.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 19:09:24.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 19:09:24.000000 goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:09:24.667273 goxlrutilityapi-1.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 19:09:05.000000 goxlrutilityapi-1.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 19:33:36.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/const.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from typing import Final
 
 from .models.patch import Patch
 from .models.request import Request
 from .models.response import Response
 from .models.status import Status
 
+# General
+DEFAULT_HOST: Final[str] = "localhost"
+DEFAULT_PORT: Final[int] = 14564
+
 # API
 KEY_DATA: Final[str] = "data"
 KEY_ID: Final[str] = "id"
 KEY_TYPE: Final[str] = "type"
 REQUEST_TYPE_GET_STATUS: Final[str] = "GetStatus"
 RESPONSE_TYPE_PATCH: Final[str] = "Patch"
 RESPONSE_TYPE_STATUS: Final[str] = "Status"
```

### Comparing `goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev1/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/websocket_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from collections.abc import Awaitable, Callable
 from typing import Any, Optional
 
 import aiohttp
 
 from .base import Base
 from .const import (
+    DEFAULT_HOST,
+    DEFAULT_PORT,
     KEY_DATA,
     KEY_ID,
     KEY_TYPE,
     MODEL_MAP,
     REQUEST_TYPE_GET_STATUS,
     RESPONSE_TYPE_STATUS,
 )
@@ -46,16 +48,16 @@
         """Disconnect from server"""
         self._logger.info("Disconnecting from WebSocket")
         if self._websocket is not None:
             await self._websocket.close()
 
     async def connect(
         self,
-        host: str = "localhost",
-        port: int = 14564,
+        host: str = DEFAULT_HOST,
+        port: int = DEFAULT_PORT,
         session: Optional[aiohttp.ClientSession] = None,
     ) -> None:
         """Connect to server"""
         if session:
             self._session = session
         else:
             self._logger.info("Creating new aiohttp client session")
```

### Comparing `goxlrutilityapi-1.0.0.dev1/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev1/pyproject.toml` & `goxlrutilityapi-1.0.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev1/setup.py` & `goxlrutilityapi-1.0.0.dev2/setup.py`

 * *Files identical despite different names*

