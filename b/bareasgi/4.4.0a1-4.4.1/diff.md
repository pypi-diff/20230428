# Comparing `tmp/bareasgi-4.4.0a1.tar.gz` & `tmp/bareasgi-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareasgi-4.4.0a1.tar", max compression
+gzip compressed data, was "bareasgi-4.4.1.tar", max compression
```

## Comparing `bareasgi-4.4.0a1.tar` & `bareasgi-4.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/LICENSE
--rw-r--r--   0        0        0     2060 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/README.md
--rw-r--r--   0        0        0      829 2023-04-28 06:44:15.843732 bareasgi-4.4.0a1/bareasgi/__init__.py
--rw-r--r--   0        0        0     5807 2023-04-28 07:11:04.832069 bareasgi-4.4.0a1/bareasgi/application.py
--rw-r--r--   0        0        0      187 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/basic_router/__init__.py
--rw-r--r--   0        0        0     2879 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/basic_router/http_router.py
--rw-r--r--   0        0        0     2931 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/basic_router/path_definition.py
--rw-r--r--   0        0        0     3153 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/basic_router/path_segment.py
--rw-r--r--   0        0        0     1368 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/basic_router/web_socket_router.py
--rw-r--r--   0        0        0     3998 2023-04-28 07:11:40.574166 bareasgi-4.4.0a1/bareasgi/core_application.py
--rw-r--r--   0        0        0      530 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/__init__.py
--rw-r--r--   0        0        0      331 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/http_callbacks.py
--rw-r--r--   0        0        0      194 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/http_errors.py
--rw-r--r--   0        0        0     9094 2023-04-28 07:37:13.321722 bareasgi-4.4.0a1/bareasgi/http/http_instance.py
--rw-r--r--   0        0        0      924 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/http_middleware.py
--rw-r--r--   0        0        0     2630 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/http_request.py
--rw-r--r--   0        0        0     5237 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/http_response.py
--rw-r--r--   0        0        0     1583 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/http/http_router.py
--rw-r--r--   0        0        0      234 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/lifespan/__init__.py
--rw-r--r--   0        0        0     3353 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/lifespan/lifespan_instance.py
--rw-r--r--   0        0        0      648 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/lifespan/lifespan_request.py
--rw-r--r--   0        0        0      201 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/middlewares/__init__.py
--rw-r--r--   0        0        0     9318 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/middlewares/compression.py
--rw-r--r--   0        0        0        0 2023-02-17 13:20:42.782353 bareasgi-4.4.0a1/bareasgi/py.typed
--rw-r--r--   0        0        0     1562 2023-02-17 13:20:42.786353 bareasgi-4.4.0a1/bareasgi/utils.py
--rw-r--r--   0        0        0      480 2023-04-28 06:44:15.843732 bareasgi-4.4.0a1/bareasgi/websockets/__init__.py
--rw-r--r--   0        0        0     1481 2023-02-17 13:20:42.786353 bareasgi-4.4.0a1/bareasgi/websockets/websocket.py
--rw-r--r--   0        0        0      315 2023-04-28 06:44:15.843732 bareasgi-4.4.0a1/bareasgi/websockets/websocket_callbacks.py
--rw-r--r--   0        0        0      124 2023-02-17 13:20:42.786353 bareasgi-4.4.0a1/bareasgi/websockets/websocket_errors.py
--rw-r--r--   0        0        0     4776 2023-04-28 06:44:15.847732 bareasgi-4.4.0a1/bareasgi/websockets/websocket_instance.py
--rw-r--r--   0        0        0      951 2023-04-28 06:44:15.847732 bareasgi-4.4.0a1/bareasgi/websockets/websocket_middleware.py
--rw-r--r--   0        0        0     1008 2023-04-28 06:44:15.847732 bareasgi-4.4.0a1/bareasgi/websockets/websocket_request.py
--rw-r--r--   0        0        0      955 2023-04-28 06:44:15.847732 bareasgi-4.4.0a1/bareasgi/websockets/websocket_router.py
--rw-r--r--   0        0        0      852 2023-04-28 07:31:59.257591 bareasgi-4.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 bareasgi-4.4.0a1/setup.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 bareasgi-4.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-17 13:20:42.782353 bareasgi-4.4.1/LICENSE
+-rw-r--r--   0        0        0     2060 2023-02-17 13:20:42.782353 bareasgi-4.4.1/README.md
+-rw-r--r--   0        0        0      829 2023-04-28 07:59:05.506233 bareasgi-4.4.1/bareasgi/__init__.py
+-rw-r--r--   0        0        0     5807 2023-04-28 07:59:05.506233 bareasgi-4.4.1/bareasgi/application.py
+-rw-r--r--   0        0        0      187 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/basic_router/__init__.py
+-rw-r--r--   0        0        0     2879 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/basic_router/http_router.py
+-rw-r--r--   0        0        0     2931 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/basic_router/path_definition.py
+-rw-r--r--   0        0        0     3153 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/basic_router/path_segment.py
+-rw-r--r--   0        0        0     1368 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/basic_router/web_socket_router.py
+-rw-r--r--   0        0        0     3978 2023-04-28 08:45:12.723779 bareasgi-4.4.1/bareasgi/core_application.py
+-rw-r--r--   0        0        0      530 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/__init__.py
+-rw-r--r--   0        0        0      331 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/http_callbacks.py
+-rw-r--r--   0        0        0      194 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/http_errors.py
+-rw-r--r--   0        0        0     9094 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/http/http_instance.py
+-rw-r--r--   0        0        0      924 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/http_middleware.py
+-rw-r--r--   0        0        0     2630 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/http_request.py
+-rw-r--r--   0        0        0     5237 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/http_response.py
+-rw-r--r--   0        0        0     1583 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/http/http_router.py
+-rw-r--r--   0        0        0      234 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/lifespan/__init__.py
+-rw-r--r--   0        0        0     3353 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/lifespan/lifespan_instance.py
+-rw-r--r--   0        0        0      648 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/lifespan/lifespan_request.py
+-rw-r--r--   0        0        0      201 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/middlewares/__init__.py
+-rw-r--r--   0        0        0     9318 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/middlewares/compression.py
+-rw-r--r--   0        0        0        0 2023-02-17 13:20:42.782353 bareasgi-4.4.1/bareasgi/py.typed
+-rw-r--r--   0        0        0     1562 2023-02-17 13:20:42.786353 bareasgi-4.4.1/bareasgi/utils.py
+-rw-r--r--   0        0        0      480 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/websockets/__init__.py
+-rw-r--r--   0        0        0     1481 2023-02-17 13:20:42.786353 bareasgi-4.4.1/bareasgi/websockets/websocket.py
+-rw-r--r--   0        0        0      315 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/websockets/websocket_callbacks.py
+-rw-r--r--   0        0        0      124 2023-02-17 13:20:42.786353 bareasgi-4.4.1/bareasgi/websockets/websocket_errors.py
+-rw-r--r--   0        0        0     4776 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/websockets/websocket_instance.py
+-rw-r--r--   0        0        0      951 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/websockets/websocket_middleware.py
+-rw-r--r--   0        0        0     1008 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/websockets/websocket_request.py
+-rw-r--r--   0        0        0      955 2023-04-28 07:59:05.510233 bareasgi-4.4.1/bareasgi/websockets/websocket_router.py
+-rw-r--r--   0        0        0      844 2023-04-28 08:45:24.011328 bareasgi-4.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2935 1970-01-01 00:00:00.000000 bareasgi-4.4.1/setup.py
+-rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 bareasgi-4.4.1/PKG-INFO
```

### Comparing `bareasgi-4.4.0a1/LICENSE` & `bareasgi-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/README.md` & `bareasgi-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/__init__.py` & `bareasgi-4.4.1/bareasgi/__init__.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/application.py` & `bareasgi-4.4.1/bareasgi/application.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/basic_router/http_router.py` & `bareasgi-4.4.1/bareasgi/basic_router/http_router.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/basic_router/path_definition.py` & `bareasgi-4.4.1/bareasgi/basic_router/path_definition.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/basic_router/path_segment.py` & `bareasgi-4.4.1/bareasgi/basic_router/path_segment.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/basic_router/web_socket_router.py` & `bareasgi-4.4.1/bareasgi/basic_router/web_socket_router.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/core_application.py` & `bareasgi-4.4.1/bareasgi/core_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
 
 class CoreApplication:
     """The core ASGI application"""
 
     def __init__(
             self,
-            http_middlewares: List[HttpMiddlewareCallback],
+            middlewares: List[HttpMiddlewareCallback],
             http_router: HttpRouter,
             ws_middlewares: List[WebSocketMiddlewareCallback],
             ws_router: WebSocketRouter,
             startup_handlers: List[LifespanRequestHandler],
             shutdown_handlers: List[LifespanRequestHandler],
             info: Dict[str, Any]
     ) -> None:
         self.info = info
-        self.http_middlewares = http_middlewares
+        self.middlewares = middlewares
         self.http_router = http_router
         self.ws_router = ws_router
         self.ws_middlewares = ws_middlewares
         self.startup_handlers = startup_handlers
         self.shutdown_handlers = shutdown_handlers
 
     async def _handle_lifespan_request(
@@ -69,15 +69,15 @@
             scope: HTTPScope,
             receive: ASGIHTTPReceiveCallable,
             send: ASGIHTTPSendCallable
     ) -> None:
         instance = HttpInstance(
             scope,
             self.http_router,
-            self.http_middlewares,
+            self.middlewares,
             self.info
         )
         await instance.process(receive, send)
 
     async def _handle_websocket_request(
             self,
             scope: WebSocketScope,
```

### Comparing `bareasgi-4.4.0a1/bareasgi/http/__init__.py` & `bareasgi-4.4.1/bareasgi/http/__init__.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/http/http_instance.py` & `bareasgi-4.4.1/bareasgi/http/http_instance.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/http/http_middleware.py` & `bareasgi-4.4.1/bareasgi/http/http_middleware.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/http/http_request.py` & `bareasgi-4.4.1/bareasgi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/http/http_response.py` & `bareasgi-4.4.1/bareasgi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/http/http_router.py` & `bareasgi-4.4.1/bareasgi/http/http_router.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/lifespan/lifespan_instance.py` & `bareasgi-4.4.1/bareasgi/lifespan/lifespan_instance.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/lifespan/lifespan_request.py` & `bareasgi-4.4.1/bareasgi/lifespan/lifespan_request.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/middlewares/compression.py` & `bareasgi-4.4.1/bareasgi/middlewares/compression.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/utils.py` & `bareasgi-4.4.1/bareasgi/utils.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/websockets/websocket.py` & `bareasgi-4.4.1/bareasgi/websockets/websocket.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/websockets/websocket_instance.py` & `bareasgi-4.4.1/bareasgi/websockets/websocket_instance.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/websockets/websocket_middleware.py` & `bareasgi-4.4.1/bareasgi/websockets/websocket_middleware.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/websockets/websocket_request.py` & `bareasgi-4.4.1/bareasgi/websockets/websocket_request.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/bareasgi/websockets/websocket_router.py` & `bareasgi-4.4.1/bareasgi/websockets/websocket_router.py`

 * *Files identical despite different names*

### Comparing `bareasgi-4.4.0a1/pyproject.toml` & `bareasgi-4.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bareasgi"
-version = "4.4.0-alpha.1"
+version = "4.4.1"
 description = "A lightweight ASGI framework"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "bareasgi" }
 ]
```

### Comparing `bareasgi-4.4.0a1/setup.py` & `bareasgi-4.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['bareutils>=4.0.0,<5.0.0', 'jetblack-asgi-typing>=0.4.0,<0.5.0']
 
 setup_kwargs = {
     'name': 'bareasgi',
-    'version': '4.4.0a1',
+    'version': '4.4.1',
     'description': 'A lightweight ASGI framework',
     'long_description': "# bareASGI\n\nA lightweight Python [ASGI](user-guide/asgi) web server framework\n(read the [docs](https://rob-blackbourn.github.io/bareASGI/)).\n\n## Overview\n\nThis is a _bare_ ASGI web server framework. The goal is to provide\na minimal implementation, with other facilities (serving static files, CORS,\nsessions, etc.) being implemented by optional packages.\n\nThe framework is targeted at micro-services which require a light footprint\n(in a container for example), or as a base for larger frameworks.\n\nPython 3.8+ is required.\n\n## Optional Packages\n\n- [bareASGI-cors](https://github.com/rob-blackbourn/bareASGI-cors) for cross origin resource sharing,\n- [bareASGI-static](https://github.com/rob-blackbourn/bareASGI-static) for serving static files,\n- [bareASGI-jinja2](https://github.com/rob-blackbourn/bareASGI-jinja2) for [Jinja2](https://github.com/pallets/jinja) template rendering,\n- [bareASGI-graphql-next](https://github.com/rob-blackbourn/bareASGI-graphql-next) for [GraphQL](https://github.com/graphql-python/graphql-core) and [graphene](https://github.com/graphql-python/graphene),\n- [bareASGI-rest](https://github.com/rob-blackbourn/bareASGI-rest) for REST support,\n- [bareASGI-prometheus](https://github.com/rob-blackbourn/bareASGI-prometheus) for [prometheus](https://prometheus.io/) metrics,\n- [bareASGI-session](https://github.com/rob-blackbourn/bareASGI-session) for sessions.\n\n## Functionality\n\nThe framework provides the basic functionality required for developing a web\napplication, including:\n\n- Http,\n- WebSockets,\n- Routing,\n- Lifecycle,\n- Middleware\n\n## Simple Server\n\nHere is a simple server with a request handler that returns some text.\n\n```python\nimport uvicorn\nfrom bareasgi import Application, HttpRequest, HttpResponse, text_writer\n\nasync def example_handler(request: HttpRequest) -> HttpResponse:\n    return HttpResponse(\n        200,\n        [(b'content-type', b'text/plain')],\n        text_writer('This is not a test')\n    )\n\napp = Application()\napp.http_router.add({'GET'}, '/', example_handler)\n\nuvicorn.run(app, port=9009)\n```\n",
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rob-blackbourn/bareasgi',
```

### Comparing `bareasgi-4.4.0a1/PKG-INFO` & `bareasgi-4.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareasgi
-Version: 4.4.0a1
+Version: 4.4.1
 Summary: A lightweight ASGI framework
 Home-page: https://github.com/rob-blackbourn/bareasgi
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

