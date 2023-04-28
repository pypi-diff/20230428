# Comparing `tmp/together_worker-0.1.3.tar.gz` & `tmp/together_worker-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together_worker-0.1.3.tar", max compression
+gzip compressed data, was "together_worker-0.1.9.tar", max compression
```

## Comparing `together_worker-0.1.3.tar` & `together_worker-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       18 2022-12-06 06:01:52.899836 together_worker-0.1.3/README.md
--rw-r--r--   0        0        0     2960 2022-12-06 06:01:52.899836 together_worker-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    13237 2022-12-06 06:01:52.899836 together_worker-0.1.3/together_worker/fast_inference.py
--rw-r--r--   0        0        0      397 2022-12-06 06:01:52.899836 together_worker-0.1.3/together_worker/profiler/client.py
--rw-r--r--   0        0        0     1234 2022-12-06 06:01:52.899836 together_worker-0.1.3/together_worker/profiler/daemon.py
--rw-r--r--   0        0        0      403 2022-12-06 06:01:52.903836 together_worker-0.1.3/together_worker/profiler/gpu_profiler.py
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 together_worker-0.1.3/setup.py
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 together_worker-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-03-17 03:39:43.972720 together_worker-0.1.9/README.md
+-rw-r--r--   0        0        0     2932 2023-03-17 03:39:43.972720 together_worker-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    14253 2023-03-17 03:39:43.972720 together_worker-0.1.9/together_worker/fast_inference.py
+-rw-r--r--   0        0        0      397 2023-03-17 03:39:43.976720 together_worker-0.1.9/together_worker/profiler/client.py
+-rw-r--r--   0        0        0     1234 2023-03-17 03:39:43.976720 together_worker-0.1.9/together_worker/profiler/daemon.py
+-rw-r--r--   0        0        0      403 2023-03-17 03:39:43.976720 together_worker-0.1.9/together_worker/profiler/gpu_profiler.py
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 together_worker-0.1.9/PKG-INFO
```

### Comparing `together_worker-0.1.3/pyproject.toml` & `together_worker-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "together_worker"
-version = "0.1.3"
+version = "0.1.9"
 description = ""
 authors = ["together <together@together.xyz>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/together-computer/together_worker"
 homepage = "https://github.com/together-computer/together_worker"
 keywords = [
@@ -20,15 +20,14 @@
     "GPT-2"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2,<3.11"
 dacite = "^1.6.0"
 together-web3 = "^0.1.0"
-influxdb-client = "^1.34.0"
 pynvml = "^11.4.1"
 netifaces = "^0.11.0"
 aiohttp = "^3.8.3"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
 darglint = "^1.8.1"
```

### Comparing `together_worker-0.1.3/together_worker/fast_inference.py` & `together_worker-0.1.9/together_worker/fast_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import asdict
 from enum import Enum
 
 import netifaces
 from aiohttp import web
 from dacite import from_dict
+from pynvml import (
+    nvmlDeviceGetCount,
+    nvmlDeviceGetHandleByIndex,
+    nvmlDeviceGetMemoryInfo,
+    nvmlDeviceGetName,
+    nvmlInit,
+)
 from together_web3.computer import (
     Instance,
     MatchEvent,
     RequestTypeLanguageModelInference,
     RequestTypeShutdown,
     ResourceTypeInstance,
     Result,
@@ -71,27 +78,37 @@
                 args[key] = coordinator_args[key]
             return args
         except Exception as e:
             logger.exception(f'get_worker_configuration_from_coordinator failed: {e}')
 
 
 def get_coordinator_join_request(args):
+    gpu_num = nvmlDeviceGetCount()
+    # assume: on a single node, all gpus are of the same type
+    if gpu_num > 0:
+        handle = nvmlDeviceGetHandleByIndex(0)
+        gpu_type = nvmlDeviceGetName(handle)
+        mem_info = nvmlDeviceGetMemoryInfo(handle)
+        gpu_mem = mem_info.total
+    else:
+        gpu_type = ""
+        gpu_mem = 0
     join = Join(
         group_name=args.get("group_name", "group1"),
         worker_name=args.get("worker_name", "worker1"),
         host_name=platform.node(),
         host_ip=get_host_ip(),
         interface_ip=get_non_loopback_ipv4_addresses(),
         instance=Instance(
             arch=platform.machine(),
             os=platform.system(),
             cpu_num=multiprocessing.cpu_count(),
-            gpu_num=args.get("gpu_num", 0),
-            gpu_type=args.get("gpu_type", ""),
-            gpu_memory=args.get("gpu_mem", 0),
+            gpu_num=args.get("gpu_num", gpu_mem),
+            gpu_type=args.get("gpu_type", gpu_type),
+            gpu_memory=args.get("gpu_mem", gpu_mem),
             resource_type=ResourceTypeInstance,
             tags={}),
         config={
             "model": args.get("model_name")
         },
     )
     return join
@@ -126,14 +143,20 @@
         self.shutdown = True
 
     def worker(self):
         pass
 
     def __init__(self, model_name: str, args: Dict[str, Any] = {}):
         args['model_name'] = model_name
+        self.nvidia_enabled = False
+        try:
+            nvmlInit()
+            self.nvidia_enabled = True
+        except Exception as e:
+            logger.info(f"nvidia-smi not available: {e}")
         self.service_domain = args.get("service_domain", ServiceDomain.together)
         self.coordinator_join_request = get_coordinator_join_request(args)
         self.coordinator: TogetherWeb3 = args.get(
             "coordinator") if self.service_domain == ServiceDomain.together else None
         self.http_host = args.get("http_host", "localhost")
         self.http_port = args.get("http_port",
                                   5001) if self.service_domain == ServiceDomain.http else 0
@@ -240,22 +263,26 @@
         match_event = match_event if isinstance(match_event, list) else [match_event]
         raw_event = raw_event if isinstance(raw_event, list) else [raw_event]
         logger.info(f"together_request {raw_event}")
         self.match_event = match_event
         self.request_json = [event["match"]["service_bid"]["job"] for event in raw_event]
         if self.request_json[0].get("request_type") == RequestTypeShutdown:
             self.dispatch_shutdown()
-        response_json = await self.loop.run_in_executor(self.executor, self.dispatch_request, self.request_json, match_event)
-        response_json = response_json if isinstance(response_json, list) else [response_json]
+        try:
+            response_json = await self.loop.run_in_executor(self.executor, self.dispatch_request, self.request_json, match_event)
+            response_json = response_json if isinstance(
+                response_json, list) else [response_json]
+        except Exception as e:
+            response_json = {"error": str(e), "failed": True}
         self.request_json = []
         self.match_event = []
         self.served += 1
         await asyncio.gather(*[self.send_result_back(match_event[i], response_json[i]) for i in range(len(response_json))])
 
-    async def send_result_back(self, match_event: MatchEvent, result_data: Dict[str, Any], partial: bool = False) -> None:
+    async def send_result_back(self, match_event: MatchEvent, result_data: Dict[str, Any], partial: bool = False, reentered: bool = False) -> None:
         try:
             # logger.info(f"send_result_back {result_data}")
             result = {
                 "ask_address": match_event.match.ask_address,
                 "bid_address": match_event.match.bid_address,
                 "ask_offer_id": match_event.match.ask_offer_id,
                 "bid_offer_id": match_event.match.bid_offer_id,
@@ -269,16 +296,19 @@
                     data_class=Result,
                     data=result,
                 ),
                 signature=None,
             ))
         except Exception as e:
             logger.error(f"send_result_back error: {e}")
+            if not partial and not reentered:
+                await self.send_result_back(match_event, {"error": str(e), "failed": True}, False, True)
 
     # Primary token streaming implementation using call_soon_threadsafe().
+
     def stream_tokens(self, token: List[int],
                       match_event: Optional[List[MatchEvent]] = None) -> None:
         self.loop.call_soon_threadsafe(
             self._dispatch_stream_tokens,
             self.served,
             token,
             match_event if match_event else self.match_event)
```

### Comparing `together_worker-0.1.3/together_worker/profiler/daemon.py` & `together_worker-0.1.9/together_worker/profiler/daemon.py`

 * *Files identical despite different names*

### Comparing `together_worker-0.1.3/PKG-INFO` & `together_worker-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: together-worker
-Version: 0.1.3
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/together-computer/together_worker
 License: MIT
 Keywords: NLP,vision,speech,deep,learning,transformer,pytorch,tensorflow,BERT,GPT-2
 Author: together
 Author-email: together@together.xyz
 Requires-Python: >=3.7.2,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
-Requires-Dist: influxdb-client (>=1.34.0,<2.0.0)
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: pynvml (>=11.4.1,<12.0.0)
 Requires-Dist: together-web3 (>=0.1.0,<0.2.0)
 Project-URL: Repository, https://github.com/together-computer/together_worker
 Description-Content-Type: text/markdown
 
 # together_worker
```

