# Comparing `tmp/rcsb.app.file-0.24.tar.gz` & `tmp/rcsb.app.file-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.app.file-0.24.tar", last modified: Sat Mar 11 00:11:46 2023, max compression
+gzip compressed data, was "rcsb.app.file-0.25.tar", last modified: Fri Apr 28 18:52:19 2023, max compression
```

## Comparing `rcsb.app.file-0.24.tar` & `rcsb.app.file-0.25.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.930862 rcsb.app.file-0.24/
--rw-r--r--   0 vsts      (1001) docker     (122)     1384 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      112 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    10140 2023-03-11 00:11:46.930862 rcsb.app.file-0.24/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     9469 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.926862 rcsb.app.file-0.24/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.926862 rcsb.app.file-0.24/rcsb/app/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.926862 rcsb.app.file-0.24/rcsb/app/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    23528 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/client/ClientUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/client/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.926862 rcsb.app.file-0.24/rcsb/app/client/front-end/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/client/front-end/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10963 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/client/front-end/client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26280 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/client/front-end/gui.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.926862 rcsb.app.file-0.24/rcsb/app/config/
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/config/setConfig.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.930862 rcsb.app.file-0.24/rcsb/app/file/
--rw-r--r--   0 vsts      (1001) docker     (122)     2260 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/ConfigProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26648 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/Definitions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19098 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/IoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1415 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/JWTAuthBearer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1539 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/JWTAuthToken.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3539 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/KvConnection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/KvRedis.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4406 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/KvSqlite.py
--rw-r--r--   0 vsts      (1001) docker     (122)      858 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/LogFilterUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7571 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/PathUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4357 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/downloadRequest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2219 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)    31002 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/pathRequest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2789 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/serverStatus.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11576 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/rcsb/app/file/uploadRequest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-11 00:11:46.926862 rcsb.app.file-0.24/rcsb.app.file.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    10140 2023-03-11 00:11:46.000000 rcsb.app.file-0.24/rcsb.app.file.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1016 2023-03-11 00:11:46.000000 rcsb.app.file-0.24/rcsb.app.file.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-11 00:11:46.000000 rcsb.app.file-0.24/rcsb.app.file.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-11 00:11:44.000000 rcsb.app.file-0.24/rcsb.app.file.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      297 2023-03-11 00:11:46.000000 rcsb.app.file-0.24/rcsb.app.file.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-11 00:11:46.000000 rcsb.app.file-0.24/rcsb.app.file.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      335 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-11 00:11:46.930862 rcsb.app.file-0.24/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2150 2023-03-11 00:10:28.000000 rcsb.app.file-0.24/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1436 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      112 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    10286 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     9615 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb/app/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb/app/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18920 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/ClientUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.408066 rcsb.app.file-0.25/rcsb/app/client/front-end/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/front-end/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8619 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/front-end/client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17731 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/client/front-end/gui.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.408066 rcsb.app.file-0.25/rcsb/app/config/
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      331 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/config/setConfig.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/rcsb/app/file/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2338 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/ConfigProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26648 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/Definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17258 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/IoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1311 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/JWTAuthBearer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1504 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/JWTAuthToken.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3539 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/KvConnection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/KvRedis.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4380 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/KvSqlite.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      858 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/LogFilterUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7571 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/PathUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4158 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/downloadRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2014 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30421 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/pathRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2661 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/serverStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4282 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/rcsb/app/file/uploadRequest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-28 18:52:19.404066 rcsb.app.file-0.25/rcsb.app.file.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10286 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1016 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-28 18:51:05.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      297 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-28 18:52:19.000000 rcsb.app.file-0.25/rcsb.app.file.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      335 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-28 18:52:19.412066 rcsb.app.file-0.25/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2150 2023-04-28 18:49:49.000000 rcsb.app.file-0.25/setup.py
```

### Comparing `rcsb.app.file-0.24/HISTORY.txt` & `rcsb.app.file-0.25/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 25-Oct-2022  - V0.20 Add additional file/directory path request endpoints (file-exists, dir-exists, list-dir, file-copy)
  5-Dec-2022  - V0.21 Resumable uploads coordinated through database and new client interface
  3-Jan-2023  - V0.22 Redis with Docker support;
                      Add additional file/directory path request endpoints (path-exists, copy-filepath, compress-dir, compress-dirpath);
                      Configuration changes to support tox 4
  1-Mar-2023  - V0.23 Updates to and reorganization of client utilities
  10-Mar-2023 - V0.24 Rewrote config file path, jwt, shell scripts, and client context
+ 18-Apr-2023 - V0.25 Streamlined Redis transactions
```

### Comparing `rcsb.app.file-0.24/LICENSE` & `rcsb.app.file-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/PKG-INFO` & `rcsb.app.file-0.25/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.app.file
-Version: 0.24
+Version: 0.25
 Summary: RCSB File Access Service Application
 Home-page: https://github.com/rcsb/py-rcsb_app_file
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -78,22 +78,20 @@
 
 To upload the entire file in one request, configure the parameters to treat the file as one chunk.
 
 Upload requires some setup by invoking the 'file-v2/getUploadParameters' endpoint first, then passing the results as parameters.
 
 To maintain sequential order, the client must wait for each response before sending the next chunk.
 
-The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in both uploadRequest and IoUtils.
+The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtils.
 
 The download endpoint is found at 'file-v1/download'.
 
 The list directory endpoint is found at 'file-v1/list-dir'.
 
-For streamlining, the upload function has been partly duplicated in uploadRequest and IoUtils, so changes to one should be performed in the other.
-
 To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in IoUtils.py.
 
 # Uploads and downloads
 
 ### HTML examples
 
 The example-upload.html, example-download.html, and example-list.html files demonstrate requests to the endpoints from HTML.
@@ -106,17 +104,16 @@
 
 Client.py usage
 ```
 
 python3 client.py
 [-h (help)]
 [--upload source_file repo_type id content_type milestone part format version]
-[--download target_file repo_type id content_type milestone part format version]
+[--download target_folder repo_type id content_type milestone part format version]
 [--list repo_type dep_id (list directory)]
-[-s (chunk file sequentially)]
 [-r (chunk file resumably)]
 [-o (overwrite files with same name)]
 [-z (zip files prior to upload)]
 [-x (expand files after upload)]
 
 ```
 
@@ -126,14 +123,22 @@
 
 # Testing and deployment
 
 Testing is easiest without Docker and using a Sqlite database.
 
 For production, use a Docker container with a Redis database.
 
+Redis with Docker requires Redis in a Docker container.
+
+Production with multiple servers will require all servers to coordinate through a single remote Redis server.
+
+Since one server could host Redis while others don't, the docker instances could be run differently, or the config files set differently, on each server.
+
+Also, multiple servers must connect to a single file system for deposition.
+
 # Deployment on local server without docker
 
 For launching without docker, edit url in deploy/LAUNCH_GUNICORN.sh
 
 From base repository directory (in `py-rcsb_app_file/`), start app with:
 ```bash
 
@@ -236,15 +241,16 @@
 
 ### Connecting to Redis remotely
 
 If Redis runs on a different machine than the files API, then the host must be set to a url
 
 Change Redis host to '#:#:#:#' and port 6379 in rcsb/app/config/config.yml.
 
-For example
+KvRedis.py should resemble
+
 ```
 
 self.kV = redis.Redis(host='1.2.3.4', port=6379, decode_responses=True)
 
 ```
 
 Remote Redis requires changing the config file settings on the machine with Redis
@@ -272,23 +278,27 @@
 ```
 docker run --name redis-container -d redis
 or (if connecting remotely to Redis container on different server)
 docker run --name redis-container -p 6379:6379 -d redis
 ```
 
 If the Redis container runs on the same machine as the files API, change Redis host to 'redis' in rcsb/app/config/config.yml.
+
+KvRedis.py should resemble
+
 ```
 
-self.kV = redis.Redis(host='redis', decode_responses=True)
+self.kV = redis.Redis(host='redis', port=6379, decode_responses=True)
 
 ```
 
 Or, if connecting remotely to Redis container on different server, change Redis host to '#:#:#:#' and port 6379 in rcsb/app/config/config.yml.
 
-For example
+KvRedis.py should resemble
+
 ```
 
 self.kV = redis.Redis(host='1.2.3.4', port=6379, decode_responses=True)
 
 ```
 
 To view Redis variables
@@ -350,16 +360,14 @@
 
 `-p` allows user to choose a port, 8000:8000 is used in this case, as the port 8000 is exposed in the current dockerfile
 
 `--link` connects to a Redis container if the container is running on the same machine as the files API 
 
 # Error handling
 
-Errors related to 'shared locks' are generally fixed by deleting the 'shared-locks' directory and, if necessary, restarting.
-
 For production, Redis variables are set to expire periodically. However, hidden files are not, so a cron job should be run periodically to remove lingering hidden files from the deposit or archive directories.
 
 After development testing with a Sqlite database, open the kv.sqlite file and delete the tables, and delete hidden files from the deposit or archives directories.
 
 After development testing with Redis, open the redis-cli and delete the variables, and delete hidden files from the deposit or archives directories.
 
 The hidden files to be deleted are those that start with the value configured in getTempFilePath, referred to above, after checking that the file modification time is beyond a specified threshold.
```

### Comparing `rcsb.app.file-0.24/README.md` & `rcsb.app.file-0.25/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 To upload the entire file in one request, configure the parameters to treat the file as one chunk.
 
 Upload requires some setup by invoking the 'file-v2/getUploadParameters' endpoint first, then passing the results as parameters.
 
 To maintain sequential order, the client must wait for each response before sending the next chunk.
 
-The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in both uploadRequest and IoUtils.
+The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtils.
 
 The download endpoint is found at 'file-v1/download'.
 
 The list directory endpoint is found at 'file-v1/list-dir'.
 
-For streamlining, the upload function has been partly duplicated in uploadRequest and IoUtils, so changes to one should be performed in the other.
-
 To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in IoUtils.py.
 
 # Uploads and downloads
 
 ### HTML examples
 
 The example-upload.html, example-download.html, and example-list.html files demonstrate requests to the endpoints from HTML.
@@ -86,17 +84,16 @@
 
 Client.py usage
 ```
 
 python3 client.py
 [-h (help)]
 [--upload source_file repo_type id content_type milestone part format version]
-[--download target_file repo_type id content_type milestone part format version]
+[--download target_folder repo_type id content_type milestone part format version]
 [--list repo_type dep_id (list directory)]
-[-s (chunk file sequentially)]
 [-r (chunk file resumably)]
 [-o (overwrite files with same name)]
 [-z (zip files prior to upload)]
 [-x (expand files after upload)]
 
 ```
 
@@ -106,14 +103,22 @@
 
 # Testing and deployment
 
 Testing is easiest without Docker and using a Sqlite database.
 
 For production, use a Docker container with a Redis database.
 
+Redis with Docker requires Redis in a Docker container.
+
+Production with multiple servers will require all servers to coordinate through a single remote Redis server.
+
+Since one server could host Redis while others don't, the docker instances could be run differently, or the config files set differently, on each server.
+
+Also, multiple servers must connect to a single file system for deposition.
+
 # Deployment on local server without docker
 
 For launching without docker, edit url in deploy/LAUNCH_GUNICORN.sh
 
 From base repository directory (in `py-rcsb_app_file/`), start app with:
 ```bash
 
@@ -216,15 +221,16 @@
 
 ### Connecting to Redis remotely
 
 If Redis runs on a different machine than the files API, then the host must be set to a url
 
 Change Redis host to '#:#:#:#' and port 6379 in rcsb/app/config/config.yml.
 
-For example
+KvRedis.py should resemble
+
 ```
 
 self.kV = redis.Redis(host='1.2.3.4', port=6379, decode_responses=True)
 
 ```
 
 Remote Redis requires changing the config file settings on the machine with Redis
@@ -252,23 +258,27 @@
 ```
 docker run --name redis-container -d redis
 or (if connecting remotely to Redis container on different server)
 docker run --name redis-container -p 6379:6379 -d redis
 ```
 
 If the Redis container runs on the same machine as the files API, change Redis host to 'redis' in rcsb/app/config/config.yml.
+
+KvRedis.py should resemble
+
 ```
 
-self.kV = redis.Redis(host='redis', decode_responses=True)
+self.kV = redis.Redis(host='redis', port=6379, decode_responses=True)
 
 ```
 
 Or, if connecting remotely to Redis container on different server, change Redis host to '#:#:#:#' and port 6379 in rcsb/app/config/config.yml.
 
-For example
+KvRedis.py should resemble
+
 ```
 
 self.kV = redis.Redis(host='1.2.3.4', port=6379, decode_responses=True)
 
 ```
 
 To view Redis variables
@@ -330,16 +340,14 @@
 
 `-p` allows user to choose a port, 8000:8000 is used in this case, as the port 8000 is exposed in the current dockerfile
 
 `--link` connects to a Redis container if the container is running on the same machine as the files API 
 
 # Error handling
 
-Errors related to 'shared locks' are generally fixed by deleting the 'shared-locks' directory and, if necessary, restarting.
-
 For production, Redis variables are set to expire periodically. However, hidden files are not, so a cron job should be run periodically to remove lingering hidden files from the deposit or archive directories.
 
 After development testing with a Sqlite database, open the kv.sqlite file and delete the tables, and delete hidden files from the deposit or archives directories.
 
 After development testing with Redis, open the redis-cli and delete the variables, and delete hidden files from the deposit or archives directories.
 
 The hidden files to be deleted are those that start with the value configured in getTempFilePath, referred to above, after checking that the file modification time is beyond a specified threshold.
```

### Comparing `rcsb.app.file-0.24/rcsb/app/client/ClientUtils.py` & `rcsb.app.file-0.25/rcsb/app/client/ClientUtils.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,24 +12,22 @@
 
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "john.westbrook@rcsb.org"
 __license__ = "Apache 2.0"
 
 import os
-import io
 import logging
 import tempfile
 from copy import deepcopy
 import math
 import json
 import requests
 import typing
 from fastapi.testclient import TestClient
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
 from rcsb.utils.io.CryptUtils import CryptUtils
 from rcsb.app.file.JWTAuthToken import JWTAuthToken
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.Definitions import Definitions
 from rcsb.app.file.main import app
 from rcsb.app.file.PathUtils import PathUtils
 from rcsb.utils.io.FileUtil import FileUtil
@@ -71,15 +69,15 @@
             contentFormat,
             version,
             hashType,
             unit_test,
         )
 
 
-# dodge circular reference to client utils by including class in same file
+# dodge circular reference error from client utils by including class in same file
 class ClientContext(object):
     def __init__(
         self,
         repositoryType,
         depositId,
         contentType,
         milestone,
@@ -110,15 +108,14 @@
             self.repositoryType,
             self.depositId,
             self.contentType,
             self.milestone,
             self.partNumber,
             self.contentFormat,
             self.version,
-            self.hashType,
             downloadFolder,
             allowOverwrite,
             returnTempFile,
         )
         self.tempFilePath = self.file.name
         return self.file
 
@@ -134,32 +131,31 @@
             self.contentType,
             self.milestone,
             self.partNumber,
             self.contentFormat,
             self.version,
             decompress,
             allowOverwrite,
-            resumable,
+            resumable
         )
         # delete local file
         self.file.close()
 
 
 class ClientUtils(object):
     def __init__(self, unit_test=False):
-        configFilePath = os.environ.get("CONFIG_FILE")
-        self.cP = ConfigProvider(configFilePath)
+        self.cP = ConfigProvider()
         self.cP.getConfig()
         self.baseUrl = self.cP.get("SERVER_HOST_AND_PORT")
         self.chunkSize = self.cP.get("CHUNK_SIZE")
         self.hashType = self.cP.get("HASH_TYPE")
         subject = self.cP.get("JWT_SUBJECT")
         self.headerD = {
             "Authorization": "Bearer "
-            + JWTAuthToken(configFilePath).createToken({}, subject)
+            + JWTAuthToken().createToken({}, subject)
         }
         self.dP = Definitions()
         self.fileFormatExtensionD = self.dP.fileFormatExtD
         self.contentTypeInfoD = self.dP.contentTypeD
         self.repoTypeList = self.dP.repoTypeList
         self.milestoneList = self.dP.milestoneList
         self.__unit_test = unit_test
@@ -174,15 +170,15 @@
         contentType,
         milestone,
         partNumber,
         contentFormat,
         version,
         decompress,
         allowOverwrite,
-        resumable,
+        resumable
     ):
         if not os.path.exists(sourceFilePath):
             logger.error("File does not exist: %r", sourceFilePath)
             return None
         # compress (externally), then hash, then upload
         # hash
         hD = CryptUtils().getFileHash(sourceFilePath, hashType=self.hashType)
@@ -200,252 +196,110 @@
             "repositoryType": repositoryType,
             "depId": depId,
             "contentType": contentType,
             "milestone": milestone,
             "partNumber": partNumber,
             "contentFormat": contentFormat,
             "version": version,
-            "hashDigest": fullTestHash,
             "allowOverwrite": allowOverwrite,
-            "resumable": resumable,
+            # "hashDigest": fullTestHash,
+            "resumable": resumable
         }
         url = os.path.join(self.baseUrl, "file-v2", "getUploadParameters")
         response = None
         if not self.__unit_test:
             response = requests.get(
                 url, params=parameters, headers=self.headerD, timeout=None
             )
         else:
             with TestClient(app) as client:
                 response = client.get(
                     url, params=parameters, headers=self.headerD, timeout=None
                 )
-        # logger.info("status code %r", response.status_code)
         if response.status_code == 200:
             result = json.loads(response.text)
             if result:
                 saveFilePath = result["filePath"]
-                chunkIndex = result["chunkIndex"]
+                chunkIndex = int(result["chunkIndex"])
                 uploadId = result["uploadId"]
-        if not saveFilePath or not uploadId:
-            logger.error("No file path or upload id were formed")
+                if chunkIndex > 0:
+                    logger.info(f"detected upload with chunk index {chunkIndex}")
+        if not saveFilePath:
+            logger.error("No file path was formed")
+            return None
+        if not uploadId:
+            logger.error("No upload id was formed")
             return None
+
         # chunk file and upload
         mD = {
             # chunk parameters
             "chunkSize": self.chunkSize,
             "chunkIndex": chunkIndex,
             "expectedChunks": expectedChunks,
             # upload file parameters
             "uploadId": uploadId,
             "hashType": self.hashType,
             "hashDigest": fullTestHash,
-            "resumable": resumable,
             # save file parameters
             "filePath": saveFilePath,
             "decompress": decompress,
             "allowOverwrite": allowOverwrite,
+            "resumable": resumable
         }
         offset = chunkIndex * self.chunkSize
         response = None
-        tmp = io.BytesIO()
-        with open(sourceFilePath, "rb") as fUpload:
-            fUpload.seek(offset)
+        with open(sourceFilePath, "rb") as of:
+            of.seek(offset)
             url = os.path.join(self.baseUrl, "file-v2", "upload")
             for _ in range(chunkIndex, mD["expectedChunks"]):
                 packetSize = min(
                     int(fileSize) - (int(mD["chunkIndex"]) * int(self.chunkSize)),
                     int(self.chunkSize),
                 )
-                tmp.truncate(packetSize)
-                tmp.seek(0)
-                tmp.write(fUpload.read(packetSize))
-                tmp.seek(0)
-
+                logger.debug("packet size %s chunk %s expected %s", packetSize, mD['chunkIndex'], expectedChunks)
                 if not self.__unit_test:
                     response = requests.post(
                         url,
                         data=deepcopy(mD),
                         headers=self.headerD,
-                        files={"chunk": tmp},
+                        files={"chunk": of.read(packetSize)},
                         stream=True,
                         timeout=None,
                     )
                 else:
                     with TestClient(app) as client:
                         response = client.post(
                             url,
                             data=deepcopy(mD),
                             headers=self.headerD,
-                            files={"chunk": tmp},
+                            files={"chunk": of.read(packetSize)},
                             timeout=None,
                         )
 
                 if response.status_code != 200:
                     logger.error(
                         "Status code %r with text %r ...terminating",
                         response.status_code,
                         response.text,
                     )
                     break
                 mD["chunkIndex"] += 1
-        return response
-
-    # file parameter is one chunk
-
-    def getUploadParameters(
-        self,
-        sourceFilePath,
-        repositoryType,
-        depId,
-        contentType,
-        milestone,
-        partNumber,
-        contentFormat,
-        version,
-        allowOverwrite,
-        resumable,
-    ):
-        if not os.path.exists(sourceFilePath):
-            logger.error("File does not exist: %r", sourceFilePath)
-            return None
-        # compress (externally), then hash, then upload
-        # hash
-        hD = CryptUtils().getFileHash(sourceFilePath, hashType=self.hashType)
-        fullTestHash = hD["hashDigest"]
-        # get upload parameters
-        saveFilePath = None
-        chunkIndex = 0
-        uploadId = None
-        parameters = {
-            "repositoryType": repositoryType,
-            "depId": depId,
-            "contentType": contentType,
-            "milestone": milestone,
-            "partNumber": partNumber,
-            "contentFormat": contentFormat,
-            "version": version,
-            "hashDigest": fullTestHash,
-            "allowOverwrite": allowOverwrite,
-            "resumable": resumable,
-        }
-        url = os.path.join(self.baseUrl, "file-v2", "getUploadParameters")
-
-        if not self.__unit_test:
-            response = requests.get(
-                url, params=parameters, headers=self.headerD, timeout=None
-            )
-        else:
-            with TestClient(app) as client:
-                response = client.get(
-                    url, params=parameters, headers=self.headerD, timeout=None
-                )
-
-        if response.status_code == 200:
-            result = json.loads(response.text)
-            if result:
-                saveFilePath = result["filePath"]
-                chunkIndex = result["chunkIndex"]
-                uploadId = result["uploadId"]
-        if not saveFilePath or not uploadId:
-            logger.error("error - no file path or upload id were formed")
-            return None
-        # compute expected chunks
-        fileSize = os.path.getsize(sourceFilePath)
-        expectedChunks = 1
-        if self.chunkSize < fileSize:
-            expectedChunks = math.ceil(fileSize / self.chunkSize)
-        return saveFilePath, chunkIndex, expectedChunks, uploadId, fullTestHash
-
-    # file parameter is one chunk
 
-    def uploadChunk(
-        self,
-        sourceFilePath,
-        saveFilePath,
-        chunkIndex,
-        expectedChunks,
-        uploadId,
-        fullTestHash,
-        decompress,
-        allowOverwrite,
-        resumable,
-    ):
-        if not os.path.exists(sourceFilePath):
-            logger.error("File does not exist: %r", sourceFilePath)
-            return None
-        # chunk file and upload
-        mD = {
-            # chunk parameters
-            "chunkSize": self.chunkSize,
-            "chunkIndex": chunkIndex,
-            "expectedChunks": expectedChunks,
-            # upload file parameters
-            "uploadId": uploadId,
-            "hashType": self.hashType,
-            "hashDigest": fullTestHash,
-            "resumable": resumable,
-            # save file parameters
-            "filePath": saveFilePath,
-            "decompress": decompress,
-            "allowOverwrite": allowOverwrite,
-        }
-        fileSize = os.path.getsize(sourceFilePath)
-        offset = chunkIndex * self.chunkSize
-        response = None
-        tmp = io.BytesIO()
-        with open(sourceFilePath, "rb") as toUpload:
-            toUpload.seek(offset)
-            packetSize = min(
-                int(fileSize) - int(offset),
-                int(self.chunkSize),
-            )
-            tmp.truncate(packetSize)
-            tmp.seek(0)
-            tmp.write(toUpload.read(packetSize))
-            tmp.seek(0)
-            url = os.path.join(self.baseUrl, "file-v2", "upload")
-
-            if not self.__unit_test:
-                response = requests.post(
-                    url,
-                    data=deepcopy(mD),
-                    headers=self.headerD,
-                    files={"chunk": tmp},
-                    stream=True,
-                    timeout=None,
-                )
-            else:
-                with TestClient(app) as client:
-                    response = client.post(
-                        url,
-                        data=deepcopy(mD),
-                        headers=self.headerD,
-                        files={"chunk": tmp},
-                        timeout=None,
-                    )
-
-            if response.status_code != 200:
-                logger.error(
-                    "Terminating with status code %r and response text: %r",
-                    response.status_code,
-                    response.text,
-                )
         return response
 
     def download(
         self,
         repositoryType: str,
         depId: str,
         contentType: str,
         milestone: str,
         partNumber: int,
         contentFormat: str,
         version: str,
-        hashType: str = "MD5",
         downloadFolder: typing.Optional[str] = None,
         allowOverwrite: bool = False,
         returnTempFile: bool = False,
         deleteTempFile: bool = True,
         chunkSize: typing.Optional[int] = None,
         chunkIndex: typing.Optional[int] = None
     ):
@@ -464,27 +318,28 @@
             fileName = f"{depId}_{contentType}{convertedMilestone}_P{partNumber}.{convertedContentFormat}.V{version}"
             downloadFilePath = os.path.join(downloadFolder, "download" + "_" + fileName)
             if os.path.exists(downloadFilePath):
                 if not allowOverwrite:
                     logger.error("File already exists: %r", downloadFilePath)
                     return None
                 os.remove(downloadFilePath)
-
+        hashType = self.hashType
         downloadUrlPrefix = os.path.join(self.baseUrl, "file-v1", "download")
         suffix = ""
         if chunkSize and chunkIndex:
             suffix = f"&chunkSize={chunkSize}&chunkIndex={chunkIndex}"
         downloadUrl = (
             f"{downloadUrlPrefix}?repositoryType={repositoryType}&depId={depId}&contentType={contentType}&milestone={milestone}"
             f"&partNumber={partNumber}&contentFormat={contentFormat}&version={version}&hashType={hashType}{suffix}"
         )
         resp = None
 
         if not self.__unit_test:
             if not returnTempFile:
+                # download file to folder, return http response
                 with requests.get(
                     downloadUrl, headers=self.headerD, timeout=None, stream=True
                 ) as response:
                     if response and response.status_code == 200:
                         with open(downloadFilePath, "ab") as ofh:
                             for chunk in response.iter_content(
                                 chunk_size=self.chunkSize
@@ -497,14 +352,15 @@
                             downloadFilePath, hashType=rspHashType
                         )
                         if not thD["hashDigest"] == rspHashDigest:
                             logger.error("Hash comparison failed")
                             return None
                         resp = response
             else:
+                # client context, return open file handle
                 with requests.get(
                     downloadUrl, headers=self.headerD, timeout=None, stream=True
                 ) as response:
                     if response and response.status_code == 200:
                         ofh = tempfile.NamedTemporaryFile(delete=deleteTempFile)
                         for chunk in response.iter_content(chunk_size=self.chunkSize):
                             if chunk:
@@ -515,14 +371,15 @@
                         if not thD["hashDigest"] == rspHashDigest:
                             logger.error("Hash comparison failed")
                             return None
                         resp = ofh
         else:
             resp = None
             if not returnTempFile:
+                # test download file, return http response
                 with TestClient(app) as client:
                     response = client.get(
                         downloadUrl, headers=self.headerD, timeout=None
                     )
                     if response and response.status_code == 200:
                         with open(downloadFilePath, "ab") as ofh:
                             ofh.write(response.content)
@@ -532,14 +389,15 @@
                             downloadFilePath, hashType=rspHashType
                         )
                         if not thD["hashDigest"] == rspHashDigest:
                             logger.error("Hash comparison failed")
                             return None
                         resp = response.status_code
             else:
+                # test client context
                 with TestClient(app) as client:
                     response = client.get(
                         downloadUrl, headers=self.headerD, timeout=None
                     )
                     if response and response.status_code == 200:
                         ofh = tempfile.NamedTemporaryFile(delete=deleteTempFile)
                         ofh.write(response.content)
@@ -658,15 +516,14 @@
             repoType,
             depId,
             contentType,
             milestone,
             partNumber,
             contentFormat,
             version,
-            hashType,
             downloadFolder,
             allowOverwrite,
             returnTempFile,
             deleteTempFile,
         )
         return file.name
```

### Comparing `rcsb.app.file-0.24/rcsb/app/client/front-end/client.py` & `rcsb.app.file-0.25/rcsb/app/client/front-end/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,39 @@
 import sys
 import concurrent.futures
 import os
 import gzip
 from concurrent.futures import ThreadPoolExecutor
-import requests
-import json
-from tqdm.auto import tqdm
 import time
-import math
 import argparse
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
-from rcsb.utils.io.CryptUtils import CryptUtils
 from rcsb.app.file.JWTAuthToken import JWTAuthToken
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.IoUtils import IoUtils
 from rcsb.app.client.ClientUtils import ClientUtils
 
 """
 author James Smith 2023
 """
 
-
-configFilePath = os.environ.get("CONFIG_FILE")
-cP = ConfigProvider(configFilePath)
+cP = ConfigProvider()
 cP.getConfig()
 
 """ modifiable variables
 """
 base_url = cP.get("SERVER_HOST_AND_PORT")
 maxChunkSize = cP.get("CHUNK_SIZE")
 hashType = cP.get("HASH_TYPE")
 """ do not alter from here
 """
 subject = cP.get("JWT_SUBJECT")
 ioU = IoUtils(cP)
 cU = ClientUtils()
 headerD = {
     "Authorization": "Bearer "
-    + JWTAuthToken(configFilePath).createToken({}, subject)
+    + JWTAuthToken().createToken({}, subject)
 }
 RESUMABLE = False
 COMPRESS = False
 DECOMPRESS = False
 OVERWRITE = False
 uploadIds = []
 uploadResults = []
@@ -56,15 +48,14 @@
 
 def upload(mD):
     global COMPRESS
     global DECOMPRESS
     global RESUMABLE
     global OVERWRITE
     global cU
-    t1 = time.perf_counter()
     readFilePath = mD["filePath"]
     respositoryType = mD["repositoryType"]
     depId = mD["depId"]
     contentType = mD["contentType"]
     milestone = mD["milestone"]
     partNumber = mD["partNumber"]
     contentFormat = mD["contentFormat"]
@@ -79,71 +70,50 @@
     # compress, then hash, then upload
     if COMPRESS:
         tempPath = readFilePath + ".gz"
         with open(readFilePath, "rb") as r:
             with gzip.open(tempPath, "wb") as w:
                 w.write(r.read())
         readFilePath = tempPath
-    # get upload parameters
-    response = cU.getUploadParameters(readFilePath, repositoryType, depId, contentType, milestone, partNumber, contentFormat, version, OVERWRITE, RESUMABLE)
+    # upload
+    response = cU.upload(readFilePath, respositoryType, depId, contentType, milestone, partNumber, contentFormat, version, DECOMPRESS, OVERWRITE, RESUMABLE)
     if not response:
-        print("error in get upload parameters")
-        return
-    saveFilePath, chunkIndex, expectedChunks, uploadId, fullTestHash = response
-    # upload chunks
-    for index in tqdm(range(chunkIndex,expectedChunks), leave=False, total=expectedChunks - chunkIndex, desc=os.path.basename(readFilePath)):
-        response = cU.uploadChunk(readFilePath, saveFilePath, index, expectedChunks, uploadId, fullTestHash, DECOMPRESS, OVERWRITE, RESUMABLE)
-        if not response:
-            print("error in upload chunk")
-            break
+        print("error in upload")
+        return None
     return response
 
 
-def download(downloadFilePath, downloadDict):
+def download(downloadFolderPath, downloadDict):
     global headerD
     global maxChunkSize
     global COMPRESS
     global DECOMPRESS
     global SEQUENTIAL
     global OVERWRITE
-    url = os.path.join(base_url, "file-v1", "downloadSize")
-    fileSize = requests.get(url, params=downloadDict, headers=headerD, timeout=None).text
-    if not fileSize or not fileSize.isnumeric():
-        print(f"error - no response for {downloadDict}")
+    global cU
+    if not os.path.exists(downloadFolderPath):
+        print(f"error - download folder does not exist - {downloadFolderPath}")
         return None
-    fileSize = int(fileSize)
-    chunkSize = maxChunkSize
-    chunks = math.ceil(fileSize / maxChunkSize)
-    url = os.path.join(base_url, "file-v1", "download")
-    responseCode = None
-    count = 0
-    if os.path.isdir(downloadFilePath):
-        print(f'error - path is a directory {downloadFilePath}')
+    response = cU.download(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version, downloadFolderPath, allowOverwrite)
+    if response and response.status_code:
+        return response.status_code
+    else:
         return None
-    if os.path.exists(downloadFilePath):
-        if OVERWRITE:
-            os.remove(downloadFilePath)
-        else:
-            print(f"error - file already exists {downloadFilePath}")
-            return None
-    with requests.get(url, params=downloadDict, headers=headerD, timeout=None, stream=True) as response:
-        with open(downloadFilePath, "ab") as ofh:
-            for chunk in tqdm(response.iter_content(chunk_size=chunkSize), leave=False, total=chunks, desc=os.path.basename(downloadFilePath)):
-                if chunk:
-                    ofh.write(chunk)
-                count += 1
-        responseCode = response.status_code
-        rspHashType = response.headers["rcsb_hash_type"]
-        rspHashDigest = response.headers["rcsb_hexdigest"]
-        thD = CryptUtils().getFileHash(downloadFilePath, hashType=rspHashType)
-        if not thD["hashDigest"] == rspHashDigest:
-            print("error - hash comparison failed")
-            sys.exit()
-    return responseCode
 
+def listDir(repoType, depId):
+    global cU
+    dirList = cU.listDir(repoType, depId)
+    if dirList and len(dirList) > 0:
+        print("\n")
+        print(f"{repoType} {depId}")
+        for fi in sorted(dirList):
+            print(f"\t{fi}")
+        print("\n")
+    else:
+        print("\nerror - not found\n")
 
 def description():
     print()
     print(signature)
     print()
 
 
@@ -153,15 +123,15 @@
         description()
         sys.exit("error - please run with -h for instructions")
     parser = argparse.ArgumentParser(description=signature, formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("-u", "--upload", nargs=8, action="append",
                         metavar=("file-path", "repo-type", "dep-id", "content-type", "milestone", "part-number", "content-format", "version"),
                         help="***** multiple uploads allowed *****")
     parser.add_argument("-d", "--download", nargs=8, action="append",
-                        metavar=("file-path", "repo-type", "dep-id", "content-type", "milestone", "part-number", "content-format", "version"),
+                        metavar=("folder-path", "repo-type", "dep-id", "content-type", "milestone", "part-number", "content-format", "version"),
                         help="***** multiple downloads allowed *****")
     parser.add_argument("-l", "--list", nargs=2, metavar=("repository-type", "dep-id"), help="***** list contents of requested directory *****")
     parser.add_argument("-r", "--resumable", action="store_true", help="***** upload resumable sequential chunks *****")
     parser.add_argument("-o", "--overwrite", action="store_true", help="***** overwrite files with same name *****")
     parser.add_argument("-z", "--zip", action="store_true", help="***** zip files prior to upload *****")
     parser.add_argument("-x", "--expand", action="store_true", help="***** unzip files after upload *****")
     args = parser.parse_args()
@@ -205,15 +175,15 @@
                     "version": version,
                 }
             )
     if args.download:
         for arglist in args.download:
             if len(arglist) < 8:
                 sys.exit(f"error - wrong number of args to download {len(arglist)}")
-            downloadFilePath = arglist[0]
+            downloadFolderPath = arglist[0]
             repositoryType = arglist[1]
             depId = arglist[2]
             contentType = arglist[3]
             milestone = arglist[4]
             if milestone.lower() == "none":
                 milestone = ""
             partNumber = arglist[5]
@@ -227,15 +197,15 @@
                 "contentFormat": contentFormat,
                 "partNumber": partNumber,
                 "version": str(version),
                 "hashType": hashType,
                 "milestone": milestone,
                 "allowOverwrite": allowOverwrite
             }
-            downloads.append((downloadFilePath, downloadDict))
+            downloads.append((downloadFolderPath, downloadDict))
     if len(uploads) > 0:
         # upload concurrent files sequential chunks
         with ThreadPoolExecutor(max_workers=10) as executor:
             futures = {executor.submit(upload, u): u for u in uploads}
             results = []
             for future in concurrent.futures.as_completed(futures):
                 results.append(future.result())
@@ -258,27 +228,12 @@
         print(f"download results {downloadResults}")
     if args.list:
         arglist = args.list
         if not len(arglist) == 2:
             sys.exit("error - list takes two args")
         repoType = arglist[0]
         depId = arglist[1]
-        parameters = {
-            "depId": depId,
-            "repositoryType": repoType
-        }
-        url = os.path.join(base_url, "file-v1", "list-dir")
-        responseCode = None
-        dirList = None
-        with requests.get(url, params=parameters, headers=headerD, timeout=None) as response:
-            responseCode = response.status_code
-            if responseCode == 200:
-                resp = response.text
-                if resp:
-                    if not isinstance(resp, dict):
-                        resp = json.loads(resp)
-                    dirList = resp["dirList"]
-        print(f"response {responseCode}")
-        if responseCode == 200:
-            for fi in sorted(dirList):
-                print(f"\t{fi}")
+        listDir(repoType, depId)
+
+
+
     print("time %.2f seconds" % (time.perf_counter() - t1))
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/ConfigProvider.py` & `rcsb.app.file-0.25/rcsb/app/file/ConfigProvider.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             if not self.__configD:
                 if self.__configFilePath:
                     self.__readConFigFromConFigYmlFile()
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return self.__configD["data"]
 
+    def getConfigFilePath(self) -> str:
+        return self.__configFilePath
+
     def getVersion(self) -> typing.Optional[str]:
         try:
             return self.__configD["version"]
         except Exception:
             pass
         return None
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/Definitions.py` & `rcsb.app.file-0.25/rcsb/app/file/Definitions.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/rcsb/app/file/IoUtils.py` & `rcsb.app.file-0.25/rcsb/app/file/IoUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 import gzip
 import hashlib
 import logging
 import os
 import typing
 import uuid
 import aiofiles
-import re
 import json
 from filelock import Timeout, FileLock
 from fastapi import HTTPException
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.PathUtils import PathUtils
 from rcsb.app.file.KvSqlite import KvSqlite
 from rcsb.app.file.KvRedis import KvRedis
 
-logging.basicConfig(level=logging.INFO, format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s")
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s",
+)
 logger = logging.getLogger()
 
 
 class IoUtils:
     """Collected utilities request I/O processing.
 
     1. Upload a single file (only write new versions)
@@ -66,15 +67,17 @@
             self.__kV = KvRedis(self.__cP)
         self.__pathU = PathUtils(self.__cP)
 
     def checkHash(self, pth: str, hashDigest: str, hashType: str) -> bool:
         tHash = self.getHashDigest(pth, hashType)
         return tHash == hashDigest
 
-    def getHashDigest(self, filePath: str, hashType: str = "SHA1", blockSize: int = 65536) -> typing.Optional[str]:
+    def getHashDigest(
+        self, filePath: str, hashType: str = "SHA1", blockSize: int = 65536
+    ) -> typing.Optional[str]:
         """Return the hash (hashType) for the input file.
 
         Args:
             filePath (str): for input file path
             hashType (str, optional): one of MD5, SHA1, or SHA256. Defaults to "SHA1".
             blockSize (int, optional): the size of incremental read operations. Defaults to 65536.
 
@@ -95,60 +98,142 @@
                 for block in iter(lambda: ifh.read(blockSize), b""):
                     hashObj.update(block)
             return hashObj.hexdigest()
         except Exception as e:
             logger.exception("Failing with file %s %r", filePath, str(e))
         return None
 
+    async def getUploadParameters(
+        self,
+        repositoryType: str,
+        depId: str,
+        contentType: str,
+        milestone: typing.Optional[str],
+        partNumber: int,
+        contentFormat: str,
+        version: str,
+        allowOverwrite: bool,
+        # hashDigest: str,
+        resumable: bool,
+    ):
+        # get save file path
+        if not self.__pathU.checkContentTypeFormat(contentType, contentFormat):
+            logging.warning("Bad content type and/or format")
+            raise HTTPException(
+                status_code=400, detail="Error - bad content type and/or format"
+            )
+        outPath = self.__pathU.getVersionedPath(
+            repositoryType=repositoryType,
+            depId=depId,
+            contentType=contentType,
+            milestone=milestone,
+            partNumber=partNumber,
+            contentFormat=contentFormat,
+            version=version,
+        )
+        if not outPath:
+            logging.warning("Error - could not make file path from parameters")
+            raise HTTPException(
+                status_code=400,
+                detail="Error - could not make file path from parameters",
+            )
+        if os.path.exists(outPath) and not allowOverwrite:
+            logging.warning("Encountered existing file - overwrite prohibited")
+            raise HTTPException(
+                status_code=400,
+                detail="Encountered existing file - overwrite prohibited",
+            )
+        dirPath, _ = os.path.split(outPath)
+        os.makedirs(dirPath, mode=0o777, exist_ok=True)
+        # get upload id
+        uploadId = None
+        if resumable:
+            uploadId = await self.getResumedUpload(
+                repositoryType=repositoryType,
+                depId=depId,
+                contentType=contentType,
+                milestone=milestone,
+                partNumber=partNumber,
+                contentFormat=contentFormat,
+                version=version,
+                # hashDigest=hashDigest,
+            )
+        if not uploadId:
+            uploadId = self.getNewUploadId()
+        # get chunk index
+        uploadCount = 0
+        if uploadId:
+            status = await self.getSession(uploadId)
+            if status:
+                status = str(status)
+                status = status.replace("'", '"')
+                status = json.loads(status)
+                if "chunkSize" in status:
+                    chunkSize = int(status["chunkSize"])
+                    tempPath = self.getTempFilePath(uploadId, dirPath)
+                    if os.path.exists(tempPath):
+                        fileSize = os.path.getsize(tempPath)
+                        uploadCount = round(fileSize / chunkSize)
+        return {"filePath": outPath, "chunkIndex": uploadCount, "uploadId": uploadId}
+
     # in-place sequential chunk
     async def upload(
-            self,
-            # chunk parameters
-            chunk: typing.IO,
-            chunkSize: int,
-            chunkIndex: int,
-            expectedChunks: int,
-            # upload file parameters
-            uploadId: str,
-            hashType: str,
-            hashDigest: str,
-            resumable: bool,
-            # save file parameters
-            filePath: str,
-            decompress: bool,
-            allowOverwrite: bool,
+        self,
+        # chunk parameters
+        chunk: typing.IO,
+        chunkSize: int,
+        chunkIndex: int,
+        expectedChunks: int,
+        # upload file parameters
+        uploadId: str,
+        hashType: str,
+        hashDigest: str,
+        # save file parameters
+        filePath: str,
+        decompress: bool,
+        allowOverwrite: bool,
+        # other
+        resumable: bool,
     ):
         if resumable:
-            repositoryType = os.path.basename(os.path.dirname(os.path.dirname(filePath)))
-            logKey = self.getPremadeLogKey(repositoryType, filePath)
+            repositoryType = os.path.basename(
+                os.path.dirname(os.path.dirname(filePath))
+            )
             key = uploadId
-            val = "uploadCount"
-            # initializes to zero
-            currentCount = int(self.__kV.getSession(key, val))  # for sequential chunks, current index = current count
-            # on first chunk upload, set expected count, record uid in log table
-            if currentCount == 0:
-                self.__kV.setSession(key, "expectedCount", expectedChunks)
+            logKey = self.getPremadeLogKey(repositoryType, filePath)
+            # on first chunk upload, set chunk size, record uid in log table
+            if chunkIndex == 0:
+                self.__kV.setSession(key, "chunkSize", chunkSize)
                 self.__kV.setLog(logKey, uploadId)
-                self.__kV.setSession(key, "timestamp", int(datetime.datetime.timestamp(datetime.datetime.now(datetime.timezone.utc))))
-                self.__kV.setSession(key, "hashDigest", hashDigest)  # if user uploads new file with same parameters before saving previous file, delete previous file
-                self.__kV.setSession(key, "uploadId", key)  # redundant, however returns id from get upload status
-            self.__kV.inc(key, val)
+                self.__kV.setSession(
+                    key,
+                    "timestamp",
+                    int(
+                        datetime.datetime.timestamp(
+                            datetime.datetime.now(datetime.timezone.utc)
+                        )
+                    ),
+                )
+
+        logger.debug("chunk %s of %s for %s", chunkIndex, expectedChunks, uploadId)
 
-        chunkOffset = chunkIndex * chunkSize
         ret = {"success": True, "statusCode": 200, "statusMessage": "Chunk uploaded"}
         dirPath, _ = os.path.split(filePath)
         tempPath = self.getTempFilePath(uploadId, dirPath)
+        contents = chunk.read()
+        # empty chunk beyond loop index from client side, don't erase temp file so keep out of try block
+        if contents and len(contents) <= 0:
+            # outside of try block an exception will exit
+            chunk.close()
+            raise HTTPException(status_code=400, detail="error - empty file")
         try:
             # save, then hash, then decompress
             # should lock, however client must wait for each response before sending next chunk, precluding race conditions (unless multifile upload problem)
             async with aiofiles.open(tempPath, "ab") as ofh:
-                await ofh.seek(chunkOffset)
-                await ofh.write(chunk.read())
-                await ofh.flush()
-                os.fsync(ofh.fileno())
+                await ofh.write(contents)
             # if last chunk
             if chunkIndex + 1 == expectedChunks:
                 if hashDigest and hashType:
                     if hashType == "SHA1":
                         hashObj = hashlib.sha1()
                     elif hashType == "SHA256":
                         hashObj = hashlib.sha256()
@@ -156,32 +241,42 @@
                         hashObj = hashlib.md5()
                     blockSize = 65536
                     # hash temp file
                     with open(tempPath, "rb") as r:
                         while hash_chunk := r.read(blockSize):
                             hashObj.update(hash_chunk)
                     hexdigest = hashObj.hexdigest()
-                    ok = (hexdigest == hashDigest)
+                    ok = hexdigest == hashDigest
                     if not ok:
-                        raise HTTPException(status_code=400, detail=f"{hashType} hash check failed")
+                        raise HTTPException(
+                            status_code=400, detail=f"{hashType} hash check failed"
+                        )
                     else:
                         # lock then save
-                        lockPath = os.path.join(os.path.dirname(filePath), "." + os.path.basename(filePath) + ".lock")
+                        lockPath = os.path.join(
+                            os.path.dirname(filePath),
+                            "." + os.path.basename(filePath) + ".lock",
+                        )
                         lock = FileLock(lockPath)
                         try:
                             with lock.acquire(timeout=60 * 60 * 4):
                                 # last minute race condition handling
                                 if os.path.exists(filePath) and not allowOverwrite:
-                                    raise HTTPException(status_code=400,
-                                                        detail="Encountered existing file - cannot overwrite")
+                                    raise HTTPException(
+                                        status_code=400,
+                                        detail="Encountered existing file - cannot overwrite",
+                                    )
                                 else:
                                     # save final version
                                     os.replace(tempPath, filePath)
                         except Timeout:
-                            raise HTTPException(status_code=400, detail=f"error - lock timed out on {filePath}")
+                            raise HTTPException(
+                                status_code=400,
+                                detail=f"error - lock timed out on {filePath}",
+                            )
                         finally:
                             lock.release()
                             if os.path.exists(lockPath):
                                 os.unlink(lockPath)
                     # remove temp file
                     if os.path.exists(tempPath):
                         os.unlink(tempPath)
@@ -197,73 +292,63 @@
                 if resumable:
                     self.clearSession(key, logKey)
         except HTTPException as exc:
             if os.path.exists(tempPath):
                 os.unlink(tempPath)
             if resumable:
                 self.clearSession(key, logKey)
-            ret = {"success": False, "statusCode": exc.status_code,
-                   "statusMessage": f"error in sequential upload {exc.detail}"}
+            ret = {
+                "success": False,
+                "statusCode": exc.status_code,
+                "statusMessage": f"error in sequential upload {exc.detail}",
+            }
             raise HTTPException(status_code=exc.status_code, detail=exc.detail)
         except Exception as exc:
             if os.path.exists(tempPath):
                 os.unlink(tempPath)
             if resumable:
                 self.clearSession(key, logKey)
-            ret = {"success": False, "statusCode": 400, "statusMessage": f"error in sequential upload {str(exc)}"}
-            raise HTTPException(status_code=400, detail=f"error in sequential upload {str(exc)}")
+            ret = {
+                "success": False,
+                "statusCode": 400,
+                "statusMessage": f"error in sequential upload {str(exc)}",
+            }
+            raise HTTPException(
+                status_code=400, detail=f"error in sequential upload {str(exc)}"
+            )
         finally:
             chunk.close()
         return ret
 
-    def getTempFilePath(self, uploadId, dirPath):
-        return os.path.join(dirPath, "._" + uploadId)
+    def getNewUploadId(self):
+        return uuid.uuid4().hex
 
     # file path functions
 
-    async def findVersion(self,
-                          repositoryType: str = "archive",
-                          depId: str = None,
-                          contentType: str = "model",
-                          milestone: str = None,
-                          partNumber: int = 1,
-                          contentFormat: str = "pdbx",
-                          version: str = "next"
-                          ):
-        primaryKey = self.getPrimaryLogKey(
-            repositoryType=repositoryType,
-            depId=depId,
-            contentType=contentType,
-            milestone=milestone,
-            partNumber=partNumber,
-            contentFormat=contentFormat,
-            version=version
-        )
-        versions = primaryKey.split(".")
-        version = versions[-1]
-        version = version.replace("V", "")
-        return version
-
-    def getPrimaryLogKey(self,
-                         repositoryType: str = "archive",
-                         depId: str = None,
-                         contentType: str = "model",
-                         milestone: str = None,
-                         partNumber: int = 1,
-                         contentFormat: str = "pdbx",
-                         version: str = "next"
-                         ):
+    def getTempFilePath(self, uploadId, dirPath):
+        return os.path.join(dirPath, "._" + uploadId)
+
+    def getPrimaryLogKey(
+        self,
+        repositoryType: str = "archive",
+        depId: str = None,
+        contentType: str = "model",
+        milestone: str = None,
+        partNumber: int = 1,
+        contentFormat: str = "pdbx",
+        version: str = "next",
+    ):
         filename = self.__pathU.getVersionedPath(
             repositoryType=repositoryType,
             depId=depId,
             contentType=contentType,
             milestone=milestone,
             partNumber=partNumber,
             contentFormat=contentFormat,
-            version=version
+            version=version,
         )
         if not filename:
             return None
         filename = os.path.basename(filename)
         filename = repositoryType + "_" + filename
         return filename
 
@@ -274,62 +359,73 @@
         filename = os.path.basename(versionedPath)
         filename = repositoryType + "_" + filename
         return filename
 
     # database functions
 
     # find upload id using file parameters
-    async def getResumedUpload(self,
-                               repositoryType: str = "archive",
-                               depId: str = None,
-                               contentType: str = "model",
-                               milestone: str = None,
-                               partNumber: int = 1,
-                               contentFormat: str = "pdbx",
-                               version: str = "next",
-                               hashDigest: str = None
-                               ):
+    async def getResumedUpload(
+        self,
+        repositoryType: str = "archive",
+        depId: str = None,
+        contentType: str = "model",
+        milestone: str = None,
+        partNumber: int = 1,
+        contentFormat: str = "pdbx",
+        version: str = "next",
+        # hashDigest: str = None,
+    ):
         filename = self.getPrimaryLogKey(
             repositoryType=repositoryType,
             depId=depId,
             contentType=contentType,
             milestone=milestone,
             partNumber=partNumber,
             contentFormat=contentFormat,
-            version=version
+            version=version,
         )
         uploadId = self.__kV.getLog(filename)
         if not uploadId:
+            # not a resumed upload
             return None
         # remove expired entries
         timestamp = int(self.__kV.getSession(uploadId, "timestamp"))
         now = datetime.datetime.timestamp(datetime.datetime.now(datetime.timezone.utc))
         duration = now - timestamp
         max_duration = self.__cP.get("KV_MAX_SECONDS")
         if duration > max_duration:
-            await self.removeExpiredEntry(uploadId=uploadId, fileName=filename, depId=depId, repositoryType=repositoryType)
+            await self.removeExpiredEntry(
+                uploadId=uploadId,
+                fileName=filename,
+                depId=depId,
+                repositoryType=repositoryType,
+            )
             return None
+
         # test if user resumes with same file as previously
-        if hashDigest is not None:
-            hashvar = self.__kV.getSession(uploadId, "hashDigest")
-            if hashvar != hashDigest:
-                await self.removeExpiredEntry(uploadId=uploadId, fileName=filename, depId=depId, repositoryType=repositoryType)
-                return None
-        else:
-            logging.warning("error - no hash")
-        return uploadId  # returns uploadId or None
+        # if hashDigest is not None:
+        #     hashvar = self.__kV.getSession(uploadId, "hashDigest")
+        #     if hashvar != hashDigest:
+        #         await self.removeExpiredEntry(uploadId=uploadId, fileName=filename, depId=depId, repositoryType=repositoryType)
+        #         return None
+        # else:
+        #     logging.warning("error - no hash")
+
+        # returns uploadId or None
+        return uploadId
 
     # remove an entry from session table and log table, remove corresponding hidden files
     # does not check expiration
-    async def removeExpiredEntry(self,
-                                 uploadId: str = None,
-                                 fileName: str = None,
-                                 depId: str = None,
-                                 repositoryType: str = None
-                                 ):
+    async def removeExpiredEntry(
+        self,
+        uploadId: str = None,
+        fileName: str = None,
+        depId: str = None,
+        repositoryType: str = None,
+    ):
         # remove expired entry and temp files
         self.__kV.clearSessionKey(uploadId)
         # still must remove log table entry (key = file parameters)
         if self.__cP.get("KV_MODE") == "sqlite":
             self.__kV.clearLogVal(uploadId)
         elif self.__cP.get("KV_MODE") == "redis":
             self.__kV.clearLog(fileName)
@@ -369,115 +465,7 @@
             return False
         return response
 
     # clear entire database
     async def clearKv(self):
         self.__kV.clearTable(self.__kV.sessionTable)
         self.__kV.clearTable(self.__kV.logTable)
-
-    # duplicates of upload request functions
-    async def getUploadParameters(
-        self,
-        repositoryType: str,
-        depId: str,
-        contentType: str,
-        milestone: str,
-        partNumber: int,
-        contentFormat: str,
-        version: str,
-        hashDigest: str,
-        allowOverwrite: bool,
-        resumable: bool,
-    ):
-        chunkIndex, uploadId = await self.getUploadStatus(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version, hashDigest, resumable)
-        filePath = await self.getSaveFilePath(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version, allowOverwrite)
-        if not filePath:
-            raise HTTPException(status_code=400, detail="Error - could not make file path from parameters")
-        return filePath, chunkIndex, uploadId
-
-    # return kv entry from file parameters, if have resumed upload, or None if don't
-    # if have resumed upload, kv response has chunk count
-    async def getUploadStatus(
-        self,
-        repositoryType: str,
-        depId: str,
-        contentType: str,
-        milestone: str,
-        partNumber: int,
-        contentFormat: str,
-        version: str,
-        hashDigest: str,
-        resumable: bool,
-    ):
-        if version is None or not re.match(r"\d+", version):
-            version = await self.findVersion(
-                repositoryType=repositoryType,
-                depId=depId,
-                contentType=contentType,
-                milestone=milestone,
-                partNumber=partNumber,
-                contentFormat=contentFormat,
-                version=version
-            )
-        uploadCount = 0
-        uploadId = None
-        if resumable:
-            uploadId = await self.getResumedUpload(
-                repositoryType=repositoryType,
-                depId=depId,
-                contentType=contentType,
-                milestone=milestone,
-                partNumber=partNumber,
-                contentFormat=contentFormat,
-                version=version,
-                hashDigest=hashDigest
-            )
-        if uploadId:
-            status = await self.getSession(uploadId)
-            if status:
-                status = str(status)
-                status = status.replace("'", '"')
-                status = json.loads(status)
-                uploadCount = status["uploadCount"]
-        else:
-            uploadId = self.getNewUploadId()
-        return uploadCount, uploadId
-
-    async def getSaveFilePath(
-        self,
-        repositoryType: str,
-        depId: str,
-        contentType: str,
-        milestone: str,
-        partNumber: int,
-        contentFormat: str,
-        version: str,
-        allowOverwrite: bool,
-    ):
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
-        pathU = PathUtils(cP)
-        if not pathU.checkContentTypeFormat(contentType, contentFormat):
-            logging.warning("Bad content type and/or format - upload rejected")
-            return None
-        outPath = None
-        outPath = pathU.getVersionedPath(
-            repositoryType=repositoryType,
-            depId=depId,
-            contentType=contentType,
-            milestone=milestone,
-            partNumber=partNumber,
-            contentFormat=contentFormat,
-            version=version
-        )
-        if not outPath:
-            logging.warning("Bad content type metadata - cannot build a valid path")
-            return None
-        if os.path.exists(outPath) and not allowOverwrite:
-            logging.warning("Encountered existing file - overwrite prohibited")
-            return None
-        dirPath, _ = os.path.split(outPath)
-        os.makedirs(dirPath, mode=0o777, exist_ok=True)
-        return outPath
-
-    def getNewUploadId(self):
-        return uuid.uuid4().hex
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/JWTAuthBearer.py` & `rcsb.app.file-0.25/rcsb/app/file/JWTAuthBearer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 ##
 # File: JWTAuthBearer.py
 # Date: 23-Aug-2021
 #
 ##
 import logging
-import os
 
 from fastapi import HTTPException
 from fastapi import Request
 from fastapi.security import HTTPAuthorizationCredentials
 from fastapi.security import HTTPBearer
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
 from rcsb.app.file.JWTAuthToken import JWTAuthToken
 
 logger = logging.getLogger(__name__)
 
 
 class JWTAuthBearer(HTTPBearer):
     def __init__(self, auto_error: bool = True):
         super(JWTAuthBearer, self).__init__(auto_error=auto_error)
-        self.__au = JWTAuthToken(os.environ["CONFIG_FILE"])
+        self.__au = JWTAuthToken()
 
     async def __call__(self, request: Request):
         credentials: HTTPAuthorizationCredentials = await super(JWTAuthBearer, self).__call__(request)
         if credentials:
             if not credentials.scheme == "Bearer":
                 raise HTTPException(status_code=403, detail="Missing Bearer details")
             if not self.validateToken(credentials.credentials):
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/JWTAuthToken.py` & `rcsb.app.file-0.25/rcsb/app/file/JWTAuthToken.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 from rcsb.app.file.ConfigProvider import ConfigProvider
 
 logger = logging.getLogger(__name__)
 
 
 class JWTAuthToken:
-    def __init__(self, configFilePath: str):
-        cP = ConfigProvider(configFilePath)
+    def __init__(self):
+        cP = ConfigProvider()
         self.__jwtSecret = cP.get("JWT_SECRET")
         self.__jwtAlgorithm = cP.get("JWT_ALGORITHM")
         self.__jwtSubject = cP.get("JWT_SUBJECT")
         self.__jwtDuration = cP.get("JWT_DURATION")
         #
 
     def decodeToken(self, token: str) -> dict:
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/KvConnection.py` & `rcsb.app.file-0.25/rcsb/app/file/KvConnection.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/rcsb/app/file/KvRedis.py` & `rcsb.app.file-0.25/rcsb/app/file/KvRedis.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/rcsb/app/file/KvSqlite.py` & `rcsb.app.file-0.25/rcsb/app/file/KvSqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from fastapi.exceptions import HTTPException
 
 
 class KvSqlite:
     def __init__(self, cP: typing.Type[ConfigProvider]):
         self.kV = None
         self.__cP = cP
-        # fix mount point
         self.filePath = self.__cP.get("KV_FILE_PATH")
         self.sessionTable = self.__cP.get("KV_SESSION_TABLE_NAME")
         self.logTable = self.__cP.get("KV_LOG_TABLE_NAME")
         # create database if not exists
         # create table if not exists
         try:
             self.kV = KvConnection(self.filePath, self.sessionTable, self.logTable)
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/LogFilterUtils.py` & `rcsb.app.file-0.25/rcsb/app/file/LogFilterUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/rcsb/app/file/PathUtils.py` & `rcsb.app.file-0.25/rcsb/app/file/PathUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/rcsb/app/file/downloadRequest.py` & `rcsb.app.file-0.25/rcsb/app/file/downloadRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import os
 import typing
 from enum import Enum
 from fastapi import APIRouter
 from fastapi import HTTPException
 from fastapi import Query
 from fastapi.responses import FileResponse, Response
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.PathUtils import PathUtils
 from rcsb.utils.io.CryptUtils import CryptUtils
 from rcsb.utils.io.FileUtil import FileUtil
 
 logger = logging.getLogger(__name__)
 
@@ -44,16 +43,15 @@
     partNumber: int = Query(1, title="Content part", description="Content part", example="1,2,3"),
     contentFormat: str = Query(None, title="Content format", description="Content format", example="pdb, pdbx, mtz, pdf"),
     version: str = Query("1", title="Version string", description="Version number or description", example="1,2,3, latest, previous"),
     hashType: HashType = Query(None, title="Hash type", description="Hash type", example="SHA256"),
     chunkSize: typing.Optional[int] = None,
     chunkIndex: typing.Optional[int] = None
 ):
-    configFilePath = os.environ.get("CONFIG_FILE")
-    cP = ConfigProvider(configFilePath)
+    cP = ConfigProvider()
     pathU = PathUtils(cP)
     filePath = fileName = mimeType = hashDigest = None
     tD = {}
     try:
         filePath = pathU.getVersionedPath(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version)
         if not filePath:
             raise HTTPException(status_code=404, detail="Bad or incomplete path metadata")
@@ -88,14 +86,13 @@
         return Response(content=data, media_type="application/octet-stream")
     else:
         return FileResponse(path=filePath, media_type=mimeType, filename=os.path.basename(filePath), headers=tD)
 
 
 @router.get("/downloadSize")
 async def downloadSize(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version):
-    configFilePath = os.environ.get("CONFIG_FILE")
-    cP = ConfigProvider(configFilePath)
+    cP = ConfigProvider()
     pathU = PathUtils(cP)
     filePath = pathU.getVersionedPath(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version)
     if not filePath or not os.path.exists(filePath):
         raise HTTPException(status_code=404, detail="error - file path does not exist}")
     return os.path.getsize(filePath)
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/main.py` & `rcsb.app.file-0.25/rcsb/app/file/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "john.westbrook@rcsb.org"
 __license__ = "Apache 2.0"
 
 import logging
-import os
 from fastapi import FastAPI
 from starlette.middleware.cors import CORSMiddleware
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
-
 
 from . import ConfigProvider
 from . import LogFilterUtils
 from . import downloadRequest  # This triggers JWTAuthBearer
 from . import serverStatus
 from . import uploadRequest
 from . import pathRequest
@@ -51,18 +48,16 @@
 )
 
 
 @app.on_event("startup")
 async def startupEvent():
     # Note that this will run every time a test is performed via, "with TestClient(app) as...",
     # but in production will only run once at startup
-    configFilePath = os.environ.get("CONFIG_FILE")
     logger.debug("Startup - running application startup placeholder method")
-    logger.debug("Using configFilePath %r", configFilePath)
-    cp = ConfigProvider.ConfigProvider(configFilePath)
+    cp = ConfigProvider.ConfigProvider()
     _ = cp.getConfig()
 
 
 @app.on_event("shutdown")
 def shutdownEvent():
     logger.debug("Shutdown - running application shutdown placeholder method")
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/pathRequest.py` & `rcsb.app.file-0.25/rcsb/app/file/pathRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,24 +20,23 @@
 
 from fastapi import APIRouter, Form
 from fastapi import Depends
 from fastapi import Query
 from fastapi import HTTPException
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
 from pydantic import Field
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.app.file.JWTAuthBearer import JWTAuthBearer
 from rcsb.app.file.PathUtils import PathUtils
 from rcsb.utils.io.FileUtil import FileUtil
 
 logger = logging.getLogger(__name__)
 
 
-provider = ConfigProvider(os.environ.get("CONFIG_FILE"))
+provider = ConfigProvider()
 jwtDisable = bool(provider.get('JWT_DISABLE'))
 if not jwtDisable:
     router = APIRouter(dependencies=[Depends(JWTAuthBearer())], tags=["status"])
 else:
     router = APIRouter(tags=["status"])
 
 
@@ -97,16 +96,15 @@
     milestone: str = Query("", title="milestone", description="milestone", example="release"),
 ):
     """Check if a file exists provided standard file parameters.
     """
     success = False
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         logger.info("Checking repositoryType %r depId %r contentType %r milestone %r format %r version %r", repositoryType, depId, contentType, milestone, contentFormat, version)
         filePath = pathU.getVersionedPath(repositoryType, depId, contentType, milestone, partNumber, contentFormat, version)
         logger.info("Checking filePath %r", filePath)
         fileName = fU.getFileName(filePath)
         success = fU.exists(filePath)
@@ -133,16 +131,15 @@
     repositoryType: str = Query(title="Repository Type", description="OneDep repository type", example="onedep-archive, onedep-deposit"),
 ):
     """Check if a file exists provided standard directory parameters.
     """
     success = False
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         logger.info("Checking repositoryType %r depId %r", repositoryType, depId)
         dirPath = pathU.getDirPath(repositoryType, depId)
         #
         success = fU.exists(dirPath)
         logger.info("success %r dirPath %r", success, dirPath)
@@ -203,16 +200,15 @@
     success = False
     fileName = None
     filePath = None
     version = "latest"
     fileVersion = None
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         logger.info(
             "Getting latest file version for repositoryType %r depId %r contentType %r milestone %r partNumber %r format %r",
             repositoryType,
             depId,
             contentType,
@@ -262,16 +258,15 @@
     milestone: str = Query("", title="milestone", description="milestone", example="release"),
 ):
     """Copy a file given standard input paramaters for both the source and destination of the file.
     """
     success = False
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         logger.info(
             "Copying repositoryType %r depId %r contentType %r milestone %r format %r version %r",
             repositoryTypeSource, depIdSource, contentTypeSource, milestone, contentFormatSource, versionSource
         )
         filePathSource = pathU.getVersionedPath(repositoryTypeSource, depIdSource, contentTypeSource, milestone, partNumberSource, contentFormatSource, versionSource)
@@ -352,16 +347,15 @@
     milestoneTarget: str = Form("", title="milestone", description="milestone", example="release"),
 ):
     """Move a file given standard input paramaters for both the source and destination of the file.
     """
     success = False
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         logger.info(
             "Moving repositoryType %r depId %r contentType %r milestone %r format %r version %r",
             repositoryTypeSource, depIdSource, contentTypeSource, milestoneSource, contentFormatSource, versionSource
         )
         filePathSource = pathU.getVersionedPath(repositoryTypeSource, depIdSource, contentTypeSource, milestoneSource, partNumberSource, contentFormatSource, versionSource)
@@ -437,16 +431,15 @@
     """List files in directory of requested depId and repositoryType (using standard input paramaters).
     """
     success = False
     dirList = []
     dirExistsCheck = None
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         # List directory of requested repositoryType and depId
         dirPath = pathU.getDirPath(repositoryType, depId)
         logger.info("Listing dirPath %r for repositoryType %r depId %r", dirPath, repositoryType, depId)
         dirExistsCheck = fU.exists(dirPath)
         if dirExistsCheck:
@@ -512,16 +505,15 @@
     """
     success = False
     compressPath = None
     dirExistsCheck = None
     dirRemovedBool = None
     try:
         fU = FileUtil()
-        configFilePath = os.environ.get("CONFIG_FILE")
-        cP = ConfigProvider(configFilePath)
+        cP = ConfigProvider()
         pathU = PathUtils(cP)
         #
         # Compress directory of requested repositoryType and depId
         dirPath = pathU.getDirPath(repositoryType, depId)
         logger.info("Compressing dirPath %r for repositoryType %r depId %r", dirPath, repositoryType, depId)
         dirExistsCheck = fU.exists(dirPath)
         if dirExistsCheck:
```

### Comparing `rcsb.app.file-0.24/rcsb/app/file/serverStatus.py` & `rcsb.app.file-0.25/rcsb/app/file/serverStatus.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import logging
 import os
 import time
 import redis
 import psutil
 import shutil
 from fastapi import APIRouter
-import rcsb.app.config.setConfig  # noqa: F401 pylint: disable=W0611
 from rcsb.app.file.ConfigProvider import ConfigProvider
 from rcsb.utils.io.ProcessStatusUtil import ProcessStatusUtil
 
 
 logger = logging.getLogger(__name__)
 
 router = APIRouter()
@@ -34,23 +33,23 @@
     with open(uptime_file, "r") as read:
         uptime_start = float(read.read())
     uptime_stop = time.time()
     seconds = uptime_stop - uptime_start
     minutes = seconds / 60
     hours = minutes / 60
     days = minutes / 24
-    # report total up time in either hours, minutes, or seconds (i.e. total hours, or total minutes, or total seconds)
+    # report total uptime in either hours, minutes, or seconds (i.e. total hours, or total minutes, or total seconds)
     return {"days_total": int(days), "hours_total": int(hours), "minutes_total": int(minutes), "seconds_total": int(seconds), "start": int(uptime_start), "stop": int(uptime_stop)}
 
 
 @router.get("/redis-status", tags=["status"])
 def getRedisStatus():
     # create database if not exists
     # create table if not exists
-    cP = ConfigProvider(os.environ.get("CONFIG_FILE"))
+    cP = ConfigProvider()
     redis_host = cP.get("REDIS_HOST")
     try:
         r = redis.Redis(host=redis_host, decode_responses=True)
     except Exception as exc:
         # already exists
         logging.warning("exception in redis status: %s %s", type(exc), exc)
     try:
@@ -59,15 +58,15 @@
         result = False
     return {"running": result}
 
 
 @router.get("/storage", tags=["status"])
 def getServerStorage():
     percent_ram_used = psutil.virtual_memory()[2]
-    cP = ConfigProvider(os.environ.get("CONFIG_FILE"))
+    cP = ConfigProvider()
     repository_dir_path = cP.get("REPOSITORY_DIR_PATH")
     disk_usage = shutil.disk_usage(repository_dir_path)
     disk_total = disk_usage[0]
     disk_used = disk_usage[1]
     disk_free = disk_usage[2]
     percent_disk_used = (disk_used / disk_total) * 100
     return {"percent_ram_used": percent_ram_used, "percent_disk_used": percent_disk_used, "total": disk_total, "used": disk_used, "free": disk_free}
```

### Comparing `rcsb.app.file-0.24/rcsb.app.file.egg-info/PKG-INFO` & `rcsb.app.file-0.25/rcsb.app.file.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.app.file
-Version: 0.24
+Version: 0.25
 Summary: RCSB File Access Service Application
 Home-page: https://github.com/rcsb/py-rcsb_app_file
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -78,22 +78,20 @@
 
 To upload the entire file in one request, configure the parameters to treat the file as one chunk.
 
 Upload requires some setup by invoking the 'file-v2/getUploadParameters' endpoint first, then passing the results as parameters.
 
 To maintain sequential order, the client must wait for each response before sending the next chunk.
 
-The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in both uploadRequest and IoUtils.
+The repository saves chunks to a temporary file that is named after the upload id and begins with "._" which is configurable from the getTempFilePath function in IoUtils.
 
 The download endpoint is found at 'file-v1/download'.
 
 The list directory endpoint is found at 'file-v1/list-dir'.
 
-For streamlining, the upload function has been partly duplicated in uploadRequest and IoUtils, so changes to one should be performed in the other.
-
 To skip endpoints and forward a server-side chunk or file from Python, use functions by the same names in IoUtils.py.
 
 # Uploads and downloads
 
 ### HTML examples
 
 The example-upload.html, example-download.html, and example-list.html files demonstrate requests to the endpoints from HTML.
@@ -106,17 +104,16 @@
 
 Client.py usage
 ```
 
 python3 client.py
 [-h (help)]
 [--upload source_file repo_type id content_type milestone part format version]
-[--download target_file repo_type id content_type milestone part format version]
+[--download target_folder repo_type id content_type milestone part format version]
 [--list repo_type dep_id (list directory)]
-[-s (chunk file sequentially)]
 [-r (chunk file resumably)]
 [-o (overwrite files with same name)]
 [-z (zip files prior to upload)]
 [-x (expand files after upload)]
 
 ```
 
@@ -126,14 +123,22 @@
 
 # Testing and deployment
 
 Testing is easiest without Docker and using a Sqlite database.
 
 For production, use a Docker container with a Redis database.
 
+Redis with Docker requires Redis in a Docker container.
+
+Production with multiple servers will require all servers to coordinate through a single remote Redis server.
+
+Since one server could host Redis while others don't, the docker instances could be run differently, or the config files set differently, on each server.
+
+Also, multiple servers must connect to a single file system for deposition.
+
 # Deployment on local server without docker
 
 For launching without docker, edit url in deploy/LAUNCH_GUNICORN.sh
 
 From base repository directory (in `py-rcsb_app_file/`), start app with:
 ```bash
 
@@ -236,15 +241,16 @@
 
 ### Connecting to Redis remotely
 
 If Redis runs on a different machine than the files API, then the host must be set to a url
 
 Change Redis host to '#:#:#:#' and port 6379 in rcsb/app/config/config.yml.
 
-For example
+KvRedis.py should resemble
+
 ```
 
 self.kV = redis.Redis(host='1.2.3.4', port=6379, decode_responses=True)
 
 ```
 
 Remote Redis requires changing the config file settings on the machine with Redis
@@ -272,23 +278,27 @@
 ```
 docker run --name redis-container -d redis
 or (if connecting remotely to Redis container on different server)
 docker run --name redis-container -p 6379:6379 -d redis
 ```
 
 If the Redis container runs on the same machine as the files API, change Redis host to 'redis' in rcsb/app/config/config.yml.
+
+KvRedis.py should resemble
+
 ```
 
-self.kV = redis.Redis(host='redis', decode_responses=True)
+self.kV = redis.Redis(host='redis', port=6379, decode_responses=True)
 
 ```
 
 Or, if connecting remotely to Redis container on different server, change Redis host to '#:#:#:#' and port 6379 in rcsb/app/config/config.yml.
 
-For example
+KvRedis.py should resemble
+
 ```
 
 self.kV = redis.Redis(host='1.2.3.4', port=6379, decode_responses=True)
 
 ```
 
 To view Redis variables
@@ -350,16 +360,14 @@
 
 `-p` allows user to choose a port, 8000:8000 is used in this case, as the port 8000 is exposed in the current dockerfile
 
 `--link` connects to a Redis container if the container is running on the same machine as the files API 
 
 # Error handling
 
-Errors related to 'shared locks' are generally fixed by deleting the 'shared-locks' directory and, if necessary, restarting.
-
 For production, Redis variables are set to expire periodically. However, hidden files are not, so a cron job should be run periodically to remove lingering hidden files from the deposit or archive directories.
 
 After development testing with a Sqlite database, open the kv.sqlite file and delete the tables, and delete hidden files from the deposit or archives directories.
 
 After development testing with Redis, open the redis-cli and delete the variables, and delete hidden files from the deposit or archives directories.
 
 The hidden files to be deleted are those that start with the value configured in getTempFilePath, referred to above, after checking that the file modification time is beyond a specified threshold.
```

### Comparing `rcsb.app.file-0.24/rcsb.app.file.egg-info/SOURCES.txt` & `rcsb.app.file-0.25/rcsb.app.file.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-0.24/setup.py` & `rcsb.app.file-0.25/setup.py`

 * *Files identical despite different names*

