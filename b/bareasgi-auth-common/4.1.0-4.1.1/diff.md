# Comparing `tmp/bareasgi_auth_common-4.1.0.tar.gz` & `tmp/bareasgi_auth_common-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareasgi_auth_common-4.1.0.tar", max compression
+gzip compressed data, was "bareasgi_auth_common-4.1.1.tar", max compression
```

## Comparing `bareasgi_auth_common-4.1.0.tar` & `bareasgi_auth_common-4.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11356 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.0/LICENSE
--rw-r--r--   0        0        0       69 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.0/README.md
--rw-r--r--   0        0        0      762 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/__init__.py
--rw-r--r--   0        0        0     2030 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/helpers.py
--rw-r--r--   0        0        0     8924 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/http_jwt_authenticator.py
--rw-r--r--   0        0        0       10 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.0/bareasgi_auth_common/py.typed
--rw-r--r--   0        0        0     5696 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/token_manager.py
--rw-r--r--   0        0        0     2583 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/types.py
--rw-r--r--   0        0        0     1134 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/utils.py
--rw-r--r--   0        0        0     4231 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/websocket_jwt_authenticator.py
--rw-r--r--   0        0        0      580 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 bareasgi_auth_common-4.1.0/setup.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 bareasgi_auth_common-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.1/LICENSE
+-rw-r--r--   0        0        0       69 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.1/README.md
+-rw-r--r--   0        0        0      762 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.1/bareasgi_auth_common/__init__.py
+-rw-r--r--   0        0        0     2030 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.1/bareasgi_auth_common/helpers.py
+-rw-r--r--   0        0        0     9010 2023-04-28 10:29:32.797600 bareasgi_auth_common-4.1.1/bareasgi_auth_common/http_jwt_authenticator.py
+-rw-r--r--   0        0        0       10 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.1/bareasgi_auth_common/py.typed
+-rw-r--r--   0        0        0     5696 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.1/bareasgi_auth_common/token_manager.py
+-rw-r--r--   0        0        0     2673 2023-04-28 10:30:23.502925 bareasgi_auth_common-4.1.1/bareasgi_auth_common/types.py
+-rw-r--r--   0        0        0      896 2023-04-28 10:28:43.332298 bareasgi_auth_common-4.1.1/bareasgi_auth_common/utils.py
+-rw-r--r--   0        0        0     4242 2023-04-28 10:25:44.759494 bareasgi_auth_common-4.1.1/bareasgi_auth_common/websocket_jwt_authenticator.py
+-rw-r--r--   0        0        0      580 2023-04-28 10:30:40.971379 bareasgi_auth_common-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 bareasgi_auth_common-4.1.1/setup.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 bareasgi_auth_common-4.1.1/PKG-INFO
```

### Comparing `bareasgi_auth_common-4.1.0/LICENSE` & `bareasgi_auth_common-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bareasgi_auth_common-4.1.0/bareasgi_auth_common/__init__.py` & `bareasgi_auth_common-4.1.1/bareasgi_auth_common/__init__.py`

 * *Files identical despite different names*

### Comparing `bareasgi_auth_common-4.1.0/bareasgi_auth_common/helpers.py` & `bareasgi_auth_common-4.1.1/bareasgi_auth_common/helpers.py`

 * *Files identical despite different names*

### Comparing `bareasgi_auth_common-4.1.0/bareasgi_auth_common/http_jwt_authenticator.py` & `bareasgi_auth_common-4.1.1/bareasgi_auth_common/http_jwt_authenticator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .token_manager import TokenManager
 from .types import (
     TokenStatus,
     BareASGIHttpError,
     UnauthorizedHttpError,
     ForbiddenHttpError
 )
-from .utils import get_http_scheme, get_host
+from .utils import get_scheme, get_host
 
 LOGGER = logging.getLogger(__name__)
 
 
 class HttpJwtAuthenticator(TokenManager):
     """JTW authentication middleware"""
 
@@ -69,16 +69,16 @@
 
     async def _renew_cookie(
             self,
             request: HttpRequest,
             token: bytes
     ) -> Optional[Mapping[str, Any]]:
 
-        host = get_host(request)
-        scheme = get_http_scheme(request)
+        host = get_host(request.scope['headers'])
+        scheme = get_scheme(request.scope['headers'], request.scope['scheme'])
         base_url = f'{scheme}://{host.decode("ascii")}'
 
         referer_url = base_url + request.scope["path"]
         if request.scope['query_string']:
             referer_url += '?' + request.scope['query_string'].decode('utf-8')
         referer = header.find(
             b'referer',
@@ -140,15 +140,15 @@
             LOGGER.debug("No path for authentication redirect")
             raise UnauthorizedHttpError(request, "Cannot authorize")
 
         path = request.scope['path']
         if request.scope['query_string']:
             path += '?' + request.scope['query_string'].decode()
 
-        scheme = get_http_scheme(request)
+        scheme = get_scheme(request.scope['headers'], request.scope['scheme'])
         host = get_host(request.scope['headers']).decode('ascii')
         base_url = f'{scheme}://{host}'
 
         redirect_url = base_url+path
         query_string = urlencode([('redirect', redirect_url)])
         location = base_url + self.authentication_path + '?' + query_string
         return location.encode()
```

### Comparing `bareasgi_auth_common-4.1.0/bareasgi_auth_common/token_manager.py` & `bareasgi_auth_common-4.1.1/bareasgi_auth_common/token_manager.py`

 * *Files identical despite different names*

### Comparing `bareasgi_auth_common-4.1.0/bareasgi_auth_common/types.py` & `bareasgi_auth_common-4.1.1/bareasgi_auth_common/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from enum import Enum, auto
 from typing import List, Optional, Tuple
 
 from bareasgi import HttpRequest, WebSocketRequest
 import bareutils.response_code as response_code
 
-from .utils import get_host, get_http_scheme, get_ws_scheme
+from .utils import get_host, get_scheme
 
 
 class TokenStatus(Enum):
     """The token status"""
     VALID = auto()
     EXPIRED = auto()
     INVALID = auto()
@@ -23,16 +23,16 @@
             self,
             request: HttpRequest,
             status: int,
             headers: Optional[List[Tuple[bytes, bytes]]],
             message: Optional[str]
     ) -> None:
         super().__init__(message)
-        host = get_host(request).decode('ascii')
-        scheme = get_http_scheme(request)
+        host = get_host(request.scope['headers']).decode('ascii')
+        scheme = get_scheme(request.scope['headers'], request.scope['scheme'])
         self.url = f'{scheme}://{host}{request.scope["path"]}'
         self.status = status
         self.headers = headers
         self.message = message
 
 
 class ForbiddenHttpError(BareASGIHttpError):
@@ -63,16 +63,16 @@
             self,
             request: WebSocketRequest,
             status: int,
             headers: Optional[List[Tuple[bytes, bytes]]],
             message: Optional[str]
     ) -> None:
         super().__init__(message)
-        host = get_host(request).decode('ascii')
-        scheme = get_ws_scheme(request)
+        host = get_host(request.scope['headers']).decode('ascii')
+        scheme = get_scheme(request.scope['headers'], request.scope['scheme'])
         self.url = f'{scheme}://{host}{request.scope["path"]}'
         self.status = status
         self.headers = headers
         self.message = message
 
 
 class ForbiddenWebSocketError(BareASGIWebSocketError):
```

### Comparing `bareasgi_auth_common-4.1.0/bareasgi_auth_common/websocket_jwt_authenticator.py` & `bareasgi_auth_common-4.1.1/bareasgi_auth_common/websocket_jwt_authenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,19 +75,19 @@
         Raises:
             UnauthorizedWebSocketError: For unauthorized requests.
             ForbiddenWebSocketError: For forbidden requests.
 
         Returns:
             bytes: The token.
         """
-        token = self.get_token_from_headers(request)
+        token = self.get_token_from_headers(request.scope['headers'])
         if token_status == TokenStatus.VALID:
             LOGGER.debug('Cookie still valid')
             assert token is not None
-            return token, None
+            return token
 
         if token_status == TokenStatus.EXPIRED and token is not None:
             raise UnauthorizedWebSocketError(request, "Expired cookie")
 
         LOGGER.warning('The token was invalid')
         raise ForbiddenWebSocketError(request, 'Invalid cookie')
```

### Comparing `bareasgi_auth_common-4.1.0/pyproject.toml` & `bareasgi_auth_common-4.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bareASGI-auth-common"
-version = "4.1.0"
+version = "4.1.1"
 description = ""
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "bareasgi_auth_common" },
 ]
```

### Comparing `bareasgi_auth_common-4.1.0/setup.py` & `bareasgi_auth_common-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=2.6,<3.0', 'bareasgi>=4.4,<5.0', 'bareclient>=5.0,<6.0']
 
 setup_kwargs = {
     'name': 'bareasgi-auth-common',
-    'version': '4.1.0',
+    'version': '4.1.1',
     'description': '',
     'long_description': '# bareASGI-auth-common\n\nCommon code for authentication with bareASGI.',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rob-blackbourn/bareASGI-auth-common',
```

### Comparing `bareasgi_auth_common-4.1.0/PKG-INFO` & `bareasgi_auth_common-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareasgi-auth-common
-Version: 4.1.0
+Version: 4.1.1
 Summary: 
 Home-page: https://github.com/rob-blackbourn/bareASGI-auth-common
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

