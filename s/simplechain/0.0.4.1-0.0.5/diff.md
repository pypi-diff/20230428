# Comparing `tmp/simplechain-0.0.4.1.tar.gz` & `tmp/simplechain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.4.1.tar", last modified: Fri Apr 28 01:29:47 2023, max compression
+gzip compressed data, was "simplechain-0.0.5.tar", last modified: Fri Apr 28 01:34:23 2023, max compression
```

## Comparing `simplechain-0.0.4.1.tar` & `simplechain-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.772291 simplechain-0.0.4.1/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.4.1/LICENSE
--rw-rw-rw-   0        0        0      602 2023-04-28 01:29:47.771291 simplechain-0.0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.4.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-28 01:29:47.772291 simplechain-0.0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-04-28 01:18:10.000000 simplechain-0.0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.525296 simplechain-0.0.4.1/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.4.1/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.575291 simplechain-0.0.4.1/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.4.1/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.586295 simplechain-0.0.4.1/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.4.1/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.4.1/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.4.1/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.614292 simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.624289 simplechain-0.0.4.1/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.4.1/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.4.1/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.4.1/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.4.1/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.629292 simplechain-0.0.4.1/simplechain/stack/
--rw-rw-rw-   0        0        0      226 2023-04-11 18:57:45.000000 simplechain-0.0.4.1/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.648291 simplechain-0.0.4.1/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.4.1/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.4.1/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.4.1/simplechain/stack/databases/sql.py
--rw-rw-rw-   0        0        0     1756 2023-04-28 01:29:21.000000 simplechain-0.0.4.1/simplechain/stack/factory.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.650292 simplechain-0.0.4.1/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.4.1/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.652293 simplechain-0.0.4.1/simplechain/stack/pdf_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.4.1/simplechain/stack/pdf_loaders/__init__.py
--rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.4.1/simplechain/stack/pdf_loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.668311 simplechain-0.0.4.1/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.4.1/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.4.1/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.4.1/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.694312 simplechain-0.0.4.1/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.4.1/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-04-27 21:44:55.000000 simplechain-0.0.4.1/simplechain/stack/text_embedders/ai21.py
--rw-rw-rw-   0        0        0      345 2023-04-11 15:48:43.000000 simplechain-0.0.4.1/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1105 2023-04-27 21:45:05.000000 simplechain-0.0.4.1/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.703306 simplechain-0.0.4.1/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.4.1/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.4.1/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.733292 simplechain-0.0.4.1/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.4.1/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-04-11 21:48:56.000000 simplechain-0.0.4.1/simplechain/stack/text_generators/llms/ai21.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.4.1/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.4.1/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.761307 simplechain-0.0.4.1/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.4.1/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-11 15:49:56.000000 simplechain-0.0.4.1/simplechain/stack/vector_databases/annoy.py
--rw-rw-rw-   0        0        0     1120 2023-04-11 15:49:25.000000 simplechain-0.0.4.1/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.4.1/simplechain/stack/vector_databases/faiss.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.4.1/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.550291 simplechain-0.0.4.1/simplechain.egg-info/
--rw-rw-rw-   0        0        0      602 2023-04-28 01:29:47.000000 simplechain-0.0.4.1/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-04-28 01:29:47.000000 simplechain-0.0.4.1/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:29:47.000000 simplechain-0.0.4.1/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-28 01:29:47.000000 simplechain-0.0.4.1/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 01:29:47.769291 simplechain-0.0.4.1/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.4.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.961273 simplechain-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      600 2023-04-28 01:34:23.961273 simplechain-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-28 01:34:23.961273 simplechain-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2023-04-28 01:34:06.000000 simplechain-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.880273 simplechain-0.0.5/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.901280 simplechain-0.0.5/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.905272 simplechain-0.0.5/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.913273 simplechain-0.0.5/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.918272 simplechain-0.0.5/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.920272 simplechain-0.0.5/simplechain/stack/
+-rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.925274 simplechain-0.0.5/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     1756 2023-04-28 01:29:21.000000 simplechain-0.0.5/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.927275 simplechain-0.0.5/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.930273 simplechain-0.0.5/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5/simplechain/stack/pdf_loaders/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5/simplechain/stack/pdf_loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.936273 simplechain-0.0.5/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.943274 simplechain-0.0.5/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-04-27 21:44:55.000000 simplechain-0.0.5/simplechain/stack/text_embedders/ai21.py
+-rw-rw-rw-   0        0        0      345 2023-04-11 15:48:43.000000 simplechain-0.0.5/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1105 2023-04-27 21:45:05.000000 simplechain-0.0.5/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.946273 simplechain-0.0.5/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.952273 simplechain-0.0.5/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-04-11 21:48:56.000000 simplechain-0.0.5/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1176 2023-03-08 18:14:03.000000 simplechain-0.0.5/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.957272 simplechain-0.0.5/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-11 15:49:56.000000 simplechain-0.0.5/simplechain/stack/vector_databases/annoy.py
+-rw-rw-rw-   0        0        0     1120 2023-04-11 15:49:25.000000 simplechain-0.0.5/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.896272 simplechain-0.0.5/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-04-28 01:34:23.000000 simplechain-0.0.5/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-04-28 01:34:23.000000 simplechain-0.0.5/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 01:34:23.000000 simplechain-0.0.5/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 01:34:23.000000 simplechain-0.0.5/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 01:34:23.959273 simplechain-0.0.5/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5/tests/__init__.py
```

### Comparing `simplechain-0.0.4.1/LICENSE` & `simplechain-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/PKG-INFO` & `simplechain-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.4.1
+Version: 0.0.5
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.4.1/README.rst` & `simplechain-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/setup.py` & `simplechain-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.1'
+VERSION = '0.0.5'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.4.1/simplechain/pipeline/module.py` & `simplechain-0.0.5/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.5/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.5/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/pipeline/providers/database.py` & `simplechain-0.0.5/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.5/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/databases/base.py` & `simplechain-0.0.5/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/databases/sql.py` & `simplechain-0.0.5/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/factory.py` & `simplechain-0.0.5/simplechain/stack/factory.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.5/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/text_embedders/ai21.py` & `simplechain-0.0.5/simplechain/stack/text_embedders/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.5/simplechain/stack/text_embedders/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/text_generators/llms/ai21.py` & `simplechain-0.0.5/simplechain/stack/text_generators/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.5/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.5/simplechain/stack/text_generators/llms/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/vector_databases/annoy.py` & `simplechain-0.0.5/simplechain/stack/vector_databases/annoy.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.5/simplechain/stack/vector_databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/stack/vector_databases/faiss.py` & `simplechain-0.0.5/simplechain/stack/vector_databases/faiss.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain/utils.py` & `simplechain-0.0.5/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.4.1/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.5/simplechain.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.4.1
+Version: 0.0.5
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.4.1/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.5/simplechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

