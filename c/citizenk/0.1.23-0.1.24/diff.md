# Comparing `tmp/citizenk-0.1.23.tar.gz` & `tmp/citizenk-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.23.tar", max compression
+gzip compressed data, was "citizenk-0.1.24.tar", max compression
```

## Comparing `citizenk-0.1.23.tar` & `citizenk-0.1.24.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.23/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.23/citizenk/agent.py
--rw-r--r--   0        0        0    18077 2023-04-28 07:38:42.095328 citizenk-0.1.23/citizenk/citizenk.py
--rw-r--r--   0        0        0    20509 2023-04-04 18:14:45.297447 citizenk-0.1.23/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.23/citizenk/murmur2.py
--rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.23/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.23/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-28 11:55:10.402330 citizenk-0.1.23/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-28 11:55:16.999595 citizenk-0.1.23/setup.py
--rw-r--r--   0        0        0     1076 2023-04-28 11:55:16.999847 citizenk-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.24/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.24/citizenk/agent.py
+-rw-r--r--   0        0        0    18296 2023-04-28 17:35:35.202323 citizenk-0.1.24/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20509 2023-04-04 18:14:45.297447 citizenk-0.1.24/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.24/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.24/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.24/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-28 17:36:40.038814 citizenk-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-28 17:36:44.480507 citizenk-0.1.24/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-28 17:36:44.480780 citizenk-0.1.24/PKG-INFO
```

### Comparing `citizenk-0.1.23/citizenk/agent.py` & `citizenk-0.1.24/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.23/citizenk/citizenk.py` & `citizenk-0.1.24/citizenk/citizenk.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,18 @@
                 request = kwargs["request"]
                 params = dict(request.query_params)
                 if "citizenk_stop_propogate" in params:
                     return await f(*args, **kwargs)
                 params["citizenk_stop_propogate"] = True
 
                 url = httpx.URL(str(request.url)).copy_with(host=host)
+                # Mainly used for testing purposes
+                if self.api_port is not None:
+                    url = url.copy_with(port=self.api_port)
+                logger.debug("Routing request to %s",url)
                 async with httpx.AsyncClient() as client:
                     r = await client.request(
                         method=request.method,
                         url=url,
                         headers=request.headers.raw,
                         params=params,
                         content=await request.body(),
@@ -457,15 +461,15 @@
                 params["citizenk_stop_propogate"] = True
 
                 response = {}
                 async with httpx.AsyncClient() as client:
                     for host in hosts:
                         url = httpx.URL(str(request.url)).copy_with(host=host)
                         # Mainly used for testing purposes
-                        if self.api_port != None:
+                        if self.api_port is not None:
                             url = url.copy_with(port=self.api_port)
                         logger.debug("Broadcast to %s",url)
                         r = await client.request(
                             method=request.method,
                             url=url,
                             headers=request.headers.raw,
                             params=params,
```

### Comparing `citizenk-0.1.23/citizenk/kafka_adapter.py` & `citizenk-0.1.24/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.23/citizenk/murmur2.py` & `citizenk-0.1.24/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.23/citizenk/topic.py` & `citizenk-0.1.24/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.23/pyproject.toml` & `citizenk-0.1.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.23"
+version = "0.1.24"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.23/setup.py` & `citizenk-0.1.24/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.23',
+    'version': '0.1.24',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.23/PKG-INFO` & `citizenk-0.1.24/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.23
+Version: 0.1.24
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

