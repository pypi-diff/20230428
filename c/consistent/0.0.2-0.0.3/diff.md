# Comparing `tmp/consistent-0.0.2.tar.gz` & `tmp/consistent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistent-0.0.2.tar", last modified: Sat Apr 22 10:39:30 2023, max compression
+gzip compressed data, was "consistent-0.0.3.tar", last modified: Fri Apr 28 08:57:13 2023, max compression
```

## Comparing `consistent-0.0.2.tar` & `consistent-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.032233 consistent-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-22 10:39:18.000000 consistent-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 10:39:30.032233 consistent-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 10:39:18.000000 consistent-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/cache/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/cache/chroma_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/base_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.028232 consistent-0.0.2/consisTent/validators/semantic_validators/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/semantic_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/semantic_validators/consistency_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/semantic_validators/openai_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-22 10:39:18.000000 consistent-0.0.2/consisTent/validators/syntactic_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:39:30.032233 consistent-0.0.2/consistent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 10:39:30.000000 consistent-0.0.2/consistent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-22 10:39:18.000000 consistent-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 10:39:30.032233 consistent-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 08:57:01.000000 consistent-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 08:57:13.945818 consistent-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 08:57:01.000000 consistent-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.941818 consistent-0.0.3/consisTent/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consisTent/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/cache/chroma_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consisTent/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/base_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consisTent/validators/semantic_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/semantic_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/semantic_validators/consistency_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/semantic_validators/labels_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/syntactic_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consistent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 08:57:01.000000 consistent-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:57:13.945818 consistent-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 08:57:01.000000 consistent-0.0.3/tests/test.py
```

### Comparing `consistent-0.0.2/LICENSE` & `consistent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `consistent-0.0.2/PKG-INFO` & `consistent-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.2
+Version: 0.0.3
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,8 +30,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# consisTent
+<img align="center" src="./logo.png">
+
+consisTent is a full blows testing framework for prompts. The goal of consisTent is to create reproducible tests for LLM based applications regardless of the FM used.
+
+
+## Installation
+
+```sh
+pip install consistent
+```
+
+## Concepts
+
+consisTent comes with 2 types of validators (testers)
```

### Comparing `consistent-0.0.2/consisTent/cache/chroma_cache.py` & `consistent-0.0.3/consisTent/cache/chroma_cache.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.2/consisTent/validators/semantic_validators/consistency_validator.py` & `consistent-0.0.3/consisTent/validators/semantic_validators/consistency_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.2/consisTent/validators/semantic_validators/openai_validator.py` & `consistent-0.0.3/consisTent/validators/semantic_validators/labels_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from langchain.output_parsers import StructuredOutputParser, ResponseSchema
 from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain.chat_models import ChatOpenAI
 
 from ..base_validator import Validator
 
 
-class OpenAIValidator(Validator):
+class LabelsValidator(Validator):
     def __init__(
         self,
         openai_key: str,
     ):
         self._model = ChatOpenAI(
             temperature=0,
             openai_api_key=openai_key,
```

### Comparing `consistent-0.0.2/consisTent/validators/syntactic_validators.py` & `consistent-0.0.3/consisTent/validators/syntactic_validators.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.2/consistent.egg-info/PKG-INFO` & `consistent-0.0.3/consistent.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.2
+Version: 0.0.3
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,8 +30,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# consisTent
+<img align="center" src="./logo.png">
+
+consisTent is a full blows testing framework for prompts. The goal of consisTent is to create reproducible tests for LLM based applications regardless of the FM used.
+
+
+## Installation
+
+```sh
+pip install consistent
+```
+
+## Concepts
+
+consisTent comes with 2 types of validators (testers)
```

### Comparing `consistent-0.0.2/consistent.egg-info/SOURCES.txt` & `consistent-0.0.3/consistent.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 consisTent/cache/base_cache.py
 consisTent/cache/chroma_cache.py
 consisTent/validators/__init__.py
 consisTent/validators/base_validator.py
 consisTent/validators/syntactic_validators.py
 consisTent/validators/semantic_validators/__init__.py
 consisTent/validators/semantic_validators/consistency_validator.py
-consisTent/validators/semantic_validators/openai_validator.py
+consisTent/validators/semantic_validators/labels_validator.py
 consistent.egg-info/PKG-INFO
 consistent.egg-info/SOURCES.txt
 consistent.egg-info/dependency_links.txt
 consistent.egg-info/requires.txt
-consistent.egg-info/top_level.txt
+consistent.egg-info/top_level.txt
+tests/test.py
```

### Comparing `consistent-0.0.2/pyproject.toml` & `consistent-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,43 +2,45 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "consistent"
-version = "0.0.2"
+version = "0.0.3"
 description = "Make sure AI model outputs are consistent"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["OpenAI", "LLM", "GPT", "Cohere"]
 dependencies = [
     "chromadb",
     "openai",
+    "js2py",
+    "jsonschema",
     "langchain",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "pre-commit", "pyflakes"]
 
 [project.urls]
 Homepage = "https://github.com/drorivry/consistent"
 
 
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"consistent/__init__.py" = ["{version}"]
+"consisTent/__init__.py" = ["{version}"]
```

