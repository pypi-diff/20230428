# Comparing `tmp/interactions-restful-1.0.1.tar.gz` & `tmp/interactions-restful-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions-restful-1.0.1.tar", last modified: Fri Apr 28 07:20:37 2023, max compression
+gzip compressed data, was "interactions-restful-1.0.2.tar", last modified: Fri Apr 28 07:59:24 2023, max compression
```

## Comparing `interactions-restful-1.0.1.tar` & `interactions-restful-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/interactions_restful/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/interactions_restful/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/backends/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/backends/flask_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/interactions_restful/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/interactions_restful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 07:20:37.000000 interactions-restful-1.0.1/interactions_restful.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:20:37.752846 interactions-restful-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-28 07:20:24.000000 interactions-restful-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:59:24.770442 interactions-restful-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-28 07:59:24.770442 interactions-restful-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:59:24.770442 interactions-restful-1.0.2/interactions_restful/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:59:24.770442 interactions-restful-1.0.2/interactions_restful/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/backends/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/backends/flask_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/interactions_restful/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:59:24.770442 interactions-restful-1.0.2/interactions_restful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-28 07:59:24.000000 interactions-restful-1.0.2/interactions_restful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 07:59:24.000000 interactions-restful-1.0.2/interactions_restful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:59:24.000000 interactions-restful-1.0.2/interactions_restful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 07:59:24.000000 interactions-restful-1.0.2/interactions_restful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 07:59:24.000000 interactions-restful-1.0.2/interactions_restful.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:59:24.770442 interactions-restful-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-28 07:59:10.000000 interactions-restful-1.0.2/setup.py
```

### Comparing `interactions-restful-1.0.1/LICENSE` & `interactions-restful-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.1/PKG-INFO` & `interactions-restful-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions-restful
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for interactions.py allowing runtime API structures
 Home-page: https://github.com/interactions-py/restful
 Author: Damego
 Author-email: damego.dev@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `interactions-restful-1.0.1/README.md` & `interactions-restful-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.1/interactions_restful/abc.py` & `interactions-restful-1.0.2/interactions_restful/abc.py`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.1/interactions_restful/backends/fast_api.py` & `interactions-restful-1.0.2/interactions_restful/backends/fast_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ..abc import BaseApi, BaseRouter
 
 __all__ = ("FastAPI", )
 
 
 class FastApiRouter(BaseRouter):
     def __init__(self, **kwargs):
+        kwargs.pop("name")  # neccessary only for flask
         self.api_router = APIRouter(**kwargs)
 
     def add_endpoint_method(self, coro: Callable[..., Coroutine], endpoint: str, method: str, **kwargs):
         self.api_router.add_api_route(
             endpoint,
             coro,
             methods=[method],
```

### Comparing `interactions-restful-1.0.1/interactions_restful/backends/flask_api.py` & `interactions-restful-1.0.2/interactions_restful/backends/flask_api.py`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.1/interactions_restful/extension.py` & `interactions-restful-1.0.2/interactions_restful/extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from threading import Thread
 from inspect import getmembers
 from typing import Type, TypeVar
 
 from interactions import Client
 
-from .abc import BaseApi, BaseRouter
+from .abc import BaseApi
 
 __all__ = ("APIClient", "setup")
 API_TYPE = TypeVar("API_TYPE", bound=BaseApi)
 
 
 class APIClient:
     bot: Client
@@ -30,23 +30,23 @@
 
     def _run_api_thread_worker(self):
         asyncio.run(self.client.run())
 
     def _register_extension_routes(self):
         for extension in self.bot.ext.values():
             has_methods = False
-            for _, coro in getmembers(extension, predicate=asyncio.iscoroutinefunction):
-                if not hasattr(coro, "__api__"):
+            for _, coro in getmembers(extension):
+                if getattr(coro, "__api__", None) is None:
                     continue
 
                 has_methods = True
 
                 if getattr(extension, "router", None) is None:
                     extension.router = self.client.create_router(name=extension.name)
-                data = coro.__api__
+                data: dict = coro.__api__
                 extension.router.add_endpoint_method(coro, data["endpoint"], data["method"], **data["kwargs"])
 
             if has_methods:
                 self.client.add_router(extension.router)
 
 
 def setup(client: Client, api: Type[API_TYPE], host: str, port: int, **kwargs) -> APIClient:
```

### Comparing `interactions-restful-1.0.1/interactions_restful.egg-info/PKG-INFO` & `interactions-restful-1.0.2/interactions_restful.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions-restful
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for interactions.py allowing runtime API structures
 Home-page: https://github.com/interactions-py/restful
 Author: Damego
 Author-email: damego.dev@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `interactions-restful-1.0.1/interactions_restful.egg-info/SOURCES.txt` & `interactions-restful-1.0.2/interactions_restful.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactions-restful-1.0.1/pyproject.toml` & `interactions-restful-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 100
 
 [tool.poetry]
 name = "interactions-restful"
-version = "1.0.1"
+version = "1.0.2"
 description = "A library for interactions.py allowing runtime API structures"
 authors = ["Damego <damego.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `interactions-restful-1.0.1/setup.py` & `interactions-restful-1.0.2/setup.py`

 * *Files identical despite different names*

