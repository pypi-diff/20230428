# Comparing `tmp/pydantic_chatcompletion-0.0.1.tar.gz` & `tmp/pydantic_chatcompletion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_chatcompletion-0.0.1.tar", last modified: Fri Apr 28 01:51:53 2023, max compression
+gzip compressed data, was "pydantic_chatcompletion-0.0.2.tar", last modified: Fri Apr 28 18:49:25 2023, max compression
```

## Comparing `pydantic_chatcompletion-0.0.1.tar` & `pydantic_chatcompletion-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 01:51:53.154406 pydantic_chatcompletion-0.0.1/
--rw-r--r--   0 wsk        (501) staff       (20)      730 2023-04-28 01:51:53.154143 pydantic_chatcompletion-0.0.1/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 01:51:53.152471 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion/
--rw-r--r--   0 wsk        (501) staff       (20)     1987 2023-04-28 01:08:41.000000 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion/__init__.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 01:51:53.153829 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      730 2023-04-28 01:51:53.000000 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      284 2023-04-28 01:51:53.000000 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-28 01:51:53.000000 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       16 2023-04-28 01:51:53.000000 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       24 2023-04-28 01:51:53.000000 pydantic_chatcompletion-0.0.1/pydantic_chatcompletion.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      866 2023-04-28 01:07:38.000000 pydantic_chatcompletion-0.0.1/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-28 01:51:53.154477 pydantic_chatcompletion-0.0.1/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 18:49:25.280637 pydantic_chatcompletion-0.0.2/
+-rw-r--r--   0 wsk        (501) staff       (20)     4158 2023-04-28 18:49:25.280357 pydantic_chatcompletion-0.0.2/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     3427 2023-04-28 14:53:00.000000 pydantic_chatcompletion-0.0.2/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 18:49:25.278560 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion/
+-rw-r--r--   0 wsk        (501) staff       (20)     1946 2023-04-28 18:47:15.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion/__init__.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 18:49:25.280005 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     4158 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      294 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       16 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       24 2023-04-28 18:49:25.000000 pydantic_chatcompletion-0.0.2/pydantic_chatcompletion.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      866 2023-04-28 18:40:28.000000 pydantic_chatcompletion-0.0.2/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-28 18:49:25.280727 pydantic_chatcompletion-0.0.2/setup.cfg
```

### Comparing `pydantic_chatcompletion-0.0.1/pydantic_chatcompletion/__init__.py` & `pydantic_chatcompletion-0.0.2/pydantic_chatcompletion/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Wrapper around OpenAI ChatCompletion that compels the language model to produce a valid Pydantic model as output via prompting and iterative error remediation.  The easiest way to go from unstructured text to structured Pydantic data.
 
-A wrapper around openai.ChatCompletion.Create that prompts the model to produce a completion data in the form of a supplied pydantic model.  It uses the pydantic json_schema to help guide the model to the required output format.
+It uses the pydantic json_schema to help guide the model to the required output format.
 
 It will retry the task with error messages if the model does not produce appropriate output data due to either a json load issue or a pydantic validation issue.
 
 """
 
 import logging
 from pydantic import BaseModel, ValidationError
@@ -15,28 +15,30 @@
 
 
 def create(messages : List[dict], model_class: BaseModel, retry=2, temperature=0, **kwargs) -> BaseModel:
 
     messages.append({"role"   : "system",
                      "content": f"Please respond ONLY with valid json that conforms to this pydantic json_schema: {model_class.schema_json()}. Do not include additional text other than the object json as we will load this object with json.loads() and pydantic."})
 
-
+    last_exception = None
     for i in range(retry+1):
         response = openai.ChatCompletion.create(messages=messages, temperature=temperature, **kwargs)
         content = response['choices'][0]['message']['content']
         try:
             json_content = json.loads(content)
         except Exception as e:
+            last_exception = e
             error_msg = f"json.loads exception: {e}"
             logging.error(error_msg)
             messages.append({"role"   : "system",
                             "content": error_msg})
             continue
         try:
             return model_class(**json_content)
         except ValidationError as e:
+            last_exception = e
             error_msg = f"pydantic exception: {e}"
             logging.error(error_msg)
             messages.append({"role"   : "system",
                             "content": error_msg})    
-    raise e
+    raise last_exception
```

### Comparing `pydantic_chatcompletion-0.0.1/pyproject.toml` & `pydantic_chatcompletion-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydantic_chatcompletion"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['openai', 'pydantic']
 description = "Wrapper around OpenAI ChatCompletion that compels the language model to produce a valid Pydantic model as output via prompting and iterative error remediation.  The easiest way to go from unstructured text to structured Pydantic data."
 readme = "README.md"
 requires-python = ">=3.9"
```

