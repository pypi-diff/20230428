# Comparing `tmp/lakeside-0.8.tar.gz` & `tmp/lakeside-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lakeside-0.8.tar", last modified: Mon Aug  6 23:43:16 2018, max compression
+gzip compressed data, was "dist/lakeside-0.9.tar", last modified: Mon Aug 13 17:07:32 2018, max compression
```

## Comparing `lakeside-0.8.tar` & `lakeside-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-08-06 23:43:16.000000 lakeside-0.8/
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      504 2018-08-06 23:43:16.000000 lakeside-0.8/PKG-INFO
-drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside/
--rwxrwxr-x   0 mjg59     (1000) mjg59     (1000)     9418 2018-08-06 00:18:54.000000 lakeside-0.8/lakeside/__init__.py
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)    37085 2018-08-06 00:18:54.000000 lakeside-0.8/lakeside/lakeside_pb2.py
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       38 2018-08-06 23:43:16.000000 lakeside-0.8/setup.cfg
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      686 2018-08-06 00:18:54.000000 lakeside-0.8/README.md
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)     1365 2018-08-06 23:42:40.000000 lakeside-0.8/setup.py
-drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside.egg-info/
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        1 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside.egg-info/dependency_links.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      504 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside.egg-info/PKG-INFO
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        9 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside.egg-info/top_level.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       27 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside.egg-info/requires.txt
--rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      223 2018-08-06 23:43:16.000000 lakeside-0.8/lakeside.egg-info/SOURCES.txt
+drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-08-13 17:07:32.000000 lakeside-0.9/
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      504 2018-08-13 17:07:32.000000 lakeside-0.9/PKG-INFO
+drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside/
+-rwxrwxr-x   0 mjg59     (1000) mjg59     (1000)     9749 2018-08-12 21:09:29.000000 lakeside-0.9/lakeside/__init__.py
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)    37085 2018-08-06 00:18:54.000000 lakeside-0.9/lakeside/lakeside_pb2.py
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       38 2018-08-13 17:07:32.000000 lakeside-0.9/setup.cfg
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      686 2018-08-06 00:18:54.000000 lakeside-0.9/README.md
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)     1365 2018-08-13 17:06:56.000000 lakeside-0.9/setup.py
+drwxrwxr-x   0 mjg59     (1000) mjg59     (1000)        0 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside.egg-info/
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        1 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside.egg-info/dependency_links.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      504 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside.egg-info/PKG-INFO
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)        9 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside.egg-info/top_level.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)       27 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside.egg-info/requires.txt
+-rw-rw-r--   0 mjg59     (1000) mjg59     (1000)      223 2018-08-13 17:07:32.000000 lakeside-0.9/lakeside.egg-info/SOURCES.txt
```

### Comparing `lakeside-0.8/lakeside/__init__.py` & `lakeside-0.9/lakeside/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # limitations under the License.
 
 from Crypto.Cipher import AES
 import random
 import requests
 import socket
 import struct
+import threading
 import time
 
 from . import lakeside_pb2
 
 key = bytearray([0x24, 0x4E, 0x6D, 0x8A, 0x56, 0xAC, 0x87, 0x91, 0x24, 0x43, 0x2D, 0x8B, 0x6C, 0xBC, 0xA2, 0xC4])
 iv = bytearray([0x77, 0x24, 0x56, 0xF2, 0xA7, 0x66, 0x4C, 0xF3, 0x39, 0x2C, 0x35, 0x97, 0xE9, 0x3E, 0x57, 0x47])
 
@@ -53,19 +54,24 @@
     return devices
 
 class device:
     def __init__(self, address, code, kind=None):
         self.address = address
         self.code = code
         self.kind = kind
+        self.keepalive = None
 
     def connect(self):
         self.s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.s.connect((self.address, 55556))
         self.update()
+        if self.keepalive is None:
+            self.keepalive = threading.Thread(target=self.ping, args=())
+            self.keepalive.daemon = True
+            self.keepalive.start()
 
     def send_packet(self, packet, response):
         cipher = AES.new(bytes(key), AES.MODE_CBC, bytes(iv))
         raw_packet = packet.SerializeToString()
 
         for i in range(16 - (len(raw_packet) % 16)):
             raw_packet += b'\0'
@@ -105,14 +111,19 @@
         packet = lakeside_pb2.T1012Packet()
         packet.sequence = random.randrange(3000000)
         packet.code = self.code
         packet.ping.type = 0        
         response = self.send_packet(packet, True)
         return response.sequence + 1
 
+    def ping(self):
+        while True:
+            time.sleep(10)
+            self.get_sequence()
+
 class bulb(device):
     def __init__(self, address, code, kind):
         return device.__init__(self, address, code, kind=kind)
 
     def connect(self):
         return device.connect(self)
```

### Comparing `lakeside-0.8/lakeside/lakeside_pb2.py` & `lakeside-0.9/lakeside/lakeside_pb2.py`

 * *Files identical despite different names*

### Comparing `lakeside-0.8/README.md` & `lakeside-0.9/README.md`

 * *Files identical despite different names*

### Comparing `lakeside-0.8/setup.py` & `lakeside-0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 import re
 from setuptools import setup, find_packages
 import sys
 import warnings
 
 dynamic_requires = []
 
-version = 0.8
+version = 0.9
 
 setup(
     name='lakeside',
-    version=0.8,
+    version=0.9,
     author='Matthew Garrett',
     author_email='mjg59@google.com',
     url='http://github.com/google/python-lakeside',
     packages=find_packages(),
     scripts=[],
     description='Python API for controlling Eufy LED bulbs',
     classifiers=[
```

