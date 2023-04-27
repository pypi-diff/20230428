# Comparing `tmp/ovos-bus-client-0.0.4a4.tar.gz` & `tmp/ovos-bus-client-0.0.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.4a4.tar", last modified: Thu Apr 27 21:10:52 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.4a5.tar", last modified: Thu Apr 27 21:59:42 2023, max compression
```

## Comparing `ovos-bus-client-0.0.4a4.tar` & `ovos-bus-client-0.0.4a5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 21:59:42.000000 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 21:59:42.000000 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:59:42.000000 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 21:59:42.000000 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 21:59:42.000000 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 21:59:42.000000 ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:59:42.470889 ovos-bus-client-0.0.4a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-27 21:59:41.000000 ovos-bus-client-0.0.4a5/setup.py
```

### Comparing `ovos-bus-client-0.0.4a4/LICENSE.md` & `ovos-bus-client-0.0.4a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/PKG-INFO` & `ovos-bus-client-0.0.4a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a4
+Version: 0.0.4a5
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import time
 import traceback
+from os import getpid
 from threading import Event, Thread
 from uuid import uuid4
 
 from ovos_utils.log import LOG
 from pyee import ExecutorEventEmitter
 from websocket import (WebSocketApp,
                        WebSocketConnectionClosedException,
                        WebSocketException)
 
 from ovos_bus_client.client.collector import MessageCollector
 from ovos_bus_client.client.waiter import MessageWaiter
+from ovos_bus_client.conf import load_message_bus_config, MessageBusClientConf, load_gui_message_bus_config
 from ovos_bus_client.message import Message, CollectionMessage, GUIMessage
 from ovos_bus_client.session import SessionManager, Session
 from ovos_bus_client.util import create_echo_function
-from ovos_bus_client.conf import load_message_bus_config, MessageBusClientConf, load_gui_message_bus_config
-
 
 try:
     from mycroft_bus_client import MessageBusClient as _MessageBusClientBase
 except ImportError:
     # TODO - code in the wild does isinstance checks
     # this conditional subclassing should be removed ASAP, it is only here for the migration period
     # mycroft_bus_client is abandonware until further notice from MycroftAI
@@ -339,15 +339,16 @@
         t.start()
         return t
 
 
 class GUIWebsocketClient(MessageBusClient):
 
     def __init__(self, host=None, port=None, route=None, ssl=None,
-                 emitter=None, cache=False):
+                 emitter=None, cache=False, client_name="ovos-gui-client"):
+        self.gui_id = f"{client_name}_{getpid()}"
         config_overrides = dict(host=host, port=port, route=route, ssl=ssl)
         config = load_gui_message_bus_config(**config_overrides)
         super().__init__(host=config.host, port=config.port, route=config.route,
                          ssl=config.ssl, emitter=emitter, cache=cache)
 
     def emit(self, message):
         """Send a message onto the message bus.
@@ -370,14 +371,19 @@
                 self.client.send(message.serialize())
             else:
                 self.client.send(json.dumps(message.__dict__))
         except WebSocketConnectionClosedException:
             LOG.warning('Could not send %s message because connection '
                         'has been closed', message.msg_type)
 
+    def on_open(self, *args):
+        super().on_open(*args)
+        self.emit(GUIMessage("mycroft.gui.connected",
+                             gui_id=self.gui_id))
+
     def on_message(self, *args):
         """Handle incoming websocket message.
 
         Args:
             message (str): GUI protocol bus message
         """
         if len(args) == 1:
```

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/message.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/message.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/session.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/session.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.4a5/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a4
+Version: 0.0.4a5
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.4a5/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a4/setup.py` & `ovos-bus-client-0.0.4a5/setup.py`

 * *Files identical despite different names*

