# Comparing `tmp/quorum_mininode_py-1.2.2.tar.gz` & `tmp/quorum_mininode_py-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_mininode_py-1.2.2.tar", last modified: Fri Apr 14 14:10:04 2023, max compression
+gzip compressed data, was "quorum_mininode_py-1.2.3.tar", last modified: Fri Apr 28 04:10:35 2023, max compression
```

## Comparing `quorum_mininode_py-1.2.2.tar` & `quorum_mininode_py-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.680225 quorum_mininode_py-1.2.2/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-04-14 14:10:04.679228 quorum_mininode_py-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.610412 quorum_mininode_py-1.2.2/quorum_mininode_py/
--rw-rw-rw-   0        0        0      607 2023-04-14 13:58:34.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.628366 quorum_mininode_py-1.2.2/quorum_mininode_py/api/
--rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/api/__init__.py
--rw-rw-rw-   0        0        0     2339 2023-03-30 11:03:37.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/api/base.py
--rw-rw-rw-   0        0        0     3822 2023-04-06 12:33:18.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/api/lightnode.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.635346 quorum_mininode_py-1.2.2/quorum_mininode_py/client/
--rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-03-30 05:11:33.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/client/_http.py
--rw-rw-rw-   0        0        0     3486 2023-04-14 13:57:42.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/client/mininode.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.647313 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/
--rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/__init__.py
--rw-rw-rw-   0        0        0     3094 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/account.py
--rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/aes.py
--rw-rw-rw-   0        0        0     1369 2023-03-30 09:45:11.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/age.py
--rw-rw-rw-   0        0        0     3856 2023-04-06 11:33:57.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/trx.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.672247 quorum_mininode_py-1.2.2/quorum_mininode_py/proto/
--rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/proto/__init__.py
--rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/proto/quorum_pb2.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.676262 quorum_mininode_py-1.2.2/quorum_mininode_py/utils/
--rw-rw-rw-   0        0        0       75 2023-04-06 11:35:51.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/utils/__init__.py
--rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.2/quorum_mininode_py/utils/url.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:10:04.622381 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-14 14:10:04.000000 quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 14:10:04.681223 quorum_mininode_py-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-04-14 13:58:23.000000 quorum_mininode_py-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.927155 quorum_mininode_py-1.2.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2440 2023-04-28 04:10:35.926158 quorum_mininode_py-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.882290 quorum_mininode_py-1.2.3/quorum_mininode_py/
+-rw-rw-rw-   0        0        0      611 2023-04-28 04:08:49.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.900227 quorum_mininode_py-1.2.3/quorum_mininode_py/api/
+-rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     3703 2023-04-28 04:08:20.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/api/base.py
+-rw-rw-rw-   0        0        0     3822 2023-04-06 12:33:18.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/api/lightnode.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.906212 quorum_mininode_py-1.2.3/quorum_mininode_py/client/
+-rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     1856 2023-04-28 03:47:53.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/client/_http.py
+-rw-rw-rw-   0        0        0     3447 2023-04-28 04:04:56.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/client/mininode.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.916197 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/
+-rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3094 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/account.py
+-rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/aes.py
+-rw-rw-rw-   0        0        0     1369 2023-03-30 09:45:11.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/age.py
+-rw-rw-rw-   0        0        0     3856 2023-04-06 11:33:57.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/trx.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.919209 quorum_mininode_py-1.2.3/quorum_mininode_py/proto/
+-rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/proto/__init__.py
+-rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/proto/quorum_pb2.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.924163 quorum_mininode_py-1.2.3/quorum_mininode_py/utils/
+-rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/utils/__init__.py
+-rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/utils/url.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.894245 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/
+-rw-rw-rw-   0        0        0     2440 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 04:10:35.927155 quorum_mininode_py-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1301 2023-04-28 04:08:49.000000 quorum_mininode_py-1.2.3/setup.py
```

### Comparing `quorum_mininode_py-1.2.2/LICENSE` & `quorum_mininode_py-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/PKG-INFO` & `quorum_mininode_py-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_mininode_py
-Version: 1.2.2
+Version: 1.2.3
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.2/README.md` & `quorum_mininode_py-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/__init__.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from quorum_mininode_py.crypto.account import (
     age_pvtkey_to_pubkey,
     create_age_keypair,
     create_private_key,
     private_key_to_pubkey,
     public_key_to_address,
 )
-from quorum_mininode_py.utils import decode_seed_url, update_seed_url
+from quorum_mininode_py.utils.url import decode_seed_url, update_seed_url
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __author__ = "liujuanjuan1984, zhangwm404"
 
 # Set default logging handler to avoid "No handler found" warnings.
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 logger.info("Version: %s", __version__)
```

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/api/lightnode.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/api/lightnode.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/client/_http.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/client/_http.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,31 +14,43 @@
         api_base: str,
         jwt_token: str = None,
     ):
         """Initializes the HttpRequest class"""
         requests.adapters.DEFAULT_RETRIES = 5
         self.api_base = api_base
         self.session = requests.Session()
-        headers = {"Content-Type": "application/json"}
+        self.headers = {"Content-Type": "application/json"}
+        self.jwt_token = jwt_token
         if jwt_token:
-            headers.update({"Authorization": f"Bearer {jwt_token}"})
-        self.session.headers.update(headers)
+            self.headers.update({"Authorization": f"Bearer {jwt_token}"})
+        self.session.headers.update(self.headers)
 
         _no_proxy = os.getenv("NO_PROXY", "")
         if self.api_base not in _no_proxy:
             os.environ["NO_PROXY"] = ",".join([_no_proxy, self.api_base])
+        self.retry_count = 0
 
     def _request(
         self,
         method: str,
         endpoint: str,
         payload: dict = None,
     ):
         url = "".join([self.api_base, endpoint])
-        resp = self.session.request(method=method, url=url, json=payload)
+        if self.retry_count > 5:
+            raise Exception("retry count > 5, check your network")
+        try:
+            resp = self.session.request(method=method, url=url, json=payload)
+        except Exception as err:
+            logger.warning("request error: %s", err)
+            self.session = requests.Session()
+            self.session.headers.update(self.headers)
+            self.retry_count += 1
+            return self._request(method, endpoint, payload)
+        self.retry_count = 0
         logger.debug("payload %s", payload)
         return resp.json()
 
     def get(self, endpoint: str, payload: dict = None):
         return self._request("get", endpoint, payload)
 
     def post(self, endpoint: str, payload: dict = None):
```

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/client/mininode.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/client/mininode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from dataclasses import dataclass
 
 import requests
 
-from quorum_mininode_py import utils
 from quorum_mininode_py.api import LightNodeAPI
 from quorum_mininode_py.client._http import HttpRequest
 from quorum_mininode_py.crypto import account as Account
+from quorum_mininode_py.utils.url import decode_seed_url
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class RumGroup:
     seed: dict = None
@@ -18,17 +18,17 @@
     group_id: str = None
     aes_key: str = None
     encryption_type: str = None
     chain_urls: list = None
 
     def __init__(self, seed_url: str):
         try:
-            info = utils.decode_seed_url(seed_url)
+            info = decode_seed_url(seed_url)
         except KeyError as err:
-            raise ValueError(f"invalid seed_url: {err}")
+            raise ValueError(f"invalid seed_url: {err}") from err
         seed = info["seed"]
         self.seed = seed
         self.seed_url = seed_url
         self.group_id = seed["group_id"]
         self.aes_key = bytes.fromhex(seed["cipher_key"])
         self.encryption_type = seed["encryption_type"]
         self.chain_urls = info["chain_urls"]
@@ -66,15 +66,15 @@
         self.group = RumGroup(seed_url)
         chain_url = self.get_best_http(self.group.chain_urls)
         if chain_url is None:
             raise Exception("no available chain url")
         self.http = HttpRequest(chain_url["baseurl"] + "/api/v1", chain_url["jwt"])
 
         self.account = RumAccount(pvtkey, age_pvtkey, self.group.encryption_type)
-        self.api = LightNodeAPI(self.http, self.group, self.account)
+        self.api = LightNodeAPI(self)
 
     def get_best_http(self, chain_urls):
         headers = {"Content-Type": "application/json"}
         best = None
         for chain_url in chain_urls:
             jwt = chain_url["jwt"]
             headers.update({"Authorization": f"Bearer {jwt}"})
@@ -88,8 +88,8 @@
                 logger.warning("get_best_http error: %s", e)
         return best
 
     def change_account(self, pvtkey, age_pvtkey=None):
         age_pvtkey = age_pvtkey or self.account.age_pvtkey
         if pvtkey != self.account.pvtkey or age_pvtkey != self.account.age_pvtkey:
             self.account = RumAccount(pvtkey, age_pvtkey, self.group.encryption_type)
-            self.api = LightNodeAPI(self.http, self.group, self.account)
+            self.api = LightNodeAPI(self)
```

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/account.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/account.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/aes.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/age.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/age.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/crypto/trx.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/trx.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/proto/quorum_pb2.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/proto/quorum_pb2.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py/utils/url.py` & `quorum_mininode_py-1.2.3/quorum_mininode_py/utils/url.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/PKG-INFO` & `quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-mininode-py
-Version: 1.2.2
+Version: 1.2.3
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.2/quorum_mininode_py.egg-info/SOURCES.txt` & `quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.2/setup.py` & `quorum_mininode_py-1.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_mininode_py",
-    version="1.2.2",
+    version="1.2.3",
     author="liujuanjuan1984, zhangwm404",
     author_email="qiaoanlu@163.com",
     description="a mini python sdk for quorum lightnode with http/https requests to quorum fullnode",
     keywords=["rumsystem", "quorum", "lightnode", "sdk"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_mininode_py",
```

