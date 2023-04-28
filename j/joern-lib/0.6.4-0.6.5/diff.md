# Comparing `tmp/joern_lib-0.6.4.tar.gz` & `tmp/joern_lib-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.6.4.tar", max compression
+gzip compressed data, was "joern_lib-0.6.5.tar", max compression
```

## Comparing `joern_lib-0.6.4.tar` & `joern_lib-0.6.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-03-04 18:32:27.321067 joern_lib-0.6.4/LICENSE
--rw-r--r--   0        0        0     2710 2023-03-04 18:32:27.321067 joern_lib-0.6.4/README.md
--rw-r--r--   0        0        0        0 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/__init__.py
--rw-r--r--   0        0        0     5583 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/client.py
--rw-r--r--   0        0        0        0 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0     2542 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     3914 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/detectors/js.py
--rw-r--r--   0        0        0     2307 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/utils.py
--rw-r--r--   0        0        0     2814 2023-03-04 18:32:27.333067 joern_lib-0.6.4/joern_lib/workspace.py
--rw-r--r--   0        0        0     1185 2023-03-04 18:32:27.333067 joern_lib-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 joern_lib-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 20:22:45.955128 joern_lib-0.6.5/LICENSE
+-rw-r--r--   0        0        0     3102 2023-04-28 20:22:45.959128 joern_lib-0.6.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/__init__.py
+-rw-r--r--   0        0        0     6605 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/client.py
+-rw-r--r--   0        0        0        0 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0     4132 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     3914 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0     2060 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/utils.py
+-rw-r--r--   0        0        0     4535 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1185 2023-04-28 20:22:45.979129 joern_lib-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 joern_lib-0.6.5/PKG-INFO
```

### Comparing `joern_lib-0.6.4/LICENSE` & `joern_lib-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.4/README.md` & `joern_lib-0.6.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 Execute single query
 
 ```
 from joern_lib import client, workspace
 from joern_lib.detectors import common as cpg
 
-connection = await client.get("http://localhost:9000", "admin", "admin")
+connection = await client.get("http://localhost:9000", "http://localhost:7072", "admin", "admin")
 
 # connection = await client.get("http://localhost:9000")
 
 res = await client.q(connection, "val a=1");
 
 # {'response': 'a: Int = 1\n'}
 ```
@@ -82,14 +82,26 @@
 Import code for analysis
 
 ```
 res = await workspace.import_code(connection, "/app", "NodeGoat")
 # True
 ```
 
+Import an existing CPG for analysis
+
+```
+res = await workspace.import_cpg(connection, "/app/sandbox/crAPI/cpg_out/crAPI-python-cpg.bin.zip", "crAPI-python")
+```
+
+Create a CPG with a remote cpggen server
+
+```
+res = await workspace.create_cpg(connection, "/app/sandbox/crAPI", out_dir="/app/sandbox/crAPI/cpg_out", languages="python", project_name="crAPI-python")
+```
+
 ### CPG core
 
 List files
 
 ```
 res = await cpg.list_files(connection)
 # list of files
```

### Comparing `joern_lib-0.6.4/joern_lib/client.py` & `joern_lib-0.6.5/joern_lib/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 import asyncio
 
+import httpx
+import os
 import orjson
 import uvloop
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-import os
 
-import httpx
 import websockets
 
 from joern_lib.utils import print_md, print_table
 
 headers = {"Content-Type": "application/json", "Accept-Encoding": "gzip"}
+CLIENT_TIMEOUT = os.getenv("HTTP_CLIENT_TIMEOUT")
 
 
 class Connection:
-    def __init__(self, httpclient, websocket):
+    def __init__(self, cpggenclient, httpclient, websocket):
+        self.cpggenclient = cpggenclient
         self.httpclient = httpclient
         self.websocket = websocket
 
     async def __aenter__(self):
         return self
 
     async def ping(self):
         await self.websocket.ping()
 
     async def close(self):
+        await self.cpggenclient.close()
         await self.httpclient.close()
         await self.websocket.close()
 
     async def __aexit__(self, exc_type, exc_value, exc_traceback):
         return await self.close()
 
 
-async def get(base_url, username=None, password=None):
+async def get(
+    base_url="http://localhost:9000",
+    cpggen_url="http://localhost:7072",
+    username=None,
+    password=None,
+):
     auth = None
     if username and password:
         auth = httpx.BasicAuth(username, password)
     base_url = base_url.rstrip("/")
-    client = httpx.AsyncClient(base_url=base_url, auth=auth)
+    client = httpx.AsyncClient(base_url=base_url, auth=auth, timeout=CLIENT_TIMEOUT)
+    cpggenclient = None
+    if cpggen_url:
+        cpggenclient = httpx.AsyncClient(base_url=cpggen_url, timeout=CLIENT_TIMEOUT)
     ws_url = f"""{base_url.replace("http://", "ws://").replace("https://", "wss://")}/connect"""
     websocket = await websockets.connect(ws_url, ping_timeout=None)
     connected_msg = await websocket.recv()
     if connected_msg != "connected":
         raise websockets.exceptions.InvalidState(
             "Didn't receive connected message from Joern server"
         )
-    return Connection(client, websocket)
+    return Connection(cpggenclient, client, websocket)
 
 
 async def send(connection, message):
     await connection.websocket.send(message)
 
 
 async def receive(connection):
@@ -62,23 +73,24 @@
         sout = sout.replace(r'"\"', '"').replace(r'\""', '"')
         if ': String = "[' in sout:
             sout = sout.split(': String = "')[-1][-1]
         elif 'String = """[' in sout:
             tmpA = sout.split("\n")[1:-2]
             sout = "[ " + "\n".join(tmpA) + "]"
         return orjson.loads(sout)
-    except Exception as e:
+    except Exception:
         return {"response": sout}
 
 
 def fix_query(query_str):
     if "\\." in query_str and "\\\\." not in query_str:
         query_str = query_str.replace("\\.", "\\\\.")
     if (
         query_str.startswith("cpg.")
+        or query_str.startswith("({cpg.")
         and ".toJson" not in query_str
         and ".plotDot" not in query_str
         and not query_str.endswith(".p")
     ):
         query_str = f"{query_str}.toJsonPretty"
     return query_str
 
@@ -174,7 +186,27 @@
     if print and len(results):
         tmpres = results[-1]
         if isinstance(tmpres, dict) and tmpres.get("response"):
             tmpres = tmpres.get("response")
         tmpA = tmpres.split('"""')[1:-1]
         print_md("\n".join([n for n in tmpA if len(n.strip()) > 1]))
     return results
+
+
+async def create_cpg(connection, src, out_dir, lang):
+    client = connection.cpggenclient
+    if not client:
+        return {
+            "error": "true",
+            "message": "No active connection to cpggen server. Pass the cpggen url to the client.get method.",
+        }, 500
+    # Suppor for url
+    url = ""
+    if src.startswith("http") or src.startswith("git"):
+        url = src
+        src = ""
+    response = await client.post(
+        url="/cpg",
+        headers=headers,
+        json={"src": src, "url": url, "out_dir": out_dir, "lang": lang},
+    )
+    return response.json()
```

### Comparing `joern_lib-0.6.4/joern_lib/detectors/js.py` & `joern_lib-0.6.5/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.4/joern_lib/utils.py` & `joern_lib-0.6.5/joern_lib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 import os
 
-from rich import box
 from rich.console import Console
-from rich.markdown import Markdown
-from rich.markup import escape
-from rich.panel import Panel
-from rich.progress import Progress
 from rich.syntax import Syntax
 from rich.table import Table
-from rich.terminal_theme import MONOKAI
-from rich.theme import Theme
-from rich.tree import Tree
 
 console = Console(
     log_time=False,
     log_path=False,
     color_system="auto",
     width=int(os.getenv("COLUMNS", 280)),
 )
```

### Comparing `joern_lib-0.6.4/joern_lib/workspace.py` & `joern_lib-0.6.5/joern_lib/workspace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from joern_lib import client
 
 
 def extract_dir(res):
     if res.get("response"):
         dir_name = res.get("response").split('String = "')[-1].split('"')[0]
         return dir_name
@@ -11,21 +13,66 @@
 async def list(connection):
     res = await client.q(connection, "workspace")
     if "[io.joern.joerncli.console.JoernProject] = empty" in res.get("response", ""):
         return None
     return res
 
 
+async def create_cpg(
+    connection, src, out_dir=None, languages="autodetect", project_name=None
+):
+    if not out_dir:
+        out_dir = os.path.join(src, "cpg_out")
+    res = await client.create_cpg(connection, src, out_dir, languages)
+    if res:
+        app_manifests = res.get("app_manifests")
+        if app_manifests:
+            first_app = app_manifests[0]
+            if not project_name and first_app.get("app"):
+                project_name = first_app.get("app")
+            cpg_path = first_app.get("cpg")
+            res = await dir_exists(connection, cpg_path)
+            if not res:
+                raise ValueError(
+                    f"CPG {cpg_path} doesn't exist for import into Joern. Check if the directory containing this CPG is mounted and accessible from the server."
+                )
+            return await import_cpg(connection, cpg_path, project_name)
+    return False
+
+
+async def import_cpg(connection, cpg_path, project_name=None):
+    if cpg_path:
+        res = await dir_exists(connection, cpg_path)
+        if not res:
+            raise ValueError(
+                f"CPG {cpg_path} doesn't exist for import into Joern. Check if the directory containing this CPG is mounted and accessible from the server."
+            )
+    if project_name:
+        res = await client.q(
+            connection, f"""importCpg("{cpg_path}", "{project_name}")"""
+        )
+    else:
+        res = await client.q(connection, f"""importCpg("{cpg_path}")""")
+    if isinstance(res, str):
+        return False
+    if "The graph has been modified" in res.get("response", ""):
+        # Execute save command
+        await client.q(connection, "save")
+        return True
+    return False
+
+
 async def import_code(connection, directory, project_name=None):
-    if directory and project_name:
+    if directory:
         res = await dir_exists(connection, directory)
         if not res:
             raise ValueError(
                 f"Directory {directory} doesn't exist for import into Joern. Check if the directory is mounted and accessible from the server."
             )
+    if project_name:
         res = await client.q(
             connection, f"""importCode("{directory}", "{project_name}")"""
         )
     else:
         res = await client.q(connection, f"""importCode("{directory}")""")
     if isinstance(res, str):
         return False
```

### Comparing `joern_lib-0.6.4/pyproject.toml` & `joern_lib-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.6.4"
+version = "0.6.5"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
```

### Comparing `joern_lib-0.6.4/PKG-INFO` & `joern_lib-0.6.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.7,<3.11
@@ -71,15 +71,15 @@
 
 Execute single query
 
 ```
 from joern_lib import client, workspace
 from joern_lib.detectors import common as cpg
 
-connection = await client.get("http://localhost:9000", "admin", "admin")
+connection = await client.get("http://localhost:9000", "http://localhost:7072", "admin", "admin")
 
 # connection = await client.get("http://localhost:9000")
 
 res = await client.q(connection, "val a=1");
 
 # {'response': 'a: Int = 1\n'}
 ```
@@ -115,14 +115,26 @@
 Import code for analysis
 
 ```
 res = await workspace.import_code(connection, "/app", "NodeGoat")
 # True
 ```
 
+Import an existing CPG for analysis
+
+```
+res = await workspace.import_cpg(connection, "/app/sandbox/crAPI/cpg_out/crAPI-python-cpg.bin.zip", "crAPI-python")
+```
+
+Create a CPG with a remote cpggen server
+
+```
+res = await workspace.create_cpg(connection, "/app/sandbox/crAPI", out_dir="/app/sandbox/crAPI/cpg_out", languages="python", project_name="crAPI-python")
+```
+
 ### CPG core
 
 List files
 
 ```
 res = await cpg.list_files(connection)
 # list of files
```

