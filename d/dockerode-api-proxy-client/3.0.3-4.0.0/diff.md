# Comparing `tmp/dockerode_api_proxy_client-3.0.3.tar.gz` & `tmp/dockerode_api_proxy_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerode_api_proxy_client-3.0.3.tar", last modified: Sun Feb  5 19:29:13 2023, max compression
+gzip compressed data, was "dockerode_api_proxy_client-4.0.0.tar", last modified: Fri Apr 28 16:12:14 2023, max compression
```

## Comparing `dockerode_api_proxy_client-3.0.3.tar` & `dockerode_api_proxy_client-4.0.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.867645 dockerode_api_proxy_client-3.0.3/
--rw-r--r--   0 thim       (501) staff       (20)     1066 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/LICENSE
--rw-r--r--   0 thim       (501) staff       (20)       23 2023-02-05 19:08:24.000000 dockerode_api_proxy_client-3.0.3/MANIFEST.in
--rw-r--r--   0 thim       (501) staff       (20)      645 2023-02-05 19:29:13.867734 dockerode_api_proxy_client-3.0.3/PKG-INFO
--rw-r--r--   0 thim       (501) staff       (20)       32 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/README.md
--rw-r--r--   0 thim       (501) staff       (20)      880 2023-02-05 19:08:24.000000 dockerode_api_proxy_client-3.0.3/pyproject.toml
--rw-r--r--   0 thim       (501) staff       (20)     1041 2023-02-05 19:29:13.868266 dockerode_api_proxy_client-3.0.3/setup.cfg
--rw-r--r--   0 thim       (501) staff       (20)      405 2022-12-18 09:14:54.000000 dockerode_api_proxy_client-3.0.3/setup.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.837459 dockerode_api_proxy_client-3.0.3/src/
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.853822 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)       22 2023-02-05 19:11:11.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/__version__.py
--rw-r--r--   0 thim       (501) staff       (20)     5718 2023-02-05 19:10:21.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/client.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.863747 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/dto/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/dto/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)     1787 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/dto/container.py
--rw-r--r--   0 thim       (501) staff       (20)      338 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/dto/image.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.864745 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/middleware/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/middleware/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)      872 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/middleware/json_web_token_middleware.py
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/py.typed
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.865651 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/settings/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/settings/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)      284 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/settings/env.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.867243 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/utils/
--rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/utils/__init__.py
--rw-r--r--   0 thim       (501) staff       (20)      207 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/utils/datatype.py
--rw-r--r--   0 thim       (501) staff       (20)      791 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/utils/formatting.py
-drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-02-05 19:29:13.862395 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/
--rw-r--r--   0 thim       (501) staff       (20)      645 2023-02-05 19:29:13.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/PKG-INFO
--rw-r--r--   0 thim       (501) staff       (20)     1067 2023-02-05 19:29:13.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/SOURCES.txt
--rw-r--r--   0 thim       (501) staff       (20)        1 2023-02-05 19:29:13.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/dependency_links.txt
--rw-r--r--   0 thim       (501) staff       (20)        1 2022-11-06 21:28:20.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/not-zip-safe
--rw-r--r--   0 thim       (501) staff       (20)       68 2023-02-05 19:29:13.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/requires.txt
--rw-r--r--   0 thim       (501) staff       (20)       32 2023-02-05 19:29:13.000000 dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/top_level.txt
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.555409 dockerode_api_proxy_client-4.0.0/
+-rw-r--r--   0 thim       (501) staff       (20)     1066 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/LICENSE
+-rw-r--r--   0 thim       (501) staff       (20)       23 2023-02-05 20:14:40.000000 dockerode_api_proxy_client-4.0.0/MANIFEST.in
+-rw-r--r--   0 thim       (501) staff       (20)      811 2023-04-28 16:12:14.555495 dockerode_api_proxy_client-4.0.0/PKG-INFO
+-rw-r--r--   0 thim       (501) staff       (20)      199 2023-03-13 18:00:12.000000 dockerode_api_proxy_client-4.0.0/README.md
+-rw-r--r--   0 thim       (501) staff       (20)     1011 2023-03-27 19:07:40.000000 dockerode_api_proxy_client-4.0.0/pyproject.toml
+-rw-r--r--   0 thim       (501) staff       (20)     1070 2023-04-28 16:12:14.558852 dockerode_api_proxy_client-4.0.0/setup.cfg
+-rw-r--r--   0 thim       (501) staff       (20)      405 2022-12-18 09:14:54.000000 dockerode_api_proxy_client-4.0.0/setup.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.491675 dockerode_api_proxy_client-4.0.0/src/
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.533516 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)       22 2023-02-05 20:14:40.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/__version__.py
+-rw-r--r--   0 thim       (501) staff       (20)     7848 2023-04-28 16:09:21.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/client.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.544597 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)     1787 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/container.py
+-rw-r--r--   0 thim       (501) staff       (20)      338 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/image.py
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/py.typed
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.548343 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/settings/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/settings/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)      284 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/settings/env.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.553521 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/
+-rw-r--r--   0 thim       (501) staff       (20)        0 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/__init__.py
+-rw-r--r--   0 thim       (501) staff       (20)      541 2023-04-28 15:55:22.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/add_authentication_header.py
+-rw-r--r--   0 thim       (501) staff       (20)      207 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/datatype.py
+-rw-r--r--   0 thim       (501) staff       (20)      791 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/formatting.py
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.540429 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/
+-rw-r--r--   0 thim       (501) staff       (20)      811 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/PKG-INFO
+-rw-r--r--   0 thim       (501) staff       (20)     1117 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 thim       (501) staff       (20)        1 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 thim       (501) staff       (20)        1 2023-04-28 16:11:55.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/not-zip-safe
+-rw-r--r--   0 thim       (501) staff       (20)       91 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/requires.txt
+-rw-r--r--   0 thim       (501) staff       (20)       32 2023-04-28 16:12:14.000000 dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/top_level.txt
+drwxr-xr-x   0 thim       (501) staff       (20)        0 2023-04-28 16:12:14.555135 dockerode_api_proxy_client-4.0.0/tests/
+-rw-r--r--   0 thim       (501) staff       (20)      881 2023-04-28 15:55:11.000000 dockerode_api_proxy_client-4.0.0/tests/test_add_authentication_header.py
+-rw-r--r--   0 thim       (501) staff       (20)      171 2023-02-17 21:55:29.000000 dockerode_api_proxy_client-4.0.0/tests/test_client.py
+-rw-r--r--   0 thim       (501) staff       (20)      389 2023-01-28 11:24:16.000000 dockerode_api_proxy_client-4.0.0/tests/test_datatype.py
+-rw-r--r--   0 thim       (501) staff       (20)      848 2022-11-10 16:49:14.000000 dockerode_api_proxy_client-4.0.0/tests/test_formatting.py
```

### Comparing `dockerode_api_proxy_client-3.0.3/LICENSE` & `dockerode_api_proxy_client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-3.0.3/pyproject.toml` & `dockerode_api_proxy_client-4.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 [tool.pytest.ini_options]
 addopts = [
   "--import-mode=importlib",
 ]
+minversion = "6.0"
+testpaths = [
+  "tests",
+]
+
+[tool.coverage.run]
+omit = ["*/main.py", "*/**/__init__.py", "*/**/__version__.py"]
 
 [tool.autoflake]
 
 # return error code if changes are needed
 check = true
 # make changes to files instead of printing diffs
 in-place = true
```

### Comparing `dockerode_api_proxy_client-3.0.3/setup.cfg` & `dockerode_api_proxy_client-4.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -18,38 +18,39 @@
 	__pycache__,
 	.venv@dockerode_api_proxy_client
 
 [metadata]
 name = dockerode-api-proxy-client
 description = Dockerode API proxy client enables communication with the side-car service Dockerode API proxy
 author = Thim Lohse
-version = 3.0.3
+version = 4.0.0
 author_email = thim.lohse@caesari.se
 license = MIT
 license_files = LICENSE
 requires_python = ">=3.9"
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 install_requires = 
-	aiohttp>=3.8.3
-	PyJWT>=2.6.0
-	setuptools>=63
+	aiohttp >=3.8.3
+	PyJWT >=2.6.0
+	setuptools >=63
+	caesari_clients >=1.1.0
 package_dir = 
 	=src
 zip_safe = no
 
 [options.extras_require]
 testing = 
-	pytest>=6.2.5
+	pytest >=6.2.5
 
 [options.package_data]
 dockerode_api_proxy_client = py.typed
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/dto/container.py` & `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/dto/container.py`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client/utils/formatting.py` & `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `dockerode_api_proxy_client-3.0.3/src/dockerode_api_proxy_client.egg-info/SOURCES.txt` & `dockerode_api_proxy_client-4.0.0/src/dockerode_api_proxy_client.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 src/dockerode_api_proxy_client.egg-info/dependency_links.txt
 src/dockerode_api_proxy_client.egg-info/not-zip-safe
 src/dockerode_api_proxy_client.egg-info/requires.txt
 src/dockerode_api_proxy_client.egg-info/top_level.txt
 src/dockerode_api_proxy_client/dto/__init__.py
 src/dockerode_api_proxy_client/dto/container.py
 src/dockerode_api_proxy_client/dto/image.py
-src/dockerode_api_proxy_client/middleware/__init__.py
-src/dockerode_api_proxy_client/middleware/json_web_token_middleware.py
 src/dockerode_api_proxy_client/settings/__init__.py
 src/dockerode_api_proxy_client/settings/env.py
 src/dockerode_api_proxy_client/utils/__init__.py
+src/dockerode_api_proxy_client/utils/add_authentication_header.py
 src/dockerode_api_proxy_client/utils/datatype.py
-src/dockerode_api_proxy_client/utils/formatting.py
+src/dockerode_api_proxy_client/utils/formatting.py
+tests/test_add_authentication_header.py
+tests/test_client.py
+tests/test_datatype.py
+tests/test_formatting.py
```

