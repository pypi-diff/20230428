# Comparing `tmp/dockerode_api_proxy_client-4.0.0.tar.gz` & `tmp/dockerode_api_proxy_client-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerode_api_proxy_client-4.0.0.tar", last modified: Fri Apr 28 16:12:14 2023, max compression
+gzip compressed data, was "dockerode_api_proxy_client-5.0.0.tar", last modified: Fri Apr 28 16:20:33 2023, max compression
```

## Comparing `dockerode_api_proxy_client-4.0.0.tar` & `dockerode_api_proxy_client-5.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.555409 dockerode_api_proxy_client-4.0.0/
--rw-r--r--   0 thim       (501) staff       (20)     1066 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/LICENSE
--rw-r--r--   0 thim       (501) staff       (20)       23 2023-02-05 20:14:40.000000 dockerode_api_proxy_client-4.0.0/MANIFEST.in
--rw-r--r--   0 thim       (501) staff       (20)      811 2023-04-28 16:12:14.555495 dockerode_api_proxy_client-4.0.0/PKG-INFO
--rw-r--r--   0 thim       (501) staff       (20)      199 2023-03-13 18:00:12.000000 dockerode_api_proxy_client-4.0.0/README.md
--rw-r--r--   0 thim       (501) staff       (20)     1011 2023-03-27 19:07:40.000000 dockerode_api_proxy_client-4.0.0/pyproject.toml
--rw-r--r--   0 thim       (501) staff       (20)     1070 2023-04-28 16:12:14.558852 dockerode_api_proxy_client-4.0.0/setup.cfg
--rw-r--r--   0 thim       (501) staff       (20)      405 2022-12-18 09:14:54.000000 dockerode_api_proxy_client-4.0.0/setup.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.491675 dockerode_api_proxy_client-4.0.0/src/
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.533516 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)       22 2023-02-05 20:14:40.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/__version__.py
--rw-r--r--   0 thim       (501) staff       (20)     7848 2023-04-28 16:09:21.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/client.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.544597 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)     1787 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/container.py
--rw-r--r--   0 thim       (501) staff       (20)      338 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/image.py
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/py.typed
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.548343 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/settings/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/settings/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)      284 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/settings/env.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.553521 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)      541 2023-04-28 15:55:22.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/add_authentication_header.py
--rw-r--r--   0 thim       (501) staff       (20)      207 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/datatype.py
--rw-r--r--   0 thim       (501) staff       (20)      791 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/formatting.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.540429 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/
--rw-r--r--   0 thim       (501) staff       (20)      811 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/PKG-INFO
--rw-r--r--   0 thim       (501) staff       (20)     1117 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/SOURCES.txt
--rw-r--r--   0 thim       (501) staff       (20)        1 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/dependency_links.txt
--rw-r--r--   0 thim       (501) staff       (20)        1 2023-04-28 16:11:55.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/not-zip-safe
--rw-r--r--   0 thim       (501) staff       (20)       91 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/requires.txt
--rw-r--r--   0 thim       (501) staff       (20)       32 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/top_level.txt
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.555135 dockerode_api_proxy_client-4.0.0/tests/
--rw-r--r--   0 thim       (501) staff       (20)      881 2023-04-28 15:55:11.000000 dockerode_api_proxy_client-4.0.0/tests/test_add_authentication_header.py
--rw-r--r--   0 thim       (501) staff       (20)      171 2023-02-17 21:55:29.000000 dockerode_api_proxy_client-4.0.0/tests/test_client.py
--rw-r--r--   0 thim       (501) staff       (20)      389 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-4.0.0/tests/test_datatype.py
--rw-r--r--   0 thim       (501) staff       (20)      848 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/tests/test_formatting.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.476548 dockerode_api_proxy_client-5.0.0/
+-rw-r--r--   0 thim       (501) staff       (20)     1066 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/LICENSE
+-rw-r--r--   0 thim       (501) staff       (20)       23 2023-02-05 20:14:40.000000 dockerode_api_proxy_client-5.0.0/MANIFEST.in
+-rw-r--r--   0 thim       (501) staff       (20)      811 2023-04-28 16:20:33.476650 dockerode_api_proxy_client-5.0.0/PKG-INFO
+-rw-r--r--   0 thim       (501) staff       (20)      199 2023-03-13 18:00:12.000000 dockerode_api_proxy_client-5.0.0/README.md
+-rw-r--r--   0 thim       (501) staff       (20)     1011 2023-03-27 19:07:40.000000 dockerode_api_proxy_client-5.0.0/pyproject.toml
+-rw-r--r--   0 thim       (501) staff       (20)     1070 2023-04-28 16:20:33.477327 dockerode_api_proxy_client-5.0.0/setup.cfg
+-rw-r--r--   0 thim       (501) staff       (20)      405 2022-12-18 09:14:54.000000 dockerode_api_proxy_client-5.0.0/setup.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.407877 dockerode_api_proxy_client-5.0.0/src/
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.443515 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)       22 2023-02-05 20:14:40.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/__version__.py
+-rw-r--r--   0 thim       (501) staff       (20)     8009 2023-04-28 16:18:56.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/client.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.453293 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/dto/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/dto/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)     1787 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/dto/container.py
+-rw-r--r--   0 thim       (501) staff       (20)      338 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/dto/image.py
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/py.typed
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.461805 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/settings/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/settings/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)      284 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/settings/env.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.466102 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/utils/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/utils/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)      207 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/utils/datatype.py
+-rw-r--r--   0 thim       (501) staff       (20)      791 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/utils/formatting.py
+-rw-r--r--   0 thim       (501) staff       (20)      445 2023-04-28 16:15:27.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/utils/get_authentication_header.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.451256 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/
+-rw-r--r--   0 thim       (501) staff       (20)      811 2023-04-28 16:20:33.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/PKG-INFO
+-rw-r--r--   0 thim       (501) staff       (20)     1117 2023-04-28 16:20:33.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 thim       (501) staff       (20)        1 2023-04-28 16:20:33.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 thim       (501) staff       (20)        1 2023-04-28 16:11:55.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/not-zip-safe
+-rw-r--r--   0 thim       (501) staff       (20)       91 2023-04-28 16:20:33.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/requires.txt
+-rw-r--r--   0 thim       (501) staff       (20)       32 2023-04-28 16:20:33.000000 dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/top_level.txt
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:20:33.475790 dockerode_api_proxy_client-5.0.0/tests/
+-rw-r--r--   0 thim       (501) staff       (20)      171 2023-02-17 21:55:29.000000 dockerode_api_proxy_client-5.0.0/tests/test_client.py
+-rw-r--r--   0 thim       (501) staff       (20)      389 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-5.0.0/tests/test_datatype.py
+-rw-r--r--   0 thim       (501) staff       (20)      848 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-5.0.0/tests/test_formatting.py
+-rw-r--r--   0 thim       (501) staff       (20)      816 2023-04-28 16:15:38.000000 dockerode_api_proxy_client-5.0.0/tests/test_get_authentication_header.py
```

### Comparing `dockerode_api_proxy_client-4.0.0/LICENSE` & `dockerode_api_proxy_client-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-4.0.0/PKG-INFO` & `dockerode_api_proxy_client-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerode_api_proxy_client
-Version: 4.0.0
+Version: 5.0.0
 Summary: Dockerode API proxy client enables communication with the side-car service Dockerode API proxy
 Author: Thim Lohse
 Author-email: thim.lohse@caesari.se
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `dockerode_api_proxy_client-4.0.0/pyproject.toml` & `dockerode_api_proxy_client-5.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-4.0.0/setup.cfg` & `dockerode_api_proxy_client-5.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	__pycache__,
 	.venv@dockerode_api_proxy_client
 
 [metadata]
 name = dockerode-api-proxy-client
 description = Dockerode API proxy client enables communication with the side-car service Dockerode API proxy
 author = Thim Lohse
-version = 4.0.0
+version = 5.0.0
 author_email = thim.lohse@caesari.se
 license = MIT
 license_files = LICENSE
 requires_python = ">=3.9"
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/client.py` & `dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, List, Optional, Dict, Type
 from dockerode_api_proxy_client.settings.env import get_environment_enum
 from dockerode_api_proxy_client.dto.image import ImageInfo
 from dockerode_api_proxy_client.dto.container import ContainerInfo, ContainerInspectInfo
-from dockerode_api_proxy_client.utils.add_authentication_header import (
-    add_authentication_header,
+from dockerode_api_proxy_client.utils.get_authentication_header import (
+    get_authentication_header,
+    extend_headers,
 )
 from dockerode_api_proxy_client.utils.formatting import camel_case_keys, define_dict
 from caesari_clients.base.generic_rest_client import GenericRestClient
 
 
 class ApiProxyClient(GenericRestClient):
     def __init__(self, host: str, request_timeout: int = 10, *args, **kwargs) -> None:
@@ -27,83 +28,71 @@
                 return data
             return list(map(lambda entry: Dataclass(**entry), data))
         return data
 
     async def get_all_images(self, *args, **kwargs) -> List[ImageInfo]:
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
-
-        response = await self._get(
-            "v1/image",
-            headers=authenticated_headers,
-            *args,
-        )
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
+        response = await self._get("v1/image", *args, **kwargs)
         data = response["data"]
         result: List[ImageInfo] = self._transform_response(ImageInfo, data)
         return result
 
     async def pull_image_on_remote(
         self, image: str, *args, **kwargs
     ) -> List[ImageInfo]:
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
         defined_params = {image: image}
         pull_params = camel_case_keys(define_dict(defined_params))
         response = await self._post(
             "v1/image/pull",
             json=pull_params,
-            headers=authenticated_headers,
             *args,
+            **kwargs,
         )
         data = response["data"]
         result: List[ImageInfo] = self._transform_response(ImageInfo, data)
         return result
 
     async def get_all_containers(self, *args, **kwargs) -> List[ContainerInfo]:
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._get(
-            "v1/container",
-            *args,
-            headers=authenticated_headers,
-        )
+        response = await self._get("v1/container", *args, **kwargs)
         data = response["data"]
         result: List[ContainerInfo] = self._transform_response(ContainerInfo, data)
         return result
 
     async def get_container_by_id(self, id: str, *args, **kwargs):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._get(
-            f"v1/container/{id}",
-            headers=authenticated_headers,
-            *args,
-        )
+        response = await self._get(f"v1/container/{id}", *args, **kwargs)
         data = response["data"]
         return data
 
     async def inspect_container_by_id(
         self, id: str, *args, **kwargs
     ) -> ContainerInspectInfo:
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._get(
-            f"v1/container/{id}/inspect",
-            headers=authenticated_headers,
-            *args,
-        )
+        response = await self._get(f"v1/container/{id}/inspect", *args, **kwargs)
         data = response["data"]
         result: ContainerInspectInfo = self._transform_response(
             ContainerInspectInfo, data
         )
         return result
 
     async def create(
@@ -115,113 +104,102 @@
         exposed_ports: Optional[Dict[str, Dict[str, None]]] = None,
         keep_alive: Optional[bool] = None,
         *args,
         **kwargs,
     ):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
         defined_params = {
             "image": image,
             "env": env,
             "name": name,
             "labels": labels,
             "exposed_ports": exposed_ports,
             "keep_alive": keep_alive,
         }
         create_params = camel_case_keys(define_dict(defined_params))
         response = await self._post(
             "v1/container/create",
             json=create_params,
-            headers=authenticated_headers,
             *args,
+            **kwargs,
         )
         data = response["data"]
         return data
 
     async def rename(
         self,
         id: str,
         name: str,
         *args,
         **kwargs,
     ):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
         defined_params = {
             "name": name,
         }
         create_params = camel_case_keys(define_dict(defined_params))
         response = await self._post(
             f"v1/container/{id}/rename",
             json=create_params,
-            headers=authenticated_headers,
             *args,
+            **kwargs,
         )
         data = response["data"]
         return data
 
     async def start(self, id: str, *args, **kwargs):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._post(
-            f"v1/container/{id}/start",
-            headers=authenticated_headers,
-            *args,
-        )
+        response = await self._post(f"v1/container/{id}/start", *args, **kwargs)
         data = response["data"]
         return data
 
     async def pause(self, id: str, *args, **kwargs):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._post(
-            f"v1/container/{id}/pause",
-            headers=authenticated_headers,
-            *args,
-        )
+        response = await self._post(f"v1/container/{id}/pause", *args, **kwargs)
         data = response["data"]
         return data
 
     async def restart(self, id: str, *args, **kwargs):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._post(
-            f"v1/container/{id}/restart",
-            headers=authenticated_headers,
-            *args,
-        )
+        response = await self._post(f"v1/container/{id}/restart", *args, **kwargs)
         data = response["data"]
         return data
 
     async def stop(self, id: str, *args, **kwargs):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._post(
-            f"v1/container/{id}/stop", headers=authenticated_headers, *args
-        )
+        response = await self._post(f"v1/container/{id}/stop", *args, **kwargs)
         data = response["data"]
         return data
 
     async def remove(self, id: str, *args, **kwargs):
         headers = kwargs.get("headers", {})
         jwt_secret = get_environment_enum().JWT_SECRET
-        authenticated_headers = add_authentication_header(jwt_secret, headers)
+        authenticated_headers = get_authentication_header(jwt_secret)
+        kwargs["headers"] = extend_headers(headers, authenticated_headers)
 
-        response = await self._delete(
-            f"v1/container/{id}",
-            headers=authenticated_headers,
-            *args,
-        )
+        response = await self._delete(f"v1/container/{id}", *args, **kwargs)
         data = response["data"]
         return data
```

### Comparing `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/container.py` & `dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/dto/container.py`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/formatting.py` & `dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/PKG-INFO` & `dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerode-api-proxy-client
-Version: 4.0.0
+Version: 5.0.0
 Summary: Dockerode API proxy client enables communication with the side-car service Dockerode API proxy
 Author: Thim Lohse
 Author-email: thim.lohse@caesari.se
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/SOURCES.txt` & `dockerode_api_proxy_client-5.0.0/src/dockerode_api_proxy_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 src/dockerode_api_proxy_client.egg-info/top_level.txt
 src/dockerode_api_proxy_client/dto/__init__.py
 src/dockerode_api_proxy_client/dto/container.py
 src/dockerode_api_proxy_client/dto/image.py
 src/dockerode_api_proxy_client/settings/__init__.py
 src/dockerode_api_proxy_client/settings/env.py
 src/dockerode_api_proxy_client/utils/__init__.py
-src/dockerode_api_proxy_client/utils/add_authentication_header.py
 src/dockerode_api_proxy_client/utils/datatype.py
 src/dockerode_api_proxy_client/utils/formatting.py
-tests/test_add_authentication_header.py
+src/dockerode_api_proxy_client/utils/get_authentication_header.py
 tests/test_client.py
 tests/test_datatype.py
-tests/test_formatting.py
+tests/test_formatting.py
+tests/test_get_authentication_header.py
```

### Comparing `dockerode_api_proxy_client-4.0.0/tests/test_add_authentication_header.py` & `dockerode_api_proxy_client-5.0.0/tests/test_get_authentication_header.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dockerode_api_proxy_client.utils.add_authentication_header import (
+from dockerode_api_proxy_client.utils.get_authentication_header import (
     extend_headers,
-add_authentication_header
+get_authentication_header
 )
 
 
 empty_headers = {}
 existing_headers = {"Accept": "application/json"}
 
 auth_headers = {"Authorization": "Bearer <token_here/>"}
@@ -17,12 +17,11 @@
 
 
 def test_extend_header_object():
     expected = {"Authorization": "Bearer <token_here/>", "Accept": "application/json"}
     assert extend_headers(existing_headers, auth_headers) == expected
 
 
-def test_add_authorization_header():
-    authenticated_headers = add_authentication_header("jwt_secret", empty_headers)
-    assert authenticated_headers != empty_headers
+def test_get_authorization_header():
+    authenticated_headers = get_authentication_header("jwt_secret")
     assert "Authorization" in authenticated_headers
```

### Comparing `dockerode_api_proxy_client-4.0.0/tests/test_formatting.py` & `dockerode_api_proxy_client-5.0.0/tests/test_formatting.py`

 * *Files identical despite different names*

