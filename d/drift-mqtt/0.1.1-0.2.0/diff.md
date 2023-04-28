# Comparing `tmp/drift_mqtt-0.1.1-py3-none-any.whl.zip` & `tmp/drift_mqtt-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9325 bytes, number of entries: 8
--rw-r--r--  2.0 unx        6 b- defN 22-Sep-27 15:01 drift_mqtt/VERSION
--rw-r--r--  2.0 unx      394 b- defN 22-Sep-27 15:01 drift_mqtt/__init__.py
--rw-r--r--  2.0 unx     4166 b- defN 22-Sep-27 15:01 drift_mqtt/client.py
--rw-r--r--  2.0 unx    16725 b- defN 22-Sep-27 15:01 drift_mqtt-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1550 b- defN 22-Sep-27 15:01 drift_mqtt-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-27 15:01 drift_mqtt-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Sep-27 15:01 drift_mqtt-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      629 b- defN 22-Sep-27 15:01 drift_mqtt-0.1.1.dist-info/RECORD
-8 files, 23573 bytes uncompressed, 8227 bytes compressed:  65.1%
+Zip file size: 9398 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-28 11:37 drift_mqtt/VERSION
+-rw-r--r--  2.0 unx      394 b- defN 23-Apr-28 11:37 drift_mqtt/__init__.py
+-rw-r--r--  2.0 unx     4142 b- defN 23-Apr-28 11:37 drift_mqtt/client.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1802 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      629 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/RECORD
+8 files, 23801 bytes uncompressed, 8300 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: drift_mqtt/__init__.py
 Comment: 
 
 Filename: drift_mqtt/client.py
 Comment: 
 
-Filename: drift_mqtt-0.1.1.dist-info/LICENSE
+Filename: drift_mqtt-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: drift_mqtt-0.1.1.dist-info/METADATA
+Filename: drift_mqtt-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: drift_mqtt-0.1.1.dist-info/WHEEL
+Filename: drift_mqtt-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: drift_mqtt-0.1.1.dist-info/top_level.txt
+Filename: drift_mqtt-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_mqtt-0.1.1.dist-info/RECORD
+Filename: drift_mqtt-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_mqtt/VERSION

```diff
@@ -1 +1 @@
-0.1.1
+0.2.0
```

## drift_mqtt/client.py

```diff
@@ -33,16 +33,17 @@
     def __init__(self, uri: str, client_id: str = "drift-mqtt-client"):
         """Init
         :param uri - <protocol>://<host>:<port>
         :param client_id - must be unique! if not - will cause disconnects
         """
         self._uri = urlparse(uri)
         self._transport = "websockets" if self._uri.scheme == "ws" else "tcp"
-        # TODO: check if we need v311 or v5 # pylint: disable=fixme
-        self._client = PahoClient(client_id=client_id, transport=self._transport)
+        self._client = PahoClient(
+            client_id=client_id, transport=self._transport, protocol=mqtt.MQTTv5
+        )
         self._client.on_connect = self.on_connect
         self._client.on_disconnect = self.on_disconnect
         self._client.on_subscribe = self.on_subscribe
         self._client.on_message = self.on_message
         self._client.reconnect_delay_set(min_delay=1, max_delay=30)
         self._client.enable_logger()
         self._subscriptions = []
```

## Comparing `drift_mqtt-0.1.1.dist-info/LICENSE` & `drift_mqtt-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `drift_mqtt-0.1.1.dist-info/METADATA` & `drift_mqtt-0.2.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-mqtt
-Version: 0.1.1
+Version: 0.2.0
 Summary: A wrapper around Python Paho Mqtt library
 Home-page: https://gitlab.panda.technology/drift/sdk/drift-mqtt
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,23 +15,35 @@
 Requires-Dist: pylint (~=2.15.3) ; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.1.3) ; extra == 'test'
 Requires-Dist: pytest-mock (~=3.8.2) ; extra == 'test'
 
 # Drift MQTT tools
 
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/panda-official/DriftMqtt/ci)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/panda-official/DriftMqtt/ci.yml?branch=develop)](https://github.com/panda-official/DriftMqtt/actions)
 ![PyPI](https://img.shields.io/pypi/v/drift-mqtt)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/drift-mqtt)
 
 
 A collection of helpers to work with MQTT:
 * `Client` - wrapper around `paho.mqtt.Client` that correctly handles subscriptions after reconnect
 
 
+## Installation
+
+```bash
+pip install drift-mqtt
+```
+
+Or get the latest version from GitHub:
+```bash
+pip install git+https://github.com/panda-official/DriftMqtt.git
+```
+
+
 ## Usage
 
 Producer
 ```python
 from drift_mqtt import Client
```

