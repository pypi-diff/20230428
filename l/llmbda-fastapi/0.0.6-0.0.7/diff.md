# Comparing `tmp/llmbda_fastapi-0.0.6.tar.gz` & `tmp/llmbda_fastapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmbda_fastapi-0.0.6.tar", last modified: Fri Apr 28 00:43:15 2023, max compression
+gzip compressed data, was "llmbda_fastapi-0.0.7.tar", last modified: Fri Apr 28 01:23:00 2023, max compression
```

## Comparing `llmbda_fastapi-0.0.6.tar` & `llmbda_fastapi-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.709080 llmbda_fastapi-0.0.6/
--rw-r--r--   0 jackykoh   (501) staff       (20)     2453 2023-04-28 00:43:15.708876 llmbda_fastapi-0.0.6/PKG-INFO
--rw-r--r--   0 jackykoh   (501) staff       (20)     2260 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.6/README.md
-drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.707069 llmbda_fastapi-0.0.6/llmbda_fastapi/
--rw-r--r--   0 jackykoh   (501) staff       (20)      139 2023-04-28 00:42:42.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/__init__.py
--rw-r--r--   0 jackykoh   (501) staff       (20)     3878 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/chains.py
-drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.708669 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/
--rw-r--r--   0 jackykoh   (501) staff       (20)      109 2023-04-28 00:39:06.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/__init__.py
--rw-r--r--   0 jackykoh   (501) staff       (20)     5362 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/input_components.py
--rw-r--r--   0 jackykoh   (501) staff       (20)     1833 2023-04-28 00:43:10.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/upload_file.py
--rw-r--r--   0 jackykoh   (501) staff       (20)     3606 2023-04-27 01:44:36.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/transformations.py
-drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.707838 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/
--rw-r--r--   0 jackykoh   (501) staff       (20)     2453 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 jackykoh   (501) staff       (20)      412 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 jackykoh   (501) staff       (20)        1 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 jackykoh   (501) staff       (20)      337 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/requires.txt
--rw-r--r--   0 jackykoh   (501) staff       (20)       15 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/top_level.txt
--rw-r--r--   0 jackykoh   (501) staff       (20)       38 2023-04-28 00:43:15.709137 llmbda_fastapi-0.0.6/setup.cfg
--rw-r--r--   0 jackykoh   (501) staff       (20)     1025 2023-04-27 01:44:36.000000 llmbda_fastapi-0.0.6/setup.py
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 01:23:00.801132 llmbda_fastapi-0.0.7/
+-rw-r--r--   0 jackykoh   (501) staff       (20)     2453 2023-04-28 01:23:00.800939 llmbda_fastapi-0.0.7/PKG-INFO
+-rw-r--r--   0 jackykoh   (501) staff       (20)     2260 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.7/README.md
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 01:23:00.799258 llmbda_fastapi-0.0.7/llmbda_fastapi/
+-rw-r--r--   0 jackykoh   (501) staff       (20)      139 2023-04-28 01:07:38.000000 llmbda_fastapi-0.0.7/llmbda_fastapi/__init__.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     3878 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.7/llmbda_fastapi/chains.py
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 01:23:00.800730 llmbda_fastapi-0.0.7/llmbda_fastapi/frontend/
+-rw-r--r--   0 jackykoh   (501) staff       (20)      109 2023-04-28 00:39:06.000000 llmbda_fastapi-0.0.7/llmbda_fastapi/frontend/__init__.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     5362 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.7/llmbda_fastapi/frontend/input_components.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     1948 2023-04-28 01:22:56.000000 llmbda_fastapi-0.0.7/llmbda_fastapi/frontend/upload_file.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     3606 2023-04-27 01:44:36.000000 llmbda_fastapi-0.0.7/llmbda_fastapi/transformations.py
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 01:23:00.799975 llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/
+-rw-r--r--   0 jackykoh   (501) staff       (20)     2453 2023-04-28 01:23:00.000000 llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (501) staff       (20)      412 2023-04-28 01:23:00.000000 llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)        1 2023-04-28 01:23:00.000000 llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)      337 2023-04-28 01:23:00.000000 llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)       15 2023-04-28 01:23:00.000000 llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)       38 2023-04-28 01:23:00.801187 llmbda_fastapi-0.0.7/setup.cfg
+-rw-r--r--   0 jackykoh   (501) staff       (20)     1025 2023-04-27 01:44:36.000000 llmbda_fastapi-0.0.7/setup.py
```

### Comparing `llmbda_fastapi-0.0.6/PKG-INFO` & `llmbda_fastapi-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmbda_fastapi
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 
 # Llmbda FastAPI
```

### Comparing `llmbda_fastapi-0.0.6/README.md` & `llmbda_fastapi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.6/llmbda_fastapi/chains.py` & `llmbda_fastapi-0.0.7/llmbda_fastapi/chains.py`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/input_components.py` & `llmbda_fastapi-0.0.7/llmbda_fastapi/frontend/input_components.py`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/upload_file.py` & `llmbda_fastapi-0.0.7/llmbda_fastapi/frontend/upload_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,21 +20,28 @@
     else:
         raise TypeError("'content' needs to be of type str, bytes or io.BytesIO.")
     return content_bytes
 
 
 def _get_file_upload_urls(dataset_id: str, files: List[str]):
     url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
-    return requests.post(
+    response = requests.post(
         url=url + f"/datasets/{dataset_id}/get_file_upload_urls",
         headers={
             "Authorization": RELEVANCE_AUTH_TOKEN,
         },
-        json=dict(files=files),
-    ).json()
+        json={
+            "files" : files
+        },
+    )
+    try:
+        return response.json()
+    except:
+        print(response.text)
+        raise 
 
 def _upload_media(presigned_url: str, media_content: bytes):
     if not isinstance(media_content, bytes):
         raise ValueError(
             f"media needs to be in a bytes format. Currently in {type(media_content)}"
         )
     return requests.put(
```

### Comparing `llmbda_fastapi-0.0.6/llmbda_fastapi/transformations.py` & `llmbda_fastapi-0.0.7/llmbda_fastapi/transformations.py`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/PKG-INFO` & `llmbda_fastapi-0.0.7/llmbda_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmbda-fastapi
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 
 # Llmbda FastAPI
```

### Comparing `llmbda_fastapi-0.0.6/setup.py` & `llmbda_fastapi-0.0.7/setup.py`

 * *Files identical despite different names*

