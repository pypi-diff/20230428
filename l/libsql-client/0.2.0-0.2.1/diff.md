# Comparing `tmp/libsql-client-0.2.0.tar.gz` & `tmp/libsql-client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsql-client-0.2.0.tar", max compression
+gzip compressed data, was "libsql-client-0.2.1.tar", max compression
```

## Comparing `libsql-client-0.2.0.tar` & `libsql-client-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-02-27 08:58:08.764134 libsql-client-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2907 2023-04-19 12:23:21.137820 libsql-client-0.2.0/README.md
--rw-r--r--   0        0        0      268 2023-04-19 10:43:28.755257 libsql-client-0.2.0/libsql_client/__init__.py
--rw-r--r--   0        0        0     3039 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/client.py
--rw-r--r--   0        0        0      993 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/config.py
--rw-r--r--   0        0        0      801 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/create_client.py
--rw-r--r--   0        0        0       85 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/hrana/__init__.py
--rw-r--r--   0        0        0    13911 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/hrana/client.py
--rw-r--r--   0        0        0     4816 2023-04-20 09:18:36.654076 libsql-client-0.2.0/libsql_client/hrana/convert.py
--rw-r--r--   0        0        0     1610 2023-04-17 12:00:30.661316 libsql-client-0.2.0/libsql_client/hrana/id_alloc.py
--rw-r--r--   0        0        0     3974 2023-04-17 12:00:30.661316 libsql-client-0.2.0/libsql_client/hrana/proto.py
--rw-r--r--   0        0        0     3441 2023-04-17 12:00:30.661316 libsql-client-0.2.0/libsql_client/http.py
--rw-r--r--   0        0        0     3048 2023-04-20 09:22:06.451040 libsql-client-0.2.0/libsql_client/result.py
--rw-r--r--   0        0        0     4896 2023-04-20 09:19:13.406247 libsql-client-0.2.0/libsql_client/sqlite3.py
--rw-r--r--   0        0        0     6347 2023-04-19 11:59:20.956756 libsql-client-0.2.0/libsql_client/sync.py
--rw-r--r--   0        0        0      933 2023-04-24 11:57:58.823118 libsql-client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 libsql-client-0.2.0/setup.py
--rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 libsql-client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-27 08:58:08.764134 libsql-client-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2912 2023-04-27 07:46:00.306317 libsql-client-0.2.1/README.md
+-rw-r--r--   0        0        0      268 2023-04-19 10:43:28.755257 libsql-client-0.2.1/libsql_client/__init__.py
+-rw-r--r--   0        0        0     3039 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/client.py
+-rw-r--r--   0        0        0      993 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/config.py
+-rw-r--r--   0        0        0      801 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/create_client.py
+-rw-r--r--   0        0        0       85 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/hrana/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-28 14:43:03.375368 libsql-client-0.2.1/libsql_client/hrana/client.py
+-rw-r--r--   0        0        0    12135 2023-04-28 14:43:03.379368 libsql-client-0.2.1/libsql_client/hrana/conn.py
+-rw-r--r--   0        0        0     4816 2023-04-20 09:18:36.654076 libsql-client-0.2.1/libsql_client/hrana/convert.py
+-rw-r--r--   0        0        0     1610 2023-04-17 12:00:30.661316 libsql-client-0.2.1/libsql_client/hrana/id_alloc.py
+-rw-r--r--   0        0        0     3974 2023-04-17 12:00:30.661316 libsql-client-0.2.1/libsql_client/hrana/proto.py
+-rw-r--r--   0        0        0     3441 2023-04-17 12:00:30.661316 libsql-client-0.2.1/libsql_client/http.py
+-rw-r--r--   0        0        0     3071 2023-04-28 14:52:18.017515 libsql-client-0.2.1/libsql_client/result.py
+-rw-r--r--   0        0        0     4896 2023-04-20 09:19:13.406247 libsql-client-0.2.1/libsql_client/sqlite3.py
+-rw-r--r--   0        0        0     6347 2023-04-19 11:59:20.956756 libsql-client-0.2.1/libsql_client/sync.py
+-rw-r--r--   0        0        0      960 2023-04-28 15:10:54.208794 libsql-client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 libsql-client-0.2.1/setup.py
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 libsql-client-0.2.1/PKG-INFO
```

### Comparing `libsql-client-0.2.0/LICENSE.md` & `libsql-client-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/README.md` & `libsql-client-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 This package also provides a synchronous version of the client, which can be created by calling `create_client_sync()`. It supports the same methods as the default `asyncio` client, except that they block the calling thread:
 
 ```python
 import libsql_client
 
 url = "file:local.db"
-with libsql_client.create_client(url) as client:
+with libsql_client.create_client_sync(url) as client:
     result_set = client.execute("SELECT * from users")
     print(len(result_set.rows), "rows")
     for row in result_set.rows:
         print(row)
 ```
 
 The synchronous client is just a thin wrapper around the asynchronous client, but it runs the event loop in a background thread.
```

### Comparing `libsql-client-0.2.0/libsql_client/client.py` & `libsql-client-0.2.1/libsql_client/client.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/config.py` & `libsql-client-0.2.1/libsql_client/config.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/create_client.py` & `libsql-client-0.2.1/libsql_client/create_client.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/hrana/client.py` & `libsql-client-0.2.1/libsql_client/hrana/conn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,169 +1,190 @@
 from __future__ import annotations
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, TypeVar, cast
+from typing import Any, Callable, Dict, Optional, TypeVar, cast
 import aiohttp
 import asyncio
 import json
-import urllib.parse
 
-from ..client import Client, InArgs, InStatement, LibsqlError, Transaction
-from ..config import _Config
-from ..result import ResultSet
+from ..client import LibsqlError
 from . import proto
-from .convert import (
-    _stmt_to_proto, _result_set_from_proto,
-    _batch_to_proto, _batch_results_from_proto,
-    _error_from_proto,
-)
+from .convert import _error_from_proto
 from .id_alloc import IdAlloc
 
-def _create_hrana_client(config: _Config) -> HranaClient:
-    assert config.scheme in ("ws", "wss")
-    url = urllib.parse.urlunparse((
-        config.scheme, config.authority, config.path,
-        "", "", "",
-    ))
-    return HranaClient(url, auth_token=config.auth_token)
-
 @dataclass
 class _ResponseState:
     type: str
     future: asyncio.Future[proto.Response]
 
 @dataclass
 class _StreamState:
     stream_id: int
     closed: Optional[BaseException]
 
-class HranaClient(Client):
-    _socket_task: asyncio.Task[None]
-    _send_msg_queue: asyncio.Queue[Optional[str]]
-    _closed: Optional[BaseException]
+class HranaConn:
+    _connect_task: asyncio.Task[aiohttp.ClientWebSocketResponse]
+    _receive_task: Optional[asyncio.Task[None]]
+    _send_task: Optional[asyncio.Task[None]]
+
+    _socket: Optional[aiohttp.ClientWebSocketResponse]
+    _send_msg_queue: asyncio.Queue[str]
 
     _recvd_hello: bool
     _response_map: Dict[int, _ResponseState]
     _request_id_alloc: IdAlloc
     _stream_id_alloc: IdAlloc
 
-    def __init__(self, url: str, *, auth_token: Optional[str] = None):
-        self._socket_task = asyncio.create_task(self._run_socket_task(url))
-        self._socket_task.add_done_callback(self._socket_task_done)
+    exception: Optional[BaseException]
+
+    def __init__(self, session: aiohttp.ClientSession, url: str, auth_token: Optional[str] = None):
+        self._connect_task = asyncio.create_task(self._do_connect(session, url))
+        self._connect_task.add_done_callback(self._done_connect)
+        self._receive_task = None
+        self._send_task = None
+
+        self._socket = None
         self._send_msg_queue = asyncio.Queue()
-        self._closed = None
 
         self._recvd_hello = False
         self._response_map = {}
         self._request_id_alloc = IdAlloc()
         self._stream_id_alloc = IdAlloc()
 
+        self.exception = None
+
         self._send({"type": "hello", "jwt": auth_token})
 
-    async def _run_socket_task(self, url: str) -> None:
-        async with aiohttp.ClientSession() as session:
-            socket = await session.ws_connect(
-                url,
-                protocols=["hrana1"],
-                autoclose=False,
-                autoping=True,
-            )
-            await self._run_socket(socket)
-
-    async def _run_socket(self, socket: aiohttp.ClientWebSocketResponse) -> None:
-        async def do_receive() -> None:
-            while True:
-                msg = await socket.receive()
-                if msg.type == aiohttp.WSMsgType.TEXT:
-                    try:
-                        self._receive(msg.data)
-                    except Exception as e:
-                        await socket.close(code=3007, message="Could not handle message".encode())
-                        raise
-                elif msg.type == aiohttp.WSMsgType.BINARY:
-                    await socket.close(code=3003, message="Only text messages are accepted".encode())
-                    raise LibsqlError("Received a binary WebSocket message", "HRANA_PROTO_ERROR")
-                elif msg.type == aiohttp.WSMsgType.PING:
-                    await socket.pong(msg.data)
-                elif msg.type == aiohttp.WSMsgType.PONG:
-                    pass
-                elif msg.type == aiohttp.WSMsgType.CLOSE:
-                    code = cast(aiohttp.WSCloseCode, msg.data)
-                    reason = cast(str, msg.extra)
-                    raise LibsqlError(
-                        f"WebSocket was closed with code {code}: {reason!r}",
-                        "WEBSOCKET_CLOSED",
-                    )
-                elif msg.type in (aiohttp.WSMsgType.CLOSING, aiohttp.WSMsgType.CLOSED):
-                    break
-                elif msg.type == aiohttp.WSMsgType.ERROR:
-                    raise msg.data
-                else:
-                    raise LibsqlError(
-                        f"Received unexpected WebSocket message {msg.type!r}",
-                        "HRANA_PROTO_ERROR",
-                    )
-
-        async def do_send() -> None:
-            while True:
-                msg_str = await self._send_msg_queue.get()
-                if msg_str is None:
-                    break
-                await socket.send_str(msg_str)
-            await socket.close()
+    async def _do_connect(self, session: aiohttp.ClientSession, url: str) -> aiohttp.ClientWebSocketResponse:
+        return await session.ws_connect(
+            url,
+            protocols=["hrana1"],
+            autoclose=False,
+            autoping=True,
+        )
+
+    def _done_connect(self, task: asyncio.Task[aiohttp.ClientWebSocketResponse]) -> None:
+        e: Optional[BaseException]
+        if task.cancelled():
+            e = LibsqlError("The connect task was cancelled", "CLIENT_CLOSED")
+        else:
+            e = task.exception()
+        if e is not None:
+            self._set_exception(e)
+
+        if self.exception is not None:
+            return
+
+        socket = task.result()
+        receive_task = asyncio.create_task(self._do_receive(socket))
+        send_task = asyncio.create_task(self._do_send(socket))
+
+        receive_task.add_done_callback(self._done_receive)
+        send_task.add_done_callback(self._done_send)
+
+        self._socket = socket
+        self._receive_task = receive_task
+        self._send_task = send_task
+
+    async def _do_receive(self, socket: aiohttp.ClientWebSocketResponse) -> None:
+        while True:
+            msg = await socket.receive()
+            if msg.type == aiohttp.WSMsgType.TEXT:
+                try:
+                    self._receive(msg.data)
+                except Exception as e:
+                    await socket.close(code=3007, message="Could not handle message".encode())
+                    raise
+            elif msg.type == aiohttp.WSMsgType.BINARY:
+                await socket.close(code=3003, message="Only text messages are accepted".encode())
+                raise LibsqlError("Received a binary WebSocket message", "HRANA_PROTO_ERROR")
+            elif msg.type == aiohttp.WSMsgType.PING:
+                await socket.pong(msg.data)
+            elif msg.type == aiohttp.WSMsgType.PONG:
+                pass
+            elif msg.type == aiohttp.WSMsgType.CLOSE:
+                code = cast(aiohttp.WSCloseCode, msg.data)
+                reason = cast(str, msg.extra)
+                raise LibsqlError(
+                    f"WebSocket was closed with code {code}: {reason!r}",
+                    "HRANA_WEBSOCKET_ERROR",
+                )
+            elif msg.type == aiohttp.WSMsgType.CLOSING:
+                pass
+            elif msg.type == aiohttp.WSMsgType.CLOSED:
+                raise LibsqlError("WebSocket was closed", "HRANA_WEBSOCKET_ERROR")
+            elif msg.type == aiohttp.WSMsgType.ERROR:
+                raise msg.data
+            else:
+                raise LibsqlError(
+                    f"Received unexpected WebSocket message {msg.type!r}",
+                    "HRANA_PROTO_ERROR",
+                )
+
+    async def _do_send(self, socket: aiohttp.ClientWebSocketResponse) -> None:
+        while True:
+            msg_str = await self._send_msg_queue.get()
+            await socket.send_str(msg_str)
+
+    def _done_receive(self, task: asyncio.Task[None]) -> None:
+        e: Optional[BaseException]
+        if task.cancelled():
+            e = LibsqlError("The receive task was cancelled", "CLIENT_CLOSED")
+        else:
+            e = task.exception()
 
-        try:
-            receiver = asyncio.create_task(do_receive())
-            sender = asyncio.create_task(do_send())
-            await asyncio.gather(receiver, sender)
-            await socket.close()
-        except Exception as e:
-            await socket.close(code=3000, message="Client encountered an internal error".encode())
-            raise
-        finally:
-            receiver.cancel()
-            sender.cancel()
-
-    def _socket_task_done(self, fut: asyncio.Future[None]) -> None:
-        if fut.cancelled():
-            self._set_closed(LibsqlError("Client task was cancelled", "CLIENT_CLOSED"))
-        e = fut.exception()
         if e is not None:
-            self._set_closed(e)
+            if self._send_task is not None:
+                self._send_task.cancel()
+            self._set_exception(e)
+
+    def _done_send(self, task: asyncio.Task[None]) -> None:
+        e: Optional[BaseException]
+        if task.cancelled():
+            e = LibsqlError("The send task was cancelled", "CLIENT_CLOSED")
         else:
-            self._set_closed(LibsqlError("Client task has terminated", "CLIENT_CLOSED"))
+            e = task.exception()
+
+        if e is not None:
+            self._set_exception(e)
+
+        if self._receive_task is not None:
+            self._receive_task.cancel()
 
     def _send(self, msg: proto.ClientMsg) -> None:
-        assert self._closed is None
+        assert self.exception is None
         self._send_msg_queue.put_nowait(json.dumps(msg))
 
-    def _set_closed(self, e: BaseException) -> None:
-        if self._closed is not None:
+    def _set_exception(self, e: BaseException) -> None:
+        if self.exception is not None:
             return
-        self._closed = e
-        self._send_msg_queue.put_nowait(None)
+        self.exception = e
+
+        for task in (self._connect_task, self._receive_task, self._send_task):
+            if task is not None:
+                task.cancel()
 
         for request_id, response_state in self._response_map.items():
             response_state.future.set_exception(e)
             self._request_id_alloc.free(request_id)
         self._response_map.clear()
 
-    def _send_request(self, request: proto.Request) -> asyncio.Future[proto.Response]:
+    def send_request(self, request: proto.Request) -> asyncio.Future[proto.Response]:
         future = asyncio.get_running_loop().create_future()
 
-        if self._closed is not None:
-            future.set_exception(LibsqlError("Client is closed", "CLIENT_CLOSED"))
+        if self.exception is not None:
+            future.set_exception(self.exception)
             return future
 
         request_id = self._request_id_alloc.alloc()
         self._response_map[request_id] = _ResponseState(request["type"], future)
         self._send({"type": "request", "request_id": request_id, "request": request})
         return future
 
     def _receive(self, text: str) -> None:
-        if self._closed is not None:
+        if self.exception is not None:
             return
 
         try:
             msg = json.loads(text)
         except ValueError as e:
             raise LibsqlError("Server message is not valid JSON", "HRANA_PROTO_ERROR") from e
 
@@ -212,163 +233,93 @@
             if fut.cancelled():
                 e = asyncio.CancelledError("Stream opening was cancelled")
             else:
                 e = fut.exception()
             if e is not None:
                 self._close_stream(stream_state, e)
 
-        open_fut = self._send_request({
+        open_fut = self.send_request({
             "type": "open_stream",
             "stream_id": stream_id,
         })
         open_fut.add_done_callback(open_done)
 
         return HranaStream(self, stream_state)
 
     def _close_stream(self, stream_state: _StreamState, e: BaseException) -> None:
-        if stream_state.closed is not None or self._closed is not None:
+        if stream_state.closed is not None or self.exception is not None:
             return
         stream_state.closed = e
 
         def close_done(_fut: asyncio.Future[proto.Response]) -> None:
             self._stream_id_alloc.free(stream_state.stream_id)
 
-        close_fut = self._send_request({
+        close_fut = self.send_request({
             "type": "close_stream",
             "stream_id": stream_state.stream_id,
         })
         close_fut.add_done_callback(close_done)
 
-    async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
-        with self.open_stream() as stream:
-            proto_stmt = _stmt_to_proto(stmt, args)
-            proto_result_fut = stream.execute(proto_stmt)
-        return _result_set_from_proto(await proto_result_fut)
-
-    async def batch(self, stmts: List[InStatement]) -> List[ResultSet]:
-        with self.open_stream() as stream:
-            proto_batch = _batch_to_proto(stmts)
-            proto_result_fut = stream.batch(proto_batch)
-        return _batch_results_from_proto(await proto_result_fut, len(stmts))
-
-    def transaction(self) -> "HranaTransaction":
-        stream = self.open_stream()
-        return HranaTransaction(stream)
-
     async def close(self) -> None:
-        self._set_closed(LibsqlError("Client was manually closed", "CLIENT_CLOSED"))
-        await self._socket_task
-
-    @property
-    def closed(self) -> bool:
-        return self._closed is not None
+        self._set_exception(LibsqlError("Client was manually closed", "CLIENT_CLOSED"))
+        if self._socket is not None:
+            await self._socket.close()
 
 class HranaStream:
-    _client: HranaClient
+    _conn: HranaConn
     _state: _StreamState
 
-    def __init__(self, client: HranaClient, state: _StreamState):
-        self._client = client
+    def __init__(self, conn: HranaConn, state: _StreamState):
+        self._conn = conn
         self._state = state
 
     def execute(self, stmt: proto.Stmt) -> asyncio.Future[proto.StmtResult]:
         if self._state.closed is not None:
             raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
 
         request: proto.ExecuteReq = {
             "type": "execute",
             "stream_id": self._state.stream_id,
             "stmt": stmt,
         }
-        response_fut = self._client._send_request(request)
+        response_fut = self._conn.send_request(request)
 
         def get_result(response: proto.Response) -> proto.StmtResult:
             return cast(proto.ExecuteResp, response)["result"]
         return _map_future(response_fut, get_result)
 
     def batch(self, batch: proto.Batch) -> asyncio.Future[proto.BatchResult]:
         if self._state.closed is not None:
             raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
 
         request: proto.BatchReq = {
             "type": "batch",
             "stream_id": self._state.stream_id,
             "batch": batch,
         }
-        response_fut = self._client._send_request(request)
+        response_fut = self._conn.send_request(request)
 
         def get_result(response: proto.Response) -> proto.BatchResult:
             return cast(proto.BatchResp, response)["result"]
         return _map_future(response_fut, get_result)
 
     def close(self) -> None:
         e = LibsqlError("Stream was manually closed", "STREAM_CLOSED")
-        self._client._close_stream(self._state, e)
+        self._conn._close_stream(self._state, e)
 
     @property
     def closed(self) -> bool:
         return self._state.closed is not None
 
     def __enter__(self) -> HranaStream:
         return self
 
     def __exit__(self, _exc_type: Any, _exc_value: Any, _traceback: Any) -> None:
         self.close()
 
-class HranaTransaction(Transaction):
-    _stream: HranaStream
-    _begin_fut: asyncio.Future[proto.StmtResult]
-
-    def __init__(self, stream: HranaStream):
-        self._stream = stream
-        self._begin_fut = stream.execute({
-            "sql": "BEGIN",
-            "want_rows": False,
-        })
-
-    async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
-        await self._begin_fut
-        if self._stream.closed:
-            raise LibsqlError("The transaction is closed", "TRANSACTION_CLOSED")
-
-        proto_stmt = _stmt_to_proto(stmt, args)
-        proto_result = await self._stream.execute(proto_stmt)
-        return _result_set_from_proto(proto_result)
-
-    async def rollback(self) -> None:
-        await self._begin_fut
-        if self._stream.closed:
-            return
-
-        fut = self._stream.execute({
-            "sql": "ROLLBACK",
-            "want_rows": False,
-        })
-        self._stream.close()
-        await fut
-
-    async def commit(self) -> None:
-        await self._begin_fut
-        if self._stream.closed:
-            raise LibsqlError("The transaction is closed", "TRANSACTION_CLOSED")
-
-        fut = self._stream.execute({
-            "sql": "COMMIT",
-            "want_rows": False,
-        })
-        self._stream.close()
-        await fut
-
-    def close(self) -> None:
-        self._stream.close()
-
-    @property
-    def closed(self) -> bool:
-        return self._stream.closed
-
 T = TypeVar("T")
 R = TypeVar("R")
 
 def _map_future(fut: asyncio.Future[T], f: Callable[[T], R]) -> asyncio.Future[R]:
     ret: asyncio.Future[R] = asyncio.get_running_loop().create_future()
     def done(fut: asyncio.Future[T]) -> None:
         if fut.cancelled():
```

### Comparing `libsql-client-0.2.0/libsql_client/hrana/convert.py` & `libsql-client-0.2.1/libsql_client/hrana/convert.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/hrana/id_alloc.py` & `libsql-client-0.2.1/libsql_client/hrana/id_alloc.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/hrana/proto.py` & `libsql-client-0.2.1/libsql_client/hrana/proto.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/http.py` & `libsql-client-0.2.1/libsql_client/http.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/result.py` & `libsql-client-0.2.1/libsql_client/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from __future__ import annotations
 from collections.abc import Sequence
 from typing import Dict, Iterator, List, Optional, Tuple, Union, overload
 
 Value = Union[None, str, int, float, bytes]
 
 class ResultSet:
     """Result of an SQL statement.
 
     The result is composed of columns and rows. Every row is represented as a `Row` object and the length of
     every row is equal to the number of columns.
     """
 
     _columns: Tuple[str, ...]
-    _rows: List["Row"]
+    _rows: List[Row]
     _rows_affected: int
     _last_insert_rowid: Optional[int]
     __slots__ = ["_columns", "_rows", "_rows_affected", "_last_insert_rowid"]
 
     def __init__(
         self,
         columns: Tuple[str, ...],
@@ -31,27 +32,27 @@
     def __iter__(self) -> Iterator["Row"]:
         return self._rows.__iter__()
 
     def __len__(self) -> int:
         return len(self._rows)
 
     @overload
-    def __getitem__(self, key: int) -> "Row": pass
+    def __getitem__(self, key: int) -> Row: pass
     @overload
-    def __getitem__(self, key: slice) -> List["Row"]: pass
+    def __getitem__(self, key: slice) -> List[Row]: pass
 
-    def __getitem__(self, key: Union[int, slice]) -> Union["Row", List["Row"]]:
+    def __getitem__(self, key: Union[int, slice]) -> Union[Row, List[Row]]:
         return self._rows[key]
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self._columns
 
     @property
-    def rows(self) -> List["Row"]:
+    def rows(self) -> List[Row]:
         return self._rows
 
     @property
     def rows_affected(self) -> int:
         return self._rows_affected
 
     @property
```

### Comparing `libsql-client-0.2.0/libsql_client/sqlite3.py` & `libsql-client-0.2.1/libsql_client/sqlite3.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/libsql_client/sync.py` & `libsql-client-0.2.1/libsql_client/sync.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.0/pyproject.toml` & `libsql-client-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsql-client"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     "Jan Špaček <honza@chiselstrike.com>",
     "ChiselStrike",
 ]
 description = "Python SDK for libSQL"
 homepage = "https://github.com/libsql/libsql-client-py"
 repository = "https://github.com/libsql/libsql-client-py"
@@ -14,14 +14,15 @@
 classifiers = [
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 aiohttp = "^3.0"
+typing-extensions = "^4.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 pytest-asyncio = "^0.20.3"
 mypy = "^1.2"
 requests = "^2.28.2"
```

### Comparing `libsql-client-0.2.0/setup.py` & `libsql-client-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['libsql_client', 'libsql_client.hrana']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiohttp>=3.0,<4.0']
+['aiohttp>=3.0,<4.0', 'typing-extensions>=4.5,<5.0']
 
 setup_kwargs = {
     'name': 'libsql-client',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Python SDK for libSQL',
-    'long_description': '# Python SDK for libSQL\n\n**[API reference][reference] | [Github][github] | [PyPI][pypi]**\n\n[reference]: https://libsql.org/libsql-client-py/reference.html\n[github]: https://github.com/libsql/libsql-client-py\n[pypi]: https://pypi.org/project/libsql-client/\n\nThis is the source repository of the Python SDK for libSQL. You can either connect to a local SQLite database or to a remote libSQL server ([sqld][sqld]).\n\n[sqld]: https://github.com/libsql/sqld\n\n## Installation\n\n```\npip install libsql-client\n```\n\n## Getting Started\n\nConnecting to a local SQLite database:\n\n```python\nimport asyncio\nimport libsql_client\n\nasync def main():\n    url = "file:local.db"\n    async with libsql_client.create_client(url) as client:\n        result_set = await client.execute("SELECT * from users")\n        print(len(result_set.rows), "rows")\n        for row in result_set.rows:\n            print(row)\n\nasyncio.run(main())\n```\n\nTo connect to a remote libSQL server ([sqld][sqld]), just change the URL:\n\n```python\nurl = "ws://localhost:8080"\n```\n\n## Supported URLs\n\nThe client can connect to the database using different methods depending on the scheme (protocol) of the passed URL:\n\n* `file:` connects to a local SQLite database (using the builtin `sqlite3` package)\n  * `file:/absolute/path` or `file:///absolute/path` is an absolute path on local filesystem\n  * `file:relative/path` is a relative path on local filesystem\n  * (`file://path` is not a valid URL)\n* `ws:` or `wss:` connect to sqld using WebSockets (the Hrana protocol).\n* `http:` or `https:` connect to sqld using HTTP. The `transaction()` API is not available in this case.\n* `libsql:` is equivalent to `wss:`.\n\n## Synchronous API\n\nThis package also provides a synchronous version of the client, which can be created by calling `create_client_sync()`. It supports the same methods as the default `asyncio` client, except that they block the calling thread:\n\n```python\nimport libsql_client\n\nurl = "file:local.db"\nwith libsql_client.create_client(url) as client:\n    result_set = client.execute("SELECT * from users")\n    print(len(result_set.rows), "rows")\n    for row in result_set.rows:\n        print(row)\n```\n\nThe synchronous client is just a thin wrapper around the asynchronous client, but it runs the event loop in a background thread.\n\n## Contributing to this package\n\nFirst, please install Python and [Poetry][poetry]. To install all dependencies for local development to a\nvirtual environment, run:\n\n[poetry]: https://python-poetry.org/\n\n```\npoetry install --with dev\n```\n\nTo run the tests, use:\n\n```\npoetry run pytest\n```\n\nTo check types with MyPy, use:\n\n```\npoetry run mypy\n```\n\n## License\n\nThis project is licensed under the MIT license.\n\n### Contribution\n\nUnless you explicitly state otherwise, any contribution intentionally submitted for inclusion in `libsql-client` by you, shall be licensed as MIT, without any additional terms or conditions.\n',
+    'long_description': '# Python SDK for libSQL\n\n**[API reference][reference] | [Github][github] | [PyPI][pypi]**\n\n[reference]: https://libsql.org/libsql-client-py/reference.html\n[github]: https://github.com/libsql/libsql-client-py\n[pypi]: https://pypi.org/project/libsql-client/\n\nThis is the source repository of the Python SDK for libSQL. You can either connect to a local SQLite database or to a remote libSQL server ([sqld][sqld]).\n\n[sqld]: https://github.com/libsql/sqld\n\n## Installation\n\n```\npip install libsql-client\n```\n\n## Getting Started\n\nConnecting to a local SQLite database:\n\n```python\nimport asyncio\nimport libsql_client\n\nasync def main():\n    url = "file:local.db"\n    async with libsql_client.create_client(url) as client:\n        result_set = await client.execute("SELECT * from users")\n        print(len(result_set.rows), "rows")\n        for row in result_set.rows:\n            print(row)\n\nasyncio.run(main())\n```\n\nTo connect to a remote libSQL server ([sqld][sqld]), just change the URL:\n\n```python\nurl = "ws://localhost:8080"\n```\n\n## Supported URLs\n\nThe client can connect to the database using different methods depending on the scheme (protocol) of the passed URL:\n\n* `file:` connects to a local SQLite database (using the builtin `sqlite3` package)\n  * `file:/absolute/path` or `file:///absolute/path` is an absolute path on local filesystem\n  * `file:relative/path` is a relative path on local filesystem\n  * (`file://path` is not a valid URL)\n* `ws:` or `wss:` connect to sqld using WebSockets (the Hrana protocol).\n* `http:` or `https:` connect to sqld using HTTP. The `transaction()` API is not available in this case.\n* `libsql:` is equivalent to `wss:`.\n\n## Synchronous API\n\nThis package also provides a synchronous version of the client, which can be created by calling `create_client_sync()`. It supports the same methods as the default `asyncio` client, except that they block the calling thread:\n\n```python\nimport libsql_client\n\nurl = "file:local.db"\nwith libsql_client.create_client_sync(url) as client:\n    result_set = client.execute("SELECT * from users")\n    print(len(result_set.rows), "rows")\n    for row in result_set.rows:\n        print(row)\n```\n\nThe synchronous client is just a thin wrapper around the asynchronous client, but it runs the event loop in a background thread.\n\n## Contributing to this package\n\nFirst, please install Python and [Poetry][poetry]. To install all dependencies for local development to a\nvirtual environment, run:\n\n[poetry]: https://python-poetry.org/\n\n```\npoetry install --with dev\n```\n\nTo run the tests, use:\n\n```\npoetry run pytest\n```\n\nTo check types with MyPy, use:\n\n```\npoetry run mypy\n```\n\n## License\n\nThis project is licensed under the MIT license.\n\n### Contribution\n\nUnless you explicitly state otherwise, any contribution intentionally submitted for inclusion in `libsql-client` by you, shall be licensed as MIT, without any additional terms or conditions.\n',
     'author': 'Jan Špaček',
     'author_email': 'honza@chiselstrike.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/libsql/libsql-client-py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libsql-client-0.2.0/PKG-INFO` & `libsql-client-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: libsql-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for libSQL
 Home-page: https://github.com/libsql/libsql-client-py
 License: MIT
 Author: Jan Špaček
 Author-email: honza@chiselstrike.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiohttp (>=3.0,<4.0)
+Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Documentation, https://libsql.org/libsql-client-py/
 Project-URL: Repository, https://github.com/libsql/libsql-client-py
 Description-Content-Type: text/markdown
 
 # Python SDK for libSQL
 
 **[API reference][reference] | [Github][github] | [PyPI][pypi]**
@@ -78,15 +79,15 @@
 
 This package also provides a synchronous version of the client, which can be created by calling `create_client_sync()`. It supports the same methods as the default `asyncio` client, except that they block the calling thread:
 
 ```python
 import libsql_client
 
 url = "file:local.db"
-with libsql_client.create_client(url) as client:
+with libsql_client.create_client_sync(url) as client:
     result_set = client.execute("SELECT * from users")
     print(len(result_set.rows), "rows")
     for row in result_set.rows:
         print(row)
 ```
 
 The synchronous client is just a thin wrapper around the asynchronous client, but it runs the event loop in a background thread.
```

