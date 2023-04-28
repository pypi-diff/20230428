# Comparing `tmp/quorum_mininode_py-1.2.3.tar.gz` & `tmp/quorum_mininode_py-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_mininode_py-1.2.3.tar", last modified: Fri Apr 28 04:10:35 2023, max compression
+gzip compressed data, was "quorum_mininode_py-1.2.4.tar", last modified: Fri Apr 28 04:21:18 2023, max compression
```

## Comparing `quorum_mininode_py-1.2.3.tar` & `quorum_mininode_py-1.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.927155 quorum_mininode_py-1.2.3/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-04-28 04:10:35.926158 quorum_mininode_py-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.882290 quorum_mininode_py-1.2.3/quorum_mininode_py/
--rw-rw-rw-   0        0        0      611 2023-04-28 04:08:49.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.900227 quorum_mininode_py-1.2.3/quorum_mininode_py/api/
--rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/api/__init__.py
--rw-rw-rw-   0        0        0     3703 2023-04-28 04:08:20.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/api/base.py
--rw-rw-rw-   0        0        0     3822 2023-04-06 12:33:18.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/api/lightnode.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.906212 quorum_mininode_py-1.2.3/quorum_mininode_py/client/
--rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1856 2023-04-28 03:47:53.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/client/_http.py
--rw-rw-rw-   0        0        0     3447 2023-04-28 04:04:56.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/client/mininode.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.916197 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/
--rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/__init__.py
--rw-rw-rw-   0        0        0     3094 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/account.py
--rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/aes.py
--rw-rw-rw-   0        0        0     1369 2023-03-30 09:45:11.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/age.py
--rw-rw-rw-   0        0        0     3856 2023-04-06 11:33:57.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/trx.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.919209 quorum_mininode_py-1.2.3/quorum_mininode_py/proto/
--rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/proto/__init__.py
--rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/proto/quorum_pb2.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.924163 quorum_mininode_py-1.2.3/quorum_mininode_py/utils/
--rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/utils/__init__.py
--rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.3/quorum_mininode_py/utils/url.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:10:35.894245 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-28 04:10:35.000000 quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 04:10:35.927155 quorum_mininode_py-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-04-28 04:08:49.000000 quorum_mininode_py-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.173768 quorum_mininode_py-1.2.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2440 2023-04-28 04:21:18.171773 quorum_mininode_py-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.096974 quorum_mininode_py-1.2.4/quorum_mininode_py/
+-rw-rw-rw-   0        0        0      611 2023-04-28 04:19:21.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.113930 quorum_mininode_py-1.2.4/quorum_mininode_py/api/
+-rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     3705 2023-04-28 04:18:02.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/api/base.py
+-rw-rw-rw-   0        0        0     3822 2023-04-06 12:33:18.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/api/lightnode.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.151826 quorum_mininode_py-1.2.4/quorum_mininode_py/client/
+-rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     1858 2023-04-28 04:16:53.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/client/_http.py
+-rw-rw-rw-   0        0        0     3447 2023-04-28 04:04:56.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/client/mininode.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.160803 quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/
+-rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3094 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/account.py
+-rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/aes.py
+-rw-rw-rw-   0        0        0     1369 2023-03-30 09:45:11.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/age.py
+-rw-rw-rw-   0        0        0     3856 2023-04-06 11:33:57.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/trx.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.164792 quorum_mininode_py-1.2.4/quorum_mininode_py/proto/
+-rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/proto/__init__.py
+-rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/proto/quorum_pb2.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.169778 quorum_mininode_py-1.2.4/quorum_mininode_py/utils/
+-rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/utils/__init__.py
+-rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.4/quorum_mininode_py/utils/url.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:21:18.107952 quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/
+-rw-rw-rw-   0        0        0     2440 2023-04-28 04:21:18.000000 quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-28 04:21:18.000000 quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 04:21:18.000000 quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-28 04:21:18.000000 quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-28 04:21:18.000000 quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 04:21:18.174766 quorum_mininode_py-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1301 2023-04-28 04:18:37.000000 quorum_mininode_py-1.2.4/setup.py
```

### Comparing `quorum_mininode_py-1.2.3/LICENSE` & `quorum_mininode_py-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/PKG-INFO` & `quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum_mininode_py
-Version: 1.2.3
+Name: quorum-mininode-py
+Version: 1.2.4
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.3/README.md` & `quorum_mininode_py-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/__init__.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     create_age_keypair,
     create_private_key,
     private_key_to_pubkey,
     public_key_to_address,
 )
 from quorum_mininode_py.utils.url import decode_seed_url, update_seed_url
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __author__ = "liujuanjuan1984, zhangwm404"
 
 # Set default logging handler to avoid "No handler found" warnings.
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 logger.info("Version: %s", __version__)
```

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/api/base.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         self.group_id = client.group.group_id
         self._group = client.group
         self._account = client.account
         self._retry = 0
 
     def _get(self, endpoint: str, payload: dict = None):
         """api _get"""
-        if self._retry > 5:
-            raise Exception("retry 5 times, check your network")
+        if self._retry >= 3:
+            raise Exception("retry 3 times, check your network")
         try:
             resp = self._http.get(endpoint, payload)
         except Exception as err:
             logger.error("request failed: %s", err)
             chain_url = self._client.get_best_http(self._client.group.chain_urls)
             if chain_url is None:
                 raise Exception("no available chain url") from err
@@ -35,16 +35,16 @@
             self._retry += 1
             return self._get(endpoint, payload)
         self._retry = 0
         return resp
 
     def _post(self, endpoint: str, payload: dict = None):
         """api _post"""
-        if self._retry > 5:
-            raise Exception("retry 5 times, check your network")
+        if self._retry >= 3:
+            raise Exception("retry 3 times, check your network")
         try:
             resp = self._http.post(endpoint, payload)
         except Exception as err:
             logger.error("request failed: %s", err)
             chain_url = self._client.get_best_http(self._client.group.chain_urls)
             if chain_url is None:
                 raise Exception("no available chain url") from err
```

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/api/lightnode.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/api/lightnode.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/client/_http.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/client/_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     def _request(
         self,
         method: str,
         endpoint: str,
         payload: dict = None,
     ):
         url = "".join([self.api_base, endpoint])
-        if self.retry_count > 5:
-            raise Exception("retry count > 5, check your network")
+        if self.retry_count >= 3:
+            raise Exception("retry count >=3 , check your network")
         try:
             resp = self.session.request(method=method, url=url, json=payload)
         except Exception as err:
             logger.warning("request error: %s", err)
             self.session = requests.Session()
             self.session.headers.update(self.headers)
             self.retry_count += 1
```

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/client/mininode.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/client/mininode.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/account.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/account.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/aes.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/age.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/age.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/crypto/trx.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/crypto/trx.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/proto/quorum_pb2.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/proto/quorum_pb2.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py/utils/url.py` & `quorum_mininode_py-1.2.4/quorum_mininode_py/utils/url.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/PKG-INFO` & `quorum_mininode_py-1.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum-mininode-py
-Version: 1.2.3
+Name: quorum_mininode_py
+Version: 1.2.4
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.3/quorum_mininode_py.egg-info/SOURCES.txt` & `quorum_mininode_py-1.2.4/quorum_mininode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.3/setup.py` & `quorum_mininode_py-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_mininode_py",
-    version="1.2.3",
+    version="1.2.4",
     author="liujuanjuan1984, zhangwm404",
     author_email="qiaoanlu@163.com",
     description="a mini python sdk for quorum lightnode with http/https requests to quorum fullnode",
     keywords=["rumsystem", "quorum", "lightnode", "sdk"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_mininode_py",
```

