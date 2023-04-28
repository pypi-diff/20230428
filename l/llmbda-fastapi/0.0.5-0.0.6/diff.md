# Comparing `tmp/llmbda_fastapi-0.0.5.tar.gz` & `tmp/llmbda_fastapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmbda_fastapi-0.0.5.tar", last modified: Wed Apr 26 11:15:57 2023, max compression
+gzip compressed data, was "llmbda_fastapi-0.0.6.tar", last modified: Fri Apr 28 00:43:15 2023, max compression
```

## Comparing `llmbda_fastapi-0.0.5.tar` & `llmbda_fastapi-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.526163 llmbda_fastapi-0.0.5/
--rw-rw-rw-   0        0        0     2537 2023-04-26 11:15:57.526163 llmbda_fastapi-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2335 2023-04-24 08:52:38.000000 llmbda_fastapi-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.511614 llmbda_fastapi-0.0.5/llmbda_fastapi/
--rw-rw-rw-   0        0        0      143 2023-04-26 11:15:47.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/__init__.py
--rw-rw-rw-   0        0        0     3978 2023-04-24 08:41:21.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/chains.py
-drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.525163 llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/
--rw-rw-rw-   0        0        0       54 2023-04-24 10:31:44.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/__init__.py
--rw-rw-rw-   0        0        0     5555 2023-04-24 06:58:04.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/input_components.py
--rw-rw-rw-   0        0        0     3730 2023-04-26 11:13:25.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/transformations.py
-drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.521613 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/
--rw-rw-rw-   0        0        0     2537 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 11:15:57.527167 llmbda_fastapi-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-24 11:12:55.000000 llmbda_fastapi-0.0.5/setup.py
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.709080 llmbda_fastapi-0.0.6/
+-rw-r--r--   0 jackykoh   (501) staff       (20)     2453 2023-04-28 00:43:15.708876 llmbda_fastapi-0.0.6/PKG-INFO
+-rw-r--r--   0 jackykoh   (501) staff       (20)     2260 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.6/README.md
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.707069 llmbda_fastapi-0.0.6/llmbda_fastapi/
+-rw-r--r--   0 jackykoh   (501) staff       (20)      139 2023-04-28 00:42:42.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/__init__.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     3878 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/chains.py
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.708669 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/
+-rw-r--r--   0 jackykoh   (501) staff       (20)      109 2023-04-28 00:39:06.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/__init__.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     5362 2023-04-26 00:40:47.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/input_components.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     1833 2023-04-28 00:43:10.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/upload_file.py
+-rw-r--r--   0 jackykoh   (501) staff       (20)     3606 2023-04-27 01:44:36.000000 llmbda_fastapi-0.0.6/llmbda_fastapi/transformations.py
+drwxr-xr-x   0 jackykoh   (501) staff       (20)        0 2023-04-28 00:43:15.707838 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/
+-rw-r--r--   0 jackykoh   (501) staff       (20)     2453 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (501) staff       (20)      412 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)        1 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)      337 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)       15 2023-04-28 00:43:15.000000 llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (501) staff       (20)       38 2023-04-28 00:43:15.709137 llmbda_fastapi-0.0.6/setup.cfg
+-rw-r--r--   0 jackykoh   (501) staff       (20)     1025 2023-04-27 01:44:36.000000 llmbda_fastapi-0.0.6/setup.py
```

### Comparing `llmbda_fastapi-0.0.5/PKG-INFO` & `llmbda_fastapi-0.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,76 @@
-Metadata-Version: 2.1
-Name: llmbda_fastapi
-Version: 0.0.5
-Home-page: https://relevanceai.com/
-Author: Relevance AI
-Author-email: jacky@relevanceai.com
-Description-Content-Type: text/markdown
-
-# Llmbda FastAPI
-
-## Add your fastapi endpoints to your Relevance Notebook for chaining.
-1. Install:
-```
-pip install llmbda_fastapi
-```
-
-2. Set your Relevance Auth Token from cloud.relevanceai.com/sdk/api:
-```
-SET RELEVANCE_AUTH_TOKEN=xxx
-```
-or
-```
-export RELEVANCE_AUTH_TOKEN=xxx
-```
-
-3. Include these 2 lines of code:
-```
-PUBLIC_URL = "https://whereyourapiishosted.com/"
-
-from fastapi import FastAPI
-app = FastAPI()
-
-from llmbda_fastapi import create_transformations
-create_transformations(app.routes, PUBLIC_URL)
-```
-
-If you are working off a local computer you can use ngrok to create a public url:
-```
-pip install pyngrok
-```
-
-```
-from fastapi import FastAPI
-app = FastAPI()
-
-#add this for ngrok
-from pyngrok import ngrok
-PUBLIC_URL = ngrok.connect(8000).public_url
-
-#add this
-from llmbda_fastapi import create_transformations
-create_transformations(app.routes, PUBLIC_URL)
-```
-
-4. Add these options to your existing api endpoints, for example this is a endpoint to "Run code in your local environment"
-
-```
-from fastapi import APIRouter, Query
-from pydantic import BaseModel
-from llmbda_fastapi.frontend import input_components
-
-router = APIRouter()
-
-#Optionally specify frontend_component to make this input be displayed as a specific frontend component
-class ExecuteCodeParams(BaseModel):
-    code : str = Query(..., description="Code to run", frontend_component=input_components.BaseTextArea())
-    #the name and description of this will be automatically picked up and displayed in the notebook
-
-class ExecuteCodeResponseParams(BaseModel):
-    results : str = Query(" ", description="Return whats printed by the code")
-
-# This is the actual transformation
-def evaluate_code(code):
-    print("Executing code: " + code)
-    output = eval(code)
-    print(output)
-    return {"results" : str(output)}
-
-# This is the API endpoint for the transformation
-# The name and description of this will be automatically picked up and displayed in the notebook. Make sure to set response_model and query parameters if they are required.
-@router.post("/run_code", name="Run Code", description="Run Code Locally - Test", tags=["coding"], response_model=ExecuteCodeResponseParams)
-def run_code_api(commons: ExecuteCodeParams):
-    return evaluate_code(commons.code)
-```
+# Llmbda FastAPI
+
+## Add your fastapi endpoints to your Relevance Notebook for chaining.
+1. Install:
+```
+pip install llmbda_fastapi
+```
+
+2. Set your Relevance Auth Token from cloud.relevanceai.com/sdk/api:
+```
+SET RELEVANCE_AUTH_TOKEN=xxx
+```
+or
+```
+export RELEVANCE_AUTH_TOKEN=xxx
+```
+
+3. Include these 2 lines of code:
+```
+PUBLIC_URL = "https://whereyourapiishosted.com/"
+
+from fastapi import FastAPI
+app = FastAPI()
+
+from llmbda_fastapi import create_transformations
+create_transformations(app.routes, PUBLIC_URL)
+```
+
+If you are working off a local computer you can use ngrok to create a public url:
+```
+pip install pyngrok
+```
+
+```
+from fastapi import FastAPI
+app = FastAPI()
+
+#add this for ngrok
+from pyngrok import ngrok
+PUBLIC_URL = ngrok.connect(8000).public_url
+
+#add this
+from llmbda_fastapi import create_transformations
+create_transformations(app.routes, PUBLIC_URL)
+```
+
+4. Add these options to your existing api endpoints, for example this is a endpoint to "Run code in your local environment"
+
+```
+from fastapi import APIRouter, Query
+from pydantic import BaseModel
+from llmbda_fastapi.frontend import input_components
+
+router = APIRouter()
+
+#Optionally specify frontend_component to make this input be displayed as a specific frontend component
+class ExecuteCodeParams(BaseModel):
+    code : str = Query(..., description="Code to run", frontend_component=input_components.BaseTextArea())
+    #the name and description of this will be automatically picked up and displayed in the notebook
+
+class ExecuteCodeResponseParams(BaseModel):
+    results : str = Query(" ", description="Return whats printed by the code")
+
+# This is the actual transformation
+def evaluate_code(code):
+    print("Executing code: " + code)
+    output = eval(code)
+    print(output)
+    return {"results" : str(output)}
+
+# This is the API endpoint for the transformation
+# The name and description of this will be automatically picked up and displayed in the notebook. Make sure to set response_model and query parameters if they are required.
+@router.post("/run_code", name="Run Code", description="Run Code Locally - Test", tags=["coding"], response_model=ExecuteCodeResponseParams)
+def run_code_api(commons: ExecuteCodeParams):
+    return evaluate_code(commons.code)
+```
```

### Comparing `llmbda_fastapi-0.0.5/README.md` & `llmbda_fastapi-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,84 @@
-# Llmbda FastAPI
-
-## Add your fastapi endpoints to your Relevance Notebook for chaining.
-1. Install:
-```
-pip install llmbda_fastapi
-```
-
-2. Set your Relevance Auth Token from cloud.relevanceai.com/sdk/api:
-```
-SET RELEVANCE_AUTH_TOKEN=xxx
-```
-or
-```
-export RELEVANCE_AUTH_TOKEN=xxx
-```
-
-3. Include these 2 lines of code:
-```
-PUBLIC_URL = "https://whereyourapiishosted.com/"
-
-from fastapi import FastAPI
-app = FastAPI()
-
-from llmbda_fastapi import create_transformations
-create_transformations(app.routes, PUBLIC_URL)
-```
-
-If you are working off a local computer you can use ngrok to create a public url:
-```
-pip install pyngrok
-```
-
-```
-from fastapi import FastAPI
-app = FastAPI()
-
-#add this for ngrok
-from pyngrok import ngrok
-PUBLIC_URL = ngrok.connect(8000).public_url
-
-#add this
-from llmbda_fastapi import create_transformations
-create_transformations(app.routes, PUBLIC_URL)
-```
-
-4. Add these options to your existing api endpoints, for example this is a endpoint to "Run code in your local environment"
-
-```
-from fastapi import APIRouter, Query
-from pydantic import BaseModel
-from llmbda_fastapi.frontend import input_components
-
-router = APIRouter()
-
-#Optionally specify frontend_component to make this input be displayed as a specific frontend component
-class ExecuteCodeParams(BaseModel):
-    code : str = Query(..., description="Code to run", frontend_component=input_components.BaseTextArea())
-    #the name and description of this will be automatically picked up and displayed in the notebook
-
-class ExecuteCodeResponseParams(BaseModel):
-    results : str = Query(" ", description="Return whats printed by the code")
-
-# This is the actual transformation
-def evaluate_code(code):
-    print("Executing code: " + code)
-    output = eval(code)
-    print(output)
-    return {"results" : str(output)}
-
-# This is the API endpoint for the transformation
-# The name and description of this will be automatically picked up and displayed in the notebook. Make sure to set response_model and query parameters if they are required.
-@router.post("/run_code", name="Run Code", description="Run Code Locally - Test", tags=["coding"], response_model=ExecuteCodeResponseParams)
-def run_code_api(commons: ExecuteCodeParams):
-    return evaluate_code(commons.code)
-```
+Metadata-Version: 2.1
+Name: llmbda_fastapi
+Version: 0.0.6
+Home-page: https://relevanceai.com/
+Author: Relevance AI
+Author-email: jacky@relevanceai.com
+Description-Content-Type: text/markdown
+
+# Llmbda FastAPI
+
+## Add your fastapi endpoints to your Relevance Notebook for chaining.
+1. Install:
+```
+pip install llmbda_fastapi
+```
+
+2. Set your Relevance Auth Token from cloud.relevanceai.com/sdk/api:
+```
+SET RELEVANCE_AUTH_TOKEN=xxx
+```
+or
+```
+export RELEVANCE_AUTH_TOKEN=xxx
+```
+
+3. Include these 2 lines of code:
+```
+PUBLIC_URL = "https://whereyourapiishosted.com/"
+
+from fastapi import FastAPI
+app = FastAPI()
+
+from llmbda_fastapi import create_transformations
+create_transformations(app.routes, PUBLIC_URL)
+```
+
+If you are working off a local computer you can use ngrok to create a public url:
+```
+pip install pyngrok
+```
+
+```
+from fastapi import FastAPI
+app = FastAPI()
+
+#add this for ngrok
+from pyngrok import ngrok
+PUBLIC_URL = ngrok.connect(8000).public_url
+
+#add this
+from llmbda_fastapi import create_transformations
+create_transformations(app.routes, PUBLIC_URL)
+```
+
+4. Add these options to your existing api endpoints, for example this is a endpoint to "Run code in your local environment"
+
+```
+from fastapi import APIRouter, Query
+from pydantic import BaseModel
+from llmbda_fastapi.frontend import input_components
+
+router = APIRouter()
+
+#Optionally specify frontend_component to make this input be displayed as a specific frontend component
+class ExecuteCodeParams(BaseModel):
+    code : str = Query(..., description="Code to run", frontend_component=input_components.BaseTextArea())
+    #the name and description of this will be automatically picked up and displayed in the notebook
+
+class ExecuteCodeResponseParams(BaseModel):
+    results : str = Query(" ", description="Return whats printed by the code")
+
+# This is the actual transformation
+def evaluate_code(code):
+    print("Executing code: " + code)
+    output = eval(code)
+    print(output)
+    return {"results" : str(output)}
+
+# This is the API endpoint for the transformation
+# The name and description of this will be automatically picked up and displayed in the notebook. Make sure to set response_model and query parameters if they are required.
+@router.post("/run_code", name="Run Code", description="Run Code Locally - Test", tags=["coding"], response_model=ExecuteCodeResponseParams)
+def run_code_api(commons: ExecuteCodeParams):
+    return evaluate_code(commons.code)
+```
```

### Comparing `llmbda_fastapi-0.0.5/llmbda_fastapi/chains.py` & `llmbda_fastapi-0.0.6/llmbda_fastapi/chains.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import os
-import json
-import atexit
-import requests
-from typing import List
-from fastapi.routing import APIRoute
-
-RELEVANCE_AUTH_TOKEN = os.getenv("RELEVANCE_AUTH_TOKEN")
-
-def routes_to_chains(api_routes, url, id_suffix=""):
-    chains_list = []
-    id_list = []
-    for route in api_routes:
-        if isinstance(route, APIRoute):
-            id_list.append(route.unique_id + id_suffix)
-            input_schema = {}
-            request_body = ""
-            if route.body_field:
-                input_schema = json.loads(route.body_field.type_.schema_json())
-                for k,v in input_schema["properties"].items():
-                    if v["type"] == "string":
-                        request_body += f'"{k}" : "{{{{ params.{k} }}}}",'
-                    else:
-                        request_body += f'"{k}" : {{{{ params.{k} }}}},'
-                request_body = "{ " + request_body[:-1] + " }"
-
-            output_schema = {}
-            if route.response_field:
-                output_raw_schema = json.loads(route.response_field.type_.schema_json())
-                for k, v in output_raw_schema.items():
-                    output_schema[k] = f"{{{{ steps.api_call.output.response_body.{k} }}}}"
-
-            if url.endswith("/"):
-                full_path = url[:-1] + route.path
-            else:
-                full_path = url + route.path
-
-            chains_list.append({
-                "public":False,
-                "studio_id":route.unique_id + id_suffix,
-                "params_schema":input_schema,
-                "publicly_triggerable":False,
-                "project":RELEVANCE_AUTH_TOKEN.split(":")[0],
-                "title":route.summary if route.summary else route.name,
-                "description":route.description,
-                "transformations" : {
-                    "steps":[
-                        {
-                            "name":"api_call",
-                            "transformation":"api_call",
-                            "params":{
-                                "url": full_path,
-                                "method":"POST",
-                                "headers":{
-                                    "Content-Type":"application/json",
-                                    # **headers
-                                },
-                                "body":request_body,
-                                "response_type":"json"
-                            },
-                            "output":{
-                                "response_body":"{{response_body}}",
-                                "status":"{{status}}"
-                            }
-                        }
-                    ],
-                    "output":output_schema
-                }
-            })
-    return chains_list, id_list
-
-def upload_chains(chains):
-    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
-    results = requests.post(
-        f"{url}/latest/studios/bulk_update",
-        headers={
-            "Authorization" : RELEVANCE_AUTH_TOKEN
-        },
-        json={
-            "updates": chains
-        }
-    )
-    print("Uploaded chains: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-    
-def cleanup_chains(chain_id_list):
-    results = requests.post(
-        f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com/latest/studios/bulk_delete",
-        headers={
-            "Authorization" : RELEVANCE_AUTH_TOKEN
-        },
-        json={"ids": chain_id_list}
-    )
-    print("Successfully deleted chains from cloud: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-
-def create_chains(api_routes, url, id_suffix=""):
-    chains, chain_id_list = routes_to_chains(api_routes, url, id_suffix=id_suffix)
-    upload_chains(chains)
-    atexit.register(cleanup_chains, chain_id_list)
+import os
+import json
+import atexit
+import requests
+from typing import List
+from fastapi.routing import APIRoute
+
+RELEVANCE_AUTH_TOKEN = os.getenv("RELEVANCE_AUTH_TOKEN")
+
+def routes_to_chains(api_routes, url, id_suffix=""):
+    chains_list = []
+    id_list = []
+    for route in api_routes:
+        if isinstance(route, APIRoute):
+            id_list.append(route.unique_id + id_suffix)
+            input_schema = {}
+            request_body = ""
+            if route.body_field:
+                input_schema = json.loads(route.body_field.type_.schema_json())
+                for k,v in input_schema["properties"].items():
+                    if v["type"] == "string":
+                        request_body += f'"{k}" : "{{{{ params.{k} }}}}",'
+                    else:
+                        request_body += f'"{k}" : {{{{ params.{k} }}}},'
+                request_body = "{ " + request_body[:-1] + " }"
+
+            output_schema = {}
+            if route.response_field:
+                output_raw_schema = json.loads(route.response_field.type_.schema_json())
+                for k, v in output_raw_schema.items():
+                    output_schema[k] = f"{{{{ steps.api_call.output.response_body.{k} }}}}"
+
+            if url.endswith("/"):
+                full_path = url[:-1] + route.path
+            else:
+                full_path = url + route.path
+
+            chains_list.append({
+                "public":False,
+                "studio_id":route.unique_id + id_suffix,
+                "params_schema":input_schema,
+                "publicly_triggerable":False,
+                "project":RELEVANCE_AUTH_TOKEN.split(":")[0],
+                "title":route.summary if route.summary else route.name,
+                "description":route.description,
+                "transformations" : {
+                    "steps":[
+                        {
+                            "name":"api_call",
+                            "transformation":"api_call",
+                            "params":{
+                                "url": full_path,
+                                "method":"POST",
+                                "headers":{
+                                    "Content-Type":"application/json",
+                                    # **headers
+                                },
+                                "body":request_body,
+                                "response_type":"json"
+                            },
+                            "output":{
+                                "response_body":"{{response_body}}",
+                                "status":"{{status}}"
+                            }
+                        }
+                    ],
+                    "output":output_schema
+                }
+            })
+    return chains_list, id_list
+
+def upload_chains(chains):
+    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
+    results = requests.post(
+        f"{url}/latest/studios/bulk_update",
+        headers={
+            "Authorization" : RELEVANCE_AUTH_TOKEN
+        },
+        json={
+            "updates": chains
+        }
+    )
+    print("Uploaded chains: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+    
+def cleanup_chains(chain_id_list):
+    results = requests.post(
+        f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com/latest/studios/bulk_delete",
+        headers={
+            "Authorization" : RELEVANCE_AUTH_TOKEN
+        },
+        json={"ids": chain_id_list}
+    )
+    print("Successfully deleted chains from cloud: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+
+def create_chains(api_routes, url, id_suffix=""):
+    chains, chain_id_list = routes_to_chains(api_routes, url, id_suffix=id_suffix)
+    upload_chains(chains)
+    atexit.register(cleanup_chains, chain_id_list)
     return chain_id_list
```

### Comparing `llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/input_components.py` & `llmbda_fastapi-0.0.6/llmbda_fastapi/frontend/input_components.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-"""
-    All components are here
-"""
-from dataclasses import dataclass, field
-
-class Component:
-    """
-    Base class for all components
-    """
-
-@dataclass
-class APIKeyInput(Component):
-    valueKey: str = ""
-    type: str = "apiKeyInput"
-    props: dict = field(default_factory=lambda: {
-        "apiKey": ""
-    })
-
-
-@dataclass
-class FieldSelector(Component):
-    type: str = "fieldSelector"
-    props: dict = field(
-        default_factory=lambda: {"onlyTypes": ["vector"], "multiple": False}
-    )
-
-
-@dataclass
-class FileUpload(Component):
-    title: str = "Upload your files."
-    description: str = "You can upload your files here."
-    type: str = "fileUpload"
-    props: dict = field(
-        default_factory=lambda: {
-            "accept": "*",  # optional, filters accepted file/mime-types. See https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file#limiting_accepted_file_types
-            "multiple": True,  # optional, enables multiple files uploaded
-        }
-    )
-
-
-@dataclass
-class AdvancedFilters(Component):
-    valueKey: str = "filters"
-    type: str = "advancedFilterInput"
-    props: dict = field(default_factory=lambda: {"optional": True})
-
-
-@dataclass
-class BaseInput(Component):
-    type: str = "baseInput"
-    props: dict = field(
-        default_factory=lambda: {
-            "type": "text",
-            "value": "default",
-        }
-    )
-
-@dataclass
-class BaseTextArea(Component):
-    type: str = "baseTextArea"
-    props: dict = field(
-        default_factory=lambda: {
-            "type": "text",
-            "placeholder": "Enter value...",
-            "rows" : 2,
-            "maxlength" : 500
-        }
-    )
-    
-@dataclass
-class PromptArea(Component):
-    type: str = "playgroundPrompt"
-
-@dataclass
-class BaseDropdown(Component):
-    type: str = "baseDropdown"
-    props: dict = field(default_factory=lambda: {})
-
-@dataclass
-class BoolDropdown(Component):
-    type: str = "baseDropdown"
-    props: dict = field(default_factory=lambda: {
-        "options": [
-            {
-                "label": "Yes",
-                "value": True,
-            },
-            {
-                "label": "No",
-                "value": False,
-            },
-        ],
-        "multiple": False,
-        "optional": True,
-        "value": True
-    })
-
-@dataclass
-class SentenceListInput(Component):
-    type: str = "sentenceListInput"
-    props: dict = field(default_factory=lambda: {
-    })
-
-@dataclass
-class BooleanChecklist(Component):
-    type: str = "booleanChecklist"
-    props: dict = field(default_factory=lambda: {
-        "labelMap" : {"example":{"description": "This is what users see for example", "value" : False}}
-    })
-
-@dataclass
-class TagsInput(Component):
-    type: str = "tagsInput"
-    props: dict = field(default_factory=lambda: {"props": {"separators": [","]}})
-
-@dataclass
-class TaxonomyBuilder(Component):
-    type: str = "taxonomyBuilder"
-    props: dict = field(default_factory=lambda: {})
-
-@dataclass
-class SliderInput(Component):
-    type: str = "baseInput"
-    props: dict = field(
-        default_factory=lambda: {"type": "number", "max": 100, "step": 1, "min": 1}
-    )
-
-@dataclass
-class DynamicTextInput(Component):
-    type: str = "dynamicInput"
-    props: dict = field(
-        default_factory=lambda: {
-            "outputLabel": "Output field name:",  # Optional, defaults to "This will be stored as:",
-            "template": "_surveytag_.{ vector_fields }.{ value }",  # Required, use `{ value }` to reference current component's value. Can reference other fields by `valueKey`
-        }
-    )
-
-
-@dataclass
-class AggregateTagsSelector(Component):
-    type: str = "aggregateTagsSelector"
-    props: dict = field(
-        default_factory=lambda: {
-            "aggregationQuery": {  # Required
-                "groupby": [
-                    {
-                        "name": "field",  #
-                        "field": "{ field }",  # Use this to refer to the selected field
-                        "agg": "category",
-                    }
-                ]
-            },
-            "aggregationResultField": "field",  # Required, sHould match `name` in aggregationQuery
-            "maxRunResults": 20,  # maximum number of tags to get from aggregate, defaults to 20
-        }
-    )
-
-
-@dataclass
-class AggregateSelector(Component):
-    type: str = "aggregateSelector"
-    props: dict = field(
-        default_factory=lambda: {
-            "aggregationQuery": {  # Required
-                "groupby": [
-                    {
-                        "name": "field",  #
-                        "field": "{ field }",  # Use this to refer to the selected field
-                        "agg": "category",
-                    }
-                ]
-            },
-            "aggregationResultField": "field",  # Required, sHould match `name` in aggregationQuery
-            "maxRunResults": 20,  # maximum number of tags to get from aggregate, defaults to 20
-        }
-    )
-
-
-@dataclass
-class ExplorerSelector(Component):
-    type: str = "explorerSelector"
-    props: dict = field(default_factory=lambda: {})
-
-
-@dataclass
-class TagPairInput(Component):
-    type: str = "pairInput"
-    props: dict = field(default_factory=lambda: {"addTagText": "Add new tag"})
-
-
-@dataclass
-class DatasetInput(Component):
-    type: str = "datasetNameInput"
+"""
+    All components are here
+"""
+from dataclasses import dataclass, field
+
+class Component:
+    """
+    Base class for all components
+    """
+
+@dataclass
+class APIKeyInput(Component):
+    valueKey: str = ""
+    type: str = "apiKeyInput"
+    props: dict = field(default_factory=lambda: {
+        "apiKey": ""
+    })
+
+
+@dataclass
+class FieldSelector(Component):
+    type: str = "fieldSelector"
+    props: dict = field(
+        default_factory=lambda: {"onlyTypes": ["vector"], "multiple": False}
+    )
+
+
+@dataclass
+class FileUpload(Component):
+    title: str = "Upload your files."
+    description: str = "You can upload your files here."
+    type: str = "fileUpload"
+    props: dict = field(
+        default_factory=lambda: {
+            "accept": "*",  # optional, filters accepted file/mime-types. See https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file#limiting_accepted_file_types
+            "multiple": True,  # optional, enables multiple files uploaded
+        }
+    )
+
+
+@dataclass
+class AdvancedFilters(Component):
+    valueKey: str = "filters"
+    type: str = "advancedFilterInput"
+    props: dict = field(default_factory=lambda: {"optional": True})
+
+
+@dataclass
+class BaseInput(Component):
+    type: str = "baseInput"
+    props: dict = field(
+        default_factory=lambda: {
+            "type": "text",
+            "value": "default",
+        }
+    )
+
+@dataclass
+class BaseTextArea(Component):
+    type: str = "baseTextArea"
+    props: dict = field(
+        default_factory=lambda: {
+            "type": "text",
+            "placeholder": "Enter value...",
+            "rows" : 2,
+            "maxlength" : 500
+        }
+    )
+    
+@dataclass
+class PromptArea(Component):
+    type: str = "playgroundPrompt"
+
+@dataclass
+class BaseDropdown(Component):
+    type: str = "baseDropdown"
+    props: dict = field(default_factory=lambda: {})
+
+@dataclass
+class BoolDropdown(Component):
+    type: str = "baseDropdown"
+    props: dict = field(default_factory=lambda: {
+        "options": [
+            {
+                "label": "Yes",
+                "value": True,
+            },
+            {
+                "label": "No",
+                "value": False,
+            },
+        ],
+        "multiple": False,
+        "optional": True,
+        "value": True
+    })
+
+@dataclass
+class SentenceListInput(Component):
+    type: str = "sentenceListInput"
+    props: dict = field(default_factory=lambda: {
+    })
+
+@dataclass
+class BooleanChecklist(Component):
+    type: str = "booleanChecklist"
+    props: dict = field(default_factory=lambda: {
+        "labelMap" : {"example":{"description": "This is what users see for example", "value" : False}}
+    })
+
+@dataclass
+class TagsInput(Component):
+    type: str = "tagsInput"
+    props: dict = field(default_factory=lambda: {"props": {"separators": [","]}})
+
+@dataclass
+class TaxonomyBuilder(Component):
+    type: str = "taxonomyBuilder"
+    props: dict = field(default_factory=lambda: {})
+
+@dataclass
+class SliderInput(Component):
+    type: str = "baseInput"
+    props: dict = field(
+        default_factory=lambda: {"type": "number", "max": 100, "step": 1, "min": 1}
+    )
+
+@dataclass
+class DynamicTextInput(Component):
+    type: str = "dynamicInput"
+    props: dict = field(
+        default_factory=lambda: {
+            "outputLabel": "Output field name:",  # Optional, defaults to "This will be stored as:",
+            "template": "_surveytag_.{ vector_fields }.{ value }",  # Required, use `{ value }` to reference current component's value. Can reference other fields by `valueKey`
+        }
+    )
+
+
+@dataclass
+class AggregateTagsSelector(Component):
+    type: str = "aggregateTagsSelector"
+    props: dict = field(
+        default_factory=lambda: {
+            "aggregationQuery": {  # Required
+                "groupby": [
+                    {
+                        "name": "field",  #
+                        "field": "{ field }",  # Use this to refer to the selected field
+                        "agg": "category",
+                    }
+                ]
+            },
+            "aggregationResultField": "field",  # Required, sHould match `name` in aggregationQuery
+            "maxRunResults": 20,  # maximum number of tags to get from aggregate, defaults to 20
+        }
+    )
+
+
+@dataclass
+class AggregateSelector(Component):
+    type: str = "aggregateSelector"
+    props: dict = field(
+        default_factory=lambda: {
+            "aggregationQuery": {  # Required
+                "groupby": [
+                    {
+                        "name": "field",  #
+                        "field": "{ field }",  # Use this to refer to the selected field
+                        "agg": "category",
+                    }
+                ]
+            },
+            "aggregationResultField": "field",  # Required, sHould match `name` in aggregationQuery
+            "maxRunResults": 20,  # maximum number of tags to get from aggregate, defaults to 20
+        }
+    )
+
+
+@dataclass
+class ExplorerSelector(Component):
+    type: str = "explorerSelector"
+    props: dict = field(default_factory=lambda: {})
+
+
+@dataclass
+class TagPairInput(Component):
+    type: str = "pairInput"
+    props: dict = field(default_factory=lambda: {"addTagText": "Add new tag"})
+
+
+@dataclass
+class DatasetInput(Component):
+    type: str = "datasetNameInput"
     props: dict = field(default_factory=lambda: {})
```

### Comparing `llmbda_fastapi-0.0.5/llmbda_fastapi/transformations.py` & `llmbda_fastapi-0.0.6/llmbda_fastapi/transformations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,100 @@
-import os
-import json
-import atexit
-import requests
-from fastapi.routing import APIRoute
-
-RELEVANCE_AUTH_TOKEN = os.getenv("RELEVANCE_AUTH_TOKEN")
-
-def routes_to_transformations(api_routes, url, id_suffix=""):
-    tfs_list = []
-    id_list = []
-    for route in api_routes:
-        if isinstance(route, APIRoute):
-            id_list.append(route.unique_id + id_suffix)
-            input_schema = {}
-            if route.body_field:
-                input_schema = json.loads(route.body_field.type_.schema_json())
-
-            for k, v in input_schema["properties"].items():
-                if "title" in v:
-                    if "metadata" not in v:
-                        v['metadata'] = {}
-                    v['metadata']['title'] = v['title']
-                    del v['title']
-                if "description" in v:
-                    if "metadata" not in v:
-                        v['metadata'] = {}
-                    v['metadata']['description'] = v['description']
-                    del v['description']
-
-            output_schema = {}
-            if route.response_field:
-                output_schema = json.loads(route.response_field.type_.schema_json())
-
-            if url.endswith("/"):
-                url = url[:-1]
-            route_path = route.path
-            if route_path.startswith("/"):
-                route_path = route_path[1:]
-            full_path = url + "/" + route_path
-
-            tfs_list.append({
-                "_id" : route.unique_id + id_suffix,
-                "transformation_id" : route.unique_id + id_suffix,
-                "name" : route.summary if route.summary else route.name,
-                "description" : route.description,
-                "studio_api_path" : full_path,
-                "execution_type" : "studio-api",
-                "input_schema" : input_schema,
-                "output_schema" : output_schema,
-            })
-    return tfs_list, id_list
-
-def list_transformations():
-    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
-    results = requests.post(
-        f"{url}/latest/studios/transformations/custom/list",
-        headers={
-            "Authorization" : RELEVANCE_AUTH_TOKEN
-        },
-        json={
-            "page" : 1,
-            "page_size" : 10
-        }
-    )
-    print("List of transformations: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-
-def cleanup_transformations(transformation_id_list):
-    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
-    results = requests.post(
-        f"{url}/latest/studios/transformations/custom/bulk_delete",
-        headers={
-            "Authorization" : RELEVANCE_AUTH_TOKEN
-        },
-        json={"ids": transformation_id_list}
-    )
-    print("Successfully deleted transformations from cloud: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-
-def upload_transformations(tfs):
-    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
-    results = requests.post(
-        f"{url}/latest/studios/transformations/custom/bulk_update",
-        headers={
-            "Authorization" : RELEVANCE_AUTH_TOKEN
-        },
-        json={
-            "updates": tfs
-        }
-    )
-    print("Uploaded transformations: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-
-def create_transformations(api_routes, url, id_suffix=""):
-    tfs_list, id_list = routes_to_transformations(api_routes, url, id_suffix=id_suffix)
-    upload_transformations(tfs_list)
-    atexit.register(cleanup_transformations, id_list)
+import os
+import json
+import atexit
+import requests
+from fastapi.routing import APIRoute
+
+RELEVANCE_AUTH_TOKEN = os.getenv("RELEVANCE_AUTH_TOKEN")
+
+def routes_to_transformations(api_routes, url, id_suffix=""):
+    tfs_list = []
+    id_list = []
+    for route in api_routes:
+        if isinstance(route, APIRoute):
+            uid = route.unique_id + id_suffix
+            id_list.append(uid)
+            input_schema = {}
+            if route.body_field:
+                input_schema = json.loads(route.body_field.type_.schema_json())
+
+            for k, v in input_schema["properties"].items():
+                if "title" in v:
+                    if "metadata" not in v:
+                        v['metadata'] = {}
+                    v['metadata']['title'] = v['title']
+                    del v['title']
+                if "description" in v:
+                    if "metadata" not in v:
+                        v['metadata'] = {}
+                    v['metadata']['description'] = v['description']
+                    del v['description']
+
+            output_schema = {}
+            if route.response_field:
+                output_schema = json.loads(route.response_field.type_.schema_json())
+
+            if url.endswith("/"):
+                url = url[:-1]
+            route_path = route.path
+            if route_path.startswith("/"):
+                route_path = route_path[1:]
+            full_path = url + "/" + route_path
+
+            tfs_list.append({
+                "_id" : uid,
+                "transformation_id" : uid,
+                "name" : route.summary if route.summary else route.name,
+                "description" : route.description,
+                "studio_api_path" : full_path,
+                "execution_type" : "studio-api",
+                "input_schema" : input_schema,
+                "output_schema" : output_schema,
+            })
+    return tfs_list, id_list
+
+def list_transformations():
+    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
+    results = requests.post(
+        f"{url}/latest/studios/transformations/custom/list",
+        headers={
+            "Authorization" : RELEVANCE_AUTH_TOKEN
+        },
+        json={
+            "page" : 1,
+            "page_size" : 10
+        }
+    )
+    print("List of transformations: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+
+def cleanup_transformations(transformation_id_list):
+    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
+    results = requests.post(
+        f"{url}/latest/studios/transformations/custom/bulk_delete",
+        headers={
+            "Authorization" : RELEVANCE_AUTH_TOKEN
+        },
+        json={"ids": transformation_id_list}
+    )
+    print("Successfully deleted transformations from cloud: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+
+def upload_transformations(tfs):
+    url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
+    results = requests.post(
+        f"{url}/latest/studios/transformations/custom/bulk_update",
+        headers={
+            "Authorization" : RELEVANCE_AUTH_TOKEN
+        },
+        json={
+            "updates": tfs
+        }
+    )
+    print("Uploaded transformations: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+
+def create_transformations(api_routes, url, id_suffix=""):
+    tfs_list, id_list = routes_to_transformations(api_routes, url, id_suffix=id_suffix)
+    upload_transformations(tfs_list)
+    atexit.register(cleanup_transformations, id_list)
     return tfs_list
```

### Comparing `llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/PKG-INFO` & `llmbda_fastapi-0.0.6/llmbda_fastapi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 2.1
-Name: llmbda-fastapi
-Version: 0.0.5
-Home-page: https://relevanceai.com/
-Author: Relevance AI
-Author-email: jacky@relevanceai.com
-Description-Content-Type: text/markdown
-
-# Llmbda FastAPI
-
-## Add your fastapi endpoints to your Relevance Notebook for chaining.
-1. Install:
-```
-pip install llmbda_fastapi
-```
-
-2. Set your Relevance Auth Token from cloud.relevanceai.com/sdk/api:
-```
-SET RELEVANCE_AUTH_TOKEN=xxx
-```
-or
-```
-export RELEVANCE_AUTH_TOKEN=xxx
-```
-
-3. Include these 2 lines of code:
-```
-PUBLIC_URL = "https://whereyourapiishosted.com/"
-
-from fastapi import FastAPI
-app = FastAPI()
-
-from llmbda_fastapi import create_transformations
-create_transformations(app.routes, PUBLIC_URL)
-```
-
-If you are working off a local computer you can use ngrok to create a public url:
-```
-pip install pyngrok
-```
-
-```
-from fastapi import FastAPI
-app = FastAPI()
-
-#add this for ngrok
-from pyngrok import ngrok
-PUBLIC_URL = ngrok.connect(8000).public_url
-
-#add this
-from llmbda_fastapi import create_transformations
-create_transformations(app.routes, PUBLIC_URL)
-```
-
-4. Add these options to your existing api endpoints, for example this is a endpoint to "Run code in your local environment"
-
-```
-from fastapi import APIRouter, Query
-from pydantic import BaseModel
-from llmbda_fastapi.frontend import input_components
-
-router = APIRouter()
-
-#Optionally specify frontend_component to make this input be displayed as a specific frontend component
-class ExecuteCodeParams(BaseModel):
-    code : str = Query(..., description="Code to run", frontend_component=input_components.BaseTextArea())
-    #the name and description of this will be automatically picked up and displayed in the notebook
-
-class ExecuteCodeResponseParams(BaseModel):
-    results : str = Query(" ", description="Return whats printed by the code")
-
-# This is the actual transformation
-def evaluate_code(code):
-    print("Executing code: " + code)
-    output = eval(code)
-    print(output)
-    return {"results" : str(output)}
-
-# This is the API endpoint for the transformation
-# The name and description of this will be automatically picked up and displayed in the notebook. Make sure to set response_model and query parameters if they are required.
-@router.post("/run_code", name="Run Code", description="Run Code Locally - Test", tags=["coding"], response_model=ExecuteCodeResponseParams)
-def run_code_api(commons: ExecuteCodeParams):
-    return evaluate_code(commons.code)
-```
+Metadata-Version: 2.1
+Name: llmbda-fastapi
+Version: 0.0.6
+Home-page: https://relevanceai.com/
+Author: Relevance AI
+Author-email: jacky@relevanceai.com
+Description-Content-Type: text/markdown
+
+# Llmbda FastAPI
+
+## Add your fastapi endpoints to your Relevance Notebook for chaining.
+1. Install:
+```
+pip install llmbda_fastapi
+```
+
+2. Set your Relevance Auth Token from cloud.relevanceai.com/sdk/api:
+```
+SET RELEVANCE_AUTH_TOKEN=xxx
+```
+or
+```
+export RELEVANCE_AUTH_TOKEN=xxx
+```
+
+3. Include these 2 lines of code:
+```
+PUBLIC_URL = "https://whereyourapiishosted.com/"
+
+from fastapi import FastAPI
+app = FastAPI()
+
+from llmbda_fastapi import create_transformations
+create_transformations(app.routes, PUBLIC_URL)
+```
+
+If you are working off a local computer you can use ngrok to create a public url:
+```
+pip install pyngrok
+```
+
+```
+from fastapi import FastAPI
+app = FastAPI()
+
+#add this for ngrok
+from pyngrok import ngrok
+PUBLIC_URL = ngrok.connect(8000).public_url
+
+#add this
+from llmbda_fastapi import create_transformations
+create_transformations(app.routes, PUBLIC_URL)
+```
+
+4. Add these options to your existing api endpoints, for example this is a endpoint to "Run code in your local environment"
+
+```
+from fastapi import APIRouter, Query
+from pydantic import BaseModel
+from llmbda_fastapi.frontend import input_components
+
+router = APIRouter()
+
+#Optionally specify frontend_component to make this input be displayed as a specific frontend component
+class ExecuteCodeParams(BaseModel):
+    code : str = Query(..., description="Code to run", frontend_component=input_components.BaseTextArea())
+    #the name and description of this will be automatically picked up and displayed in the notebook
+
+class ExecuteCodeResponseParams(BaseModel):
+    results : str = Query(" ", description="Return whats printed by the code")
+
+# This is the actual transformation
+def evaluate_code(code):
+    print("Executing code: " + code)
+    output = eval(code)
+    print(output)
+    return {"results" : str(output)}
+
+# This is the API endpoint for the transformation
+# The name and description of this will be automatically picked up and displayed in the notebook. Make sure to set response_model and query parameters if they are required.
+@router.post("/run_code", name="Run Code", description="Run Code Locally - Test", tags=["coding"], response_model=ExecuteCodeResponseParams)
+def run_code_api(commons: ExecuteCodeParams):
+    return evaluate_code(commons.code)
+```
```

