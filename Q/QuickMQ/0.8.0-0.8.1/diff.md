# Comparing `tmp/QuickMQ-0.8.0.tar.gz` & `tmp/QuickMQ-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickMQ-0.8.0.tar", last modified: Fri Mar 24 21:12:31 2023, max compression
+gzip compressed data, was "QuickMQ-0.8.1.tar", last modified: Fri Apr 28 14:33:04 2023, max compression
```

## Comparing `QuickMQ-0.8.0.tar` & `QuickMQ-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-03-24 21:12:31.298021 QuickMQ-0.8.0/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1071 2023-02-17 21:40:50.000000 QuickMQ-0.8.0/LICENSE
--rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-03-24 21:12:31.298021 QuickMQ-0.8.0/PKG-INFO
--rw-r--r--   0 mdrexler (29089) domain users   (700)     4522 2023-03-24 19:33:20.000000 QuickMQ-0.8.0/README.md
--rw-r--r--   0 mdrexler (29089) domain users   (700)      295 2023-03-22 22:41:02.000000 QuickMQ-0.8.0/pyproject.toml
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1506 2023-03-24 21:12:31.299021 QuickMQ-0.8.0/setup.cfg
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-03-24 21:12:31.295021 QuickMQ-0.8.0/src/
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-03-24 21:12:31.296021 QuickMQ-0.8.0/src/QuickMQ.egg-info/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-03-24 21:12:31.000000 QuickMQ-0.8.0/src/QuickMQ.egg-info/PKG-INFO
--rw-r--r--   0 mdrexler (29089) domain users   (700)      631 2023-03-24 21:12:31.000000 QuickMQ-0.8.0/src/QuickMQ.egg-info/SOURCES.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)        1 2023-03-24 21:12:31.000000 QuickMQ-0.8.0/src/QuickMQ.egg-info/dependency_links.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)       50 2023-03-24 21:12:31.000000 QuickMQ-0.8.0/src/QuickMQ.egg-info/entry_points.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)      113 2023-03-24 21:12:31.000000 QuickMQ-0.8.0/src/QuickMQ.egg-info/requires.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)        8 2023-03-24 21:12:31.000000 QuickMQ-0.8.0/src/QuickMQ.egg-info/top_level.txt
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-03-24 21:12:31.297021 QuickMQ-0.8.0/src/quickmq/
--rw-r--r--   0 mdrexler (29089) domain users   (700)      511 2023-03-24 18:38:05.000000 QuickMQ-0.8.0/src/quickmq/__init__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)       82 2023-03-24 15:38:55.000000 QuickMQ-0.8.0/src/quickmq/__version__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1469 2023-03-24 15:15:17.000000 QuickMQ-0.8.0/src/quickmq/api.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     5117 2023-03-24 14:22:31.000000 QuickMQ-0.8.0/src/quickmq/config.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)    10371 2023-03-24 20:34:37.000000 QuickMQ-0.8.0/src/quickmq/connection.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)       39 2023-03-03 20:16:51.000000 QuickMQ-0.8.0/src/quickmq/consume.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)      462 2023-03-03 21:47:49.000000 QuickMQ-0.8.0/src/quickmq/exceptions.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1193 2023-03-24 15:52:10.000000 QuickMQ-0.8.0/src/quickmq/message.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2545 2023-03-22 22:41:02.000000 QuickMQ-0.8.0/src/quickmq/publish.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)        0 2023-01-13 22:27:07.000000 QuickMQ-0.8.0/src/quickmq/py.typed
--rw-r--r--   0 mdrexler (29089) domain users   (700)     3412 2023-03-24 15:15:04.000000 QuickMQ-0.8.0/src/quickmq/session.py
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-03-24 21:12:31.298021 QuickMQ-0.8.0/test/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2446 2023-03-24 19:12:51.000000 QuickMQ-0.8.0/test/test_api.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1080 2023-03-24 18:47:08.000000 QuickMQ-0.8.0/test/test_cli.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1820 2023-03-24 14:22:30.000000 QuickMQ-0.8.0/test/test_config.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2675 2023-03-03 21:47:49.000000 QuickMQ-0.8.0/test/test_connection.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)      535 2023-03-24 18:46:03.000000 QuickMQ-0.8.0/test/test_message.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1437 2023-03-03 20:12:14.000000 QuickMQ-0.8.0/test/test_session.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.749647 QuickMQ-0.8.1/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1071 2023-02-17 21:40:50.000000 QuickMQ-0.8.1/LICENSE
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-04-28 14:33:04.750648 QuickMQ-0.8.1/PKG-INFO
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     4522 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/README.md
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      295 2023-03-22 22:41:02.000000 QuickMQ-0.8.1/pyproject.toml
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1506 2023-04-28 14:33:04.751648 QuickMQ-0.8.1/setup.cfg
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.746647 QuickMQ-0.8.1/src/
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.747648 QuickMQ-0.8.1/src/QuickMQ.egg-info/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/PKG-INFO
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      653 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        1 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       50 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/entry_points.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      113 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/requires.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        8 2023-04-28 14:33:04.000000 QuickMQ-0.8.1/src/QuickMQ.egg-info/top_level.txt
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.749647 QuickMQ-0.8.1/src/quickmq/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      511 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/src/quickmq/__init__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       82 2023-04-28 14:32:57.000000 QuickMQ-0.8.1/src/quickmq/__version__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1469 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/src/quickmq/api.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     5111 2023-03-31 21:47:11.000000 QuickMQ-0.8.1/src/quickmq/config.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)    10394 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/src/quickmq/connection.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       39 2023-03-03 20:16:51.000000 QuickMQ-0.8.1/src/quickmq/consume.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1968 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/src/quickmq/editor.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      462 2023-03-03 21:47:49.000000 QuickMQ-0.8.1/src/quickmq/exceptions.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1193 2023-04-28 14:28:11.000000 QuickMQ-0.8.1/src/quickmq/message.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2545 2023-04-28 14:28:41.000000 QuickMQ-0.8.1/src/quickmq/publish.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        0 2023-01-13 22:27:07.000000 QuickMQ-0.8.1/src/quickmq/py.typed
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     3394 2023-04-28 14:27:52.000000 QuickMQ-0.8.1/src/quickmq/session.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-04-28 14:33:04.749647 QuickMQ-0.8.1/test/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2446 2023-04-28 14:26:29.000000 QuickMQ-0.8.1/test/test_api.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1079 2023-04-28 14:27:44.000000 QuickMQ-0.8.1/test/test_cli.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1820 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/test/test_config.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2675 2023-03-03 21:47:49.000000 QuickMQ-0.8.1/test/test_connection.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      535 2023-03-29 21:03:07.000000 QuickMQ-0.8.1/test/test_message.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1437 2023-03-03 20:12:14.000000 QuickMQ-0.8.1/test/test_session.py
```

### Comparing `QuickMQ-0.8.0/LICENSE` & `QuickMQ-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/PKG-INFO` & `QuickMQ-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickMQ
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple RabbitMQ client
 Home-page: https://gitlab.ssec.wisc.edu/mdrexler/easymq
 Author: Max Drexler
 Author-email: mndrexler@wisc.edu
 License: MIT
 Keywords: rabbitmq,message publisher,amqp message
 Classifier: Programming Language :: Python :: 3
```

### Comparing `QuickMQ-0.8.0/README.md` & `QuickMQ-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/setup.cfg` & `QuickMQ-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/src/QuickMQ.egg-info/PKG-INFO` & `QuickMQ-0.8.1/src/QuickMQ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickMQ
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple RabbitMQ client
 Home-page: https://gitlab.ssec.wisc.edu/mdrexler/easymq
 Author: Max Drexler
 Author-email: mndrexler@wisc.edu
 License: MIT
 Keywords: rabbitmq,message publisher,amqp message
 Classifier: Programming Language :: Python :: 3
```

### Comparing `QuickMQ-0.8.0/src/QuickMQ.egg-info/SOURCES.txt` & `QuickMQ-0.8.1/src/QuickMQ.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/QuickMQ.egg-info/top_level.txt
 src/quickmq/__init__.py
 src/quickmq/__version__.py
 src/quickmq/api.py
 src/quickmq/config.py
 src/quickmq/connection.py
 src/quickmq/consume.py
+src/quickmq/editor.py
 src/quickmq/exceptions.py
 src/quickmq/message.py
 src/quickmq/publish.py
 src/quickmq/py.typed
 src/quickmq/session.py
 test/test_api.py
 test/test_cli.py
```

### Comparing `QuickMQ-0.8.0/src/quickmq/api.py` & `QuickMQ-0.8.1/src/quickmq/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     exchange: Optional[str] = None,
     confirm_delivery=True,
 ) -> None:
     _CURRENT_SESSION.publish(message, key, exchange, confirm_delivery)
 
 
 def publish_all(
-    messages: Iterable[Union[str, Tuple[str, Any]]],
+    messages: Iterable[Union[Any, Tuple[str, Any]]],
     exchange: Optional[str] = None,
     confirm_delivery=True,
 ) -> None:
     _CURRENT_SESSION.publish_all(messages, exchange, confirm_delivery)
 
 
 # Consuming API *implement later
```

### Comparing `QuickMQ-0.8.0/src/quickmq/config.py` & `QuickMQ-0.8.1/src/quickmq/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 import json
 import os
 import warnings
 from typing import Dict, Callable, List, Tuple, Union, Any
 from platformdirs import PlatformDirs
 import logging
 
-LOGGER = logging.getLogger('quickmq')
+LOGGER = logging.getLogger("quickmq")
 
 CFG_VALS = Union[str, int, float]
 CFG_FILE_NAME = "cfg_vars.json"
-CFG_FILE_PATH = os.path.join(
-    PlatformDirs("easymq").user_config_dir, CFG_FILE_NAME
-)
+CFG_FILE_PATH = os.path.join(PlatformDirs("easymq").user_config_dir, CFG_FILE_NAME)
 
 
 def verify_pos_float(_obj: Any) -> float:
     new_float = float(_obj)
     if new_float < 0:
         raise ValueError
     return new_float
```

### Comparing `QuickMQ-0.8.0/src/quickmq/connection.py` & `QuickMQ-0.8.1/src/quickmq/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ProbableAuthenticationError,
     StreamLostError,
 )
 
 from .config import CURRENT_CONFIG
 from .exceptions import NotAuthenticatedError
 
-LOGGER = logging.getLogger('quickmq')
+LOGGER = logging.getLogger("quickmq")
 
 
 class ServerConnection(threading.Thread):
     def __init__(
         self,
         host: str,
         port: Optional[int] = None,
@@ -77,28 +77,28 @@
     @property
     def connected(self) -> bool:
         return self._running and not self._connection.is_closed
 
     @contextmanager
     def wrapper(self):
         if not self._running:
-            LOGGER.error(f'Connection to {self.server} closed')
+            LOGGER.error(f"Connection to {self.server} closed")
             raise ConnectionAbortedError(f"Connection to {self.server} closed")
         try:
             yield
         finally:
             if self._channel.is_closed or self._confirmed_channel.is_closed:
-                LOGGER.info(f'Re-establishing channels on connection to {self.server}')
+                LOGGER.info(f"Re-establishing channels on connection to {self.server}")
                 self._channel_setup()
 
     def run(self) -> None:
         self._running = True
         while self._running:
             try:
-                self._connection.process_data_events(.005)
+                self._connection.process_data_events(0.005)
             except (
                 StreamLostError,
                 AMQPConnectionError,
                 ConnectionError,
                 ConnectionClosed,
             ) as e:
                 self._on_connection_error(e)
@@ -138,36 +138,38 @@
             )
         LOGGER.info(f"Connection established to {self.server}")
 
     def _close(self) -> None:
         self._connection.process_data_events()
         if self._connection is not None and self._connection.is_open:
             self._connection.close()
-        LOGGER.info(f'Closed connection to {self.server}')
+        LOGGER.info(f"Closed connection to {self.server}")
 
     def close(self) -> None:
         LOGGER.info(f"Closing connection to {self.server}")
         self._running = False
         if self._connection is None or self._connection.is_closed:
-            LOGGER.info(f'Closed connection to {self.server}')
+            LOGGER.info(f"Closed connection to {self.server}")
             return
         self.add_callback(self._close)
 
     def _channel_setup(self) -> None:
         if self._channel is None or self._channel.is_closed:
             self._channel = self._connection.channel()
         if self._confirmed_channel is None or self._confirmed_channel.is_closed:
             self._confirmed_channel = self._connection.channel()
             self._confirmed_channel.confirm_delivery()
 
     def add_callback(self, callback: Callable, *args, **kwargs) -> None:
         LOGGER.debug(
             f"Adding callback on {self.server}: {callback}, args: {args}, kwargs: {kwargs}"
         )
-        LOGGER.debug(f'Currently {self._callback_queue.qsize()} callbacks in queue for {self.server}')
+        LOGGER.debug(
+            f"Currently {self._callback_queue.qsize()} callbacks in queue for {self.server}"
+        )
         self._callback_queue.put((callback, args, kwargs))
 
     def __del__(self) -> None:
         self.close()
         del self._connection
 
     def __eq__(self, _obj: Any) -> bool:
@@ -175,18 +177,18 @@
             return _obj == self.server
         return super().__eq__(_obj)
 
     def __hash__(self) -> int:
         return id(self)
 
     def __str__(self) -> str:
-        return f'Connection to {self.server}'
+        return f"Connection to {self.server}"
 
     def __repr__(self) -> str:
-        return f'<ServerConnection({self.server}, {self.user}, {self.port}, {self.vhost}, connected?{self.connected})>'
+        return f"<ServerConnection({self.server}, {self.user}, {self.port}, {self.vhost}, connected?{self.connected})>"
 
 
 class ReconnectConnection(ServerConnection):
     def __init__(
         self,
         host: str,
         port: Optional[int] = None,
@@ -208,15 +210,15 @@
         self.wait_for_reconnect()
         return super().close()
 
     def _on_connection_error(self, exception: BaseException) -> None:
         self.__reconnect()
 
     def __reconnect(self) -> None:
-        LOGGER.info(f'Attempting reconnect to {self.server}')
+        LOGGER.info(f"Attempting reconnect to {self.server}")
         self._reconnecting.clear()
         tries = CURRENT_CONFIG.get("RECONNECT_TRIES")
         while self._running:
             if tries == 0:
                 self._reconnecting.set()
                 self.close()
                 LOGGER.critical(
@@ -238,20 +240,20 @@
                     f"Waiting {CURRENT_CONFIG.get('RECONNECT_DELAY')} seconds before next reconnect attempt"
                 )
                 time.sleep(CURRENT_CONFIG.get("RECONNECT_DELAY"))
             if tries < 0:
                 continue
             tries -= 1
             LOGGER.debug(f"{tries} more reconnect attempts")
-        LOGGER.info(f'Reconnect finished to {self.server}')
+        LOGGER.info(f"Reconnect finished to {self.server}")
         self._reconnecting.set()
 
     def wait_for_reconnect(self, timeout=None) -> bool:
         self._reconnecting.wait(timeout=timeout)
-        LOGGER.info(f'Connection to {self.server} reconnecting? {self.is_reconnecting}')
+        LOGGER.info(f"Connection to {self.server} reconnecting? {self.is_reconnecting}")
         return self.is_reconnecting
 
 
 class ConnectionPool:
     def __init__(self) -> None:
         self._connections: List[ServerConnection] = []
```

### Comparing `QuickMQ-0.8.0/src/quickmq/message.py` & `QuickMQ-0.8.1/src/quickmq/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     def __init__(self, message: Any) -> None:
         self._message = message
 
     def encode(self) -> bytes:
         if isinstance(self._message, bytes):
             return self._message
         try:
-            return bytes(json.dumps(self._message), encoding='utf-8')
+            return bytes(json.dumps(self._message), encoding="utf-8")
         except (TypeError, ValueError):
             raise EncodingError(f"Could not encode the message {self._message}")
 
     def decode(self) -> Any:
         return json.loads(self._message)
 
     def __str__(self) -> str:
         return f"Message: {self._message}"
 
     def __repr__(self) -> str:
-        return f'<Message: {self._message}>'
+        return f"<Message: {self._message}>"
 
 
 @dataclass
 class Packet:
     message: Message
     routing_key: str
     exchange: str
```

### Comparing `QuickMQ-0.8.0/src/quickmq/publish.py` & `QuickMQ-0.8.1/src/quickmq/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from quickmq.connection import ConnectionPool, ServerConnection
 
 from .message import Packet
 
 # Possible problem with lock when publishing to multiple servers
 
-LOGGER = logging.getLogger('quickmq')
+LOGGER = logging.getLogger("quickmq")
 
 
 class AmqpPublisher:
     def __init__(self) -> None:
         self._publishing = threading.Event()
         self._publishing.set()  # not publishing, don't want threads to block
         self._publishing_err: Optional[Exception] = None
```

### Comparing `QuickMQ-0.8.0/src/quickmq/session.py` & `QuickMQ-0.8.1/src/quickmq/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .publish import AmqpPublisher
 from .exceptions import NotAuthenticatedError, NotConnectedError
 from .connection import ConnectionPool
 from .message import Packet, Message
 from .config import CURRENT_CONFIG
 
-LOGGER = logging.getLogger('quickmq')
+LOGGER = logging.getLogger("quickmq")
 
 
 class AmqpSession:
     def __init__(self) -> None:
         self._connections = ConnectionPool()
         self._publisher = AmqpPublisher()
 
@@ -27,15 +27,14 @@
     def servers(self) -> List[str]:
         return [con.server for con in self._connections]
 
     @property
     def pool(self) -> ConnectionPool:
         return self._connections
 
-    @staticmethod
     def connection_required(func: Callable) -> Callable:
         @wraps(func)
         def check_conn(self, *args: Any, **kwargs: Any) -> Any:
             if len(self.servers) > 0:
                 return func(self, *args, **kwargs)
 
             try:
@@ -65,15 +64,15 @@
             confirm=confirm_delivery,
         )
         self._publisher.publish_to_pool(self._connections, pckt)
 
     @connection_required
     def publish_all(
         self,
-        messages: Iterable[Union[str, Tuple[str, Any]]],
+        messages: Iterable[Union[Any, Tuple[str, Any]]],
         exchange: Optional[str] = None,
         confirm_delivery=True,
     ):
         for val in messages:
             key = None
             msg = None
             if type(val) is tuple:
```

### Comparing `QuickMQ-0.8.0/test/test_api.py` & `QuickMQ-0.8.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/test/test_cli.py` & `QuickMQ-0.8.1/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     info = subprocess.run(['quickmq'], capture_output=True)
     assert 'usage' in str(info.stdout, encoding='utf-8')
 
 
 @pytest.mark.parametrize('exchange', ['amq.fanout'])
 def test_publish(create_listener):
     subprocess.run(['quickmq', 'publish', '-s=localhost', '-e=amq.fanout', '-m=Hello'])
-    rcvd_bytes = create_listener.get_message(block=False)
+    rcvd_bytes = create_listener.get_message(block=True)
     assert loads(rcvd_bytes) == 'Hello'
 
 
 @pytest.mark.parametrize('exchange', ['amq.fanout'])
 def test_publish_from_stdin(create_listener):
     proc = subprocess.Popen(['quickmq', 'publish', '-s=localhost', '-e=amq.fanout'], stdin=subprocess.PIPE)
     try:
```

### Comparing `QuickMQ-0.8.0/test/test_config.py` & `QuickMQ-0.8.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/test/test_connection.py` & `QuickMQ-0.8.1/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/test/test_message.py` & `QuickMQ-0.8.1/test/test_message.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.0/test/test_session.py` & `QuickMQ-0.8.1/test/test_session.py`

 * *Files identical despite different names*

