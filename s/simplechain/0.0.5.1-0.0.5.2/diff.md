# Comparing `tmp/simplechain-0.0.5.1.tar.gz` & `tmp/simplechain-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.5.1.tar", last modified: Fri Apr 28 01:41:05 2023, max compression
+gzip compressed data, was "simplechain-0.0.5.2.tar", last modified: Fri Apr 28 01:55:35 2023, max compression
```

## Comparing `simplechain-0.0.5.1.tar` & `simplechain-0.0.5.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.660843 simplechain-0.0.5.1/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.1/LICENSE
--rw-rw-rw-   0        0        0      602 2023-04-28 01:41:05.659842 simplechain-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-28 01:41:05.660843 simplechain-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-04-28 01:40:35.000000 simplechain-0.0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.566854 simplechain-0.0.5.1/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.1/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.594853 simplechain-0.0.5.1/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.1/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.596851 simplechain-0.0.5.1/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.1/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.1/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.1/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.605843 simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.610842 simplechain-0.0.5.1/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.1/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.1/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.1/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.1/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.613850 simplechain-0.0.5.1/simplechain/stack/
--rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.1/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.617843 simplechain-0.0.5.1/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.1/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.1/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.1/simplechain/stack/databases/sql.py
--rw-rw-rw-   0        0        0     1756 2023-04-28 01:29:21.000000 simplechain-0.0.5.1/simplechain/stack/factory.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.620842 simplechain-0.0.5.1/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.1/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.623843 simplechain-0.0.5.1/simplechain/stack/pdf_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.1/simplechain/stack/pdf_loaders/__init__.py
--rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.1/simplechain/stack/pdf_loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.629843 simplechain-0.0.5.1/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.1/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.1/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.1/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.635844 simplechain-0.0.5.1/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.1/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-04-28 01:40:22.000000 simplechain-0.0.5.1/simplechain/stack/text_embedders/ai21.py
--rw-rw-rw-   0        0        0      345 2023-04-11 15:48:43.000000 simplechain-0.0.5.1/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1105 2023-04-27 21:45:05.000000 simplechain-0.0.5.1/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.638842 simplechain-0.0.5.1/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.1/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.1/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.643842 simplechain-0.0.5.1/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.1/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-04-11 21:48:56.000000 simplechain-0.0.5.1/simplechain/stack/text_generators/llms/ai21.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.1/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.5.1/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.656842 simplechain-0.0.5.1/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.1/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-11 15:49:56.000000 simplechain-0.0.5.1/simplechain/stack/vector_databases/annoy.py
--rw-rw-rw-   0        0        0     1120 2023-04-11 15:49:25.000000 simplechain-0.0.5.1/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.1/simplechain/stack/vector_databases/faiss.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.1/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.587844 simplechain-0.0.5.1/simplechain.egg-info/
--rw-rw-rw-   0        0        0      602 2023-04-28 01:41:05.000000 simplechain-0.0.5.1/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-04-28 01:41:05.000000 simplechain-0.0.5.1/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:41:05.000000 simplechain-0.0.5.1/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-28 01:41:05.000000 simplechain-0.0.5.1/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 01:41:05.657842 simplechain-0.0.5.1/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.225388 simplechain-0.0.5.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.2/LICENSE
+-rw-rw-rw-   0        0        0      602 2023-04-28 01:55:35.223387 simplechain-0.0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-28 01:55:35.225388 simplechain-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-04-28 01:55:05.000000 simplechain-0.0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.135386 simplechain-0.0.5.2/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.2/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.158386 simplechain-0.0.5.2/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.2/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.161388 simplechain-0.0.5.2/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.2/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.2/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.2/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.168389 simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.173386 simplechain-0.0.5.2/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.2/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.2/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.2/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.2/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.176387 simplechain-0.0.5.2/simplechain/stack/
+-rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.2/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.185387 simplechain-0.0.5.2/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.2/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.2/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.2/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     1756 2023-04-28 01:29:21.000000 simplechain-0.0.5.2/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.187388 simplechain-0.0.5.2/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.2/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.190405 simplechain-0.0.5.2/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.2/simplechain/stack/pdf_loaders/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.2/simplechain/stack/pdf_loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.194406 simplechain-0.0.5.2/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.2/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.2/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.2/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.201391 simplechain-0.0.5.2/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.2/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0     2146 2023-04-28 01:54:45.000000 simplechain-0.0.5.2/simplechain/stack/text_embedders/ai21.py
+-rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.2/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1103 2023-04-28 01:52:29.000000 simplechain-0.0.5.2/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.203385 simplechain-0.0.5.2/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.2/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.2/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.214390 simplechain-0.0.5.2/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.2/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2196 2023-04-28 01:54:45.000000 simplechain-0.0.5.2/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.2/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1165 2023-04-28 01:54:17.000000 simplechain-0.0.5.2/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.220387 simplechain-0.0.5.2/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.2/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3152 2023-04-28 01:53:49.000000 simplechain-0.0.5.2/simplechain/stack/vector_databases/annoy.py
+-rw-rw-rw-   0        0        0     1129 2023-04-28 01:53:17.000000 simplechain-0.0.5.2/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.2/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.2/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.153386 simplechain-0.0.5.2/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      602 2023-04-28 01:55:34.000000 simplechain-0.0.5.2/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-04-28 01:55:35.000000 simplechain-0.0.5.2/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 01:55:34.000000 simplechain-0.0.5.2/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 01:55:34.000000 simplechain-0.0.5.2/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 01:55:35.222387 simplechain-0.0.5.2/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.2/tests/__init__.py
```

### Comparing `simplechain-0.0.5.1/LICENSE` & `simplechain-0.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/PKG-INFO` & `simplechain-0.0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.1/README.rst` & `simplechain-0.0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/setup.py` & `simplechain-0.0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5.1'
+VERSION = '0.0.5.2'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.5.1/simplechain/pipeline/module.py` & `simplechain-0.0.5.2/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.5.2/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/pipeline/providers/database.py` & `simplechain-0.0.5.2/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.5.2/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/stack/databases/base.py` & `simplechain-0.0.5.2/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/stack/databases/sql.py` & `simplechain-0.0.5.2/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/stack/factory.py` & `simplechain-0.0.5.2/simplechain/stack/factory.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.5.2/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/stack/text_embedders/ai21.py` & `simplechain-0.0.5.2/simplechain/stack/text_embedders/ai21.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import List, Dict
 
-import numpy as np
 import requests
 
 from pydantic import root_validator
 
 from simplechain.stack.text_embedders.base import TextEmbedder
 from simplechain.utils import get_from_dict_or_env
 
@@ -21,25 +20,25 @@
         )
 
         values["ai21_api_key"] = ai21_api_key
         cls.ai21_api_key = ai21_api_key
 
         return values
 
-    def embed(self, text: str) -> np.ndarray:
+    def embed(self, text: str) -> List[float]:
         # Assumes the text is less than 2000 characters
         text = text.replace("\n", " ")
         text = text[:2000]
         response = requests.post('https://api.ai21.com/studio/v1/experimental/embed',
                                  json={'texts': [text]},
                                  headers={'Authorization': f'Bearer {self.ai21_api_key}'})
         embedding = response.json()['results'][0]['embedding']
-        return np.array(embedding)
+        return embedding
 
-    def embed_all(self, texts: List[str]) -> List[np.ndarray]:
+    def embed_all(self, texts: List[str]) -> List[List[float]]:
         # Breaks the strings with 2000+ characters into smaller strings
         for i, s in enumerate(texts):
             if len(s) > 2000:
                 texts.pop(i)
                 for j in range(0, len(s), 2000):
                     texts.insert(i + j, s[j:j + 2000])
```

### Comparing `simplechain-0.0.5.1/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.5.2/simplechain/stack/text_embedders/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,14 @@
             values, "openai_api_key", "OPENAI_API_KEY"
         )
         values["openai_api_key"] = openai_api_key
         openai.api_key = openai_api_key
 
         return values
 
-    def embed(self, text: str) -> np.ndarray:
+    def embed(self, text: str) -> List[float]:
         text = text.replace("\n", " ")
         return openai.Embedding.create(input=[text], model=self.model_name)['data'][0]['embedding']
 
-
-    def embed_all(self, texts: List[str]) -> List[np.ndarray]:
+    def embed_all(self, texts: List[str]) -> List[List[float]]:
         embeddings = openai.Embedding.create(input=texts, model=self.model_name)
         return [embedding['embedding'] for embedding in embeddings['data']]
-
```

### Comparing `simplechain-0.0.5.1/simplechain/stack/text_generators/llms/ai21.py` & `simplechain-0.0.5.2/simplechain/stack/text_generators/llms/ai21.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pydantic import root_validator
 
 from simplechain.stack.text_generators.llms.llm import TextGeneratorLLM
 from simplechain.utils import get_from_dict_or_env
 
 import ai21
 
+
 class TextGeneratorAI21(TextGeneratorLLM):
     """OpenAI text generator."""
     model_name = "j2-grande-instruct"
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key exists in environment."""
```

### Comparing `simplechain-0.0.5.1/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.5.2/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.5.2/simplechain/stack/text_generators/llms/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from typing import Dict
 
 import openai
 from pydantic import root_validator
 
 from simplechain.stack.text_generators.llms.llm import TextGeneratorLLM
 from simplechain.utils import get_from_dict_or_env
```

### Comparing `simplechain-0.0.5.1/simplechain/stack/vector_databases/annoy.py` & `simplechain-0.0.5.2/simplechain/stack/vector_databases/annoy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import os
 from typing import Tuple, List, Any, Literal
 
-import numpy as np
 from annoy import AnnoyIndex
 
 from simplechain.stack.vector_databases.base import VectorDatabase
 
 
 def get_index(path_to_file: str, embed_size: int,
               metric: Literal["angular", "euclidean", "manhattan", "hamming", "dot"]) -> AnnoyIndex:
@@ -42,26 +41,26 @@
         self.path_to_index_file = path_to_index_file
         self.index = get_index(path_to_index_file, embed_size, metric)
         self.i = 0
 
         self.path_to_metadata_file = path_to_metadata_file
         self.metadata = get_metadata(path_to_metadata_file)
 
-    def add(self, embed: np.ndarray, metadata: Any):
+    def add(self, embed: List[float], metadata: Any):
         """
         Add an embed and its metadata to the database
         :param embed:
         :param metadata:
         :return:
         """
         self.index.add_item(self.i, embed)
         self.i += 1
         self.metadata.append(metadata)
 
-    def add_all(self, embeds: np.ndarray, metadatas: List[Any]):
+    def add_all(self, embeds: List[List[float]], metadatas: List[Any]):
         """
         Add a list of embeds and their metadatas to the database
         :param embeds:
         :param metadatas:
         :return:
         """
         for embed, metadata in zip(embeds, metadatas):
@@ -74,15 +73,15 @@
         self.index.save(self.path_to_index_file)
 
         # Save metadata to json
         metadata_json = json.dumps(self.metadata)
         with open(self.path_to_metadata_file, "w") as f:
             f.write(metadata_json)
 
-    def get_nearest_neighbors(self, query_embed: np.ndarray, k: int = 1) -> List[Tuple[Any, float]]:
+    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1) -> List[Tuple[Any, float]]:
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param query_embed:
         :param k:
         :return: k nearest neighbors with their distances
         """
         nearest_neighbors = self.index.get_nns_by_vector(query_embed, k, include_distances=True)
```

### Comparing `simplechain-0.0.5.1/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.5.2/simplechain/stack/vector_databases/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from typing import Tuple, List, Any
 
 import numpy as np
 
 
 class VectorDatabase(ABC):
     @abstractmethod
-    def add(self, embed: np.ndarray, metadata: Any):
+    def add(self, embed: List[float], metadata: Any):
         """
         Add a name and its embed to the database
         :param metadata:
         :param embed:
         :return:
         """
         pass
 
     @abstractmethod
-    def add_all(self, embeds: np.ndarray, metadatas: List[Any]):
+    def add_all(self, embeds: List[List[float]], metadatas: List[Any]):
         """
         Add a list of names and their embeds to the database
         :param metadatas:
         :param embeds:
         :return:
         """
         pass
@@ -30,15 +30,15 @@
         """
         Build the database
         :return:
         """
         pass
 
     @abstractmethod
-    def get_nearest_neighbors(self, query_embed: np.ndarray, k: int = 1) -> List[Tuple[str, float]]:
+    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1) -> List[Tuple[str, float]]:
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param query_embed:
         :param k:
         :return: k nearest neighbors as strings with their distances
         """
         pass
```

### Comparing `simplechain-0.0.5.1/simplechain/stack/vector_databases/faiss.py` & `simplechain-0.0.5.2/simplechain/stack/vector_databases/faiss.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain/utils.py` & `simplechain-0.0.5.2/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.1/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.5.2/simplechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.1/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.5.2/simplechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

