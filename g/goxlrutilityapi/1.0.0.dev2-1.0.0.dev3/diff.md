# Comparing `tmp/goxlrutilityapi-1.0.0.dev2.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev2.tar", last modified: Fri Apr 28 19:33:37 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev3.tar", last modified: Fri Apr 28 21:23:12 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev2.tar` & `goxlrutilityapi-1.0.0.dev3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 19:33:36.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 19:33:37.000000 goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:33:37.618425 goxlrutilityapi-1.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 19:33:24.000000 goxlrutilityapi-1.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:23:12.423908 goxlrutilityapi-1.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 21:23:12.423908 goxlrutilityapi-1.0.0.dev3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:23:12.423908 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 21:23:10.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:23:12.423908 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:23:12.423908 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 21:23:12.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 21:23:12.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:23:12.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 21:23:12.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 21:23:12.000000 goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:23:12.423908 goxlrutilityapi-1.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 21:22:58.000000 goxlrutilityapi-1.0.0.dev3/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 import asyncio
 from collections.abc import Awaitable, Callable
 from typing import Optional
 
 import typer
 
 from ._version import __version__
+from .const import KEY_DATA, KEY_ID, KEY_TYPE
 from .exceptions import (
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
 )
 from .logger import setup_logger
+from .models.patch import Patch
 from .models.response import Response
+from .models.status import Status
 from .websocket_client import WebsocketClient
 
 app = typer.Typer()
 
 loop = asyncio.new_event_loop()
 asyncio.set_event_loop(loop)
 websocket_client = WebsocketClient()
@@ -35,49 +38,56 @@
             name="Websocket Listener",
         )
     except (
         BadMessageException,
         ConnectionClosedException,
         ConnectionErrorException,
     ) as error:
-        typer.secho(
-            f"Error: {error}",
-            fg=typer.colors.RED,
-        )
+        typer.secho(f"Error: {error}", fg=typer.colors.RED)
         loop.stop()
 
 
-async def message_callback(data: Response) -> None:
-    """Message callback function"""
-    typer.secho(data.json(), fg=typer.colors.GREEN)
+async def patch_callback(response: Response[Patch]) -> None:
+    """Patch response callback function"""
+    typer.secho(
+        response.json(
+            include={
+                KEY_ID,
+                KEY_TYPE,
+                KEY_DATA,
+            },
+            exclude_unset=True,
+        ),
+        fg=typer.colors.GREEN,
+    )
 
 
 @app.command(name="get_status", short_help="Get Status of GoXLR")
 def get_status(debug: bool = False) -> None:
     """Get Status of GoXLR"""
     if debug:
         setup_logger("DEBUG")
     setup_websocket()
     try:
-        response: Response = loop.run_until_complete(websocket_client.get_status())
+        status: Status = loop.run_until_complete(websocket_client.get_status())
     except BadMessageException as error:
         typer.secho(
             f"Failed to get status from GoXLR: {error}",
             fg=typer.colors.RED,
         )
         return
-    typer.secho(response.json(), fg=typer.colors.GREEN)
+    typer.secho(status.json(), fg=typer.colors.GREEN)
 
 
 @app.command(name="listen_for_messages", short_help="Listen for messages")
 def listen_for_messages(debug: bool = False) -> None:
     """Listen for messages"""
     if debug:
         setup_logger("DEBUG")
-    setup_websocket(message_callback)
+    setup_websocket(patch_callback)
     typer.secho("Listening for messages...", fg=typer.colors.GREEN)
     loop.run_forever()
 
 
 @app.command(name="version", short_help="Module Version")
 def version() -> None:
     """Module Version"""
```

### Comparing `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GoXLR Utility API: Constants"""
 
-from collections.abc import Callable
-from typing import Final
+from typing import Any, Final
 
+from .models import DefaultBaseModel
 from .models.patch import Patch
 from .models.request import Request
 from .models.response import Response
 from .models.status import Status
 
 # General
 DEFAULT_HOST: Final[str] = "localhost"
@@ -17,16 +17,16 @@
 KEY_ID: Final[str] = "id"
 KEY_TYPE: Final[str] = "type"
 REQUEST_TYPE_GET_STATUS: Final[str] = "GetStatus"
 RESPONSE_TYPE_PATCH: Final[str] = "Patch"
 RESPONSE_TYPE_STATUS: Final[str] = "Status"
 
 # Models
-MODEL_PATCH: Final[Callable] = Patch
-MODEL_REQUEST: Final[Callable] = Request
-MODEL_RESPONSE: Final[Callable] = Response
-MODEL_STATUS: Final[Callable] = Status
+MODEL_PATCH: type[Patch] = Patch
+MODEL_REQUEST: type[Request] = Request
+MODEL_RESPONSE: type[Response[Any]] = Response
+MODEL_STATUS: type[Status] = Status
 
-MODEL_MAP = {
+MODEL_MAP: Final[dict[str, type[DefaultBaseModel]]] = {
     RESPONSE_TYPE_PATCH: MODEL_PATCH,
     RESPONSE_TYPE_STATUS: MODEL_STATUS,
 }
```

### Comparing `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev3/goxlrutilityapi/websocket_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,38 @@
     DEFAULT_HOST,
     DEFAULT_PORT,
     KEY_DATA,
     KEY_ID,
     KEY_TYPE,
     MODEL_MAP,
     REQUEST_TYPE_GET_STATUS,
+    RESPONSE_TYPE_PATCH,
     RESPONSE_TYPE_STATUS,
 )
 from .exceptions import (
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
 )
+from .models.patch import Patch
 from .models.request import Request
 from .models.response import Response
+from .models.status import Status
 
 
 class WebsocketClient(Base):
     """Websocket Client"""
 
     def __init__(self) -> None:
         """Initialize Websocket Client"""
         super().__init__()
         self._current_id: int = 1
-        self._responses: dict[int, tuple[asyncio.Future[Response], Optional[str]]] = {}
+        self._responses: dict[
+            int, tuple[asyncio.Future[Response[Any]], Optional[str]]
+        ] = {}
         self._session: Optional[aiohttp.ClientSession] = None
         self._websocket: Optional[aiohttp.ClientWebSocketResponse] = None
 
     @property
     def connected(self) -> bool:
         """Get connection state."""
         return self._websocket is not None and not self._websocket.closed
@@ -84,53 +89,58 @@
         self._logger.info("Connected to WebSocket")
 
     async def _send_message(
         self,
         request: Request,
         wait_for_response: bool = True,
         response_type: Optional[str] = None,
-    ) -> Response:
+    ) -> Response[Any]:
         """Send a message to the WebSocket"""
         if not self.connected or self._websocket is None:
             raise ConnectionClosedException("Connection is closed")
 
         self._current_id += 1
         request.id = self._current_id
 
-        future: asyncio.Future[Response] = asyncio.get_running_loop().create_future()
+        future: asyncio.Future[
+            Response[Any]
+        ] = asyncio.get_running_loop().create_future()
         self._responses[request.id] = future, response_type
         await self._websocket.send_str(request.json())
         self._logger.debug("Sent message: %s", request.json())
         if wait_for_response:
             try:
                 return await future
             finally:
                 self._responses.pop(request.id)
-        return Response(
+        return Response[None](
             id=request.id,
             data=None,
             type=None,
         )
 
-    async def get_status(self) -> Response:
+    async def get_status(self) -> Status:
         """Get status from GoXLR"""
         self._logger.info("Getting status from GoXLR")
-        return await self._send_message(
+        response: Response[Status] = await self._send_message(
             Request(data=REQUEST_TYPE_GET_STATUS),
             wait_for_response=True,
             response_type=RESPONSE_TYPE_STATUS,
         )
+        if response.data is None:
+            raise BadMessageException("Message data is missing")
+        return response.data
 
     async def listen(
         self,
-        callback: Optional[Callable[[Response], Awaitable[None]]] = None,
+        patch_callback: Optional[Callable[[Response[Patch]], Awaitable[None]]] = None,
     ) -> None:
-        """Listen for messages and map to modules"""
+        """Listen for patches from GoXLR"""
 
-        async def _callback_message(message: dict) -> None:
+        async def _message_callback(message: dict) -> None:
             """Message callback"""
             self._logger.debug("New message")
 
             # Get message ID
             message_id = message.get(KEY_ID)
 
             if (message_data := message.get(KEY_DATA)) is None:
@@ -139,71 +149,76 @@
             # Get key of first object in message data
             if (message_type := next(iter(message_data))) is None:
                 raise BadMessageException("Message type is missing")
 
             self._logger.debug("Message ID: %s", message_id)
             self._logger.debug("Message type: %s", message_type)
 
-            response = Response(
-                id=message_id,
-                data=message_data.get(message_type),
-                type=message_type,
-            )
-
-            if response.data is None:
-                raise BadMessageException("Message data is missing")
-
             # Find model from module
             if (model := MODEL_MAP.get(message_type)) is None:
                 self._logger.warning("Unknown model: %s", message_type)
             else:
+                response = Response[Any](
+                    id=message_id,
+                    data=message_data.get(message_type),
+                    type=message_type,
+                )
+
+                if response.data is None:
+                    raise BadMessageException("Message data is missing")
+
                 try:
                     if isinstance(response.data, list):
                         response.data = [model(**item) for item in response.data]
                     else:
                         response.data = model(**response.data)
                 except TypeError as error:
                     raise BadMessageException(
                         f"Failed to create model '{message_type}' with data:\n{response.data}"
                     ) from error
 
-                if callback is not None:
-                    await callback(response)
-
-            self._logger.info(
-                "Response: %s",
-                response.json(
-                    include={
-                        KEY_ID,
-                        KEY_TYPE,
-                    },
-                    exclude_unset=True,
-                ),
-            )
-
-            if message_id is not None:
-                response_tuple = self._responses.get(message_id)
-                if response_tuple is not None:
-                    future, response_type = response_tuple
-                    if response_type is not None and response_type != message_type:
-                        self._logger.info(
-                            "Response type '%s' does not match requested type '%s'.",
-                            message_type,
-                            response_type,
-                        )
-                    else:
-                        try:
-                            future.set_result(response)
-                        except asyncio.InvalidStateError:
-                            self._logger.debug(
-                                "Future already set for response ID: %s",
-                                message_id,
+                self._logger.info(
+                    "Response: %s",
+                    response.json(
+                        include={
+                            KEY_ID,
+                            KEY_TYPE,
+                        },
+                        exclude_unset=True,
+                    ),
+                )
+
+                if message_id is not None:
+                    response_tuple = self._responses.get(message_id)
+                    if response_tuple is not None:
+                        future, response_type = response_tuple
+                        if response_type is not None and response_type != message_type:
+                            self._logger.info(
+                                "Response type '%s' does not match requested type '%s'.",
+                                message_type,
+                                response_type,
                             )
+                        else:
+                            try:
+                                future.set_result(response)
+                            except asyncio.InvalidStateError:
+                                self._logger.debug(
+                                    "Future already set for response ID: %s",
+                                    message_id,
+                                )
+
+                if patch_callback is not None and message_type == RESPONSE_TYPE_PATCH:
+                    try:
+                        await patch_callback(Response[Patch](**response.dict()))
+                    except TypeError as error:
+                        raise BadMessageException(
+                            f"Failed to create model '{message_type}' with data:\n{response.data}"
+                        ) from error
 
-        await self._listen_for_messages(callback=_callback_message)
+        await self._listen_for_messages(callback=_message_callback)
 
     async def _listen_for_messages(
         self,
         callback: Callable[[dict[Any, Any]], Awaitable[None]],
     ) -> None:
         """Listen for messages"""
         if not self.connected:
```

### Comparing `goxlrutilityapi-1.0.0.dev2/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev3/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev2/pyproject.toml` & `goxlrutilityapi-1.0.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev2/setup.py` & `goxlrutilityapi-1.0.0.dev3/setup.py`

 * *Files identical despite different names*

