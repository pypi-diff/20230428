# Comparing `tmp/xapi-python-0.0.2.tar.gz` & `tmp/xapi-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.0.2.tar", last modified: Thu Apr 27 06:57:11 2023, max compression
+gzip compressed data, was "xapi-python-0.0.3.tar", last modified: Fri Apr 28 08:36:24 2023, max compression
```

## Comparing `xapi-python-0.0.2.tar` & `xapi-python-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.0.2/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-27 06:57:11.094159 xapi-python-0.0.2/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5591 2023-04-26 13:10:27.000000 xapi-python-0.0.2/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1075 2023-04-27 06:52:41.000000 xapi-python-0.0.2/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-27 06:57:11.094159 xapi-python-0.0.2/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1011 2023-04-27 06:53:55.000000 xapi-python-0.0.2/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5636 2023-04-27 06:31:53.000000 xapi-python-0.0.2/tests/test_connect.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.0.2/tests/test_socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.0.2/tests/test_stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-26 11:04:33.000000 xapi-python-0.0.2/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-04-27 06:12:53.000000 xapi-python-0.0.2/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2041 2023-04-27 06:06:45.000000 xapi-python-0.0.2/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.0.2/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      200 2023-04-24 12:09:22.000000 xapi-python-0.0.2/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-26 08:53:56.000000 xapi-python-0.0.2/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-26 09:47:15.000000 xapi-python-0.0.2/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1104 2023-04-26 06:51:38.000000 xapi-python-0.0.2/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.0.3/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-28 08:36:24.787298 xapi-python-0.0.3/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5591 2023-04-26 13:10:27.000000 xapi-python-0.0.3/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1075 2023-04-28 08:33:22.000000 xapi-python-0.0.3/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-28 08:36:24.787298 xapi-python-0.0.3/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1011 2023-04-28 08:32:12.000000 xapi-python-0.0.3/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5636 2023-04-27 06:31:53.000000 xapi-python-0.0.3/tests/test_connect.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.0.3/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.0.3/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-26 11:04:33.000000 xapi-python-0.0.3/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-04-28 08:32:24.000000 xapi-python-0.0.3/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2055 2023-04-28 08:16:16.000000 xapi-python-0.0.3/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.0.3/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      200 2023-04-24 12:09:22.000000 xapi-python-0.0.3/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-28 08:30:55.000000 xapi-python-0.0.3/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-26 09:47:15.000000 xapi-python-0.0.3/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1103 2023-04-28 08:15:26.000000 xapi-python-0.0.3/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.0.2/LICENSE` & `xapi-python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/PKG-INFO` & `xapi-python-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
```

### Comparing `xapi-python-0.0.2/README.md` & `xapi-python-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/pyproject.toml` & `xapi-python-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xapi-python"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Paweł Knioła", email="pawel.kn@gmail.com" },
 ]
 description = "The xStation5 API Python library"
 keywords = ["python", "trading", "websocket", "trading-api", "forex", "xapi", "forex-trading", "exchange-api", "forex-data", "xstation5", "xtb", "xopenhub", "forex-api", "xopenhub-api", "xtb-api", "xstation-api", "x-trade-brokers", "bfbcapital", "xstation"]
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `xapi-python-0.0.2/setup.py` & `xapi-python-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,10 +16,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.0.2",
+    version="0.0.3",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.0.2/tests/test_connect.py` & `xapi-python-0.0.3/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/tests/test_socket.py` & `xapi-python-0.0.3/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/tests/test_stream.py` & `xapi-python-0.0.3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/tests/test_xapi.py` & `xapi-python-0.0.3/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/xapi/connection.py` & `xapi-python-0.0.3/xapi/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import websockets.client
 import websockets.exceptions
 import asyncio
 import json
 
 class Connection():
     def __init__(self):
-        self.safe = False
+        self.safe = True
         self._conn = None
 
     async def connect(self, url):
         try:
-            self._conn = await websockets.client.connect(url, close_timeout=0)
+            self._conn = await websockets.client.connect(url, close_timeout=0, max_size=None)
 
         except asyncio.exceptions.TimeoutError:
             raise ConnectionClosed("Connection timed out")
 
         except ConnectionRefusedError:
             raise ConnectionClosed("Connection refused")
```

### Comparing `xapi-python-0.0.2/xapi/enums.py` & `xapi-python-0.0.3/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/xapi/socket.py` & `xapi-python-0.0.3/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/xapi/stream.py` & `xapi-python-0.0.3/xapi/stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.2/xapi/xapi.py` & `xapi-python-0.0.3/xapi/xapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         await self.stream.disconnect()
 
 async def connect(
         accountId: str,
         password: str,
         host: str = "ws.xtb.com",
         type: str = "real",
-        safe: bool = False
+        safe: bool = True
     ):
 
     x = XAPI()
 
     x.stream.safe = safe
     x.socket.safe = safe
```

### Comparing `xapi-python-0.0.2/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.0.3/xapi_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
```

