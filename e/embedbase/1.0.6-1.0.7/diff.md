# Comparing `tmp/embedbase-1.0.6.tar.gz` & `tmp/embedbase-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.6.tar", max compression
+gzip compressed data, was "embedbase-1.0.7.tar", max compression
```

## Comparing `embedbase-1.0.6.tar` & `embedbase-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-28 08:45:19.347723 embedbase-1.0.6/LICENSE
--rw-r--r--   0        0        0     6124 2023-04-28 08:45:19.347723 embedbase-1.0.6/README.md
--rw-r--r--   0        0        0      121 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/__init__.py
--rw-r--r--   0        0        0     3447 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/api.py
--rw-r--r--   0        0        0    16193 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2463 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/base.py
--rw-r--r--   0        0        0     1164 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4823 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     8011 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4479 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/logging_utils.py
--rw-r--r--   0        0        0      661 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     2101 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/utils.py
--rw-r--r--   0        0        0     3585 2023-04-28 08:45:19.411726 embedbase-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     7605 1970-01-01 00:00:00.000000 embedbase-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-28 19:29:43.399867 embedbase-1.0.7/LICENSE
+-rw-r--r--   0        0        0     5952 2023-04-28 19:29:43.399867 embedbase-1.0.7/README.md
+-rw-r--r--   0        0        0      121 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/__init__.py
+-rw-r--r--   0        0        0     3447 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/api.py
+-rw-r--r--   0        0        0    16193 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2463 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/base.py
+-rw-r--r--   0        0        0     1164 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4823 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0      504 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/pinecone_db.py
+-rw-r--r--   0        0        0     8011 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4479 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0      411 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/weaviate_db.py
+-rw-r--r--   0        0        0       77 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      661 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-04-28 19:29:43.467867 embedbase-1.0.7/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-04-28 19:29:43.467867 embedbase-1.0.7/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     2101 2023-04-28 19:29:43.467867 embedbase-1.0.7/embedbase/utils.py
+-rw-r--r--   0        0        0     3584 2023-04-28 19:29:43.467867 embedbase-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7433 1970-01-01 00:00:00.000000 embedbase-1.0.7/PKG-INFO
```

### Comparing `embedbase-1.0.6/LICENSE` & `embedbase-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/README.md` & `embedbase-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 
 <p align="center">
 <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
   <h1 align="center">Embedbase</h1>
 
 
-<h3 align="center">Add memory to AI with embeddings</h3>
+<h3 align="center">Seamless data connections to LLMs</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
     <br />
     <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
       <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
     </a>
     <br />
     <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
       <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     </a>
-    <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
+    <p align="center">Open-source API & SDK to sync your data and easily hook them up to LLMs</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
@@ -45,23 +45,20 @@
 
 ## The 3 ways to use Embedbase
 
 - [Embedbase Cloud](#managed-instance): **Build embeddings-powered apps in minutes** | `npm i embedbase-js` | ⏱️ 3min
 - [Embedbase.py](#getting-started): **Choose your own db, embeddings models, and get started with a simple** | `pip install embedbase` | ⏱️ 5 min
 - [Embedbase self-hosted](https://docs.embedbase.xyz/tutorials/self-host-on-render): **Get Embedbase Cloud on your infra** | `docker-compose up` | ⏱️ 15 min
 
-## Examples
-
-Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
 
 ## What are people building
 
-- [Creating a recommendation engine: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
-- [Creating chat with your data experiences: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
-- [Creating a talk with your docs experience: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
+- [Recommendation Engines: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
+- [Chat with your data: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
+- [Talk to your docs: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
 
 ## Getting started
 
 Let's install Python dependencies:
 
 ```bash
 pip install embedbase sentence-transformers
```

### Comparing `embedbase-1.0.6/embedbase/__main__.py` & `embedbase-1.0.7/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/api.py` & `embedbase-1.0.7/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/app.py` & `embedbase-1.0.7/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/database/base.py` & `embedbase-1.0.7/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/database/db_utils.py` & `embedbase-1.0.7/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/database/memory_db.py` & `embedbase-1.0.7/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/database/postgres_db.py` & `embedbase-1.0.7/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/database/supabase_db.py` & `embedbase-1.0.7/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/embedding/base.py` & `embedbase-1.0.7/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/embedding/cohere.py` & `embedbase-1.0.7/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/embedding/openai.py` & `embedbase-1.0.7/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/firebase_auth.py` & `embedbase-1.0.7/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/logging_utils.py` & `embedbase-1.0.7/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/models.py` & `embedbase-1.0.7/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/settings.py` & `embedbase-1.0.7/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/strings.py` & `embedbase-1.0.7/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/embedbase/utils.py` & `embedbase-1.0.7/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.6/pyproject.toml` & `embedbase-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.6"
+version = "1.0.7"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
-
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
@@ -28,15 +27,15 @@
 [tool.poetry.scripts]
 # Entry points for the package
 "embedbase" = "embedbase.__main__:run_app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-fastapi = "^0.70.0"
+fastapi = "^0.95.1"
 uvicorn = {extras = ["standard"], version = "^0.15.0"}
 pandas = "^1.3.4"
 openai = "^0.27.0"
 tenacity = "^8.0.1"
 gunicorn = "^20.1.0"
 pydantic_yaml = {extras = ["pyyaml"], version = "^0.4.0"}
 tiktoken = "^0.3.3"
```

### Comparing `embedbase-1.0.6/PKG-INFO` & `embedbase-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.6
+Version: 1.0.7
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: fastapi (>=0.70.0,<0.71.0)
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic_yaml[pyyaml] (>=0.4.0,<0.5.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn[standard] (>=0.15.0,<0.16.0)
@@ -36,29 +36,29 @@
 
 
 <p align="center">
 <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
   <h1 align="center">Embedbase</h1>
 
 
-<h3 align="center">Add memory to AI with embeddings</h3>
+<h3 align="center">Seamless data connections to LLMs</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
     <br />
     <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
       <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
     </a>
     <br />
     <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
       <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     </a>
-    <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
+    <p align="center">Open-source API & SDK to sync your data and easily hook them up to LLMs</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
@@ -79,23 +79,20 @@
 
 ## The 3 ways to use Embedbase
 
 - [Embedbase Cloud](#managed-instance): **Build embeddings-powered apps in minutes** | `npm i embedbase-js` | ⏱️ 3min
 - [Embedbase.py](#getting-started): **Choose your own db, embeddings models, and get started with a simple** | `pip install embedbase` | ⏱️ 5 min
 - [Embedbase self-hosted](https://docs.embedbase.xyz/tutorials/self-host-on-render): **Get Embedbase Cloud on your infra** | `docker-compose up` | ⏱️ 15 min
 
-## Examples
-
-Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
 
 ## What are people building
 
-- [Creating a recommendation engine: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
-- [Creating chat with your data experiences: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
-- [Creating a talk with your docs experience: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
+- [Recommendation Engines: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
+- [Chat with your data: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
+- [Talk to your docs: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
 
 ## Getting started
 
 Let's install Python dependencies:
 
 ```bash
 pip install embedbase sentence-transformers
```

