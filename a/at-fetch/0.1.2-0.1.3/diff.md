# Comparing `tmp/at_fetch-0.1.2.tar.gz` & `tmp/at_fetch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "at_fetch-0.1.2.tar", max compression
+gzip compressed data, was "at_fetch-0.1.3.tar", max compression
```

## Comparing `at_fetch-0.1.2.tar` & `at_fetch-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      684 2023-04-27 16:27:38.947280 at_fetch-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-27 03:45:51.032926 at_fetch-0.1.2/fetch/__init__.py
--rw-r--r--   0        0        0      367 2023-04-28 04:17:27.298737 at_fetch-0.1.2/fetch/const.py
--rw-r--r--   0        0        0     2863 2023-04-28 04:16:52.314620 at_fetch-0.1.2/fetch/fetch.py
--rw-r--r--   0        0        0      363 2023-04-28 04:18:01.090851 at_fetch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 at_fetch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      727 2023-04-28 04:19:15.503100 at_fetch-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 03:45:51.032926 at_fetch-0.1.3/fetch/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-28 04:17:27.298737 at_fetch-0.1.3/fetch/const.py
+-rw-r--r--   0        0        0     2863 2023-04-28 04:16:52.314620 at_fetch-0.1.3/fetch/fetch.py
+-rw-r--r--   0        0        0      363 2023-04-28 04:19:28.911145 at_fetch-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 at_fetch-0.1.3/PKG-INFO
```

### Comparing `at_fetch-0.1.2/README.md` & `at_fetch-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 from fetch.fetch import Fetch
 import asyncio
 import time
 
 
 async def main():
     request = Fetch()
-    start_time = 1502913600
+    start_time = 1533684900
     end_time = 1533687900
     symbol = "btcusdt"
     interval = "1m"
     start = time.time()
     # await asyncio.sleep(1)
     res = await request.get_all_klines_data(
         "http://47.243.179.153:8000/api/kline/spot", symbol, interval, start_time, end_time
     )
     end = time.time()
     exec_time = end - start
-    print("res", len(res))
     print("exec_time", exec_time)
+    # res已经是按照顺序的dataframe数据格式
+    print(res)
 
 
 asyncio.run(main())
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `at_fetch-0.1.2/fetch/fetch.py` & `at_fetch-0.1.3/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `at_fetch-0.1.2/PKG-INFO` & `at_fetch-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: at-fetch
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: thecatshidog
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,25 +35,26 @@
 from fetch.fetch import Fetch
 import asyncio
 import time
 
 
 async def main():
     request = Fetch()
-    start_time = 1502913600
+    start_time = 1533684900
     end_time = 1533687900
     symbol = "btcusdt"
     interval = "1m"
     start = time.time()
     # await asyncio.sleep(1)
     res = await request.get_all_klines_data(
         "http://47.243.179.153:8000/api/kline/spot", symbol, interval, start_time, end_time
     )
     end = time.time()
     exec_time = end - start
-    print("res", len(res))
     print("exec_time", exec_time)
+    # res已经是按照顺序的dataframe数据格式
+    print(res)
 
 
 asyncio.run(main())
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

