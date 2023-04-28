# Comparing `tmp/sonos-websocket-0.0.5.tar.gz` & `tmp/sonos-websocket-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonos-websocket-0.0.5.tar", last modified: Thu Apr 13 04:24:20 2023, max compression
+gzip compressed data, was "sonos-websocket-0.1.0.tar", last modified: Fri Apr 28 19:42:05 2023, max compression
```

## Comparing `sonos-websocket-0.0.5.tar` & `sonos-websocket-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:24:20.927635 sonos-websocket-0.0.5/sonos_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-13 04:24:09.000000 sonos-websocket-0.0.5/sonos_websocket/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:24:20.931635 sonos-websocket-0.0.5/sonos_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 04:24:20.000000 sonos-websocket-0.0.5/sonos_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:42:05.358315 sonos-websocket-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-28 19:42:05.358315 sonos-websocket-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:42:05.358315 sonos-websocket-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:42:05.358315 sonos-websocket-0.1.0/sonos_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/sonos_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/sonos_websocket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/sonos_websocket/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/sonos_websocket/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-28 19:41:47.000000 sonos-websocket-0.1.0/sonos_websocket/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:42:05.358315 sonos-websocket-0.1.0/sonos_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-28 19:42:05.000000 sonos-websocket-0.1.0/sonos_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-28 19:42:05.000000 sonos-websocket-0.1.0/sonos_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:42:05.000000 sonos-websocket-0.1.0/sonos_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 19:42:05.000000 sonos-websocket-0.1.0/sonos_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 19:42:05.000000 sonos-websocket-0.1.0/sonos_websocket.egg-info/top_level.txt
```

### Comparing `sonos-websocket-0.0.5/PKG-INFO` & `sonos-websocket-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.5
+Version: 0.1.0
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sonos-websocket-0.0.5/README.md` & `sonos-websocket-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.5/pyproject.toml` & `sonos-websocket-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.5/sonos_websocket/__main__.py` & `sonos-websocket-0.1.0/sonos_websocket/__main__.py`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.5/sonos_websocket/websocket.py` & `sonos-websocket-0.1.0/sonos_websocket/websocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Handler for Sonos websockets."""
 import asyncio
 import logging
 import sys
 from typing import Any, cast
 
 import aiohttp
+from aiohttp import WSMsgType
 
 from .const import API_KEY, MAX_ATTEMPTS
 from .exception import (
     SonosWebsocketError,
     SonosWSConnectionError,
     Unauthorized,
     Unsupported,
@@ -84,28 +85,32 @@
     async def send_command(
         self, command: dict[str, Any], options: dict[str, Any] | None = None
     ) -> list[dict[str, Any]]:
         """Send commands over the websocket and handle their responses."""
         attempt = 1
         while attempt <= MAX_ATTEMPTS:
             if not self.ws or self.ws.closed:
-                _LOGGER.debug("Websocket not available, reconnecting")
                 await self.connect()
                 assert self.ws
 
             payload = [command, options or {}]
             _LOGGER.debug("Sending command: %s", payload)
             try:
                 async with asyncio_timeout(3):
                     await self.ws.send_json(payload)
-                    return await self.ws.receive_json()
+                    msg = await self.ws.receive()
             except asyncio.TimeoutError:
                 _LOGGER.error("Command timed out")
-            except TypeError as exc:
-                _LOGGER.error("Bad response received: %s", exc)
+            else:
+                if msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSED, WSMsgType.CLOSING):
+                    _LOGGER.debug("Websocket closed, will try again")
+                elif msg.type != WSMsgType.TEXT:
+                    _LOGGER.error("Received non-text message: %s", msg.type.name)
+                else:
+                    return msg.json()
             attempt += 1
 
         command_name = command.get("command", "Empty")
         raise SonosWebsocketError(
             f"{command_name} command failed after {MAX_ATTEMPTS} attempts"
         )
```

### Comparing `sonos-websocket-0.0.5/sonos_websocket.egg-info/PKG-INFO` & `sonos-websocket-0.1.0/sonos_websocket.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.5
+Version: 0.1.0
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

