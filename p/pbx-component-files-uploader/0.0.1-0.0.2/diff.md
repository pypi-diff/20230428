# Comparing `tmp/pbx-component-files-uploader-0.0.1.tar.gz` & `tmp/pbx_component_files_uploader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbx-component-files-uploader-0.0.1.tar", max compression
+gzip compressed data, was "pbx_component_files_uploader-0.0.2.tar", max compression
```

## Comparing `pbx-component-files-uploader-0.0.1.tar` & `pbx_component_files_uploader-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1091 2022-01-24 09:20:19.425531 pbx-component-files-uploader-0.0.1/LICENSE
--rw-r--r--   0        0        0       23 2022-01-24 11:55:11.639481 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/__init__.py
--rw-r--r--   0        0        0      518 2022-01-25 12:35:01.185391 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/exceptions/errors.py
--rw-r--r--   0        0        0     2200 2022-01-26 14:30:55.271335 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/ext/selectel/auth.py
--rw-r--r--   0        0        0     1988 2022-01-26 14:30:57.992813 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/ext/selectel/selectel.py
--rw-r--r--   0        0        0     1658 2022-01-26 14:32:08.638558 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/ext/selectel/token.py
--rw-r--r--   0        0        0      416 2022-01-24 12:34:19.547710 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/interfaces/base_uploader.py
--rw-r--r--   0        0        0      801 2022-01-26 07:09:36.893235 pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/uploader.py
--rw-r--r--   0        0        0      660 2022-01-26 14:35:08.875787 pbx-component-files-uploader-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      417 2022-01-26 14:33:44.774088 pbx-component-files-uploader-0.0.1/README.md
--rw-r--r--   0        0        0     1262 2022-01-26 14:35:47.207672 pbx-component-files-uploader-0.0.1/setup.py
--rw-r--r--   0        0        0     1206 2022-01-26 14:35:47.207672 pbx-component-files-uploader-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/LICENSE
+-rw-r--r--   0        0        0      427 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-28 07:55:18.616871 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/__init__.py
+-rw-r--r--   0        0        0      491 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/exceptions/errors.py
+-rw-r--r--   0        0        0     2141 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/auth.py
+-rw-r--r--   0        0        0     2045 2023-04-28 08:11:14.105329 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/selectel.py
+-rw-r--r--   0        0        0     1610 2023-04-28 07:56:24.891596 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/token.py
+-rw-r--r--   0        0        0      402 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/interfaces/base_uploader.py
+-rw-r--r--   0        0        0      799 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/uploader.py
+-rw-r--r--   0        0        0      638 2023-04-28 07:57:01.522893 pbx_component_files_uploader-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pbx_component_files_uploader-0.0.2/PKG-INFO
```

### Comparing `pbx-component-files-uploader-0.0.1/LICENSE` & `pbx_component_files_uploader-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/ext/selectel/auth.py` & `pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/auth.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import time
-from logging import Logger
-from pbx_component_files_uploader.exceptions.errors import EmptyAuthField
-from .token import Token
-
-import requests
-
-
-class Auth:
-    AUTH_URL = 'https://auth.selcdn.ru/'
-
-    def __init__(self, authData: dict, tokenCacheDir: str, requests: requests, logger: Logger):
-        self.tokenCacheDir = tokenCacheDir
-        if not tokenCacheDir:
-            raise EmptyAuthField('token_cache_dir')
-        self.check_auth_data(authData=authData)
-        self.username = authData.get('username', '')
-        self.password = authData.get('password', '')
-        self.container = authData.get('container', '')
-
-        self.requests = requests
-        self.logger = logger
-        self.token = Token(tokenCacheDir=tokenCacheDir, logger=logger).load()
-
-    def check_auth_data(self, authData: dict) -> None:
-        for k, v in authData.items():
-            if not v:
-                raise EmptyAuthField(k)
-
-    def update_auth_token(self, new_token, storage_url, expires):
-        self.token.secret = new_token
-        self.token.storageUrl = storage_url
-        self.token.expiresAt = int(time.time()) + int(expires)
-        self.token.update()
-
-    def authenticate(self):
-        self.logger.debug('Need to authenticate with %s:%s',
-                          self.username, self.password)
-        resp = self.requests.get(self.AUTH_URL, headers={
-            'X-Auth-User': self.username,
-            'X-Auth-Key': self.password
-        })
-        if resp.status_code != 204:
-            self.logger.debug(
-                'Got an unexpected response from auth: %s', resp.content)
-            raise Exception("Selectel: Unexpected status code: %s" %
-                            resp.status_code)
-        self.update_auth_token(
-            resp.headers['X-Auth-Token'], resp.headers['X-Storage-Url'], resp.headers['X-Expire-Auth-Token'])
-
-    def get_storage_data(self) -> dict:
-        if self.token.is_expired():
-            self.authenticate()
-
-        return {
-            'secret': self.token.secret,
-            'storage_url': self.token.storageUrl,
-            'container': self.container
-        }
+import time
+from logging import Logger
+from pbx_component_files_uploader.exceptions.errors import EmptyAuthField
+from .token import Token
+
+import requests
+
+
+class Auth:
+    AUTH_URL = 'https://auth.selcdn.ru/'
+
+    def __init__(self, authData: dict, tokenCacheDir: str, requests: requests, logger: Logger):
+        self.tokenCacheDir = tokenCacheDir
+        if not tokenCacheDir:
+            raise EmptyAuthField('token_cache_dir')
+        self.check_auth_data(authData=authData)
+        self.username = authData.get('username', '')
+        self.password = authData.get('password', '')
+        self.container = authData.get('container', '')
+
+        self.requests = requests
+        self.logger = logger
+        self.token = Token(tokenCacheDir=tokenCacheDir, logger=logger).load()
+
+    def check_auth_data(self, authData: dict) -> None:
+        for k, v in authData.items():
+            if not v:
+                raise EmptyAuthField(k)
+
+    def update_auth_token(self, new_token, storage_url, expires):
+        self.token.secret = new_token
+        self.token.storageUrl = storage_url
+        self.token.expiresAt = int(time.time()) + int(expires)
+        self.token.update()
+
+    def authenticate(self):
+        self.logger.debug('Need to authenticate with %s:%s',
+                          self.username, self.password)
+        resp = self.requests.get(self.AUTH_URL, headers={
+            'X-Auth-User': self.username,
+            'X-Auth-Key': self.password
+        })
+        if resp.status_code != 204:
+            self.logger.debug(
+                'Got an unexpected response from auth: %s', resp.content)
+            raise Exception("Selectel: Unexpected status code: %s" %
+                            resp.status_code)
+        self.update_auth_token(
+            resp.headers['X-Auth-Token'], resp.headers['X-Storage-Url'], resp.headers['X-Expire-Auth-Token'])
+
+    def get_storage_data(self) -> dict:
+        if self.token.is_expired():
+            self.authenticate()
+
+        return {
+            'secret': self.token.secret,
+            'storage_url': self.token.storageUrl,
+            'container': self.container
+        }
```

### Comparing `pbx-component-files-uploader-0.0.1/pbx_component_files_uploader/ext/selectel/selectel.py` & `pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/selectel.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         srcFile = Path(srcFilePath)
         if not srcFile.is_file():
             raise ValueError(f'No such file [{srcFilePath}]')
 
         if not dstFileName:
             raise ValueError('Empty [dstFileName] field')
 
+        errorDesc = ''
         for i in range(self.DEFAULT_RETRIES):
             try:
                 storageData = self.auth.get_storage_data()
 
                 headers = {
                     'X-Auth-Token': storageData.get('secret')
                 }
@@ -46,11 +47,11 @@
 
                 response = requests.put(
                     url=url, data=srcFile.open(mode='rb'), headers=headers)
 
                 if response.status_code == 201:
                     return response.url
             except Exception as e:
-                log.debug(
-                    f'Attempt [{i + 1}]. Failed to upload. Cause [{e.__cause__}]')
+                log.debug(f'Attempt [{i + 1}]. Failed to upload. Cause [{e.__cause__}]')
+                errorDesc = str(e)
 
-        raise UploadError(400, f'Failed upload file [{srcFilePath}]')
+        raise UploadError(400, f'Failed upload file [{srcFilePath}]. Cause [{errorDesc}]')
```

### Comparing `pbx-component-files-uploader-0.0.1/PKG-INFO` & `pbx_component_files_uploader-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: pbx-component-files-uploader
-Version: 0.0.1
+Version: 0.0.2
 Summary: Files uploader to custom storages
 Home-page: https://github.com/leadvertex/pbx-component-files-uploader
 License: MIT
 Keywords: leadvertex,selectel,storage,remote storage,uploader
 Author: Ivan Kalashnikov
 Author-email: ivan@leadvertex.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (==2.27.1)
 Project-URL: Repository, https://github.com/leadvertex/pbx-component-files-uploader
 Description-Content-Type: text/markdown
 
 # pbx-lv2-records-uploader
 
 Simple selectel upload
 
 ```python
+    from pbx_component_files_uploader.uploader import Uploader
+
     api = Uploader(Uploader.SERVICE_SELECTEL, {
         'username': 'user',
         'password': 'pass',
         'container': 'container_name'
     }, {
         'token_cache_dir': '/path/to/cache/dir'
     })
 
     uploadedFileUrl = api.upload(
         '/path/to/src/file', 'dst_folder/dst_filename')
-        
-    print(uploadedFileUrl)
 ```
```

