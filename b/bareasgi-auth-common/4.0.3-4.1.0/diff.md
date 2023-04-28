# Comparing `tmp/bareASGI-auth-common-4.0.3.tar.gz` & `tmp/bareasgi_auth_common-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareASGI-auth-common-4.0.3.tar", max compression
+gzip compressed data, was "bareasgi_auth_common-4.1.0.tar", max compression
```

## Comparing `bareASGI-auth-common-4.0.3.tar` & `bareasgi_auth_common-4.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11356 2021-08-16 13:49:38.650078 bareASGI-auth-common-4.0.3/LICENSE
--rw-r--r--   0        0        0       69 2021-08-16 13:49:38.650078 bareASGI-auth-common-4.0.3/README.md
--rw-r--r--   0        0        0      421 2021-10-22 10:53:03.082757 bareASGI-auth-common-4.0.3/bareasgi_auth_common/__init__.py
--rw-r--r--   0        0        0     1679 2021-10-22 10:53:03.082757 bareASGI-auth-common-4.0.3/bareasgi_auth_common/helpers.py
--rw-r--r--   0        0        0     8183 2021-11-15 12:48:13.064044 bareASGI-auth-common-4.0.3/bareasgi_auth_common/jwt_authenticator.py
--rw-r--r--   0        0        0       10 2021-10-22 10:49:35.918440 bareASGI-auth-common-4.0.3/bareasgi_auth_common/py.typed
--rw-r--r--   0        0        0     5492 2021-10-22 15:25:43.663467 bareASGI-auth-common-4.0.3/bareasgi_auth_common/token_manager.py
--rw-r--r--   0        0        0     1372 2021-10-22 10:53:03.086757 bareASGI-auth-common-4.0.3/bareasgi_auth_common/types.py
--rw-r--r--   0        0        0      850 2021-10-22 10:53:03.086757 bareASGI-auth-common-4.0.3/bareasgi_auth_common/utils.py
--rw-r--r--   0        0        0      583 2021-11-15 12:48:19.932207 bareASGI-auth-common-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      778 2021-11-15 12:48:25.698978 bareASGI-auth-common-4.0.3/setup.py
--rw-r--r--   0        0        0      762 2021-11-15 12:48:25.699347 bareASGI-auth-common-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.0/LICENSE
+-rw-r--r--   0        0        0       69 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.0/README.md
+-rw-r--r--   0        0        0      762 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/__init__.py
+-rw-r--r--   0        0        0     2030 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/helpers.py
+-rw-r--r--   0        0        0     8924 2023-04-28 10:20:07.887269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/http_jwt_authenticator.py
+-rw-r--r--   0        0        0       10 2023-04-28 09:19:46.001395 bareasgi_auth_common-4.1.0/bareasgi_auth_common/py.typed
+-rw-r--r--   0        0        0     5696 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/token_manager.py
+-rw-r--r--   0        0        0     2583 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/types.py
+-rw-r--r--   0        0        0     1134 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/utils.py
+-rw-r--r--   0        0        0     4231 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/bareasgi_auth_common/websocket_jwt_authenticator.py
+-rw-r--r--   0        0        0      580 2023-04-28 10:20:07.891269 bareasgi_auth_common-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 bareasgi_auth_common-4.1.0/setup.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 bareasgi_auth_common-4.1.0/PKG-INFO
```

### Comparing `bareASGI-auth-common-4.0.3/LICENSE` & `bareasgi_auth_common-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bareASGI-auth-common-4.0.3/bareasgi_auth_common/helpers.py` & `bareasgi_auth_common-4.1.0/bareasgi_auth_common/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Helper functions"""
 
 from datetime import timedelta
 from typing import Optional, Sequence
 
 from bareasgi import Application
 
-from .jwt_authenticator import JwtAuthenticator
+from .http_jwt_authenticator import HttpJwtAuthenticator
+from .websocket_jwt_authenticator import WebSocketJwtAuthenticator
 
 
 def add_jwt_auth_middleware(
         app: Application,
         secret: str,
         lease_expiry: timedelta,
         issuer: str,
@@ -37,21 +38,34 @@
             path. Defaults to None.
         whitelist (Sequence[str], optional): Routes for which
             authentication is not required. Defaults to None.
 
     Returns:
         Application: The ASGI application.
     """
-    jwt_authenticator = JwtAuthenticator(
+    http_jwt_authenticator = HttpJwtAuthenticator(
         secret,
         lease_expiry,
         issuer,
         cookie_name,
         domain,
         path,
         session_expiry,
         token_renewal_path,
         authentication_path,
         whitelist
     )
-    app.middlewares.append(jwt_authenticator)
+    app.middlewares.append(http_jwt_authenticator)
+
+    ws_jwt_authenticator = WebSocketJwtAuthenticator(
+        secret,
+        lease_expiry,
+        issuer,
+        cookie_name,
+        domain,
+        path,
+        session_expiry,
+        whitelist
+    )
+    app.ws_middlewares.append(ws_jwt_authenticator)
+
     return app
```

### Comparing `bareASGI-auth-common-4.0.3/bareasgi_auth_common/jwt_authenticator.py` & `bareasgi_auth_common-4.1.0/bareasgi_auth_common/http_jwt_authenticator.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 from urllib.parse import urlencode
 
 from bareasgi import HttpRequest, HttpRequestCallback, HttpResponse, text_writer
 from bareclient import HttpClient
 from bareutils import header, response_code, encode_set_cookie
 
 from .token_manager import TokenManager
-from .types import TokenStatus, BareASGIError, UnauthorizedError, ForbiddenError
-from .utils import get_scheme, get_host
+from .types import (
+    TokenStatus,
+    BareASGIHttpError,
+    UnauthorizedHttpError,
+    ForbiddenHttpError
+)
+from .utils import get_http_scheme, get_host
 
 LOGGER = logging.getLogger(__name__)
 
 
-class JwtAuthenticator(TokenManager):
+class HttpJwtAuthenticator(TokenManager):
     """JTW authentication middleware"""
 
     def __init__(
             self,
             secret: str,
             lease_expiry: timedelta,
             issuer: str,
@@ -65,15 +70,16 @@
     async def _renew_cookie(
             self,
             request: HttpRequest,
             token: bytes
     ) -> Optional[Mapping[str, Any]]:
 
         host = get_host(request)
-        base_url = f'{get_scheme(request)}://{host.decode("ascii")}'
+        scheme = get_http_scheme(request)
+        base_url = f'{scheme}://{host.decode("ascii")}'
 
         referer_url = base_url + request.scope["path"]
         if request.scope['query_string']:
             referer_url += '?' + request.scope['query_string'].decode('utf-8')
         referer = header.find(
             b'referer',
             request.scope['headers'],
@@ -123,27 +129,27 @@
             else:
                 LOGGER.debug(
                     "Received unhandled response code %s",
                     response.status
                 )
 
         LOGGER.debug('Cookie not renewed - failed to authenticate')
-        raise UnauthorizedError(request, 'Failed to authenticate')
+        raise UnauthorizedHttpError(request, 'Failed to authenticate')
 
     def _make_authenticate_location(self, request: HttpRequest) -> bytes:
         if self.authentication_path is None:
             LOGGER.debug("No path for authentication redirect")
-            raise UnauthorizedError(request, "Cannot authorize")
+            raise UnauthorizedHttpError(request, "Cannot authorize")
 
         path = request.scope['path']
         if request.scope['query_string']:
             path += '?' + request.scope['query_string'].decode()
 
-        scheme = get_scheme(request)
-        host = get_host(request).decode('ascii')
+        scheme = get_http_scheme(request)
+        host = get_host(request.scope['headers']).decode('ascii')
         base_url = f'{scheme}://{host}'
 
         redirect_url = base_url+path
         query_string = urlencode([('redirect', redirect_url)])
         location = base_url + self.authentication_path + '?' + query_string
         return location.encode()
 
@@ -154,43 +160,56 @@
         return False
 
     async def get_token_and_cookie(
             self,
             request: HttpRequest,
             token_status: TokenStatus
     ) -> Tuple[bytes, Optional[bytes]]:
-        token = self.get_token_from_headers(request)
+        """Get the token and the cookie
+
+        Args:
+            request (HttpRequest): The request.
+            token_status (TokenStatus): The token status.
+
+        Raises:
+            UnauthorizedHttpError: For unauthorized requests.
+            ForbiddenHttpError: For forbidden requests.
+
+        Returns:
+            Tuple[bytes, Optional[bytes]]: The token and the cookie.
+        """
+        token = self.get_token_from_headers(request.scope['headers'])
         if token_status == TokenStatus.VALID:
             LOGGER.debug('Cookie still valid')
             assert token is not None
             return token, None
 
         if token_status == TokenStatus.EXPIRED and token is not None:
             LOGGER.debug('Attempting to renew cookie')
 
             cookie_kwargs = await self._renew_cookie(request, token)
             if cookie_kwargs is None:
                 LOGGER.debug("Unable to renew cookie")
-                raise UnauthorizedError(request, 'Unable to renew cookie')
+                raise UnauthorizedHttpError(request, 'Unable to renew cookie')
 
             token = cast(bytes, cookie_kwargs['value'])
             cookie = encode_set_cookie(**cookie_kwargs)
             return token, cookie
 
         LOGGER.warning('The token was invalid')
-        raise ForbiddenError(request, 'Invalid cookie')
+        raise ForbiddenHttpError(request, 'Invalid cookie')
 
     async def _handle_authentication(
             self,
             request: HttpRequest,
             handler: HttpRequestCallback
     ) -> HttpResponse:
         LOGGER.debug("Handling authentication request")
         try:
-            token = self.get_token_from_headers(request)
+            token = self.get_token_from_headers(request.scope['headers'])
             token_status = self.get_token_status(token)
 
             if token_status == TokenStatus.MISSING:
                 LOGGER.debug("No token - redirecting for authentication")
                 headers = [
                     (b'location', self._make_authenticate_location(request))
                 ]
@@ -205,33 +224,40 @@
             if cookie:
                 if response.headers is None:
                     response.headers = []
                 response.headers.append((b"set-cookie", cookie))
 
             return response
 
-        except BareASGIError as error:
+        except BareASGIHttpError as error:
             return HttpResponse(
                 error.status,
                 error.headers,
                 text_writer(error.message) if error.message else None
             )
         except:  # pylint: disable=bare-except
             LOGGER.exception("JWT authentication failed")
             raise
 
+    async def _handle_whitelisted(
+            self,
+            request: HttpRequest,
+            handler: HttpRequestCallback
+    ) -> HttpResponse:
+        LOGGER.debug(
+            'The path is whitelisted: "%s"',
+            request.scope['path']
+        )
+        return await handler(request)
+
     async def __call__(
             self,
             request: HttpRequest,
             handler: HttpRequestCallback
     ) -> HttpResponse:
 
         LOGGER.debug('Jwt Authentication Request: %s', request.scope["path"])
 
         if self._is_whitelisted(request.scope['path']):
-            LOGGER.debug(
-                'The path is whitelisted: "%s"',
-                request.scope['path']
-            )
-            return await handler(request)
+            return await self._handle_whitelisted(request, handler)
         else:
             return await self._handle_authentication(request, handler)
```

### Comparing `bareASGI-auth-common-4.0.3/bareasgi_auth_common/token_manager.py` & `bareasgi_auth_common-4.1.0/bareasgi_auth_common/token_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Token Manager"""
 
 from datetime import datetime, timedelta
 import logging
-from typing import Any, Mapping, Optional
+from typing import Any, Iterable, Mapping, Optional, Tuple
 
-from bareasgi.http.http_request import HttpRequest
 from bareutils import encode_set_cookie, header
 import jwt
 
 from .types import TokenStatus
 
 LOGGER = logging.getLogger(__name__)
 
@@ -95,46 +94,46 @@
         )
         payload['exp'] = datetime.utcfromtimestamp(payload['exp'])
         payload['iat'] = datetime.utcfromtimestamp(payload['iat'])
         return payload
 
     def get_token_from_headers(
             self,
-            request: HttpRequest
+            headers: Iterable[Tuple[bytes, bytes]]
     ) -> Optional[bytes]:
         """Gets the token from the headers if present.
 
         Args:
-            request (HttpRequest): The request
+            headers (Iterable[Tuple[bytes, bytes]]): The headers
 
         Returns:
             Optional[bytes]: The token or None if not found.
         """
-        tokens = header.cookie(request.scope['headers']).get(self.cookie_name)
+        tokens = header.cookie(headers).get(self.cookie_name)
         if tokens is None or not tokens:
             return None
         if len(tokens) > 1:
             LOGGER.warning('Multiple tokens in header - using first')
         token = tokens[0]
         return token
 
     def get_jwt_payload_from_headers(
             self,
-            request: HttpRequest
+            headers: Iterable[Tuple[bytes, bytes]]
     ) -> Optional[Mapping[str, Any]]:
         """Gets the payload of the JSON web token from the headers
 
         Args:
-            request (HttpRequest): The headers
+            headers (Iterable[Tuple[bytes, bytes]]): The headers
 
         Returns:
             Optional[Mapping[str, Any]]: The payload of the JSON web token if
                 present; otherwise None.
         """
-        token = self.get_token_from_headers(request)
+        token = self.get_token_from_headers(headers)
         payload = self.decode(token) if token is not None else None
         return payload
 
     def generate_cookie(self, user: str) -> bytes:
         """Generate a new cookie
 
         Args:
@@ -163,14 +162,22 @@
             domain=self.domain,
             path=self.path,
             http_only=True
         )
         return cookie
 
     def get_token_status(self, token: Optional[bytes]) -> TokenStatus:
+        """Get the status of the token.
+
+        Args:
+            token (Optional[bytes]): The token.
+
+        Returns:
+            TokenStatus: The status of the token.
+        """
         try:
             if token is None:
                 LOGGER.debug('Token missing')
                 return TokenStatus.MISSING
 
             now = datetime.utcnow()
```

### Comparing `bareASGI-auth-common-4.0.3/bareasgi_auth_common/types.py` & `bareasgi_auth_common-4.1.0/bareasgi_auth_common/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,97 @@
 """Types"""
 
 from enum import Enum, auto
 from typing import List, Optional, Tuple
 
-from bareasgi import HttpRequest
+from bareasgi import HttpRequest, WebSocketRequest
 import bareutils.response_code as response_code
 
-from .utils import get_host, get_scheme
+from .utils import get_host, get_http_scheme, get_ws_scheme
 
 
 class TokenStatus(Enum):
+    """The token status"""
     VALID = auto()
     EXPIRED = auto()
     INVALID = auto()
     MISSING = auto()
 
 
-class BareASGIError(Exception):
+class BareASGIHttpError(Exception):
 
     def __init__(
             self,
             request: HttpRequest,
             status: int,
             headers: Optional[List[Tuple[bytes, bytes]]],
             message: Optional[str]
     ) -> None:
         super().__init__(message)
         host = get_host(request).decode('ascii')
-        scheme = get_scheme(request)
+        scheme = get_http_scheme(request)
         self.url = f'{scheme}://{host}{request.scope["path"]}'
         self.status = status
         self.headers = headers
         self.message = message
 
 
-class ForbiddenError(BareASGIError):
+class ForbiddenHttpError(BareASGIHttpError):
 
     def __init__(self, request: HttpRequest, message: str) -> None:
         super().__init__(
             request,
             response_code.FORBIDDEN,
             [(b'content_type', b'text/plain')],
             message
         )
 
 
-class UnauthorizedError(BareASGIError):
+class UnauthorizedHttpError(BareASGIHttpError):
 
     def __init__(self, request: HttpRequest, message: str) -> None:
         super().__init__(
             request,
             response_code.UNAUTHORIZED,
             [(b'content_type', b'text/plain')],
             message
         )
+
+
+class BareASGIWebSocketError(Exception):
+
+    def __init__(
+            self,
+            request: WebSocketRequest,
+            status: int,
+            headers: Optional[List[Tuple[bytes, bytes]]],
+            message: Optional[str]
+    ) -> None:
+        super().__init__(message)
+        host = get_host(request).decode('ascii')
+        scheme = get_ws_scheme(request)
+        self.url = f'{scheme}://{host}{request.scope["path"]}'
+        self.status = status
+        self.headers = headers
+        self.message = message
+
+
+class ForbiddenWebSocketError(BareASGIWebSocketError):
+
+    def __init__(self, request: WebSocketRequest, message: str) -> None:
+        super().__init__(
+            request,
+            response_code.FORBIDDEN,
+            [(b'content_type', b'text/plain')],
+            message
+        )
+
+
+class UnauthorizedWebSocketError(BareASGIWebSocketError):
+
+    def __init__(self, request: WebSocketRequest, message: str) -> None:
+        super().__init__(
+            request,
+            response_code.UNAUTHORIZED,
+            [(b'content_type', b'text/plain')],
+            message
+        )
```

### Comparing `bareASGI-auth-common-4.0.3/bareasgi_auth_common/utils.py` & `bareasgi_auth_common-4.1.0/bareasgi_auth_common/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilities"""
 
 from typing import Iterable, Optional, Tuple
 
-from bareasgi import HttpRequest
+from bareasgi import HttpRequest, WebSocketRequest
 
 
 def _find_first_header(
     names: Iterable[bytes],
     headers: Iterable[Tuple[bytes, bytes]],
     default: Optional[bytes] = None
 ) -> Optional[bytes]:
@@ -22,15 +22,26 @@
         (b'x-forwarded-host', b'host'),
         request.scope['headers']
     )
     assert host is not None
     return host
 
 
-def get_scheme(request: HttpRequest) -> str:
+def get_http_scheme(request: HttpRequest) -> str:
+    scheme = _find_first_header(
+        (b'x-forwarded-proto',),
+        request.scope['headers']
+    )
+    if scheme is not None:
+        return scheme.decode('ascii')
+
+    return request.scope['scheme']
+
+
+def get_ws_scheme(request: WebSocketRequest) -> str:
     scheme = _find_first_header(
         (b'x-forwarded-proto',),
         request.scope['headers']
     )
     if scheme is not None:
         return scheme.decode('ascii')
```

### Comparing `bareASGI-auth-common-4.0.3/pyproject.toml` & `bareasgi_auth_common-4.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "bareASGI-auth-common"
-version = "4.0.3"
+version = "4.1.0"
 description = ""
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "bareasgi_auth_common" },
 ]
 repository = "https://github.com/rob-blackbourn/bareASGI-auth-common"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 bareclient = "^5.0"
-PyJWT = "^2.3"
-bareasgi = "^4.0"
+PyJWT = "^2.6"
+bareasgi = "^4.4"
 
 [tool.poetry.dev-dependencies]
-autopep8 = "^1.5"
-mypy = "^0.910"
-pytest = "^6.2"
-pylint = "^2.11"
+autopep8 = "^2.0"
+mypy = "^1.2"
+pytest = "^7.3"
+pylint = "^2.17"
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `bareASGI-auth-common-4.0.3/setup.py` & `bareasgi_auth_common-4.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['bareasgi_auth_common']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyJWT>=2.3,<3.0', 'bareasgi>=4.0,<5.0', 'bareclient>=5.0,<6.0']
+['PyJWT>=2.6,<3.0', 'bareasgi>=4.4,<5.0', 'bareclient>=5.0,<6.0']
 
 setup_kwargs = {
     'name': 'bareasgi-auth-common',
-    'version': '4.0.3',
+    'version': '4.1.0',
     'description': '',
     'long_description': '# bareASGI-auth-common\n\nCommon code for authentication with bareASGI.',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/rob-blackbourn/bareASGI-auth-common',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `bareASGI-auth-common-4.0.3/PKG-INFO` & `bareasgi_auth_common-4.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: bareasgi-auth-common
-Version: 4.0.3
+Version: 4.1.0
 Summary: 
 Home-page: https://github.com/rob-blackbourn/bareASGI-auth-common
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyJWT (>=2.3,<3.0)
-Requires-Dist: bareasgi (>=4.0,<5.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyJWT (>=2.6,<3.0)
+Requires-Dist: bareasgi (>=4.4,<5.0)
 Requires-Dist: bareclient (>=5.0,<6.0)
 Project-URL: Repository, https://github.com/rob-blackbourn/bareASGI-auth-common
 Description-Content-Type: text/markdown
 
 # bareASGI-auth-common
 
 Common code for authentication with bareASGI.
```

