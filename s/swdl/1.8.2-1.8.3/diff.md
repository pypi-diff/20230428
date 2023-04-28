# Comparing `tmp/swdl-1.8.2-py3-none-any.whl.zip` & `tmp/swdl-1.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21542 bytes, number of entries: 18
+Zip file size: 21614 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      125 b- defN 23-Feb-14 15:38 swdl/__init__.py
--rw-r--r--  2.0 unx      497 b- defN 23-Mar-09 16:52 swdl/_version.py
+-rw-r--r--  2.0 unx      497 b- defN 23-Apr-18 13:50 swdl/_version.py
 -rw-r--r--  2.0 unx     1994 b- defN 22-Mar-16 14:34 swdl/camera.py
 -rw-r--r--  2.0 unx     1567 b- defN 22-Mar-16 14:34 swdl/club.py
 -rw-r--r--  2.0 unx      550 b- defN 22-Mar-16 14:34 swdl/config.py
 -rw-r--r--  2.0 unx    18307 b- defN 23-Feb-14 15:38 swdl/labels.py
 -rw-r--r--  2.0 unx     4837 b- defN 23-Mar-09 16:51 swdl/match_data.py
--rw-r--r--  2.0 unx    15902 b- defN 23-Feb-14 15:38 swdl/matches.py
--rw-r--r--  2.0 unx    15289 b- defN 23-Feb-14 15:38 swdl/swrest.py
+-rw-r--r--  2.0 unx    15902 b- defN 23-Apr-18 12:51 swdl/matches.py
+-rw-r--r--  2.0 unx    15311 b- defN 23-Apr-18 13:49 swdl/swrest.py
 -rw-r--r--  2.0 unx      867 b- defN 23-Feb-02 08:53 swdl/team.py
--rw-r--r--  2.0 unx     1943 b- defN 23-Feb-14 15:38 swdl/tools.py
--rwxr-xr-x  2.0 unx       95 b- defN 23-Mar-09 16:52 swdl-1.8.2.data/scripts/swdl-login
--rwxr-xr-x  2.0 unx     1433 b- defN 23-Mar-09 16:52 swdl-1.8.2.data/scripts/swdl-match-info
--rw-r--r--  2.0 unx     1097 b- defN 23-Mar-09 16:52 swdl-1.8.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      562 b- defN 23-Mar-09 16:52 swdl-1.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-09 16:52 swdl-1.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-09 16:52 swdl-1.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1338 b- defN 23-Mar-09 16:52 swdl-1.8.2.dist-info/RECORD
-18 files, 66500 bytes uncompressed, 19402 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx     1945 b- defN 23-Apr-18 13:49 swdl/tools.py
+-rwxr-xr-x  2.0 unx       95 b- defN 23-Apr-18 13:50 swdl-1.8.3.data/scripts/swdl-login
+-rwxr-xr-x  2.0 unx     1433 b- defN 23-Apr-18 13:50 swdl-1.8.3.data/scripts/swdl-match-info
+-rw-r--r--  2.0 unx     1097 b- defN 23-Apr-18 13:50 swdl-1.8.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      562 b- defN 23-Apr-18 13:50 swdl-1.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 13:50 swdl-1.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-18 13:50 swdl-1.8.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1338 b- defN 23-Apr-18 13:50 swdl-1.8.3.dist-info/RECORD
+18 files, 66524 bytes uncompressed, 19474 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: swdl/team.py
 Comment: 
 
 Filename: swdl/tools.py
 Comment: 
 
-Filename: swdl-1.8.2.data/scripts/swdl-login
+Filename: swdl-1.8.3.data/scripts/swdl-login
 Comment: 
 
-Filename: swdl-1.8.2.data/scripts/swdl-match-info
+Filename: swdl-1.8.3.data/scripts/swdl-match-info
 Comment: 
 
-Filename: swdl-1.8.2.dist-info/LICENSE
+Filename: swdl-1.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: swdl-1.8.2.dist-info/METADATA
+Filename: swdl-1.8.3.dist-info/METADATA
 Comment: 
 
-Filename: swdl-1.8.2.dist-info/WHEEL
+Filename: swdl-1.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: swdl-1.8.2.dist-info/top_level.txt
+Filename: swdl-1.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: swdl-1.8.2.dist-info/RECORD
+Filename: swdl-1.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swdl/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-03-09T17:51:12+0100",
+ "date": "2023-04-18T15:49:16+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "525feb8ff7722d37182f79a030f1480ba672ebd4",
- "version": "1.8.2"
+ "full-revisionid": "69315b2932a3a85dea353b13dfc05aea5adb7bee",
+ "version": "1.8.3"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## swdl/swrest.py

```diff
@@ -56,25 +56,25 @@
 
     def _sign_in(self):
         body = {
             "email": self.username,
             "password": self.password,
             "returnSecureToken": True,
         }
-        ret = make_request(self.sign_in_url, body)
+        ret = make_request(self.sign_in_url, body, retries=7)
         self.id_token = ret["idToken"]
         self.refresh_token = ret["refreshToken"]
         self.token_expires = datetime.now() + timedelta(seconds=int(ret["expiresIn"]))
 
     def _refresh_token(self):
         body = {
             "grant_type": "refresh_token",
             "refresh_token": self.refresh_token,
         }
-        ret = make_request(self.token_url, body)
+        ret = make_request(self.token_url, body, retries=7)
         self.id_token = ret["id_token"]
         self.refresh_token = ret["refresh_token"]
         self.token_expires = datetime.now() + timedelta(seconds=int(ret["expires_in"]))
 
     @property
     def auth(self):
         if (
```

## swdl/tools.py

```diff
@@ -1,15 +1,18 @@
+import logging
 import time
 from os import PathLike
 from pathlib import Path
 from typing import Optional, Union
 
 import requests
 import simplejson as json
 
+logger = logging.getLogger(__name__)
+
 PathLike = Union[str, PathLike, Path]
 
 
 class AuthSerivceBase:
     @property
     def auth(self):
         raise NotImplementedError()
@@ -36,34 +39,34 @@
         The response as dictionary
 
     """
     auth = None
     if authorization:
         auth = authorization.auth
     exception = None
+    ret = requests.Response()
     for i in range(retries):
         time.sleep(i**2)
+
         try:
             if body is None:
                 ret = requests.get(url, auth=auth, **kwargs)
             else:
                 ret = requests.post(url, json=body, auth=auth, **kwargs)
+            ret.raise_for_status()
 
         except requests.RequestException as e:
+            logger.warning("Failed to communicate with API:")
+            logger.warning(e)
+            logger.warning(ret.text)
             exception = e
             continue
-        if ret.status_code >= 500:
-            exception = ConnectionError("Internal Server Error")
-            continue
-        if ret.status_code == 403:
-            exception = ConnectionError("Failed to authenticate")
+        try:
+            return ret.json()
+        except json.JSONDecodeError as e:
+            # Some APIs will return an empty response body which is also valid in this
+            # case
+            if ret.text == "":
+                return {"success": True}
+            exception = e
             continue
-        if ret.status_code == 200:
-            try:
-                return ret.json()
-            except json.JSONDecodeError as e:
-                if ret.text == "":
-                    return {"success": True}
-                exception = e
-                continue
-        exception = ConnectionError(ret.text)
     raise ConnectionError(f"Failed to fetch data from {url}") from exception
```

## Comparing `swdl-1.8.2.data/scripts/swdl-match-info` & `swdl-1.8.3.data/scripts/swdl-match-info`

 * *Files identical despite different names*

## Comparing `swdl-1.8.2.dist-info/LICENSE` & `swdl-1.8.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swdl-1.8.2.dist-info/METADATA` & `swdl-1.8.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swdl
-Version: 1.8.2
+Version: 1.8.3
 Summary: Soccerwatch Data Library
 Home-page: https://bitbucket.org/soccerwatch/swdl/
 Author: Christian Bodenstein
 Author-email: bodenstein@soccerwatch.tv
 License-File: LICENSE
 Requires-Dist: future
 Requires-Dist: google-cloud-storage
```

## Comparing `swdl-1.8.2.dist-info/RECORD` & `swdl-1.8.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 swdl/__init__.py,sha256=kH3KYcv8cJ_63SgLsB75BocLK7ra6uRjafGiA6x3mXo,125
-swdl/_version.py,sha256=w1WzAZ_C5_yku03Q9Mb1exKbPeTYytNK_KdoyuONnhI,497
+swdl/_version.py,sha256=wsUTgTHvO6WTe6x7Kg2DEAKyy21c0B9tMhclArf4FCY,497
 swdl/camera.py,sha256=sw129kJvFqINVP-X0d6BusShqeP4R1ZRJkefcRo9oTY,1994
 swdl/club.py,sha256=hKpCaVLW7pit3uifsg54Lfs3u6dD-jahIv2OZq1XH1Y,1567
 swdl/config.py,sha256=uMKUEW75uLjPWu-08HXbyW1YZfTy1TINUjeknRHENiI,550
 swdl/labels.py,sha256=Lnej3vLbD6q17FK_gLtvQhIda9y-MuIGJvO2TIwNII0,18307
 swdl/match_data.py,sha256=y2oViB-QknsPa-Gxf1Kjjbi-RCcUZ_QRSy_6eR5K0tE,4837
 swdl/matches.py,sha256=4SxdxMMuo86sS5rjwrEAKjy2gxX7Rm7s91UhyywAG7E,15902
-swdl/swrest.py,sha256=vNrILmWw9Bt8FMK0gDxwcfzkWziawobUJ5xcgfrriY4,15289
+swdl/swrest.py,sha256=3v1vsXlQXS-HhkWE22awb87NoAF3DmCxypG_RKQRrqs,15311
 swdl/team.py,sha256=XPRbTqSXbrej_HsE8Pi3zNPNbBO8wh6wymI_gjHJghs,867
-swdl/tools.py,sha256=LUMGHDK1Y7QtU1iHWn2ybRUeN_XoQ4DB1hjY_QBOFwE,1943
-swdl-1.8.2.data/scripts/swdl-login,sha256=HN-MQra72h9KsxddC8Ejcrgo7kVBz6DslApVmNpCk90,95
-swdl-1.8.2.data/scripts/swdl-match-info,sha256=jUbPn4Abyh8Reaz_d27vYnUre5FfoxH1kkRpseBB-dA,1433
-swdl-1.8.2.dist-info/LICENSE,sha256=SYoKT5xuN9rZoXv4nanLwmwUD8WkmZ2C_QOUcNh090I,1097
-swdl-1.8.2.dist-info/METADATA,sha256=lmpKpB3KxLH2x3ndy82sD7Y5pQ4af9ra0MrTtLHDEHA,562
-swdl-1.8.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-swdl-1.8.2.dist-info/top_level.txt,sha256=ewYoV9WP7XVlXR72d6MbUtBaYHLcNfI1TfdLZBzEjdM,5
-swdl-1.8.2.dist-info/RECORD,,
+swdl/tools.py,sha256=5bcJZER1Ib2BKNaCNOAKYj0IqrOSJrk020cgQwM9Xvk,1945
+swdl-1.8.3.data/scripts/swdl-login,sha256=HN-MQra72h9KsxddC8Ejcrgo7kVBz6DslApVmNpCk90,95
+swdl-1.8.3.data/scripts/swdl-match-info,sha256=jUbPn4Abyh8Reaz_d27vYnUre5FfoxH1kkRpseBB-dA,1433
+swdl-1.8.3.dist-info/LICENSE,sha256=SYoKT5xuN9rZoXv4nanLwmwUD8WkmZ2C_QOUcNh090I,1097
+swdl-1.8.3.dist-info/METADATA,sha256=p5O1YjYkJmZo44ZAH6wjr4RVXWiQ8kjkyEoTUSNb_Rk,562
+swdl-1.8.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+swdl-1.8.3.dist-info/top_level.txt,sha256=ewYoV9WP7XVlXR72d6MbUtBaYHLcNfI1TfdLZBzEjdM,5
+swdl-1.8.3.dist-info/RECORD,,
```

