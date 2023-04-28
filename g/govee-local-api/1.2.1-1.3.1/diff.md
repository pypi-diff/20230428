# Comparing `tmp/govee-local-api-1.2.1.tar.gz` & `tmp/govee-local-api-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govee-local-api-1.2.1.tar", last modified: Tue Feb  7 21:56:27 2023, max compression
+gzip compressed data, was "govee-local-api-1.3.1.tar", last modified: Fri Apr 28 05:42:19 2023, max compression
```

## Comparing `govee-local-api-1.2.1.tar` & `govee-local-api-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/src/govee_local_api/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/src/govee_local_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/src/govee_local_api/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/src/govee_local_api/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/src/govee_local_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/src/govee_local_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-07 21:56:27.000000 govee-local-api-1.2.1/src/govee_local_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-02-07 21:56:27.000000 govee-local-api-1.2.1/src/govee_local_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:56:27.000000 govee-local-api-1.2.1/src/govee_local_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-07 21:56:27.000000 govee-local-api-1.2.1/src/govee_local_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:56:27.830278 govee-local-api-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-02-07 21:56:15.000000 govee-local-api-1.2.1/tests/test_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 05:42:19.096511 govee-local-api-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-28 05:42:19.096511 govee-local-api-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 05:42:19.096511 govee-local-api-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 05:42:19.092511 govee-local-api-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 05:42:19.096511 govee-local-api-1.3.1/src/govee_local_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/src/govee_local_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/src/govee_local_api/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/src/govee_local_api/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/src/govee_local_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 05:42:19.096511 govee-local-api-1.3.1/src/govee_local_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-28 05:42:19.000000 govee-local-api-1.3.1/src/govee_local_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 05:42:19.000000 govee-local-api-1.3.1/src/govee_local_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 05:42:19.000000 govee-local-api-1.3.1/src/govee_local_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 05:42:19.000000 govee-local-api-1.3.1/src/govee_local_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 05:42:19.096511 govee-local-api-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-28 05:42:05.000000 govee-local-api-1.3.1/tests/test_message.py
```

### Comparing `govee-local-api-1.2.1/LICENSE` & `govee-local-api-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `govee-local-api-1.2.1/PKG-INFO` & `govee-local-api-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govee-local-api
-Version: 1.2.1
+Version: 1.3.1
 Summary: Library to comunicate with Govee local API
 Home-page: 
 Author: "Galorhallen"
 Author-email: Galorhallen <andrea.ponte1987@gmail.com>
 Project-URL: Homepage, https://github.com/Galorhallen/govee-local-api
 Project-URL: Bug Tracker, https://github.com/Galorhallen/govee-local-api/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `govee-local-api-1.2.1/pyproject.toml` & `govee-local-api-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "govee-local-api"
-version = "1.2.1"
+dynamic = ["version"]
+
 authors = [
   { name="Galorhallen", email="andrea.ponte1987@gmail.com" },
 ]
 description = "Library to comunicate with Govee local API"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: OS Independent", 
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Galorhallen/govee-local-api"
 "Bug Tracker" = "https://github.com/Galorhallen/govee-local-api/issues"
 
 [tool.black]
 target-version = ["py310"]
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 addopts = [
     "--import-mode=importlib",
-]
+]
+
+[tool.setuptools.dynamic]
+version = {attr = "govee_local_api.__version__"}
```

### Comparing `govee-local-api-1.2.1/setup.cfg` & `govee-local-api-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `govee-local-api-1.2.1/src/govee_local_api/controller.py` & `govee-local-api-1.3.1/src/govee_local_api/controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,50 +22,52 @@
 
 BROADCAST_ADDRESS = "239.255.255.250"
 BROADCAST_PORT = 4001
 LISTENING_PORT = 4002
 COMMAND_PORT = 4003
 
 DISCOVERY_INTERVAL = 10
-EVICTION_INTERVAL = DISCOVERY_INTERVAL * 3
+EVICT_INTERVAL = DISCOVERY_INTERVAL * 3
 UPDATE_INTERVAL = 5
 
 
 class GoveeController:
     def __init__(
         self,
         loop=None,
         broadcast_address: str = BROADCAST_ADDRESS,
         broadcast_port: int = BROADCAST_PORT,
         listening_address: str = "0.0.0.0",
         listening_port: int = LISTENING_PORT,
         device_command_port: int = COMMAND_PORT,
-        discovery: bool = False,
+        discovery_enabled: bool = False,
         discovery_interval: int = DISCOVERY_INTERVAL,
-        eviction_interval: int = EVICTION_INTERVAL,
-        autoupdate: bool = True,
-        autoupdate_interval: int = UPDATE_INTERVAL,
-        discovered_callback: Callable[[GoveeDevice, bool], True] = None,
+        evict_enabled: bool = False,
+        evict_interval: int = EVICT_INTERVAL,
+        update_enabled: bool = True,
+        update_interval: int = UPDATE_INTERVAL,
+        discovered_callback: Callable[[GoveeDevice, bool], bool] = None,
         evicted_callback: Callable[[GoveeDevice], None] = None,
         logger: logging.Logger = None,
     ) -> None:
         """Build a controller that handle Govee devices that support local API on local network.
 
         Args:
             loop: The asyncio event loop. If None the loop is retreived by calling ``asyncio.get_running_loop()``
             broadcast_address (str): The multicast address to use to send discovery messages. Default: 239.255.255.250
             broadcast_port (int): Devices port where discovery messages are sent. Default: 4001
             listening_port (int): Local UDP port on which the controller listen for incoming devices' messages
             device_command_port (int): The devices' port where the commands should be sent
-            discovery (bool): If true a discovery message is sent every ``discovery_interval`` seconds. Default: False
+            discovery_enabled (bool): If true a discovery message is sent every ``discovery_interval`` seconds. Default: False
             discovery_interval (int): Interval between discovery messages (if discovery is enabled). Default: 10 seconds
-            eviction_interval (int): Interval after which a device is evicted. Default 30 seconds
-            autoupdate (bool): If true the devices status is updated automatically every ``autoupdate_interval`` seconds. A successful device update reset the eviction timer for the device. Default: True
-            autoupdate_interval (int): Interval between a status update is requested to devices.
-            discovery_callback (Callable[GoveeDevice, bool]): An optional function to call when a device is discovered (or rediscovered). Default None
+            evict_enabled (bool): If true the controller automatically remove devices not seen for ``evict_interval`` seconds (requires discovery to be enabled)
+            evict_interval (int): Interval after which a device is evicted. Default 30 seconds
+            update_enabled (bool): If true the devices status is updated automatically every ``update_interval`` seconds. A successful device update reset the eviction timer for the device. Default: True
+            update_interval (int): Interval between a status update is requested to devices.
+            discovered_callback (Callable[GoveeDevice, bool]): An optional function to call when a device is discovered (or rediscovered). Default None
             evicted_callback (Callable[GoveeDevice]): An optional function to call when a device is evicted.
         """
 
         self._transport = None
         self._protocol = None
         self._broadcast_address = broadcast_address
         self._broadcast_port = broadcast_port
@@ -73,101 +75,130 @@
         self._listening_port = listening_port
         self._device_command_port = device_command_port
 
         self._loop = loop or asyncio.get_running_loop()
         self._message_factory = MessageResponseFactory()
         self._devices: dict[str, GoveeDevice] = {}
 
-        self._discovery = discovery
+        self._discovery_enabled = discovery_enabled
         self._discovery_interval = discovery_interval
-        self._autoupdate = autoupdate
-        self._autoupdate_interval = autoupdate_interval
-        self._eviction_interval = eviction_interval
+        self._update_enabled = update_enabled
+        self._update_interval = update_interval
+        self._evict_enabled = evict_enabled
+        self._evict_interval = evict_interval
 
         self._device_discovered_callback = discovered_callback
         self._device_evicted_callback = evicted_callback
 
         self._logger = logger or logging.getLogger(__name__)
 
         self._discovery_handle: asyncio.TimerHandle = None
         self._update_handle: asyncio.TimerHandle = None
 
     async def start(self):
         self._transport, self._protocol = await self._loop.create_datagram_endpoint(
             lambda: self, local_addr=(self._listening_address, self._listening_port)
         )
 
-        if self._discovery:
+        if self._discovery_enabled:
             self.send_discovery_message()
-        if self._autoupdate:
+        if self._update_enabled:
             self.send_update_message()
 
     def clenaup(self):
-        self.set_autoupdate(False)
-        self.set_discovery(False)
+        self.set_update_enabled(False)
+        self.set_discovery_enabled(False)
 
         if self._transport:
             self._transport.close()
         self._devices.clear()
 
     def add_device(self, ip: str, sku: str, fingerprint: str = None) -> None:
         device: GoveeDevice = GoveeDevice(self, ip, fingerprint, sku)
-        self._devices[ip] = device
+        self._devices[fingerprint] = device
 
-    def set_discovery(self, enabled: bool) -> None:
-        self._discovery = enabled
+    def remove_device(self, device: str | GoveeDevice) -> None:
+        if isinstance(device, GoveeDevice):
+            device = device.fingerprint
+        if device in self._devices:
+            del self._devices[device]
+
+    @property
+    def evict_enabled(self) -> bool:
+        return self._evict_enabled
+
+    def set_evict_enabled(self, enabled: bool) -> None:
+        self._evict_enabled = enabled
+
+    def set_discovery_enabled(self, enabled: bool) -> None:
+        if self._discovery_enabled == enabled:
+            return
+        self._discovery_enabled = enabled
         if enabled:
             self.send_discovery_message()
         elif self._discovery_handle:
             self._discovery_handle.cancel()
             self._discovery_handle = None
 
     @property
     def discovery(self) -> bool:
-        return self._discovery
+        return self._discovery_enabled
 
     def set_discovery_interval(self, interval: int) -> None:
         self._discovery_interval = interval
 
     @property
     def discovery_interval(self) -> int:
         return self._discovery_interval
 
-    def set_autoupdate(self, enabled: bool) -> None:
-        self._autoupdate = enabled
+    def set_device_discovered_callback(
+        self, callback: Callable[[GoveeDevice, bool], bool] | None
+    ) -> Callable[[GoveeDevice, bool], bool] | None:
+        old_callback = self._device_discovered_callback
+        self._device_discovered_callback = callback
+        return old_callback
+
+    def set_update_enabled(self, enabled: bool) -> None:
+        if self._update_enabled == enabled:
+            return
+        self._update_enabled = enabled
         if enabled:
             self.send_update_message()
         elif self._update_handle:
             self._update_handle.cancel()
             self._update_handle = None
 
     @property
-    def autoupdate(self) -> bool:
-        return self._autoupdate
+    def update_enabled(self) -> bool:
+        return self._update_enabled
 
     def send_discovery_message(self):
         message: ScanMessage = ScanMessage()
-        self._transport.sendto(
-            bytes(message), (self._broadcast_address, self._broadcast_port)
-        )
-
-        if self._discovery:
-            self._discovery_handler = self._loop.call_later(
-                self._discovery_interval, self.send_discovery_message
+        if self._transport:
+            self._transport.sendto(
+                bytes(message), (self._broadcast_address, self._broadcast_port)
             )
 
+            if self._discovery_enabled:
+                self._discovery_handle = self._loop.call_later(
+                    self._discovery_interval, self.send_discovery_message
+                )
+
     def send_update_message(self, device: GoveeDevice = None):
-        if device:
-            self._send_update_message(device=device)
-        else:
-            for d in self._devices.values():
-                self._send_update_message(device=d)
+        if self._transport:
+            if device:
+                self._send_update_message(device=device)
+            else:
+                for d in self._devices.values():
+                    self._send_update_message(device=d)
 
-        if self._autoupdate:
-            self._loop.call_later(self._autoupdate_interval, self.send_update_message)
+            if self._update_enabled:
+                self._update_handle = self._loop.call_later(
+                    self._update_interval, self.send_update_message
+                )
 
     async def turn_on_off(self, device: GoveeDevice, status: bool) -> None:
         self._send_message(OnOffMessage(status), device)
 
     async def set_brightness(self, device: GoveeDevice, brightness: int) -> None:
         self._send_message(BrightnessMessage(brightness), device)
 
@@ -176,26 +207,27 @@
     ) -> None:
         if rgb:
             self._send_message(ColorMessage(rgb=rgb, temperature=None), device)
         else:
             self._send_message(ColorMessage(rgb=None, temperature=temperature), device)
 
     def get_device_by_ip(self, ip: str) -> GoveeDevice | None:
-        return self._devices.get(ip, None)
+        return next(
+            (device for device in self._devices.values() if device.ip == ip),
+            None,
+        )
 
     def get_device_by_sku(self, sku: str) -> GoveeDevice | None:
-        return next(device for device in self._devices.values() if device.sku == sku)
-
-    def get_device_by_fingerprint(self, fingerprint: str) -> GoveeDevice | None:
         return next(
-            device
-            for device in self._devices.values()
-            if device.fingerprint == fingerprint
+            (device for device in self._devices.values() if device.sku == sku), None
         )
 
+    def get_device_by_fingerprint(self, fingerprint: str) -> GoveeDevice | None:
+        return self._devices.get(fingerprint, None)
+
     @property
     def devices(self) -> list(GoveeDevice):
         return list(self._devices.values())
 
     def connection_made(self, transport):
         self._transport = transport
 
@@ -232,45 +264,48 @@
     def _handle_status_update_response(self, message: StatusResponse, addr):
         ip = addr[0]
         device = self.get_device_by_ip(ip)
         if device:
             device.update(message)
 
     async def _handle_scan_response(self, message: ScanResponse) -> None:
-        ip = message.ip
-        device = self._devices.get(ip, None)
+        fingerprint = message.device
+        device = self.get_device_by_fingerprint(fingerprint)
         is_new = device is None
 
         if is_new:
-            device = GoveeDevice(self, ip, message.device, message.sku)
+            device = GoveeDevice(self, message.ip, fingerprint, message.sku)
             if self._call_discovered_callback(device, True):
-                self._devices[ip] = device
+                self._devices[fingerprint] = device
                 self._logger.debug("Device discovered: %s", device)
             else:
                 self._logger.debug("Device %s ignored", device)
         else:
             if self._call_discovered_callback(device, True):
                 device.update_lastseen()
                 self._logger.debug("Device updated: %s", device)
 
-        self._evict()
+        if self._evict_enabled:
+            self._evict()
 
     def _call_discovered_callback(self, device: GoveeDevice, is_new: bool) -> bool:
         if not self._device_discovered_callback:
             return True
         return self._device_discovered_callback(device, is_new)
 
     def _send_message(self, message: GoveeMessage, device: GoveeDevice) -> None:
         self._transport.sendto(bytes(message), (device.ip, self._device_command_port))
 
     def _evict(self):
         now = datetime.now()
-        for ip, device in self._devices.items():
+        devices = dict(self._devices)
+        for fingerprint, device in devices.items():
             diff: timedelta = now - device.lastseen
-            if diff.total_seconds() >= self._eviction_interval:
+            if diff.total_seconds() >= self._evict_interval:
                 device._controller = None
-                del self._devices[ip]
+                del self._devices[fingerprint]
                 if self._device_evicted_callback and callable(
                     self._device_evicted_callback
                 ):
                     self._logger.debug("Device evicted: %s", device)
                     self._device_evicted_callback(device)
+        self._devices = devices
```

### Comparing `govee-local-api-1.2.1/src/govee_local_api/device.py` & `govee-local-api-1.3.1/src/govee_local_api/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Tuple
+from typing import Tuple, Any
 from datetime import datetime
 
 from .message import StatusResponse
 
 
 class GoveeDevice:
     def __init__(self, controller, ip: str, fingerprint: str, sku: str) -> None:
@@ -16,14 +16,18 @@
 
         self._is_on: bool = False
         self._rgb_color = (0, 0, 0)
         self._temperature_color = 0
         self._brightness = 0
 
     @property
+    def controller(self):
+        return self._controller
+
+    @property
     def ip(self) -> str:
         return self._ip
 
     @property
     def fingerprint(self) -> str:
         return self._fingerprint
 
@@ -49,37 +53,55 @@
 
     @property
     def temperature_color(self) -> int:
         return self._temperature_color
 
     async def turn_on(self) -> None:
         await self._controller.turn_on_off(self, True)
+        self._is_on = True
 
     async def turn_off(self) -> None:
         await self._controller.turn_on_off(self, False)
+        self._is_on = False
 
     async def set_brightness(self, value: int) -> None:
         await self._controller.set_brightness(self, value)
+        self._brightness = value
 
     async def set_rgb_color(self, red: int, green: int, blue: int) -> None:
-        await self._controller.set_color(self, rgb=(red, green, blue), temperature=None)
+        rgb = (red, green, blue)
+        await self._controller.set_color(self, rgb=rgb, temperature=None)
+        self._rgb_color = rgb
 
     async def set_temperature(self, temperature: int) -> None:
         await self._controller.set_color(self, temperature=temperature, rgb=None)
+        self._temperature_color = temperature
 
     def update(self, message: StatusResponse) -> None:
         self._is_on = message.is_on
         self._brightness = message.brightness
         self._rgb_color = message.color
         self._temperature_color = message.color_temperature
         self.update_lastseen()
 
     def update_lastseen(self) -> None:
         self._lastseen = datetime.now()
 
+    def as_dict(self) -> dict[str, Any]:
+        return {
+            "ip": self._ip,
+            "fingerprint": self._fingerprint,
+            "sku": self._sku,
+            "lastseen": self._lastseen,
+            "on": self._is_on,
+            "brightness": self._brightness,
+            "color": self._rgb_color,
+            "colorTemperature": self._temperature_color,
+        }
+
     def __str__(self) -> str:
         result = f"<GoveeDevice ip={self.ip}, fingerprint={self.fingerprint}, sku={self.sku}, lastseen={self._lastseen}, is_on={self._is_on}"
         return result + (
             f", brightness={self._brightness}, color={self._rgb_color}, temperature={self._temperature_color}>"
             if self._is_on
             else ">"
         )
```

### Comparing `govee-local-api-1.2.1/src/govee_local_api/message.py` & `govee-local-api-1.3.1/src/govee_local_api/message.py`

 * *Files identical despite different names*

### Comparing `govee-local-api-1.2.1/src/govee_local_api.egg-info/PKG-INFO` & `govee-local-api-1.3.1/src/govee_local_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govee-local-api
-Version: 1.2.1
+Version: 1.3.1
 Summary: Library to comunicate with Govee local API
 Home-page: 
 Author: "Galorhallen"
 Author-email: Galorhallen <andrea.ponte1987@gmail.com>
 Project-URL: Homepage, https://github.com/Galorhallen/govee-local-api
 Project-URL: Bug Tracker, https://github.com/Galorhallen/govee-local-api/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `govee-local-api-1.2.1/tests/test_message.py` & `govee-local-api-1.3.1/tests/test_message.py`

 * *Files identical despite different names*

