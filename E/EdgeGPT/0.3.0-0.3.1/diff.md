# Comparing `tmp/EdgeGPT-0.3.0.tar.gz` & `tmp/EdgeGPT-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.0.tar", last modified: Sun Apr 23 16:47:14 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.1.tar", last modified: Fri Apr 28 13:59:43 2023, max compression
```

## Comparing `EdgeGPT-0.3.0.tar` & `EdgeGPT-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:47:14.004706 EdgeGPT-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:47:14.008706 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-23 16:47:14.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 16:47:13.000000 EdgeGPT-0.3.0/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-23 16:46:44.000000 EdgeGPT-0.3.0/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-28 13:59:42.000000 EdgeGPT-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:43.081182 EdgeGPT-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.0/LICENSE` & `EdgeGPT-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.0/PKG-INFO` & `EdgeGPT-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.0/README.md` & `EdgeGPT-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.0/setup.py` & `EdgeGPT-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.0",
+    version="0.3.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.0/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.1/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.0/src/EdgeGPT.py` & `EdgeGPT-0.3.1/src/EdgeGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
 from typing import Literal
 from typing import Optional
 from typing import Union
-from BingImageCreator import ImageGenAsync
+
 import certifi
 import httpx
 import websockets.client as websockets
+from BingImageCreator import ImageGenAsync
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.live import Live
 from rich.markdown import Markdown
@@ -91,66 +92,74 @@
 
 class NotAllowedToAccess(Exception):
     pass
 
 
 class ConversationStyle(Enum):
     creative = [
-                "nlu_direct_response_filter",
-                "deepleo",
-                "disable_emoji_spoken_text",
-                "responsible_ai_policy_235",
-                "enablemm",
-                "h3imaginative","travelansgnd","dv3sugg","clgalileo","gencontentv3",
-                "dv3sugg",
-                "responseos",
-                "e2ecachewrite",
-                "cachewriteext",
-                "nodlcpcwrite",
-                "travelansgnd"
-            ]
+        "nlu_direct_response_filter",
+        "deepleo",
+        "disable_emoji_spoken_text",
+        "responsible_ai_policy_235",
+        "enablemm",
+        "h3imaginative",
+        "travelansgnd",
+        "dv3sugg",
+        "clgalileo",
+        "gencontentv3",
+        "dv3sugg",
+        "responseos",
+        "e2ecachewrite",
+        "cachewriteext",
+        "nodlcpcwrite",
+        "travelansgnd",
+    ]
     balanced = [
-                "nlu_direct_response_filter",
-                "deepleo",
-                "disable_emoji_spoken_text",
-                "responsible_ai_policy_235",
-                "enablemm",
-                "galileo",
-                "dv3sugg",
-                "responseos",
-                "e2ecachewrite",
-                "cachewriteext",
-                "nodlcpcwrite",
-                "travelansgnd"
-            ]
-    precise = ["nlu_direct_response_filter",
-                "deepleo",
-                "disable_emoji_spoken_text",
-                "responsible_ai_policy_235",
-                "enablemm",
-                "galileo",
-                "dv3sugg",
-                "responseos",
-                "e2ecachewrite",
-                "cachewriteext",
-                "nodlcpcwrite",
-                "travelansgnd","h3precise","clgalileo"]
+        "nlu_direct_response_filter",
+        "deepleo",
+        "disable_emoji_spoken_text",
+        "responsible_ai_policy_235",
+        "enablemm",
+        "galileo",
+        "dv3sugg",
+        "responseos",
+        "e2ecachewrite",
+        "cachewriteext",
+        "nodlcpcwrite",
+        "travelansgnd",
+    ]
+    precise = [
+        "nlu_direct_response_filter",
+        "deepleo",
+        "disable_emoji_spoken_text",
+        "responsible_ai_policy_235",
+        "enablemm",
+        "galileo",
+        "dv3sugg",
+        "responseos",
+        "e2ecachewrite",
+        "cachewriteext",
+        "nodlcpcwrite",
+        "travelansgnd",
+        "h3precise",
+        "clgalileo",
+    ]
 
 
 CONVERSATION_STYLE_TYPE = Optional[
     Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
 
 def _append_identifier(msg: dict) -> str:
     """
     Appends special character to end of message to identify end of message
     """
     # Convert dict to json string
-    return json.dumps(msg) + DELIMITER
+    return json.dumps(msg, ensure_ascii=False) + DELIMITER
 
 
 def _get_ran_hex(length: int = 32) -> str:
     """
     Returns random hex string
     """
     return "".join(random.choice("0123456789abcdef") for _ in range(length))
@@ -206,15 +215,15 @@
                         "InternalSearchResult",
                         "Disengaged",
                         "InternalLoaderMessage",
                         "RenderCardRequest",
                         "AdsQuery",
                         "SemanticSerp",
                         "GenerateContentQuery",
-                        "SearchQuery"
+                        "SearchQuery",
                     ],
                     "sliceIds": [
                         "chk1cf",
                         "nopreloadsscf",
                         "winlongmsg2tf",
                         "perfimpcomb",
                         "sugdivdis",
@@ -226,15 +235,15 @@
                         "scctl",
                         "330uaugs0",
                         "0329resp",
                         "udscahrfon",
                         "udstrblm5",
                         "404e2ewrt",
                         "408nodedups0",
-                        "403tvlansgnd"
+                        "403tvlansgnd",
                     ],
                     "traceId": _get_ran_hex(32),
                     "isStartOfSession": self.invocation_id == 0,
                     "message": {
                         "author": "user",
                         "inputMethod": "Keyboard",
                         "text": prompt,
@@ -370,32 +379,53 @@
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
                     try:
                         if not draw:
-                            resp_txt = response["arguments"][0]["messages"][0]["adaptiveCards"][
-                                0
-                            ]["body"][0].get("text")
+                            resp_txt = response["arguments"][0]["messages"][0][
+                                "adaptiveCards"
+                            ][0]["body"][0].get("text")
+                            if(resp_txt == None):
+                                resp_txt = ""
                         yield False, resp_txt
-                    except:
-                        draw = True
+                    except Exception as exc:
+                        print(exc)
+                        if not draw:
+                            continue
                         for item in cookies:
-                            if(item["name"] == "_U"):
+                            if item["name"] == "_U":
                                 U = item["value"]
                         async with ImageGenAsync(U, True) as image_generator:
-                            images = await image_generator.get_images(response["arguments"][0]["messages"][0]["text"])
+                            images = await image_generator.get_images(
+                                response["arguments"][0]["messages"][0]["text"],
+                            )
                         cache = resp_txt
-                        resp_txt = cache+"\n![image0]("+images[0]+")\n![image1]("+images[1]+")\n![image0]("+images[2]+")\n![image3]("+images[3]+")"
+                        resp_txt = (
+                            cache
+                            + "\n![image0]("
+                            + images[0]
+                            + ")\n![image1]("
+                            + images[1]
+                            + ")\n![image0]("
+                            + images[2]
+                            + ")\n![image3]("
+                            + images[3]
+                            + ")"
+                        )
                         yield False, resp_txt
                 elif response.get("type") == 2:
                     if draw:
-                        cache = response["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
-                        response["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"] = cache+resp_txt
+                        cache = response["item"]["messages"][1]["adaptiveCards"][0][
+                            "body"
+                        ][0]["text"]
+                        response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
+                            "text"
+                        ] = (cache + resp_txt)
                     final = True
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.recv()
 
@@ -444,15 +474,15 @@
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
-            cookies=self.cookies
+            cookies=self.cookies,
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return None
 
     async def ask_stream(
@@ -468,15 +498,15 @@
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
-            cookies=self.cookies
+            cookies=self.cookies,
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
@@ -597,15 +627,18 @@
             else:
                 async for final, response in bot.ask_stream(
                     prompt=question,
                     conversation_style=args.style,
                     wss_link=args.wss_link,
                 ):
                     if not final:
-                        print(response[wrote:], end="", flush=True)
+                        if not wrote:
+                            print(response, end="", flush=True)
+                        else:
+                            print(response[wrote:], end="", flush=True)
                         wrote = len(response)
                 print()
     await bot.close()
 
 
 def main() -> None:
     print(
@@ -650,15 +683,15 @@
         "--prompt",
         type=str,
         default="",
         required=False,
         help="prompt to start with",
     )
     args = parser.parse_args()
-    if args.cookie_file == "":
+    if not args.cookie_file:
         parser.print_help()
         parser.exit(
             1,
             "ERROR: use --cookie-file or set the COOKIE_FILE environment variable",
         )
     try:
         args.cookies = json.loads(Path(args.cookie_file).read_text(encoding="utf-8"))
```

