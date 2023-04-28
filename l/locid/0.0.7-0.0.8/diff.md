# Comparing `tmp/locid-0.0.7.tar.gz` & `tmp/locid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locid-0.0.7.tar", last modified: Fri Apr 28 05:45:38 2023, max compression
+gzip compressed data, was "locid-0.0.8.tar", last modified: Fri Apr 28 11:00:41 2023, max compression
```

## Comparing `locid-0.0.7.tar` & `locid-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bahum      (501) staff       (20)        0 2023-04-28 05:45:38.583863 locid-0.0.7/
--rw-r--r--   0 bahum      (501) staff       (20)     1514 2022-02-26 13:12:03.000000 locid-0.0.7/LICENSE
--rw-r--r--   0 bahum      (501) staff       (20)      442 2023-04-28 05:45:38.584064 locid-0.0.7/PKG-INFO
--rw-r--r--   0 bahum      (501) staff       (20)     1453 2023-03-09 13:18:01.000000 locid-0.0.7/README.md
-drwxr-xr-x   0 bahum      (501) staff       (20)        0 2023-04-28 05:45:38.577795 locid-0.0.7/locid/
--rw-r--r--   0 bahum      (501) staff       (20)       16 2023-04-28 05:45:24.000000 locid-0.0.7/locid/__init__.py
--rw-r--r--   0 bahum      (501) staff       (20)    11242 2023-03-09 13:18:01.000000 locid-0.0.7/locid/ble.py
--rwxr-xr-x   0 bahum      (501) staff       (20)     3953 2023-04-28 05:42:08.000000 locid-0.0.7/locid/cli.py
--rw-r--r--   0 bahum      (501) staff       (20)     3528 2023-03-09 13:18:01.000000 locid-0.0.7/locid/json_rpc_io.py
--rwxr-xr-x   0 bahum      (501) staff       (20)     9320 2023-04-28 04:28:55.000000 locid-0.0.7/locid/locid.py
--rw-r--r--   0 bahum      (501) staff       (20)     4001 2023-01-24 15:13:42.000000 locid-0.0.7/locid/locid_jsonrpc_proto_async.py
--rw-r--r--   0 bahum      (501) staff       (20)     3397 2023-04-28 04:41:16.000000 locid-0.0.7/locid/locid_jsonrpc_proto_sync.py
--rwxr-xr-x   0 bahum      (501) staff       (20)     4000 2023-03-09 15:36:20.000000 locid-0.0.7/locid/rtb_serial_protocol.py
-drwxr-xr-x   0 bahum      (501) staff       (20)        0 2023-04-28 05:45:38.583391 locid-0.0.7/locid.egg-info/
--rw-r--r--   0 bahum      (501) staff       (20)      442 2023-04-28 05:45:38.000000 locid-0.0.7/locid.egg-info/PKG-INFO
--rw-r--r--   0 bahum      (501) staff       (20)      390 2023-04-28 05:45:38.000000 locid-0.0.7/locid.egg-info/SOURCES.txt
--rw-r--r--   0 bahum      (501) staff       (20)        1 2023-04-28 05:45:38.000000 locid-0.0.7/locid.egg-info/dependency_links.txt
--rw-r--r--   0 bahum      (501) staff       (20)       41 2023-04-28 05:45:38.000000 locid-0.0.7/locid.egg-info/entry_points.txt
--rw-r--r--   0 bahum      (501) staff       (20)       15 2023-04-28 05:45:38.000000 locid-0.0.7/locid.egg-info/requires.txt
--rw-r--r--   0 bahum      (501) staff       (20)        6 2023-04-28 05:45:38.000000 locid-0.0.7/locid.egg-info/top_level.txt
--rw-r--r--   0 bahum      (501) staff       (20)      588 2023-04-28 05:45:38.585189 locid-0.0.7/setup.cfg
--rw-r--r--   0 bahum      (501) staff       (20)       94 2023-01-21 08:01:26.000000 locid-0.0.7/setup.py
+drwxr-xr-x   0 bahum      (501) staff       (20)        0 2023-04-28 11:00:41.583057 locid-0.0.8/
+-rw-r--r--   0 bahum      (501) staff       (20)     1514 2022-02-26 13:12:03.000000 locid-0.0.8/LICENSE
+-rw-r--r--   0 bahum      (501) staff       (20)      442 2023-04-28 11:00:41.583255 locid-0.0.8/PKG-INFO
+-rw-r--r--   0 bahum      (501) staff       (20)     1821 2023-04-28 07:46:32.000000 locid-0.0.8/README.md
+drwxr-xr-x   0 bahum      (501) staff       (20)        0 2023-04-28 11:00:41.578831 locid-0.0.8/locid/
+-rw-r--r--   0 bahum      (501) staff       (20)       16 2023-04-28 07:41:19.000000 locid-0.0.8/locid/__init__.py
+-rw-r--r--   0 bahum      (501) staff       (20)    11242 2023-03-09 13:18:01.000000 locid-0.0.8/locid/ble.py
+-rwxr-xr-x   0 bahum      (501) staff       (20)     3953 2023-04-28 05:42:08.000000 locid-0.0.8/locid/cli.py
+-rw-r--r--   0 bahum      (501) staff       (20)     3528 2023-03-09 13:18:01.000000 locid-0.0.8/locid/json_rpc_io.py
+-rwxr-xr-x   0 bahum      (501) staff       (20)     9687 2023-04-28 10:59:08.000000 locid-0.0.8/locid/locid.py
+-rw-r--r--   0 bahum      (501) staff       (20)     4001 2023-01-24 15:13:42.000000 locid-0.0.8/locid/locid_jsonrpc_proto_async.py
+-rw-r--r--   0 bahum      (501) staff       (20)     3397 2023-04-28 04:41:16.000000 locid-0.0.8/locid/locid_jsonrpc_proto_sync.py
+-rwxr-xr-x   0 bahum      (501) staff       (20)     4000 2023-03-09 15:36:20.000000 locid-0.0.8/locid/rtb_serial_protocol.py
+drwxr-xr-x   0 bahum      (501) staff       (20)        0 2023-04-28 11:00:41.582637 locid-0.0.8/locid.egg-info/
+-rw-r--r--   0 bahum      (501) staff       (20)      442 2023-04-28 11:00:41.000000 locid-0.0.8/locid.egg-info/PKG-INFO
+-rw-r--r--   0 bahum      (501) staff       (20)      390 2023-04-28 11:00:41.000000 locid-0.0.8/locid.egg-info/SOURCES.txt
+-rw-r--r--   0 bahum      (501) staff       (20)        1 2023-04-28 11:00:41.000000 locid-0.0.8/locid.egg-info/dependency_links.txt
+-rw-r--r--   0 bahum      (501) staff       (20)       41 2023-04-28 11:00:41.000000 locid-0.0.8/locid.egg-info/entry_points.txt
+-rw-r--r--   0 bahum      (501) staff       (20)       15 2023-04-28 11:00:41.000000 locid-0.0.8/locid.egg-info/requires.txt
+-rw-r--r--   0 bahum      (501) staff       (20)        6 2023-04-28 11:00:41.000000 locid-0.0.8/locid.egg-info/top_level.txt
+-rw-r--r--   0 bahum      (501) staff       (20)      588 2023-04-28 11:00:41.584068 locid-0.0.8/setup.cfg
+-rw-r--r--   0 bahum      (501) staff       (20)       94 2023-01-21 08:01:26.000000 locid-0.0.8/setup.py
```

### Comparing `locid-0.0.7/LICENSE` & `locid-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/README.md` & `locid-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # LOC.id Python bindings
 
 Library for interacting with locid devices over serial adapters (/LOC.id USB-dongles) and bluetooth.
 
-(Note: A public (stripped down version) fork for customers is available at [locid-py-pub](https://git.rtb-bl.de/ampel/locid/locid-py))
-
 ## Installation
 
-**Directly from git**
+**Directly from GitLab (master)**
+
+```shell
+pip install git+ssh://git@git.rtb-bl.de/ampel/locid/locid-py.git
+```
+
+**Pypi**
 
 ```shell
-pip install git+https://git.rtb-bl.de/ampel/locid/locid-py.git
+pip install locid
 ```
 
+_(Deployed from time to time for customers / third party integrations, see [pypi locid](https://pypi.org/project/locid/#history))_.
+
 ## Command line utility
 
 When installed via pip, locid-py installs a little command line utilty. 
 
 Execute `locid -h` for a list of supported commands.
 
 ## Usage / Examples
 
-- [(USB-)Serial/UART Example](/example.py) (Nordic USB-Dongle)
-- [Bluetooth Example](/example_bluetooth.py) (Regular Bluetooth Adapter / HCI)
+- [(USB-)Serial/UART Example](/example_locid_dongle.py) (Nordic USB-Dongle)
+- [Bluetooth Example](/example_bluetooth_hci.py) (Regular Bluetooth Adapter / HCI)
 
 ## Integration
 
 ### As a git submodule
 
 To integrate locid-py directly in your project, navigate to the directory or your project's python scripts and execute:
 
@@ -33,36 +39,37 @@
 git submodule add git@git.rtb-bl.de:ampel/locid/locid-py.git
 ```
 
 Inside your scripts, you can include the library as follows:
 
 ```python
 import sys
+import os
 
 # add locid python bindings from subdirectory
-sys.path.insert(0, "locid-py")
+sys.path.insert(0, os.path.join(os.path.dirname(__file__), "locid-py"))
 from locid.ble import *
 
 async with LocIdBleClient(BLE_MAC) as locid:
     await locid.jsonrpc_request("locid.ping")
 ```
 
 ### In requirements.txt
 
 Add in your requirements.txt
 
 ```
 pyserial
 # ...
 
-git+https://git.rtb-bl.de/ampel/locid/locid-py.git
+git+ssh://git@git.rtb-bl.de/ampel/locid/locid-py.git
 ```
 
 Then use the standard way to install your requirements:
 
 ```shell
 pip install -r requirements.txt
 ```
 
+## Firmware
 
-
-
+Firmware (for Nordic/Laird USB Dongles) is available from [LOC.id BLE Archive (master)](https://git.rtb-bl.de/ampel/locid/RTB_LOC.id/-/jobs/artifacts/master/download?job=build). Download, extract & install from `build-usb/src` folder.
```

### Comparing `locid-0.0.7/locid/ble.py` & `locid-0.0.8/locid/ble.py`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/locid/cli.py` & `locid-0.0.8/locid/cli.py`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/locid/json_rpc_io.py` & `locid-0.0.8/locid/json_rpc_io.py`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/locid/locid.py` & `locid-0.0.8/locid/locid.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self.device_port = device_port
         self.serial = None
 
         self._jsonrpc_id = 0
         self._error_callback = None
         self._status_callback = None
         self._notification_callback = None
+        self._user_action_callback = None
         self._usb_forward_callback = None
         self._user_connected_callback = None
         self._user_disconnected_callback = None
 
         self.jsonrpc_conds = dict()
         self.jsonrpc_responses = dict()
 
@@ -169,16 +170,21 @@
     def on_error(self, callback):
         self._error_callback = callback
 
     def on_client_request(self, callback):
         self._usb_forward_callback = callback
 
     def on_notification(self, callback):
+        """" Sets a (generic) notification handler """
         self._notification_callback = callback
 
+    def on_user_action(self, callback):
+        """" Sets a user action handler (e.g. handsender button press events) """
+        self._user_action_callback = callback
+
     def on_user_min_prox_changed(self, old, prox):
         logging.info("on_user_min_prox_changed", old, prox)
 
     def on_user_connected(self, user_id):
         logging.info("on_user_connected: %s", user_id)
         if self._user_connected_callback:
             self._user_connected_callback(self, user_id)
@@ -237,15 +243,15 @@
             logging.debug("<<< %s", line)
 
             j = None
             try:
                 j = json.loads(line)
             except json.decoder.JSONDecodeError as e:
                 logging.error("json dec error: %s", e)
-                print(line)
+                logging.error("in line: %s", line)
                 if self._error_callback:
                     self._error_callback(e)
                 continue
 
             # logging.debug("json: %s", j)
 
             # jsonrpc responses (and errors)
@@ -255,35 +261,37 @@
                 with cond:
                     cond.notify()
                 del self.jsonrpc_conds[j['id']]
 
             # jsonrpc notifications
             elif 'method' in j:
                 method = j['method']
+                params = j.get("params")
                 if method == 'locid.status':
                     self.handle_status_notification(j['result'])
 
-                # elif method == 'locid.user.prox_changed':
-                #     print("TODO")
-
                 elif method == 'locid.usbForward' or method == 'locid.hostForward':
                     logging.debug("locid.usbForward: %s", j)
 
                     data = j.get("params", {}).get("data")
                     if data is None:
                         logging.error("missing data arg")
                     else:
                         if self._usb_forward_callback:
                             self._usb_forward_callback(data)
 
-                else:
-                    if self._notification_callback:
-                        self._notification_callback(j)
-                    else:
-                        logger.warning("Unhandled notification (set notification_callback property to handle): %s", j)
+                if self._notification_callback:
+                    self._notification_callback(j)
+
+                if method == 'locid.user.action' and self._user_action_callback is not None:
+                    action_id = params['action_id']
+                    self._user_action_callback(action_id, params)
+
+                # elif method == 'locid.user.prox_changed':
+                #     print("TODO")
 
         logging.debug("thread exit")
 
 
 class LocIdUSBDongle(LocIdSerialTransportThread, LocIdJsonRpcProtocol):
 
     @classmethod
```

### Comparing `locid-0.0.7/locid/locid_jsonrpc_proto_async.py` & `locid-0.0.8/locid/locid_jsonrpc_proto_async.py`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/locid/locid_jsonrpc_proto_sync.py` & `locid-0.0.8/locid/locid_jsonrpc_proto_sync.py`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/locid/rtb_serial_protocol.py` & `locid-0.0.8/locid/rtb_serial_protocol.py`

 * *Files identical despite different names*

### Comparing `locid-0.0.7/setup.cfg` & `locid-0.0.8/setup.cfg`

 * *Files identical despite different names*

