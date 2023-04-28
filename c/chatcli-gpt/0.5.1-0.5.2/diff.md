# Comparing `tmp/chatcli_gpt-0.5.1.tar.gz` & `tmp/chatcli_gpt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcli_gpt-0.5.1.tar", max compression
+gzip compressed data, was "chatcli_gpt-0.5.2.tar", max compression
```

## Comparing `chatcli_gpt-0.5.1.tar` & `chatcli_gpt-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.5.1/LICENSE
--rw-r--r--   0        0        0     3497 2023-04-26 14:21:31.185327 chatcli_gpt-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.5.1/chatcli_gpt/__init__.py
--rw-r--r--   0        0        0       30 2023-04-15 05:23:10.942580 chatcli_gpt-0.5.1/chatcli_gpt/__main__.py
--rw-r--r--   0        0        0    13883 2023-04-26 14:53:43.773831 chatcli_gpt-0.5.1/chatcli_gpt/cli.py
--rw-r--r--   0        0        0     3380 2023-04-25 15:59:19.286886 chatcli_gpt-0.5.1/chatcli_gpt/conversation.py
--rw-r--r--   0        0        0     8092 2023-04-26 15:08:09.711600 chatcli_gpt-0.5.1/chatcli_gpt/log.py
--rw-r--r--   0        0        0     4638 2023-04-26 13:47:15.250569 chatcli_gpt-0.5.1/chatcli_gpt/plugins.py
--rw-r--r--   0        0        0     1328 2023-04-26 15:10:50.708465 chatcli_gpt-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 chatcli_gpt-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3497 2023-04-26 14:21:31.185327 chatcli_gpt-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.5.2/chatcli_gpt/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-15 05:23:10.942580 chatcli_gpt-0.5.2/chatcli_gpt/__main__.py
+-rw-r--r--   0        0        0    13883 2023-04-28 15:52:31.592839 chatcli_gpt-0.5.2/chatcli_gpt/cli.py
+-rw-r--r--   0        0        0     3380 2023-04-25 15:59:19.286886 chatcli_gpt-0.5.2/chatcli_gpt/conversation.py
+-rw-r--r--   0        0        0     3878 2023-04-28 16:06:47.437825 chatcli_gpt-0.5.2/chatcli_gpt/data/default_log
+-rw-r--r--   0        0        0     4350 2023-04-28 15:48:27.290508 chatcli_gpt-0.5.2/chatcli_gpt/log.py
+-rw-r--r--   0        0        0     4785 2023-04-28 15:48:22.850466 chatcli_gpt-0.5.2/chatcli_gpt/plugins.py
+-rw-r--r--   0        0        0     1328 2023-04-28 15:48:27.290508 chatcli_gpt-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 chatcli_gpt-0.5.2/PKG-INFO
```

### Comparing `chatcli_gpt-0.5.1/LICENSE` & `chatcli_gpt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.5.1/README.md` & `chatcli_gpt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.5.1/chatcli_gpt/cli.py` & `chatcli_gpt-0.5.2/chatcli_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.5.1/chatcli_gpt/conversation.py` & `chatcli_gpt-0.5.2/chatcli_gpt/conversation.py`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.5.1/chatcli_gpt/plugins.py` & `chatcli_gpt-0.5.2/chatcli_gpt/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import json
 import subprocess
 from pathlib import Path
 import duckduckgo_search
 import wolframalpha
 import requests
 import openai
+import prompt_toolkit
 
 
 BLOCK_PATTERNS = {
     "bash": r"EVALUATE:\n+```(?:bash)?\n(.*?)```",
     "pyeval": r"EVALUATE:\n+```(?:python)?\n(.*?)```",
     "search": r"SEARCH\((.*)\)",
     "wolfram": r"WOLFRAM\((.*)\)",
@@ -131,9 +132,10 @@
         output_blocks.append(f"RESULT:\n```\n{output['result']}\n```")
     if output.get("error"):
         output_blocks.append(f"ERROR:\n```\n{output['error']}\n```")
     return "\n".join(output_blocks)
 
 
 if __name__ == "__main__":
-    input_text = sys.stdin.read()
+    print("(Finish input with <Alt-Enter> or <Esc><Enter>)")
+    input_text = prompt_toolkit.prompt(multiline=True, prompt=">>> ", continuation_prompt="... ")
     print(evaluate_plugins(input_text, sys.argv[1:]))
```

### Comparing `chatcli_gpt-0.5.1/pyproject.toml` & `chatcli_gpt-0.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatcli-gpt"
-version = "0.5.1"
+version = "0.5.2"
 description = "A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations."
 readme = "README.md"
 license = "MIT"
 authors = ["Adam Kelly <adam@cthulahoops.org>"]
 repository = "https://github.com/cthulahoops/chatcli"
 
 [tool.poetry.dependencies]
```

### Comparing `chatcli_gpt-0.5.1/PKG-INFO` & `chatcli_gpt-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcli-gpt
-Version: 0.5.1
+Version: 0.5.2
 Summary: A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations.
 Home-page: https://github.com/cthulahoops/chatcli
 License: MIT
 Author: Adam Kelly
 Author-email: adam@cthulahoops.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

