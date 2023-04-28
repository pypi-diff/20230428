# Comparing `tmp/one-api-tool-0.2.6.tar.gz` & `tmp/one-api-tool-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.6.tar", last modified: Fri Apr 28 08:38:58 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.7.tar", last modified: Fri Apr 28 08:45:55 2023, max compression
```

## Comparing `one-api-tool-0.2.6.tar` & `one-api-tool-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.173565 one-api-tool-0.2.6/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.6/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:38:58.173412 one-api-tool-0.2.6/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1742 2023-04-27 13:04:23.000000 one-api-tool-0.2.6/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.171953 one-api-tool-0.2.6/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-28 08:38:58.000000 one-api-tool-0.2.6/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.172478 one-api-tool-0.2.6/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.6/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:38:58.172920 one-api-tool-0.2.6/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.6/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.6/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.6/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-28 08:38:58.173608 one-api-tool-0.2.6/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1031 2023-04-28 08:34:25.000000 one-api-tool-0.2.6/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.401738 one-api-tool-0.2.7/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.7/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:45:55.401589 one-api-tool-0.2.7/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1742 2023-04-27 13:04:23.000000 one-api-tool-0.2.7/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.400317 one-api-tool-0.2.7/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2298 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-28 08:45:55.000000 one-api-tool-0.2.7/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.400718 one-api-tool-0.2.7/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.2.7/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:45:55.401205 one-api-tool-0.2.7/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.7/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-04-27 08:57:27.000000 one-api-tool-0.2.7/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9512 2023-04-26 11:27:45.000000 one-api-tool-0.2.7/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-28 08:45:55.401787 one-api-tool-0.2.7/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1031 2023-04-28 08:45:48.000000 one-api-tool-0.2.7/setup.py
```

### Comparing `one-api-tool-0.2.6/LICENSE` & `one-api-tool-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.6/PKG-INFO` & `one-api-tool-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.6
+Version: 0.2.7
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.6/README.md` & `one-api-tool-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.6/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.7/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.6
+Version: 0.2.7
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.6/oneapi/commands/one_api_requst.py` & `one-api-tool-0.2.7/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.6/oneapi/one_api.py` & `one-api-tool-0.2.7/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.6/setup.py` & `one-api-tool-0.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.6",
+    version="0.2.7",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

