# Comparing `tmp/azuresphere-device-api-1.0.2.tar.gz` & `tmp/azuresphere-device-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuresphere-device-api-1.0.2.tar", last modified: Thu Dec  1 09:22:19 2022, max compression
+gzip compressed data, was "azuresphere-device-api-1.1.0.tar", last modified: Fri Apr 28 03:06:42 2023, max compression
```

## Comparing `azuresphere-device-api-1.0.2.tar` & `azuresphere-device-api-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 09:22:19.607744 azuresphere-device-api-1.0.2/
--rw-rw-rw-   0        0        0     1093 2022-09-13 10:22:34.000000 azuresphere-device-api-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2397 2022-12-01 09:22:19.609800 azuresphere-device-api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1907 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-01 09:22:19.411689 azuresphere-device-api-1.0.2/azuresphere_device_api/
--rw-rw-rw-   0        0        0      176 2022-12-01 09:21:47.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/__init__.py
--rw-rw-rw-   0        0        0     3475 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/app.py
--rw-rw-rw-   0        0        0      714 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/capabilities.py
--rw-rw-rw-   0        0        0     5398 2022-09-13 10:22:34.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/certificate.py
-drwxrwxrwx   0        0        0        0 2022-12-01 09:22:19.605375 azuresphere-device-api-1.0.2/azuresphere_device_api/certs/
--rw-rw-rw-   0        0        0      826 2022-09-13 10:22:34.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/certs/device_rest_api_certificate.pem
--rw-rw-rw-   0        0        0     3557 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/device.py
--rw-rw-rw-   0        0        0     3594 2022-12-01 09:21:47.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/devices.py
--rw-rw-rw-   0        0        0    14392 2022-12-01 09:21:47.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/error_handler.py
--rw-rw-rw-   0        0        0      980 2022-09-13 10:22:34.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/exceptions.py
--rw-rw-rw-   0        0        0      545 2022-09-13 10:22:34.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/image.py
--rw-rw-rw-   0        0        0     1836 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/manufacturing.py
--rw-rw-rw-   0        0        0     8220 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/network.py
--rw-rw-rw-   0        0        0     3017 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/sideload.py
--rw-rw-rw-   0        0        0    10248 2022-09-23 15:37:46.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/utils.py
--rw-rw-rw-   0        0        0     2180 2022-11-14 16:59:37.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/validation.py
--rw-rw-rw-   0        0        0    15076 2022-11-14 16:59:37.000000 azuresphere-device-api-1.0.2/azuresphere_device_api/wifi.py
-drwxrwxrwx   0        0        0        0 2022-12-01 09:22:19.596340 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/
--rw-rw-rw-   0        0        0     2397 2022-12-01 09:22:19.000000 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2022-12-01 09:22:19.000000 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 09:22:19.000000 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-01 09:22:17.000000 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       42 2022-12-01 09:22:19.000000 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-12-01 09:22:19.000000 azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2022-09-13 10:22:34.000000 azuresphere-device-api-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      870 2022-12-01 09:22:19.626699 azuresphere-device-api-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2411 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1907 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.561559 azuresphere-device-api-1.1.0/azuresphere_device_api/
+-rw-rw-rw-   0        0        0      201 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/__init__.py
+-rw-rw-rw-   0        0        0     3475 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/app.py
+-rw-rw-rw-   0        0        0      714 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/capabilities.py
+-rw-rw-rw-   0        0        0     5398 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/certificate.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/azuresphere_device_api/certs/
+-rw-rw-rw-   0        0        0      826 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/certs/device_rest_api_certificate.pem
+-rw-rw-rw-   0        0        0     3557 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/device.py
+-rw-rw-rw-   0        0        0     3558 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/devices.py
+-rw-rw-rw-   0        0        0    14392 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/error_handler.py
+-rw-rw-rw-   0        0        0      980 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/exceptions.py
+-rw-rw-rw-   0        0        0      545 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/image.py
+-rw-rw-rw-   0        0        0     1856 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/manufacturing.py
+-rw-rw-rw-   0        0        0     8220 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/network.py
+-rw-rw-rw-   0        0        0     3017 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/sideload.py
+-rw-rw-rw-   0        0        0    11952 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/utils.py
+-rw-rw-rw-   0        0        0     2180 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/validation.py
+-rw-rw-rw-   0        0        0    15076 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/wifi.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.561559 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/
+-rw-rw-rw-   0        0        0     2411 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 03:06:28.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1129 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/setup.cfg
```

### Comparing `azuresphere-device-api-1.0.2/LICENSE.txt` & `azuresphere-device-api-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/PKG-INFO` & `azuresphere-device-api-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: azuresphere-device-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: A library for interacting with Azure Sphere devices using the inbuilt REST server.
-Author: Microsoft
-Author-email: azspheremfrsamplesup@microsoft.com
-License: MIT
+Author-email: Microsoft <azspheremfrsamplesup@microsoft.com>
+Keywords: azure,sphere,device,api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `azuresphere-device-api-1.0.2/README.md` & `azuresphere-device-api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/app.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/app.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/capabilities.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/capabilities.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/certificate.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/certificate.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/certs/device_rest_api_certificate.pem` & `azuresphere-device-api-1.1.0/azuresphere_device_api/certs/device_rest_api_certificate.pem`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/device.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/device.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/devices.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/devices.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 import re
 from sys import platform
+from packaging import version
 
 from azuresphere_device_api import utils
 from azuresphere_device_api.exceptions import ValidationError
 
 
 def set_active_device_ip_address(ip_address: str) -> None:
     """Sets the device IP address used in all requests.
 
     :param ip_address: The device IP address to use.
     :type ip_address: string
     """
-    if platform in ("linux", "linux2") and ip_address != '192.168.35.2':
-        raise ValidationError(
-            f"ERROR: Cannot set active device IP address {ip_address} on Linux. Linux does not have multi-board support.")
-
-    regex_pattern = '^192.168.35.\\b([2-9]|[1-9][0-9]|1[0-9][0-9]|2[0-4][0-9]|25[0-5])\\b$'
+    regex_pattern = '^192.168.35.\\b([2-9]|[1-9][0-9]|1[0-9][0-9]|2[0-4][0-9]|25[0-4])\\b$'
     pattern_matches = re.findall(regex_pattern, ip_address)
 
     if not pattern_matches:
         raise ValidationError(
-            f"ERROR: Cannot set active device IP address {ip_address}, range is 192.168.35.2-192.168.35.255")
+            f"ERROR: Cannot set active device IP address {ip_address}, range is 192.168.35.2-192.168.35.254")
 
     utils.set_device_ip_address(ip_address)
 
 
 def get_active_device_ip_address() -> str:
     """Returns the device IP address currently used in all requests.
 
@@ -45,15 +42,17 @@
     :rtype: Tuple(int, dict[str, str])
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
     if platform == "win32":
         return utils.get_request("api/service/devices", api_type=utils.AzureSphereDeviceApiRequestType.LOCAL_DEVICE_URL)
 
-    if platform in ("linux", "linux2"):
+    if "linux" in platform:
+        if utils.get_sdk_version() >= version.parse("23.04"):
+            return utils.get_request("api/service/devices", api_type=utils.AzureSphereDeviceApiRequestType.LOCAL_DEVICE_URL)
         return _list_linux_devices()
 
     raise ValidationError(
         "ERROR: Cannot get attached devices, unsupported operating system.")
 
 
 def _linux_netifaces_ioctl():
@@ -62,45 +61,39 @@
     """
     import socket
     import fcntl
     import struct
     import array
     MAX_BYTES = 4096
     SIOCGIFCONF = 0x8912
-
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     names = array.array('B', MAX_BYTES * b'\0')
-
     ioctl_buff_addr, _ioctl_buff_length = names.buffer_info()
     mutable_byte_buffer = struct.pack('iL', MAX_BYTES, ioctl_buff_addr)
     # query ioctl (io control) for interface names
     mutated_byte_buffer = fcntl.ioctl(
         sock.fileno(), SIOCGIFCONF, mutable_byte_buffer)
     ioctl_byte_count, _names_address_out = struct.unpack(
         'iL', mutated_byte_buffer)
-
     ioctl_buff = names.tobytes()
     ioctl_buff = ioctl_buff[:ioctl_byte_count]
     ifaces = {}
-
     # each ioctl entry is 40 bytes long
     for i in range(0, ioctl_byte_count, 40):
         # the first 16 bytes are the name
         name = str(ioctl_buff[i: i+16].strip(b'\0'), encoding="utf8")
         # bytes 20-24 are ip address octets.
         # decode as human readable string.
         ip = '.'.join([str(octet) for octet in ioctl_buff[i+20:i+24]])
         ifaces[name] = ip
-
     return ifaces
 
 
 def _list_linux_devices() -> list:
     """Linux method of getting attached devices.
-
     :return: List of attached devices on success.
     :rtype: Tuple(int, dict[str, str])
     """
     devices = []
     if "sl0" in _linux_netifaces_ioctl():
         devices = [{"IpAddress": "192.168.35.2", "DeviceConnectionPath": ""}]
     return devices
```

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/error_handler.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/error_handler.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/exceptions.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/image.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/image.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/manufacturing.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/manufacturing.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     :type manufacturing_state: str
     :accepted-parameters manufacturing_state: DeviceComplete, Module1Complete
     :return: An empty response on success. An exception will be thrown on error.
     :rtype: dict[str, str]
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
-    valid_settable_manufacturing_states = ["DeviceComplete", "Module1Complete"]
+    valid_settable_manufacturing_states = ["Unknown", "Blank", "DeviceComplete", "Module1Complete"]
 
     if manufacturing_state not in valid_settable_manufacturing_states:
         raise ValidationError(
             "ERROR: Cannot set manufacturing state, manufacturing state supplied is invalid.")
 
     return utils.put_request(
         "device/manufacturing_state", {
```

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/network.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/network.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/sideload.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/sideload.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/utils.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 # Licensed under the MIT License.
 
 from enum import Enum, auto, unique
 from http import HTTPStatus
 from pathlib import Path
 from typing import Any
 from uuid import UUID
+from sys import platform
 import requests
 from requests_toolbelt.adapters import host_header_ssl
 
 from azuresphere_device_api.error_handler import handle_status_code_errors
-from azuresphere_device_api.exceptions import UnknownDeviceError, DeviceError
+from azuresphere_device_api.exceptions import UnknownDeviceError, DeviceError, AzureSphereDeviceApiException, ValidationError
 from azuresphere_device_api.validation import set_current_device_api_version
 
+from packaging import version
+import os
+
 _CURRENT_DEVICE_IP = "192.168.35.2"
+_SDK_VERSION = None
 
 CURRENT_DIR = Path(__file__).parent
 _CERT_PATH = (CURRENT_DIR / "certs/device_rest_api_certificate.pem").absolute()
 
 
 @unique
 class AzureSphereDeviceApiRequestType(Enum):
@@ -54,21 +59,60 @@
     except requests.exceptions.ConnectionError as conn_err:
         raise DeviceError(
             f"Device connection timed out for {get_device_ip_address()}. Please ensure your device is connected and has development mode enabled.") from conn_err
     except Exception as other_exception:
         raise UnknownDeviceError from other_exception
 
 
+def get_sdk_path() -> str:
+    sdk_path = os.environ.get("AzureSphereDefaultSDKDir")
+
+    if sdk_path == "" or sdk_path is None:
+        raise AzureSphereDeviceApiException(
+            "Cannot retrieve the SDK path, 'AzureSphereDefaultSDKDir' environment variable is not set! Is the SDK installed and available?")
+
+    return sdk_path
+
+
+def get_sdk_version() -> version.Version:
+    global _SDK_VERSION
+    if _SDK_VERSION is not None:
+        return _SDK_VERSION
+
+    sdk_version_path = os.path.join(get_sdk_path(), "VERSION")
+
+    if os.path.exists(sdk_version_path):
+        with open(sdk_version_path, "r", encoding="utf8") as version_file:
+            version_number = version_file.read().strip()
+            period_count = len(
+                [char for char in version_number if char == "."])
+            if period_count > 3:
+                chunked = version_number.split(".")
+                preview_version = chunked[-1]
+                version_number = ".".join(chunked[:3]) + f"- {preview_version}"
+
+            _SDK_VERSION = version.parse(version_number)
+            return _SDK_VERSION
+
+    raise AzureSphereDeviceApiException(
+        "Cannot retrieve the SDK version, version file does not exist! Is the SDK installed and available?")
+
+
 def set_device_ip_address(ip_address: str):
     """Sets the device IP address used in all requests.
 
     :param ip_address: The device IP address to use.
     :type ip_address: string
     """
     global _CURRENT_DEVICE_IP
+
+    if "linux" in platform and ip_address != "192.168.35.2" and get_sdk_version() < version.parse("23.04"):
+        raise ValidationError(
+            f"ERROR: Cannot set active device IP address to '{ip_address}'. This SDK version does not support multiple devices.")
+
     _CURRENT_DEVICE_IP = ip_address
 
 
 def get_device_ip_address() -> str:
     """Returns the device IP address currently used in all requests.
     """
     return _CURRENT_DEVICE_IP
```

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/validation.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/validation.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api/wifi.py` & `azuresphere-device-api-1.1.0/azuresphere_device_api/wifi.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/PKG-INFO` & `azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: azuresphere-device-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: A library for interacting with Azure Sphere devices using the inbuilt REST server.
-Author: Microsoft
-Author-email: azspheremfrsamplesup@microsoft.com
-License: MIT
+Author-email: Microsoft <azspheremfrsamplesup@microsoft.com>
+Keywords: azure,sphere,device,api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `azuresphere-device-api-1.0.2/azuresphere_device_api.egg-info/SOURCES.txt` & `azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE.txt
 README.md
 pyproject.toml
-setup.cfg
 azuresphere_device_api/__init__.py
 azuresphere_device_api/app.py
 azuresphere_device_api/capabilities.py
 azuresphere_device_api/certificate.py
 azuresphere_device_api/device.py
 azuresphere_device_api/devices.py
 azuresphere_device_api/error_handler.py
```

