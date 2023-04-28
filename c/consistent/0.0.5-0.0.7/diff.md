# Comparing `tmp/consistent-0.0.5.tar.gz` & `tmp/consistent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistent-0.0.5.tar", last modified: Fri Apr 28 09:30:46 2023, max compression
+gzip compressed data, was "consistent-0.0.7.tar", last modified: Fri Apr 28 10:31:17 2023, max compression
```

## Comparing `consistent-0.0.5.tar` & `consistent-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.517675 consistent-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 09:30:32.000000 consistent-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-28 09:30:46.517675 consistent-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-28 09:30:32.000000 consistent-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.513675 consistent-0.0.5/consisTent/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.513675 consistent-0.0.5/consisTent/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/cache/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/cache/chroma_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.517675 consistent-0.0.5/consisTent/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/validators/base_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.517675 consistent-0.0.5/consisTent/validators/semantic_validators/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/validators/semantic_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/validators/semantic_validators/consistency_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/validators/semantic_validators/labels_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 09:30:32.000000 consistent-0.0.5/consisTent/validators/syntactic_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.517675 consistent-0.0.5/consistent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-28 09:30:46.000000 consistent-0.0.5/consistent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 09:30:46.000000 consistent-0.0.5/consistent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:30:46.000000 consistent-0.0.5/consistent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 09:30:46.000000 consistent-0.0.5/consistent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:30:46.000000 consistent-0.0.5/consistent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 09:30:32.000000 consistent-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:30:46.517675 consistent-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:46.517675 consistent-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-28 09:30:32.000000 consistent-0.0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 10:31:02.000000 consistent-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-28 10:31:17.105385 consistent-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-28 10:31:02.000000 consistent-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/cache/chroma_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/base_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/validators/semantic_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/semantic_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/semantic_validators/consistency_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/semantic_validators/labels_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/syntactic_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consistent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 10:31:02.000000 consistent-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:31:17.105385 consistent-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-28 10:31:02.000000 consistent-0.0.7/tests/test.py
```

### Comparing `consistent-0.0.5/LICENSE` & `consistent-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `consistent-0.0.5/PKG-INFO` & `consistent-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.5
+Version: 0.0.7
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,14 +32,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img align="center" src="./logo.png">
 
+[![tests](https://github.com/drorIvry/consisTent/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/drorIvry/consisTent/actions/workflows/pre-commit.yml)
+
+[![release](https://github.com/drorIvry/consisTent/actions/workflows/python-publish.yml/badge.svg)](https://github.com/drorIvry/consisTent/actions/workflows/python-publish.yml)
+
 consisTent is a full blows testing framework for prompts. The goal of consisTent is to create reproducible tests for LLM based applications regardless of the FM used.
 
 
 ## Installation
 
 ```sh
 pip install consistent
@@ -72,20 +76,38 @@
 This type of validators is used to assert the quality of the response with more "soft" parameters for example, check if something is factually correct, check for hallucinations, check for labels like "funny"/"interesting" etc... another type of semantic validator is the semantic consistency validator where you provide a seed of validated input and a threshold, and the test will assert the semantic distance of the new output from the seed cluster.
 
 **Semantic validators are used to assert the CONTENT of the response**
 
 ### example
 
 ```python
+import consisTent
+
 seed = [
-    'the cat sat on the mat',
-    'the feline layed on the carpet',
-    ...
+    "the cat sat on the mat",
+    "the feline layed on the carpet",
 ]
 
 
-consisTent.ConsistencyValidator().validate(
+consisTent.ConsistencyValidator(
+    seed_size=2,
+    consistency_threshold=0.5,
+).validate(
     seed=seed,
-    model_output='the dog sat on the mat',
+    model_output="the dog sat on the mat",
 )
+```
 
+### Label Test
+
+```python
+OPENAI_KEY = "XXXXXXXXXXXXXXX"
+
+consisTent.LabelsValidator(openai_key=OPENAI_KEY).validate(
+    labels=[
+        "funny",
+        "short",
+        "about rabbits",
+    ],
+    model_output="What do you call a rabbit that tells jokes? A funny bunny!",
+)
 ```
```

### Comparing `consistent-0.0.5/consisTent/cache/chroma_cache.py` & `consistent-0.0.7/consisTent/cache/chroma_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
             documents=[document],
         )
 
     def calculate_distance(
         self,
         query_text: str,
     ):
-        if len(self._cache_ids > self._size):
+        if len(self._cache_ids) > self._size:
             self.push_to_cache(query_text)
             return 0
 
         result = self._collection.query(
             query_texts=[query_text],
             n_results=len(
                 self._cache_ids,
             ),
         )
 
-        distances = result["distances"]
+        distances = result["distances"][0]
 
         return sum(distances) / len(distances)
```

### Comparing `consistent-0.0.5/consisTent/validators/semantic_validators/consistency_validator.py` & `consistent-0.0.7/consisTent/validators/semantic_validators/consistency_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.5/consisTent/validators/semantic_validators/labels_validator.py` & `consistent-0.0.7/consisTent/validators/semantic_validators/labels_validator.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,71 +16,71 @@
             temperature=0,
             openai_api_key=openai_key,
             max_tokens=1000,
         )
 
         response_schemas = [
             ResponseSchema(
-                name="criteria",
-                description="This is the input_criteria from the user",
+                name="label",
+                description="This is the input_label from the user",
             ),
             ResponseSchema(
                 name="passed",
-                description="This is the validation result of the input against this criteria",  # noqa E501
+                description="This is the validation boolean result of the input against this labels. values are true / false",  # noqa E501
             ),
             ResponseSchema(
                 name="match_score",
                 description="A score 0-100 of how close you think the match is between user input and your match",  # noqa E501
             ),
             ResponseSchema(
                 name="reason",
-                description="Why did the input failed / passed this criteria",
+                description="Why did the input failed / passed this labels",
             ),
         ]
 
         output_parser = StructuredOutputParser.from_response_schemas(response_schemas)
         format_instructions = output_parser.get_format_instructions()
 
         self._template = """
         you are an input validator.
-        given a set of criteria your goal is to decide
-        if the input matches the given criteria.
+        given a set of labels your goal is to decide
+        if the input matches the given labels.
 
         {format_instructions}
 
         Wrap your final output with closed and open brackets (a list of json objects)
 
-        CRITERIA:
-        {criteria}
+        labels:
+        {labels}
 
         INPUT:
         {user_input}
 
         YOUR RESPONSE:
             """
 
         self._prompt = ChatPromptTemplate(
             messages=[HumanMessagePromptTemplate.from_template(self._template)],
-            input_variables=["criteria", "user_input"],
+            input_variables=["labels", "user_input"],
             partial_variables={"format_instructions": format_instructions},
         )
 
     def validate(
         self,
-        criteria: List[str],
+        labels: List[str],
         model_output: str,
     ):
-        parsed_criteria = ", ".join(criteria)
+        parsed_labels = ", ".join(labels)
 
         _input = self._prompt.format_prompt(
-            criteria=parsed_criteria,
+            labels=parsed_labels,
             user_input=model_output,
         )
 
         output = self._model(_input.to_messages())
 
         structured_data = json.loads(output.content)
 
         for entry in structured_data:
             assert (
                 entry["passed"] is True
-            ), f"llm validation check validation failed on {entry['criteria']} for {entry['reason']}"  # noqa: E501
+            ), f"llm validation check validation failed on {entry['label']} for {entry['reason']}"  # noqa: E501
```

### Comparing `consistent-0.0.5/consisTent/validators/syntactic_validators.py` & `consistent-0.0.7/consisTent/validators/syntactic_validators.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.5/consistent.egg-info/PKG-INFO` & `consistent-0.0.7/consistent.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.5
+Version: 0.0.7
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,14 +32,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img align="center" src="./logo.png">
 
+[![tests](https://github.com/drorIvry/consisTent/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/drorIvry/consisTent/actions/workflows/pre-commit.yml)
+
+[![release](https://github.com/drorIvry/consisTent/actions/workflows/python-publish.yml/badge.svg)](https://github.com/drorIvry/consisTent/actions/workflows/python-publish.yml)
+
 consisTent is a full blows testing framework for prompts. The goal of consisTent is to create reproducible tests for LLM based applications regardless of the FM used.
 
 
 ## Installation
 
 ```sh
 pip install consistent
@@ -72,20 +76,38 @@
 This type of validators is used to assert the quality of the response with more "soft" parameters for example, check if something is factually correct, check for hallucinations, check for labels like "funny"/"interesting" etc... another type of semantic validator is the semantic consistency validator where you provide a seed of validated input and a threshold, and the test will assert the semantic distance of the new output from the seed cluster.
 
 **Semantic validators are used to assert the CONTENT of the response**
 
 ### example
 
 ```python
+import consisTent
+
 seed = [
-    'the cat sat on the mat',
-    'the feline layed on the carpet',
-    ...
+    "the cat sat on the mat",
+    "the feline layed on the carpet",
 ]
 
 
-consisTent.ConsistencyValidator().validate(
+consisTent.ConsistencyValidator(
+    seed_size=2,
+    consistency_threshold=0.5,
+).validate(
     seed=seed,
-    model_output='the dog sat on the mat',
+    model_output="the dog sat on the mat",
 )
+```
 
+### Label Test
+
+```python
+OPENAI_KEY = "XXXXXXXXXXXXXXX"
+
+consisTent.LabelsValidator(openai_key=OPENAI_KEY).validate(
+    labels=[
+        "funny",
+        "short",
+        "about rabbits",
+    ],
+    model_output="What do you call a rabbit that tells jokes? A funny bunny!",
+)
 ```
```

### Comparing `consistent-0.0.5/consistent.egg-info/SOURCES.txt` & `consistent-0.0.7/consistent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `consistent-0.0.5/pyproject.toml` & `consistent-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "consistent"
-version = "0.0.5"
+version = "0.0.7"
 description = "Make sure AI model outputs are consistent"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,15 +30,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "pre-commit", "pyflakes"]
 
 [project.urls]
 Homepage = "https://github.com/drorivry/consistent"
 
 
 [tool.bumpver]
-current_version = "0.0.5"
+current_version = "0.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

