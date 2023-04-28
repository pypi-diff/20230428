# Comparing `tmp/difft-1.1.9-py3-none-any.whl.zip` & `tmp/difft-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 10679 bytes, number of entries: 14
+Zip file size: 11386 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-07 07:19 difft/__init__.py
 -rw-r--r--  2.0 unx     1393 b- defN 22-Mar-23 03:50 difft/attachment.py
 -rw-r--r--  2.0 unx     2989 b- defN 22-Apr-26 07:15 difft/auth.py
--rw-r--r--  2.0 unx    11070 b- defN 22-Aug-08 03:50 difft/client.py
+-rw-r--r--  2.0 unx    12895 b- defN 23-Apr-28 02:49 difft/client.py
 -rw-r--r--  2.0 unx     7741 b- defN 22-Sep-19 09:37 difft/command.py
--rw-r--r--  2.0 unx      573 b- defN 22-Mar-24 08:59 difft/constants.py
--rw-r--r--  2.0 unx     3817 b- defN 22-Jul-01 13:58 difft/difft_ws_listener.py
--rw-r--r--  2.0 unx     2888 b- defN 22-Oct-10 10:00 difft/message.py
+-rw-r--r--  2.0 unx      616 b- defN 23-Apr-28 02:49 difft/constants.py
+-rw-r--r--  2.0 unx     3883 b- defN 23-Apr-10 13:55 difft/difft_ws_listener.py
+-rw-r--r--  2.0 unx     3140 b- defN 23-Feb-01 07:30 difft/message.py
 -rw-r--r--  2.0 unx      304 b- defN 22-Apr-26 06:29 difft/utils.py
--rw-r--r--  2.0 unx      326 b- defN 22-Oct-10 10:00 difft-1.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-10 10:00 difft-1.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 22-Oct-10 10:00 difft-1.1.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Oct-10 10:00 difft-1.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1044 b- defN 22-Oct-10 10:00 difft-1.1.9.dist-info/RECORD
-14 files, 32293 bytes uncompressed, 8969 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx      275 b- defN 23-Apr-28 02:49 difft-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 02:49 difft-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-28 02:49 difft-1.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-28 02:49 difft-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1044 b- defN 23-Apr-28 02:49 difft-1.2.1.dist-info/RECORD
+14 files, 34427 bytes uncompressed, 9676 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: difft/message.py
 Comment: 
 
 Filename: difft/utils.py
 Comment: 
 
-Filename: difft-1.1.9.dist-info/METADATA
+Filename: difft-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: difft-1.1.9.dist-info/WHEEL
+Filename: difft-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: difft-1.1.9.dist-info/entry_points.txt
+Filename: difft-1.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: difft-1.1.9.dist-info/top_level.txt
+Filename: difft-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: difft-1.1.9.dist-info/RECORD
+Filename: difft-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## difft/client.py

```diff
@@ -1,15 +1,18 @@
+import os
 import base64
 import hashlib
 import hmac
 import json
 import logging
+
 import requests
 from Crypto.Cipher import AES
 from Crypto.Random import get_random_bytes
+
 from difft import constants
 from difft.auth import Authenticator
 
 
 class DifftClient:
     BLOCK_SIZE = 16
 
@@ -141,14 +144,54 @@
                                                     json=delete_attachment_auth_body, auth=self._auth)
         delete_attachment_auth_obj = json.loads(delete_attachment_auth_resp.text)
         if delete_attachment_auth_obj.get("status") != 0:
             logging.error(delete_attachment_auth_obj.get("reason"))
             return False
         return True
 
+    def upload_pic(self, picture_path, raw_response=False):
+        """
+        Upload picture so we can refer to it within messages.
+        :param picture_path: any filename
+        :return: online image url
+                 {
+                      "ver": 1,
+                      "status": 0,
+                      "reason": "success",
+                      "data": {
+                        "url": "https://difft-oss.s3.ap-southeast-1.amazonaws.com/50ab44ae13bf26337a1c1d3a0cdcc53c?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIASJTLN2W46QBZ6M65%2F20221122%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20221122T113605Z&X-Amz-Expires=300&X-Amz-SignedHeaders=host&x-id=GetObject&X-Amz-Signature=84ee194a240902561a749626d0eaa690cce885e5bc1056fd0ee1a70d8313a35d"
+                      }
+                 }
+        """
+        if not os.path.exists(picture_path):
+            raise Exception("file %s not found" % picture_path)
+
+        filename = os.path.basename(picture_path)
+
+        with open(picture_path, "rb") as fd:
+            content = base64.b64encode(fd.read())
+
+        payload ={
+            'file_name': filename,
+            # make it serializable to json
+            'content': content.decode('utf-8'),
+        }
+        res = requests.post(url=self._host + constants.URL_UPLOAD_PIC, json=payload, auth=self._auth)
+        if res.status_code != 200:
+            raise Exception("failed to upload image, server responded with %d" % res.status_code)
+        envelope = res.json()
+        if envelope.get("status") != 0:
+            raise Exception("pic upload failed", envelope.get("errors"), envelope.get("error"))
+
+        # done managing error cases, send back data
+        if raw_response:
+            return envelope
+        else:
+            return envelope.get("data").get("url")
+
     def send_message(self, msg, raw_response=False):
         """
         Send message
         :param msg: MessageRequest
         :param raw_response: whether to get raw response or not
         :return: list of fail reason, 
                 [
```

## difft/constants.py

```diff
@@ -9,8 +9,9 @@
 
 URL_ISEXIST = "/v1/file/isExists"
 URL_UPLOAD_ATTACHMENT = "/v1/file/uploadInfo"
 URL_DOWNLOAD_ATTACHMENT = "/v1/file/download"
 URL_DEL_ATTACHMENT = "/v1/file/delAuthorize"
 URL_SEND_MSG = "/v1/messages"
 URL_ACCOUNT = "/v1/accounts"
-URL_GROUP = "/v1/groups"
+URL_GROUP = "/v1/groups"
+URL_UPLOAD_PIC = "/difftoss/v1/uploadPic"
```

## difft/difft_ws_listener.py

```diff
@@ -1,14 +1,15 @@
 import logging
 import websocket
 import rel
 import json
 import time
 from difft.auth import Authenticator
 from difft.constants import *
+import traceback
 
 
 
 class DifftWsListener:
     def __init__(self, appid, key, domain='openapi.test.difft.org') -> None:
         if not isinstance(appid, str):
             raise Exception('appid should be type str')
@@ -51,14 +52,15 @@
             self.ws.run_forever(ping_interval=30, dispatcher=rel, ping_timeout=5)
             self.fetch(self.ws)
             
             rel.signal(2, rel.abort)  # Keyboard Interrupt
             rel.dispatch()
         except Exception as e:
             logging.error("[DifftWsListener] got error: {}, my appid: {}".format(e, self._appid))
+            logging.error(traceback.print_exc())
             # retry in 15 sec
             logging.info("[DifftWsListener] will retry in 15 seconds")
             time.sleep(15)
             self.start()
 
     def on_message(self, ws, message):
         logging.debug("[DifftWsListener] recieve data: {}".format(message))
```

## difft/message.py

```diff
@@ -65,22 +65,29 @@
         return self
 
     def recall(self, source, timestamp, refID=""):
         self.message_request['type'] = 'RECALL'
         self.message_request['recall'] = dict(realSource=dict(source=source, sourceDevice=1, timestamp=timestamp), refID=refID)
         return self
 
-    def card(self, appid, id, content,fixedWidth=False, creator=None, timestamp=None):
+    def card(self, appid, id, content,fixedWidth=False, creator=None, timestamp=None, height=None):
         self.message_request['type'] = 'CARD'
         self.message_request['card'] = dict(appID=appid, id=id, content=content)
         if fixedWidth:
             self.message_request['card']['fixedWidth'] = fixedWidth
         if creator:
             self.message_request['card']['creator'] = creator
         if timestamp:
             self.message_request['card']['timestamp'] = timestamp
+        if height:
+            self.message_request['card']['height'] = height
+        return self
+
+    def forwarded(self, forwarded):
+        self.message_request['type'] = 'FORWARD'
+        self.message_request['forwarded'] = forwarded
         return self
 
     def build(self):
         return self.message_request
```

## Comparing `difft-1.1.9.dist-info/RECORD` & `difft-1.2.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 difft/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 difft/attachment.py,sha256=VkjvBxZ8heVeZlZl6eaDNy8uErWmZIir9YBBQAT-qYw,1393
 difft/auth.py,sha256=j36_rPOs8ui-Scgcy_2mvrGVhxYfN1_tYr-pX3i4amo,2989
-difft/client.py,sha256=f2Bm8CqfPBwkmxNUkvee4St45ochwvWfM6Q6UzN7aU8,11070
+difft/client.py,sha256=2s0CbaNSdixG6oCVxJGP6kZMgXv9W5LRVDuVtLkjfYw,12895
 difft/command.py,sha256=LAwS1QpaSUF71q9EMH5HSvHIibt-mmxUiprGKbG7B94,7741
-difft/constants.py,sha256=QiROfHXvP_OPGtFsqTEwsjNaeqx_rD5f9aegIcYk6is,573
-difft/difft_ws_listener.py,sha256=fvB1wEsaB-RsGUe1HzeJcT2tDVga2fMUawx3Gptb8vI,3817
-difft/message.py,sha256=ejN2dyi2jHGUKmtjd9fHFuCa9JDJCNMlBcaXVQegnLc,2888
+difft/constants.py,sha256=UmrzrMxWshok9baW0eSvG18uFoiUbRgBg1od3SvOOI8,616
+difft/difft_ws_listener.py,sha256=PGcW1l3jykDT5tqYItBJ3QK0bln3yWqbhobFIUC-hac,3883
+difft/message.py,sha256=PFm1ODr0yKp0uk0I_G9v1OSCU_JF-wWvpCBivWoW0k0,3140
 difft/utils.py,sha256=IFi1g4ZMUCiTfFkt2a7X5mkpM47o_UedoXAgiMiQ5-A,304
-difft-1.1.9.dist-info/METADATA,sha256=sPDE-07yyJdht_SHygROTxUKsRMg8xn1Qgolrb4Y5bo,326
-difft-1.1.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-difft-1.1.9.dist-info/entry_points.txt,sha256=rObsennM971X_sZQFleWPv_Qr9xVVDskX-57AQ5FaFE,50
-difft-1.1.9.dist-info/top_level.txt,sha256=chJ57utNQdklgBoF42UEt4t2wgtXWqUUcehueecHAgM,6
-difft-1.1.9.dist-info/RECORD,,
+difft-1.2.1.dist-info/METADATA,sha256=CVNiep0aZ7PJHMZQDQl5oBeeyfCKa6URu_jSw1BmFJM,275
+difft-1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+difft-1.2.1.dist-info/entry_points.txt,sha256=AJDFoxGSgqUFYD9iCLUu_SloZLFFkMIckDuOBpeAWsQ,49
+difft-1.2.1.dist-info/top_level.txt,sha256=chJ57utNQdklgBoF42UEt4t2wgtXWqUUcehueecHAgM,6
+difft-1.2.1.dist-info/RECORD,,
```

