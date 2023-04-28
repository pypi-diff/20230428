# Comparing `tmp/sapcloudconnectorpythonsocket-0.1.3-py2.py3-none-any.whl.zip` & `tmp/sapcloudconnectorpythonsocket-0.1.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7288 bytes, number of entries: 9
+Zip file size: 7331 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 14:00 sap-cloud-connector-python-socket/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 14:01 sap-cloud-connector-python-socket/sap-cloud-connector-python-socket.py
--rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-24 12:22 sapcloudconnectorpythonsocket/__init__.py
--rw-rw-rw-  2.0 fat    10358 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2401 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      937 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD
-9 files, 15230 bytes uncompressed, 5608 bytes compressed:  63.2%
+-rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-28 10:48 sapcloudconnectorpythonsocket/__init__.py
+-rw-rw-rw-  2.0 fat    10479 b- defN 23-Apr-28 10:47 sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-28 10:48 sapcloudconnectorpythonsocket-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2401 b- defN 23-Apr-28 10:48 sapcloudconnectorpythonsocket-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-28 10:48 sapcloudconnectorpythonsocket-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-28 10:48 sapcloudconnectorpythonsocket-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      937 b- defN 23-Apr-28 10:48 sapcloudconnectorpythonsocket-0.1.4.dist-info/RECORD
+9 files, 15351 bytes uncompressed, 5651 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sapcloudconnectorpythonsocket/__init__.py
 Comment: 
 
 Filename: sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE
+Filename: sapcloudconnectorpythonsocket-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA
+Filename: sapcloudconnectorpythonsocket-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/WHEEL
+Filename: sapcloudconnectorpythonsocket-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/top_level.txt
+Filename: sapcloudconnectorpythonsocket-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD
+Filename: sapcloudconnectorpythonsocket-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sapcloudconnectorpythonsocket/__init__.py

```diff
@@ -1,14 +1,14 @@
 """
 sap-cloud-connector-python-socket
 
 Python Socket to connect to the SAP Cloud Connector via Connectivity Service
 """
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
 from sapcloudconnectorpythonsocket.sapcloudconnectorpythonsocket import CloudConnectorSocket
 
 __all__ = [
     CloudConnectorSocket
```

## sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py

```diff
@@ -3,15 +3,15 @@
 """
 import functools
 import socket
 import struct
 import base64
 import logging
 
-logger = logging.getLogger('sapcloudconnectorpythonsocket')
+logger = logging.getLogger("sapcloudconnectorpythonsocket")
 logger.addHandler(logging.NullHandler())
 
 
 def format_status_byte(status_byte) -> str:
     """helper function to log the CC specific error bytes"""
     status_byte_messages = {
         b"\x00": "SUCCESS: Success",
@@ -71,21 +71,25 @@
         try:
             # Initial connection to proxy server
             super(CloudConnectorSocket, self).connect((proxy_host, proxy_port))
         except Exception as e:
             self.close()
             raise Exception(f"EXCEPTION AT INITIAL CONNECT: {e}")
             
+        logger.info("Initial Proxy Connect succeeded")
         
         try:                
             # Connected to proxy server, now negotiate authentication
             self.negotiate_auth(dest_host, dest_port, token, location_id)
         except Exception as e:
             self.close()
             raise Exception(f"EXCEPTION NEGOTIATIONG {e}")
+        
+        logger.info("Cloud Connector Socket Ready")
+
 
                 
     def negotiate_auth(self, dest_host, dest_port, token, location_id):
         """SAP Cloud Connector specific authentication scheme"""
         self.settimeout(None)   # apparently needed for make file to set to blocking https://stackoverflow.com/questions/3432102/python-socket-connection-timeout
         writer = self.makefile("wb")
         reader = self.makefile("rb", 0)  # buffering=0 renamed in Python 3
```

## Comparing `sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE` & `sapcloudconnectorpythonsocket-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA` & `sapcloudconnectorpythonsocket-0.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapcloudconnectorpythonsocket
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Package to open socket to SAP Cloud Connector via Connectivity Proxy
 Home-page: https://github.com/fyx99/sap-cloud-connector-python-socket
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD` & `sapcloudconnectorpythonsocket-0.1.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sap-cloud-connector-python-socket/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sap-cloud-connector-python-socket/sap-cloud-connector-python-socket.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sapcloudconnectorpythonsocket/__init__.py,sha256=RA6VspWt6kfqEeTOlBITEEg6i2y4mxQVmUHNNOxj9H0,338
-sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py,sha256=80MrhtLdNfPb6HYwEYCS9f2YZCKbOXloRiXlg33YMxg,10358
-sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
-sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA,sha256=U7RXSZENOwKjULSArDJvwWevPo4fd82NcMURNXXZ6oI,2401
-sapcloudconnectorpythonsocket-0.1.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-sapcloudconnectorpythonsocket-0.1.3.dist-info/top_level.txt,sha256=Sr63qbSm-90o-CQ-qwd4EKcLFznczAzm416CC87q0pA,30
-sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD,,
+sapcloudconnectorpythonsocket/__init__.py,sha256=sgvgwSzA9wc60z7DUpKOm7uiGT9w_I3cwHXfAmYGabg,338
+sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py,sha256=5jxbb3WOqwaUNlngBpSXrjcTCM7joPERFXK9Q7rHb58,10479
+sapcloudconnectorpythonsocket-0.1.4.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
+sapcloudconnectorpythonsocket-0.1.4.dist-info/METADATA,sha256=mTg2XnA14aOrshSXWHoVfMQjHABBMd9z77DU4iXnK6I,2401
+sapcloudconnectorpythonsocket-0.1.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+sapcloudconnectorpythonsocket-0.1.4.dist-info/top_level.txt,sha256=Sr63qbSm-90o-CQ-qwd4EKcLFznczAzm416CC87q0pA,30
+sapcloudconnectorpythonsocket-0.1.4.dist-info/RECORD,,
```

