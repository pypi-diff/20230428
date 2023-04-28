# Comparing `tmp/one-api-tool-0.2.5.tar.gz` & `tmp/one-api-tool-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.5.tar", last modified: Thu Apr 27 12:38:59 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.6.tar", last modified: Fri Apr 28 08:38:58 2023, max compression
```

## Comparing `one-api-tool-0.2.5.tar` & `one-api-tool-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:38:59.441331 one-api-tool-0.2.5/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.5/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 12:38:59.441116 one-api-tool-0.2.5/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.5/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:38:59.437417 one-api-tool-0.2.5/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-27 12:38:59.000000 one-api-tool-0.2.5/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      609 2023-04-27 12:38:59.000000 one-api-tool-0.2.5/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-27 12:38:59.000000 one-api-tool-0.2.5/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-27 12:38:59.000000 one-api-tool-0.2.5/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-04-27 12:38:59.000000 one-api-tool-0.2.5/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-27 12:38:59.000000 one-api-tool-0.2.5/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:38:59.438238 one-api-tool-0.2.5/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.5/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:38:59.439370 one-api-tool-0.2.5/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.5/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2492 2023-04-27 09:10:04.000000 one-api-tool-0.2.5/oneapi/commands/one_api_eval_file.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2206 2023-04-27 10:07:56.000000 one-api-tool-0.2.5/oneapi/commands/one_api_eval_one.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.5/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6750 2023-04-27 12:30:38.000000 one-api-tool-0.2.5/oneapi/one_ai_eval.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.5/oneapi/one_api.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:38:59.440257 one-api-tool-0.2.5/oneapi/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-27 09:08:42.000000 one-api-tool-0.2.5/oneapi/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      858 2023-04-27 11:27:56.000000 one-api-tool-0.2.5/oneapi/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     5651 2023-04-27 12:02:51.000000 one-api-tool-0.2.5/oneapi/prompt_template/prompter.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-27 12:38:59.440785 one-api-tool-0.2.5/oneapi/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-27 02:46:39.000000 one-api-tool-0.2.5/oneapi/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2819 2023-04-27 11:59:07.000000 one-api-tool-0.2.5/oneapi/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-27 12:38:59.441417 one-api-tool-0.2.5/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1334 2023-04-27 12:33:52.000000 one-api-tool-0.2.5/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.173565 one-api-tool-0.2.6/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.6/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:38:58.173412 one-api-tool-0.2.6/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1742 2023-04-27 13:04:23.000000 one-api-tool-0.2.6/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.171953 one-api-tool-0.2.6/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.172478 one-api-tool-0.2.6/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.6/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.172920 one-api-tool-0.2.6/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.6/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.6/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.6/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-28 08:38:58.173608 one-api-tool-0.2.6/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1031 2023-04-28 08:34:25.000000 one-api-tool-0.2.6/setup.py
```

### Comparing `one-api-tool-0.2.5/LICENSE` & `one-api-tool-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.5/PKG-INFO` & `one-api-tool-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.5
+Version: 0.2.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OneAPI
-Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+Use a single line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
+
 ## Usage
 ### 1. (Recommended method) Set your key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
@@ -27,37 +29,37 @@
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Change to your Azure OpenAI resource's endpoint value.",
+    "api": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
-Antropic config:
+Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
-`api_key` OpenAI API key is availalle on the [website](https://platform.openai.com/account/api-keys), Clade API key here [website](https://console.anthropic.com/account/keys)
+`api_key`: Obtain your OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and your Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
+`api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
-`api_type` Currently supported: "open_ai", "azure" or "claude".
+`api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from a local configuration file.:
+Initialize the `OneAPITool` object from a local configuration file:
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
-### 2. (Not recommended) Writing the configuration directly into the code
+
+### 2. (Not recommended) Write the configuration directly into the code
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
 print(res)
-```
```

### Comparing `one-api-tool-0.2.5/README.md` & `one-api-tool-0.2.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # OneAPI
-Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+Use a single line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
+
 ## Usage
 ### 1. (Recommended method) Set your key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
@@ -15,37 +17,37 @@
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Change to your Azure OpenAI resource's endpoint value.",
+    "api": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
-Antropic config:
+Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
-`api_key` OpenAI API key is availalle on the [website](https://platform.openai.com/account/api-keys), Clade API key here [website](https://console.anthropic.com/account/keys)
+`api_key`: Obtain your OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and your Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
+`api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
-`api_type` Currently supported: "open_ai", "azure" or "claude".
+`api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from a local configuration file.:
+Initialize the `OneAPITool` object from a local configuration file:
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
-### 2. (Not recommended) Writing the configuration directly into the code
+
+### 2. (Not recommended) Write the configuration directly into the code
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
-print(res)
-```
+print(res)
```

### Comparing `one-api-tool-0.2.5/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.6/one_api_tool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.5
+Version: 0.2.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OneAPI
-Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+Use a single line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
+
 ## Usage
 ### 1. (Recommended method) Set your key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
@@ -27,37 +29,37 @@
     "api_type": "open_ai"
 }
 ```
 Azure OpenAI config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
-    "api": "Change to your Azure OpenAI resource's endpoint value.",
+    "api": "Replace with your Azure OpenAI resource's endpoint value.",
     "api_type": "azure"
 }
 ```
-Antropic config:
+Anthropic config:
 ```json
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
-`api_key` OpenAI API key is availalle on the [website](https://platform.openai.com/account/api-keys), Clade API key here [website](https://console.anthropic.com/account/keys)
+`api_key`: Obtain your OpenAI API key from the [OpenAI website](https://platform.openai.com/account/api-keys) and your Claude API key from the [Anthropic website](https://console.anthropic.com/account/keys).
 
-`api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
+`api`: The base API used to send requests. You may also specify a proxy URL like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard. The API format is usually: `https://{your_organization}.openai.azure.com/`.
 
-`api_type` Currently supported: "open_ai", "azure" or "claude".
+`api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
-Initialize the `OneAPITool` object from a local configuration file.:
+Initialize the `OneAPITool` object from a local configuration file:
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
-### 2. (Not recommended) Writing the configuration directly into the code
+
+### 2. (Not recommended) Write the configuration directly into the code
 ```python
 from oneapi import OneAPITool
 res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
 print(res)
-```
```

### Comparing `one-api-tool-0.2.5/oneapi/commands/one_api_eval_file.py` & `one-api-tool-0.2.6/oneapi/commands/one_api_requst.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-import os
 import sys
+import os
 import argparse
-sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/../../"))
-from oneapi.one_ai_eval import eval_one_file, EvalConfig
-from oneapi import prompt_template
-def main():
-    parser = argparse.ArgumentParser(description="one-eval-file [<args>]")
-    parser.add_argument("-c", "--config_file", type=str, help="config file path", required=True)
-    parser.add_argument("-tp", "--template_path",type=str, default=None, help="eval prompt template path", required=False)
-    parser.add_argument("-ep", "--eval_data_path",type=str, help="", required=True)
-    parser.add_argument("-op", "--output_path",type=str, default="", help="", required=False)
-    parser.add_argument("-m", "--model",type=str, default="", help="eval_model_name", required=False)
-    parser.add_argument("-ec", "--eval_categories", default=None, nargs="+",help="only evaluate chosen categories", required=False)
-    parser.add_argument("-sn", "--sample_num", type=int, default=0, help="", required=False)
-    parser.add_argument("-i", "--interval",type=int, default=1, help="request interval, gpt-4 need longer interval, e.g.,10s", required=False)
-    parser.add_argument("-r", "--retry",type=bool, default=True, help="", required=False)
-    parser.add_argument("-d", "--verbose",type=bool, default=True, help="print every prompt and response detail", required=False)
-    parser.add_argument("-tt", "--temperature",type=float, default=0.1, help="0-1, higher temperature more random result", required=False)
-    parser.add_argument("-mnt", "--max_new_tokens",type=int, default=2048, help="max output token length", required=False)
 
+sys.path.append(
+    os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/../../"))
+from oneapi import OneAPITool
+
+
+def main():
+    parser = argparse.ArgumentParser(description="one-api [<args>]")
+    parser.add_argument("-c",
+                        "--config_file",
+                        type=str,
+                        help="config file path",
+                        required=True)
+    parser.add_argument("-p",
+                        "--prompt",
+                        type=str,
+                        help="question",
+                        required=True)
+    parser.add_argument("-m",
+                        "--model",
+                        type=str,
+                        default="",
+                        help="evaluate model name, e.g., gpt-35-turbo, gpt-4",
+                        required=False)
+    parser.add_argument("-tt",
+                        "--temperature",
+                        type=float,
+                        default=0.1,
+                        help="0-1, higher temperature more random result",
+                        required=False)
+    parser.add_argument("-mnt",
+                        "--max_new_tokens",
+                        type=int,
+                        default=2048,
+                        help="max output token length",
+                        required=False)
     args = parser.parse_args()
-    if not args.template_path:
-        template_path =  os.path.join(os.path.dirname(prompt_template.__file__), 'eval_prompt_template.json')
-    else:
-        template_path = args.template_path
-    eval_prompter = prompt_template.EvalPrompt.from_config(template_path, verbose=args.verbose)
-    eval_one_file(
-        EvalConfig(
-        eval_prompter=eval_prompter,
-        api_config_file=args.config_file, 
-        eval_data_path=args.eval_data_path, 
-        output_path=args.output_path, 
+    tool = OneAPITool.from_config_file(args.config_file)
+    print(
+        f"\n{'-'*20} prompt detail 🚀  {'-'*20}\n\n{args.prompt}\n\n{'-'*20} prompt end {'-'*20}"
+    )
+    response = tool.simple_chat(
+        prompt=args.prompt,
         model=args.model,
-        eval_categories=args.eval_categories,
-        sample_num=args.sample_num, 
-        request_interval=args.interval,
-        retry=args.retry,
         temperature=args.temperature,
         max_new_tokens=args.max_new_tokens,
-        ))
-    
+    )
+    print(
+        f"{'-'*20} {args.model} response ⭐️ {'-'*20}\n\n{response}\n\n{'-'*20} response end {'-'*20}\n\n"
+    )
+
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `one-api-tool-0.2.5/oneapi/one_api.py` & `one-api-tool-0.2.6/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.5/setup.py` & `one-api-tool-0.2.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(),
-    package_data={
-      "oneapi":["prompt_template/eval_prompt_template.json"]  
-    },
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
         "httpx",
         "aiohttp",
         "tokenizers",
-        "pandas",
-        "openpyxl",
-        "tabulate",
-        "XlsxWriter"
     ],
     entry_points={
         "console_scripts": [
-            "one-eval-file=oneapi.commands.one_api_eval_file:main",
-            "one-eval-line=oneapi.commands.one_api_eval_one:main",
             "one-api=oneapi.commands.one_api_requst:main"
         ]
     },
     description="Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/muximus3/OneAPI",
```

