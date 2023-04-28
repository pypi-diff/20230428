# Comparing `tmp/at_fetch-0.1.1.tar.gz` & `tmp/at_fetch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "at_fetch-0.1.1.tar", max compression
+gzip compressed data, was "at_fetch-0.1.2.tar", max compression
```

## Comparing `at_fetch-0.1.1.tar` & `at_fetch-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      684 2023-04-27 16:27:38.947280 at_fetch-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 03:45:51.032926 at_fetch-0.1.1/fetch/__init__.py
--rw-r--r--   0        0        0      367 2023-04-27 13:33:56.779724 at_fetch-0.1.1/fetch/const.py
--rw-r--r--   0        0        0     2634 2023-04-27 16:27:55.063335 at_fetch-0.1.1/fetch/fetch.py
--rw-r--r--   0        0        0      345 2023-04-27 16:32:13.700226 at_fetch-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 at_fetch-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      684 2023-04-27 16:27:38.947280 at_fetch-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 03:45:51.032926 at_fetch-0.1.2/fetch/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-28 04:17:27.298737 at_fetch-0.1.2/fetch/const.py
+-rw-r--r--   0        0        0     2863 2023-04-28 04:16:52.314620 at_fetch-0.1.2/fetch/fetch.py
+-rw-r--r--   0        0        0      363 2023-04-28 04:18:01.090851 at_fetch-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 at_fetch-0.1.2/PKG-INFO
```

### Comparing `at_fetch-0.1.1/README.md` & `at_fetch-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `at_fetch-0.1.1/fetch/fetch.py` & `at_fetch-0.1.2/fetch/fetch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
 import asyncio
 from .const import CHUNK_SIZE, CONCURRENT_LIMIT, INTERVAL
 import httpx
+import pandas as pd
 
 
 class Fetch:
     def __init__(self) -> None:
         self.semaphore = asyncio.Semaphore(CONCURRENT_LIMIT)
 
     async def get(self, url: str, params):
@@ -49,19 +50,25 @@
             raise Exception("start time gt end time")
 
         interval_timestamp = INTERVAL[interval]
         limit = diff // interval_timestamp
         limit_chunks = self.split_large_number(limit, CHUNK_SIZE)
         async_tasks = []
         new_start_time = start_time
-        for chunk in limit_chunks:
-            new_start_time = start_time + chunk * CHUNK_SIZE
+        for i, chunk in enumerate(limit_chunks):
+            new_start_time = start_time + i * CHUNK_SIZE * interval_timestamp
             params = {
                 "symbol": symbol,
                 "interval": interval,
                 "limit": chunk,
                 "start_time": new_start_time,
             }
             task = self.get(url, params)
             async_tasks.append(task)
         res = await asyncio.gather(*async_tasks)
-        return res
+        df = []
+        for item in res:
+            obj = item.json()
+            data = pd.DataFrame(obj["data"])
+            df.append(data)
+        df_res = pd.concat(df)
+        return df_res
```

### Comparing `at_fetch-0.1.1/PKG-INFO` & `at_fetch-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: at-fetch
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: thecatshidog
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## at_fetch
 
 ```
 pip install at_fetch
 poetry add at_fetch
```

