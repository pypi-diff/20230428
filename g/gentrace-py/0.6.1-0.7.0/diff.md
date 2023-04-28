# Comparing `tmp/gentrace_py-0.6.1.tar.gz` & `tmp/gentrace_py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.6.1.tar", max compression
+gzip compressed data, was "gentrace_py-0.7.0.tar", max compression
```

## Comparing `gentrace_py-0.6.1.tar` & `gentrace_py-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1058 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      967 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    25160 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6400 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/step_run.py
--rw-r--r--   0        0        0     3706 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-27 20:08:02.147147 gentrace_py-0.6.1/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12262 2023-04-27 20:08:02.151147 gentrace_py-0.6.1/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-27 20:08:02.151147 gentrace_py-0.6.1/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-27 20:08:02.151147 gentrace_py-0.6.1/gentrace/schemas.py
--rw-r--r--   0        0        0     1571 2023-04-27 20:08:02.151147 gentrace_py-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      967 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    26100 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6400 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0     3706 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12262 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/gentrace/schemas.py
+-rw-r--r--   0        0        0     1571 2023-04-28 14:26:32.002023 gentrace_py-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.7.0/PKG-INFO
```

### Comparing `gentrace_py-0.6.1/gentrace/__init__.py` & `gentrace_py-0.7.0/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/api_client.py` & `gentrace_py-0.7.0/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/configuration.py` & `gentrace_py-0.7.0/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/exceptions.py` & `gentrace_py-0.7.0/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/feedback_request.py` & `gentrace_py-0.7.0/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/feedback_request.pyi` & `gentrace_py-0.7.0/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/feedback_response.py` & `gentrace_py-0.7.0/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/feedback_response.pyi` & `gentrace_py-0.7.0/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.7.0/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.7.0/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.7.0/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.7.0/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/models/__init__.py` & `gentrace_py-0.7.0/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.7.0/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.7.0/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/providers/getters.py` & `gentrace_py-0.7.0/gentrace/providers/getters.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/providers/llms/openai.py` & `gentrace_py-0.7.0/gentrace/providers/llms/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import time
 import uuid
 from typing import Dict, Optional
 
 import openai
 import pystache
 
@@ -313,29 +314,48 @@
             stream,
         )
         return completion
 
     return wrapper
 
 
+def create_rendered_chat_messages(messages):
+    new_messages = []
+    for message in messages:
+        new_message = copy.deepcopy(message)
+        if "contentTemplate" in message and "contentInputs" in message:
+            new_message["content"] = pystache.render(
+                message["contentTemplate"], message["contentInputs"]
+            )
+
+        new_message.pop("contentTemplate", None)
+        new_message.pop("contentInputs", None)
+
+        new_messages.append(new_message)
+
+    return new_messages
+
+
 def intercept_chat_completion(original_fn, gentrace_config: Configuration):
     @classmethod
     def wrapper(cls, *args, **kwargs):
         messages = kwargs.get("messages")
         user = kwargs.get("user")
         pipeline_id = kwargs.pop("pipeline_id", None)
         stream = kwargs.get("stream")
 
         model_params = {
             k: v for k, v in kwargs.items() if k not in ["messages", "user"]
         }
 
         if stream:
+            rendered_messages = create_rendered_chat_messages(messages)
+            new_kwargs = dict(kwargs, messages=rendered_messages)
             start_time = time.time()
-            completion = original_fn(**kwargs)
+            completion = original_fn(**new_kwargs)
 
             is_self_contained = not hasattr(cls, "pipeline_run") and pipeline_id
             if is_self_contained:
                 pipeline_run_id = str(uuid.uuid4())
 
             def profiled_completion():
                 modified_response = []
@@ -377,17 +397,20 @@
                     )
 
                     if is_self_contained:
                         pipeline_run.submit()
 
             return profiled_completion()
 
-        start_time = time.time()
-        completion = original_fn(**kwargs)
+        rendered_messages = create_rendered_chat_messages(messages)
+
+        new_kwargs = dict(kwargs, messages=rendered_messages)
 
+        start_time = time.time()
+        completion = original_fn(**new_kwargs)
         end_time = time.time()
 
         elapsed_time = int((end_time - start_time) * 1000)
 
         pipeline_run = cls.pipeline_run if hasattr(cls, "pipeline_run") else None
 
         is_self_contained = not pipeline_run and pipeline_id
@@ -434,16 +457,19 @@
         user = kwargs.get("user")
         stream = kwargs.get("stream")
         pipeline_id = kwargs.pop("pipeline_id", None)
         model_params = {
             k: v for k, v in kwargs.items() if k not in ["messages", "user"]
         }
 
+        rendered_messages = create_rendered_chat_messages(messages)
+        new_kwargs = dict(kwargs, messages=rendered_messages)
+
         start_time = time.time()
-        completion = await original_fn(**kwargs)
+        completion = await original_fn(**new_kwargs)
 
         if stream:
             is_self_contained = not hasattr(cls, "pipeline_run") and pipeline_id
             if is_self_contained:
                 pipeline_run_id = str(uuid.uuid4())
 
             async def profiled_completion():
```

### Comparing `gentrace_py-0.6.1/gentrace/providers/pipeline.py` & `gentrace_py-0.7.0/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/providers/pipeline_run.py` & `gentrace_py-0.7.0/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/providers/step_run.py` & `gentrace_py-0.7.0/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/providers/utils.py` & `gentrace_py-0.7.0/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.7.0/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/rest.py` & `gentrace_py-0.7.0/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/gentrace/schemas.py` & `gentrace_py-0.7.0/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.6.1/pyproject.toml` & `gentrace_py-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.6.1"
+version = "0.7.0"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
```

### Comparing `gentrace_py-0.6.1/PKG-INFO` & `gentrace_py-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

