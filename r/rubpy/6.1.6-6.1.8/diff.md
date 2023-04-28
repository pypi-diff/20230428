# Comparing `tmp/rubpy-6.1.6.tar.gz` & `tmp/rubpy-6.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.1.6.tar", last modified: Wed Apr 26 17:37:56 2023, max compression
+gzip compressed data, was "rubpy-6.1.8.tar", last modified: Fri Apr 28 18:38:10 2023, max compression
```

## Comparing `rubpy-6.1.6.tar` & `rubpy-6.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.847161 rubpy-6.1.6/
--rw-rw-rw-   0        0        0     3378 2023-04-26 17:37:56.847161 rubpy-6.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.733400 rubpy-6.1.6/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-26 15:08:14.000000 rubpy-6.1.6/rubpy/__init__.py
--rw-rw-rw-   0        0        0    41309 2023-04-26 17:32:17.000000 rubpy-6.1.6/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.796291 rubpy-6.1.6/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.811914 rubpy-6.1.6/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.6/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.6/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.1.6/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.811914 rubpy-6.1.6/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10949 2023-04-26 14:44:17.000000 rubpy-6.1.6/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.827536 rubpy-6.1.6/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.843153 rubpy-6.1.6/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.6/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.796291 rubpy-6.1.6/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 17:37:56.847161 rubpy-6.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-26 17:32:31.000000 rubpy-6.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.205638 rubpy-6.1.8/
+-rw-rw-rw-   0        0        0     3378 2023-04-28 18:38:10.205638 rubpy-6.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.127544 rubpy-6.1.8/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-28 18:36:18.000000 rubpy-6.1.8/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    41309 2023-04-26 17:32:17.000000 rubpy-6.1.8/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.158784 rubpy-6.1.8/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.174401 rubpy-6.1.8/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.8/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.1.8/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.8/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.1.8/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.190020 rubpy-6.1.8/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    11146 2023-04-28 17:39:40.000000 rubpy-6.1.8/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.190020 rubpy-6.1.8/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.205638 rubpy-6.1.8/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.8/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.8/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:38:10.158784 rubpy-6.1.8/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 18:38:09.000000 rubpy-6.1.8/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:38:10.205638 rubpy-6.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-28 18:33:31.000000 rubpy-6.1.8/setup.py
```

### Comparing `rubpy-6.1.6/PKG-INFO` & `rubpy-6.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.6
+Version: 6.1.8
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.6 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.8 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.6/README.md` & `rubpy-6.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/client.py` & `rubpy-6.1.8/rubpy/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/crypto/crypto.py` & `rubpy-6.1.8/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/gadgets/classino.py` & `rubpy-6.1.8/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/gadgets/exceptions.py` & `rubpy-6.1.8/rubpy/gadgets/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 
 class ClientError(Exception):
     pass
 
 class SocksError(ClientError):
     pass
 
-
 class StopHandler(ClientError):
     pass
 
-
 class CancelledError(ClientError):
     pass
 
 
 class UnknownAuthMethod(SocksError):
     pass
```

### Comparing `rubpy-6.1.6/rubpy/gadgets/grouping.py` & `rubpy-6.1.8/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/gadgets/methods.py` & `rubpy-6.1.8/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/gadgets/thumbnail.py` & `rubpy-6.1.8/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/network/connection.py` & `rubpy-6.1.8/rubpy/network/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import asyncio
 import aiofiles
 import aiohttp
+from random import randint
 from time import time
 from ..crypto import Crypto
 from ..structs import results
 from ..gadgets import exceptions, methods
 
 
 def capitalize(text):
@@ -148,20 +149,23 @@
             request = {'data_enc': Crypto.encrypt(request, key=self._client._key)}
 
         request['tmp_session' if tmp_session else 'auth'] = self._client._auth
 
         if 'api_version' not in request:
             request['api_version'] = self._client.configuire['api_version']
 
+        if not method_urls[0].startswith('https://getdcmess'):
+            method_urls = [method_urls[0]] * 3
+
         for _ in range(self._client._request_retries):
             for url in method_urls:
                 try:
-                    async with self._connection.options(url) as result:
-                        if result.status != 200:
-                            continue
+                    #async with self._connection.options(url) as result:
+                    #    if result.status != 200:
+                    #        continue
 
                     async with self._connection.post(url, json=request) as result:
                         if result.status != 200:
                             continue
 
                         result = await result.json()
                         if result.get('data_enc'):
@@ -279,8 +283,10 @@
                         self._client._logger.error(
                             'websocket raised an exception',
                             extra={'data': url}, exc_info=True)
 
     async def to_keep_alive(self):
         while True:
             await asyncio.sleep(5)
-            await self._client(methods.chats.GetChatsUpdates(state=round(time()) - 200))
+            try:
+                await self._client(methods.chats.GetChatsUpdates(state=round(time()) - 200))
+            except: continue
```

### Comparing `rubpy-6.1.6/rubpy/network/proxies.py` & `rubpy-6.1.8/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/sessions/sqliteSession.py` & `rubpy-6.1.8/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/sessions/stringSession.py` & `rubpy-6.1.8/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/structs/handlers.py` & `rubpy-6.1.8/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/structs/models.py` & `rubpy-6.1.8/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/structs/results.py` & `rubpy-6.1.8/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy/structs/struct.py` & `rubpy-6.1.8/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/rubpy.egg-info/PKG-INFO` & `rubpy-6.1.8/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.6
+Version: 6.1.8
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.6 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.8 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.6/rubpy.egg-info/SOURCES.txt` & `rubpy-6.1.8/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.6/setup.py` & `rubpy-6.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.1.6',
+    version = '6.1.8',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

