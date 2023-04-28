# Comparing `tmp/cogsgpt-0.0.3.1.tar.gz` & `tmp/cogsgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-0.0.3.1.tar", last modified: Thu Apr 20 13:38:32 2023, max compression
+gzip compressed data, was "cogsgpt-0.0.4.tar", last modified: Fri Apr 28 16:47:43 2023, max compression
```

## Comparing `cogsgpt-0.0.3.1.tar` & `cogsgpt-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.3.1/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       43 2023-04-15 06:53:57.000000 cogsgpt-0.0.3.1/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5731 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3985 2023-04-20 10:29:29.000000 cogsgpt-0.0.3.1/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      129 2023-04-20 13:37:32.000000 cogsgpt-0.0.3.1/cogsgpt/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     9863 2023-04-20 13:36:33.000000 cogsgpt-0.0.3.1/cogsgpt/awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1876 2023-04-20 08:45:10.000000 cogsgpt-0.0.3.1/cogsgpt/awesome_prompts.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      166 2023-04-11 09:46:43.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/base_model.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      267 2023-04-13 09:30:09.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3929 2023-04-13 14:26:53.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/image_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2061 2023-04-13 14:42:27.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/cv/ocr.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      427 2023-04-14 03:16:26.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3188 2023-04-13 15:01:36.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1684 2023-04-20 12:10:44.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2150 2023-04-13 15:05:49.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1676 2023-04-13 15:11:04.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3795 2023-04-13 14:49:00.000000 cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1339 2023-04-20 11:56:11.000000 cogsgpt-0.0.3.1/cogsgpt/llm.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/cogsgpt/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.3.1/cogsgpt/metas/generate_response_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2750 2023-04-20 08:45:10.000000 cogsgpt-0.0.3.1/cogsgpt/metas/parse_task_examples.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7470 2023-04-20 08:45:10.000000 cogsgpt-0.0.3.1/cogsgpt/metas/task_metas.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1074 2023-04-20 11:56:04.000000 cogsgpt-0.0.3.1/cogsgpt/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.661611 cogsgpt-0.0.3.1/cogsgpt.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5731 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1059 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      136 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-20 13:38:32.000000 cogsgpt-0.0.3.1/cogsgpt.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      869 2023-04-20 13:37:23.000000 cogsgpt-0.0.3.1/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-20 13:38:32.665611 cogsgpt-0.0.3.1/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      251 2023-04-14 13:22:18.000000 cogsgpt-0.0.3.1/tests/test_awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      360 2023-04-15 07:30:49.000000 cogsgpt-0.0.3.1/tests/test_image_analisys.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      347 2023-04-15 07:30:38.000000 cogsgpt-0.0.3.1/tests/test_ocr.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      601 2023-04-13 14:19:29.000000 cogsgpt-0.0.3.1/tests/test_speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1441 2023-04-13 14:19:32.000000 cogsgpt-0.0.3.1/tests/test_text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      576 2023-04-14 03:20:51.000000 cogsgpt-0.0.3.1/tests/test_text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1970 2023-04-13 14:19:36.000000 cogsgpt-0.0.3.1/tests/test_text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1168 2023-04-14 03:20:35.000000 cogsgpt-0.0.3.1/tests/test_text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.289645 cogsgpt-0.0.4/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.4/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-24 05:08:50.000000 cogsgpt-0.0.4/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     6757 2023-04-28 16:47:43.289645 cogsgpt-0.0.4/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5013 2023-04-28 16:42:52.000000 cogsgpt-0.0.4/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      154 2023-04-24 07:01:19.000000 cogsgpt-0.0.4/cogsgpt/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)    13508 2023-04-28 11:43:48.000000 cogsgpt-0.0.4/cogsgpt/awesome_chat.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      202 2023-04-25 03:24:15.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/base_model.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1058 2023-04-26 07:16:38.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1869 2023-04-26 01:40:24.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/background_remover.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5601 2023-04-28 13:34:38.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/form_recognizer.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     7020 2023-04-27 02:47:18.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/image_analysis_v3.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     6544 2023-04-27 04:13:01.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/image_analysis_v4.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2581 2023-04-28 05:26:48.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/utils.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      599 2023-04-28 03:04:51.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3504 2023-04-27 03:53:31.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1823 2023-04-28 03:12:03.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2219 2023-04-27 03:51:10.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1710 2023-04-27 04:05:31.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3926 2023-04-27 03:48:02.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2835 2023-04-24 07:40:16.000000 cogsgpt-0.0.4/cogsgpt/llm.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      445 2023-04-24 03:37:51.000000 cogsgpt-0.0.4/cogsgpt/logger.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.4/cogsgpt/metas/generate_response_presteps.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2861 2023-04-28 03:41:32.000000 cogsgpt-0.0.4/cogsgpt/metas/parse_task_presteps.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2047 2023-04-28 01:19:48.000000 cogsgpt-0.0.4/cogsgpt/metas/prompts.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     4718 2023-04-28 13:35:33.000000 cogsgpt-0.0.4/cogsgpt/metas/task_metas.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      369 2023-04-27 02:28:37.000000 cogsgpt-0.0.4/cogsgpt/schema.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      892 2023-04-24 07:01:19.000000 cogsgpt-0.0.4/cogsgpt/utils.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     6757 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1261 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      189 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/top_level.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      934 2023-04-25 07:16:49.000000 cogsgpt-0.0.4/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-28 16:47:43.289645 cogsgpt-0.0.4/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1763 2023-04-28 13:14:29.000000 cogsgpt-0.0.4/tests/test_awesome_chat.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      550 2023-04-26 01:38:49.000000 cogsgpt-0.0.4/tests/test_bg_remove.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2840 2023-04-27 02:44:47.000000 cogsgpt-0.0.4/tests/test_form_recognizer.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     4952 2023-04-27 01:52:52.000000 cogsgpt-0.0.4/tests/test_image_analisys.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      602 2023-04-26 14:09:19.000000 cogsgpt-0.0.4/tests/test_speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1632 2023-04-26 14:18:48.000000 cogsgpt-0.0.4/tests/test_text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1232 2023-04-28 03:12:51.000000 cogsgpt-0.0.4/tests/test_text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1971 2023-04-24 07:02:12.000000 cogsgpt-0.0.4/tests/test_text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1195 2023-04-27 04:15:40.000000 cogsgpt-0.0.4/tests/test_text_translation.py
```

### Comparing `cogsgpt-0.0.3.1/LICENSE` & `cogsgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.3.1/PKG-INFO` & `cogsgpt-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.3.1
+Version: 0.0.4
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,101 +31,91 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CogsGPT
-A multi-modal LLM integrated ChatGPT with Azure Cognitive Service, inspired by HuggingGPT.
+A multi-modal LLM which integrates ChatGPT with Azure Cognitive Service.
 
-## Overview
-This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS). As the name CogsGPT suggests, it utilizes the ChatGPT model as the language center and integrates with Azure Cognitive Services to achieve multimodal capabilities to some extent.
-
-Typical user cases include:
-
-- Information extraction: Extract the main information from a doc or an image.
-- Image translation: Translate the text in an image to another language.
-- Speech summarization: Summarize a long speech into a short audio clip while retaining the main information.
-- Speech translation: Translate input speech into another language.
+**Now you can go to [CogsGPT on HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experice the full capabilities of CogsGPT!!!**
 
-There are more user cases waiting for your exploration!
+*If you find this repo useful, please consider giving it a star!*
 
-Here is a demo of creating a poem based on an image and converting it into speech in another language.
-
-![demo](./docs/demo.gif)
-
-## Getting Started
+![](./docs/imgs/CogsGPT-demo.png)
 
-### Prerequisites
+## Overview
 
-#### OpenAI Requirements
+### What is Azure Cognitive Service
+*(Answered by ChatGPT)*
 
-First, you need to register an [OpenAI](https://platform.openai.com/) account or deploy an [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service). Follow the official documents to obtain the API key and other resources. 
+> Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
-If you want to use OpenAI API, you need to set these environment variables:
-```bash
-export OPENAI_API_TYPE="openai"
-export OPENAI_API_KEY="<OpenAI API Key>"
-```
+### What is CogsGPT
+CogsGPT is a multi-modal LLM which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
-If you want to use Azure OpenAI Service, you need to set these environment variables:
-```bash
-export OPENAI_API_TYPE="azure"
-export OPENAI_API_BASE="<Azure OpenAI Service Endpoint>"
-export OPENAI_API_KEY="<Azure OpenAI Service Key>"
-```
+### How does it work
 
-#### Azure Cognitive Service Requirements
+The workflow of CogsGPT consists of three stages:
+1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to first think of the user's request carefully, and then parse it into a sequence of Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
+2. Task Execution Stage: In this stage, CogsGPT will execute the tasks one by one. The execution result will be stored for future reference.
+3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
 
-Next, you need also to deploy an [Azure Cognitive Service](https://azure.microsoft.com/en-us/products/cognitive-services/). Follow the official documents to obtain the deployment key and other resources, and set these environment variables:
-```bash
-export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
-export COGS_KEY="<Azure Cognitive Service Key>"
-export COGS_REGION="<Azure Cognitive Service Region>"
-```
+## Getting Started
 
-#### Platform Requirements
+### Prerequisites
 
-At last, follow the [instruction](https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/quickstarts/setup-platform?tabs=windows%2Cubuntu%2Cdotnet%2Cjre%2Cmaven%2Cnodejs%2Cmac%2Cpypi&pivots=programming-language-python#platform-requirements) here to check your platfrom requirments (which is necessary to use Azure Speech SDK for Python)
+- Python 3.8+
+- OpenAI API key
+- Azure Cognitive Multi-Service deployment ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
+- Set the following environment variables:
+    ```bash
+    # OpenAI
+    export OPENAI_API_TYPE="openai"
+    export OPENAI_API_KEY="<OpenAI API Key>"
+
+    # Azure Cognitive Service
+    export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
+    export COGS_KEY="<Azure Cognitive Service Key>"
+    export COGS_REGION="<Azure Cognitive Service Region>"
+    ```
 
 ### Quick Install
 
-You can now install CogsGPT with pip:
 ```bash
 pip install cogsgpt
 ```
 
 ### Usage
 
-You can use CogsGPT in your own application to process image or audio inputs within several lines of codes:
+You can use CogsGPT in your own application to process image or audio inputs within three lines of codes:
 ```python
 from cogsgpt import CogsGPT
 
-if os.environ["OPENAI_API_TYPE"] == "openai":
-    agent = CogsGPT(model_name="gpt-3.5-turbo")
-elif os.environ["OPENAI_API_TYPE"] == "azure":
-    agent = CogsGPT(deployment_name="<YOUR DEPLOYMENT NAME>", openai_api_version="<YOUR DEPLOYMENT VERSION>")
-
+agent = CogsGPT(model_name="gpt-3.5-turbo")
 agent.chat("What's the content in a.jpg?")
 ```
 
-Or you can experience an interactive console application with the following command:
-```bash
-python ./tests/test_awesome_chat.py
-```
+For more details on the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
+
+### Gradio Demo
 
-### Gradio App
+The CogsGPT Gradio demo is now available on [HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
 
-The Gradio demo is now hosted on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT). You can also run the following commands to start the demo locally:
+You can also use the following commands to run the demo locally with your own Azure Cognitive Service (Don't forget to set the environment variables first!):
 ```bash
 pip install gradio
 python app.py
 ```
 
-Now open your favorite browser and ENJOY THE CHAT!
+Now open your favorite browser and ENJOY YOUR CHAT!
+
+## Acknowledgments
+
+This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS), and is built on top of [LangChain](https://github.com/hwchase17/langchain).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
```

### Comparing `cogsgpt-0.0.3.1/README.md` & `cogsgpt-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,85 @@
 # CogsGPT
-A multi-modal LLM integrated ChatGPT with Azure Cognitive Service, inspired by HuggingGPT.
+A multi-modal LLM which integrates ChatGPT with Azure Cognitive Service.
 
-## Overview
-This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS). As the name CogsGPT suggests, it utilizes the ChatGPT model as the language center and integrates with Azure Cognitive Services to achieve multimodal capabilities to some extent.
-
-Typical user cases include:
-
-- Information extraction: Extract the main information from a doc or an image.
-- Image translation: Translate the text in an image to another language.
-- Speech summarization: Summarize a long speech into a short audio clip while retaining the main information.
-- Speech translation: Translate input speech into another language.
+**Now you can go to [CogsGPT on HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experice the full capabilities of CogsGPT!!!**
 
-There are more user cases waiting for your exploration!
+*If you find this repo useful, please consider giving it a star!*
 
-Here is a demo of creating a poem based on an image and converting it into speech in another language.
-
-![demo](./docs/demo.gif)
-
-## Getting Started
+![](./docs/imgs/CogsGPT-demo.png)
 
-### Prerequisites
+## Overview
 
-#### OpenAI Requirements
+### What is Azure Cognitive Service
+*(Answered by ChatGPT)*
 
-First, you need to register an [OpenAI](https://platform.openai.com/) account or deploy an [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service). Follow the official documents to obtain the API key and other resources. 
+> Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
-If you want to use OpenAI API, you need to set these environment variables:
-```bash
-export OPENAI_API_TYPE="openai"
-export OPENAI_API_KEY="<OpenAI API Key>"
-```
+### What is CogsGPT
+CogsGPT is a multi-modal LLM which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
-If you want to use Azure OpenAI Service, you need to set these environment variables:
-```bash
-export OPENAI_API_TYPE="azure"
-export OPENAI_API_BASE="<Azure OpenAI Service Endpoint>"
-export OPENAI_API_KEY="<Azure OpenAI Service Key>"
-```
+### How does it work
 
-#### Azure Cognitive Service Requirements
+The workflow of CogsGPT consists of three stages:
+1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to first think of the user's request carefully, and then parse it into a sequence of Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
+2. Task Execution Stage: In this stage, CogsGPT will execute the tasks one by one. The execution result will be stored for future reference.
+3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
 
-Next, you need also to deploy an [Azure Cognitive Service](https://azure.microsoft.com/en-us/products/cognitive-services/). Follow the official documents to obtain the deployment key and other resources, and set these environment variables:
-```bash
-export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
-export COGS_KEY="<Azure Cognitive Service Key>"
-export COGS_REGION="<Azure Cognitive Service Region>"
-```
+## Getting Started
 
-#### Platform Requirements
+### Prerequisites
 
-At last, follow the [instruction](https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/quickstarts/setup-platform?tabs=windows%2Cubuntu%2Cdotnet%2Cjre%2Cmaven%2Cnodejs%2Cmac%2Cpypi&pivots=programming-language-python#platform-requirements) here to check your platfrom requirments (which is necessary to use Azure Speech SDK for Python)
+- Python 3.8+
+- OpenAI API key
+- Azure Cognitive Multi-Service deployment ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
+- Set the following environment variables:
+    ```bash
+    # OpenAI
+    export OPENAI_API_TYPE="openai"
+    export OPENAI_API_KEY="<OpenAI API Key>"
+
+    # Azure Cognitive Service
+    export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
+    export COGS_KEY="<Azure Cognitive Service Key>"
+    export COGS_REGION="<Azure Cognitive Service Region>"
+    ```
 
 ### Quick Install
 
-You can now install CogsGPT with pip:
 ```bash
 pip install cogsgpt
 ```
 
 ### Usage
 
-You can use CogsGPT in your own application to process image or audio inputs within several lines of codes:
+You can use CogsGPT in your own application to process image or audio inputs within three lines of codes:
 ```python
 from cogsgpt import CogsGPT
 
-if os.environ["OPENAI_API_TYPE"] == "openai":
-    agent = CogsGPT(model_name="gpt-3.5-turbo")
-elif os.environ["OPENAI_API_TYPE"] == "azure":
-    agent = CogsGPT(deployment_name="<YOUR DEPLOYMENT NAME>", openai_api_version="<YOUR DEPLOYMENT VERSION>")
-
+agent = CogsGPT(model_name="gpt-3.5-turbo")
 agent.chat("What's the content in a.jpg?")
 ```
 
-Or you can experience an interactive console application with the following command:
-```bash
-python ./tests/test_awesome_chat.py
-```
+For more details on the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
+
+### Gradio Demo
 
-### Gradio App
+The CogsGPT Gradio demo is now available on [HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
 
-The Gradio demo is now hosted on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT). You can also run the following commands to start the demo locally:
+You can also use the following commands to run the demo locally with your own Azure Cognitive Service (Don't forget to set the environment variables first!):
 ```bash
 pip install gradio
 python app.py
 ```
 
-Now open your favorite browser and ENJOY THE CHAT!
+Now open your favorite browser and ENJOY YOUR CHAT!
+
+## Acknowledgments
+
+This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS), and is built on top of [LangChain](https://github.com/hwchase17/langchain).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,44 @@
+from __future__ import annotations
+
 import abc
 import os
 from typing import List
 
 from azure.ai.textanalytics import TextAnalyticsClient
 from azure.core.credentials import AzureKeyCredential
 
-from cogsgpt.utils import ArgsType, LanguageType
+from cogsgpt.schema import ArgsType, LanguageType
 from cogsgpt.cogsmodel import BaseModel
 
 
-COGS_KEY = os.environ['COGS_KEY']
-COGS_ENDPOINT = os.environ['COGS_ENDPOINT']
-
-
 class BaseAnalysisModel(BaseModel, abc.ABC):
     def __init__(self) -> None:
         super().__init__()
+        
+        COGS_KEY = os.environ['COGS_KEY']
+        COGS_ENDPOINT = os.environ['COGS_ENDPOINT']
         ta_credential = AzureKeyCredential(COGS_KEY)
         self.text_analytics_client = TextAnalyticsClient(
             endpoint=COGS_ENDPOINT,
             credential=ta_credential
         )
 
         self.supported_language = {
-            LanguageType.English.value: "en-us",
+            LanguageType.English.value: "en",
             LanguageType.Chinese.value: "zh-hans",
         }
     
     @abc.abstractmethod
     def _analyze(self, text: str, language: str = "en") -> List:
         pass
 
     def run(self, *args, **kwargs) -> str:
         text = kwargs[ArgsType.TEXT.value]
-        language = kwargs.get("from_language", LanguageType.English.value)
+        language = kwargs.get(ArgsType.SRC_LANGUAGE.value, LanguageType.English.value)
         language = self.supported_language[language]
         return str(self._analyze(text, language))
 
 
 class KeyPhraseModel(BaseAnalysisModel):
     def _analyze(self, text: str, language: str = "en") -> List:
         response = self.text_analytics_client.extract_key_phrases(documents=[text], language=language)
@@ -81,8 +82,14 @@
 
 class SentimentAnalysisModel(BaseAnalysisModel):
     def _analyze(self, text: str, language: str = "en") -> List:
         response = self.text_analytics_client.analyze_sentiment(documents=[text], language=language)
         return [{
             "sentence": sentence.text,
             "sentiment": sentence.sentiment,
-        } for sentence in response[0].sentences]
+        } for sentence in response[0].sentences]
+
+
+class LanguageDetectionModel(BaseAnalysisModel):
+    def _analyze(self, text: str, language: str = "en") -> List:
+        response = self.text_analytics_client.detect_language(documents=[text])
+        return [response[0].primary_language.name]
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,54 @@
+from __future__ import annotations
+
 from typing import List
 from langchain import PromptTemplate
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
 from langchain.schema import BaseMessage
 
-from cogsgpt import LLMManager
+from cogsgpt.llm import LLMManager
 from cogsgpt.cogsmodel import BaseModel
 
 
 class TextGenerationModel(BaseModel):
     def __init__(self) -> None:
         super().__init__()
         self._task_name = "text-generation"
 
-        # NOTE: LLMManger is a singleton class. It should have been instantiated in the main process.
         self._llm = LLMManager().LLM
         self._prompt = self._create_prompt()
 
     def _create_prompt(self) -> ChatPromptTemplate:
         human_message_prompt = HumanMessagePromptTemplate(
             prompt=PromptTemplate(
-                template="The user request [ {{human_input}} ] contains a {{ task_name }} task. Now you are a {{ task_name }} system, the arguments are {{ task_args }}. Just help me do {{ task_name }} and give me the result. The result should focus more on the {{ task_name}} task, no additional notes, and must be in text form without any urls.",
-                input_variables=["human_input", "task_name", "task_args"],
+                template="You are a {{ task_name }} system, the arguments are {{ task_args }}. Just help me do {{ task_name }} and give me the result. The result should focus only on the {{ task_name}} task, no additional notes, and must be in text form without any urls.",
+                input_variables=["task_name", "task_args"],
                 template_format="jinja2",
             )
         )
 
         return ChatPromptTemplate.from_messages([human_message_prompt])
 
     def _format_prompt(self, **kwargs) -> List[BaseMessage]:
         return self._prompt.format_prompt(
-            human_input=kwargs["human_input"],
             task_name=self._task_name,
             task_args=kwargs
         ).to_messages()
 
     def run(self, *args, **kwargs) -> str:
         request = self._format_prompt(**kwargs)
         return self._llm(request).content
+    
+
+class GenerativeTextSummarizationModel(TextGenerationModel):
+    def __init__(self) -> None:
+        super().__init__()
+        self._task_name = "text-summarization"
+
+
+class GenerativeTextTranslationModel(TextGenerationModel):
+    def __init__(self) -> None:
+        super().__init__()
+        self._task_name = "text-translation"
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+from __future__ import annotations
+
 import abc
 import os
 
 from azure.ai.textanalytics import TextAnalyticsClient, ExtractSummaryAction, AbstractSummaryAction
 from azure.core.credentials import AzureKeyCredential
 
-from cogsgpt.utils import ArgsType, LanguageType
+from cogsgpt.schema import ArgsType, LanguageType
 from cogsgpt.cogsmodel import BaseModel
 
 
-COGS_KEY = os.environ['COGS_KEY']
-COGS_ENDPOINT = os.environ['COGS_ENDPOINT']
-
-
 class BaseSummarizeModel(BaseModel, abc.ABC):
     def __init__(self) -> None:
         super().__init__()
+        
+        COGS_KEY = os.environ['COGS_KEY']
+        COGS_ENDPOINT = os.environ['COGS_ENDPOINT']
         ta_credential = AzureKeyCredential(COGS_KEY)
         self.text_analytics_client = TextAnalyticsClient(
             endpoint=COGS_ENDPOINT,
             credential=ta_credential
         )
 
         self.supported_language = {
-            LanguageType.English.value: "en-us",
+            LanguageType.English.value: "en",
             LanguageType.Chinese.value: "zh-hans",
         }
 
     @abc.abstractmethod
     def _summarize(self, text: str, language: str = "en") -> str:
         pass
 
     def run(self, *args, **kwargs) -> str:
         text = kwargs[ArgsType.TEXT.value]
-        language = kwargs.get("from_language", LanguageType.English.value)
+        language = kwargs.get(ArgsType.SRC_LANGUAGE.value, LanguageType.English.value)
         language = self.supported_language[language]
         return self._summarize(text, language)
 
 
 class ExtractSummarizeModel(BaseSummarizeModel):
     def _summarize(self, text: str, language: str = "en") -> str:
         poller = self.text_analytics_client.begin_analyze_actions(
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
+from __future__ import annotations
+
 import os
 import uuid
 
 import requests
 
-from cogsgpt.utils import ArgsType, LanguageType
+from cogsgpt.schema import ArgsType, LanguageType
 from cogsgpt.cogsmodel import BaseModel
 
 
-COGS_KEY = os.environ['COGS_KEY']
-COGS_ENDPOINT = os.environ['COGS_ENDPOINT']
-COGS_REGION = os.environ['COGS_REGION']
-
-
 class TextTranslationModel(BaseModel):
     def __init__(self) -> None:
         super().__init__()
+
+        COGS_KEY = os.environ['COGS_KEY']
+        COGS_REGION = os.environ['COGS_REGION']
         self.translate_endpoint = "https://api.cognitive.microsofttranslator.com/translate"
         self.headers = {
             'Ocp-Apim-Subscription-Key': COGS_KEY,
             # location required if you're using a multi-service or regional (not global) resource.
             'Ocp-Apim-Subscription-Region': COGS_REGION,
             'Content-type': 'application/json',
             'X-ClientTraceId': str(uuid.uuid4())
         }
 
         self.supported_language = {
             LanguageType.English.value: "en",
             LanguageType.Chinese.value: "zh-Hans",
         }
 
-    def _translate(self, text: str, from_language: str, to_language: str) -> str:
+    def _translate(self, text: str, src_language: str, tgt_language: str) -> str:
         body = [{
             'text': text
         }]
         params = {
             'api-version': '3.0',
-            'from': from_language,
-            'to': to_language
+            'from': src_language,
+            'to': tgt_language
         }
 
         request = requests.post(self.translate_endpoint, headers=self.headers, params=params, json=body)
         response = request.json()
         return response[0]['translations'][0]['text']
 
     def run(self, *args, **kwargs) -> str:
         text = kwargs[ArgsType.TEXT.value]
-        from_language = self.supported_language[kwargs["from_language"]]
-        to_language = self.supported_language[kwargs["to_language"]]
-        return self._translate(text, from_language, to_language)
+        src_language = self.supported_language[kwargs[ArgsType.SRC_LANGUAGE.value]]
+        tgt_language = self.supported_language[kwargs[ArgsType.TGT_LANGUAGE.value]]
+        return self._translate(text, src_language, tgt_language)
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/speech.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+from __future__ import annotations
+
 import os
 import tempfile
 import time
 
 import azure.cognitiveservices.speech as speechsdk
 
-from cogsgpt.utils import ArgsType, LanguageType
+from cogsgpt.schema import ArgsType, LanguageType
 from cogsgpt.cogsmodel import BaseModel
 
 
-COGS_KEY = os.environ['COGS_KEY']
-COGS_ENDPOINT = os.environ['COGS_ENDPOINT']
-COGS_REGION = os.environ['COGS_REGION']
-
-
 class Text2SpeechModel(BaseModel):
     def __init__(self) -> None:
         super().__init__()
+
+        COGS_KEY = os.environ['COGS_KEY']
+        COGS_REGION = os.environ['COGS_REGION']
         self.speech_config = speechsdk.SpeechConfig(subscription=COGS_KEY, region=COGS_REGION)
 
         self.supported_language = {
             LanguageType.English.value: "en-US",
             LanguageType.Chinese.value: "zh-CN",
         }
 
@@ -31,22 +31,25 @@
         
         with tempfile.NamedTemporaryFile(mode='w', suffix=".wav", delete=False) as temp_audio_file:
             speech_synthesis_stream.save_to_wav_file(temp_audio_file.name)
             return temp_audio_file.name
 
     def run(self, *args, **kwargs) -> str:
         text = kwargs[ArgsType.TEXT.value]
-        language = kwargs.get("from_language", LanguageType.English.value)
+        language = kwargs.get(ArgsType.SRC_LANGUAGE.value, LanguageType.English.value)
         language = self.supported_language[language]
         return self._text2speech(text, language)
     
 
 class Speech2TextModel(BaseModel):
     def __init__(self) -> None:
         super().__init__()
+        
+        COGS_KEY = os.environ['COGS_KEY']
+        COGS_REGION = os.environ['COGS_REGION']
         self.speech_config = speechsdk.SpeechConfig(subscription=COGS_KEY, region=COGS_REGION)
 
         self.supported_language = {
             LanguageType.English.value: "en-US",
             LanguageType.Chinese.value: "zh-CN",
         }
 
@@ -83,10 +86,10 @@
         speech_recognizer = speechsdk.SpeechRecognizer(speech_config=self.speech_config, audio_config=audio_config)
         # speech_recognition_result = speech_recognizer.recognize_once_async().get()
         speech_recognition_result = self._recognize_continuous(speech_recognizer)
         return speech_recognition_result
 
     def run(self, *args, **kwargs) -> str:
         audio_file = kwargs[ArgsType.AUDIO.value]
-        language = kwargs.get("from_language", LanguageType.English.value)
+        language = kwargs.get(ArgsType.SRC_LANGUAGE.value, LanguageType.English.value)
         language = self.supported_language[language]
         return self._speech2text(audio_file, language)
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-0.0.4/cogsgpt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.3.1
+Version: 0.0.4
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,101 +31,91 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CogsGPT
-A multi-modal LLM integrated ChatGPT with Azure Cognitive Service, inspired by HuggingGPT.
+A multi-modal LLM which integrates ChatGPT with Azure Cognitive Service.
 
-## Overview
-This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS). As the name CogsGPT suggests, it utilizes the ChatGPT model as the language center and integrates with Azure Cognitive Services to achieve multimodal capabilities to some extent.
-
-Typical user cases include:
-
-- Information extraction: Extract the main information from a doc or an image.
-- Image translation: Translate the text in an image to another language.
-- Speech summarization: Summarize a long speech into a short audio clip while retaining the main information.
-- Speech translation: Translate input speech into another language.
+**Now you can go to [CogsGPT on HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experice the full capabilities of CogsGPT!!!**
 
-There are more user cases waiting for your exploration!
+*If you find this repo useful, please consider giving it a star!*
 
-Here is a demo of creating a poem based on an image and converting it into speech in another language.
-
-![demo](./docs/demo.gif)
-
-## Getting Started
+![](./docs/imgs/CogsGPT-demo.png)
 
-### Prerequisites
+## Overview
 
-#### OpenAI Requirements
+### What is Azure Cognitive Service
+*(Answered by ChatGPT)*
 
-First, you need to register an [OpenAI](https://platform.openai.com/) account or deploy an [Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service). Follow the official documents to obtain the API key and other resources. 
+> Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
-If you want to use OpenAI API, you need to set these environment variables:
-```bash
-export OPENAI_API_TYPE="openai"
-export OPENAI_API_KEY="<OpenAI API Key>"
-```
+### What is CogsGPT
+CogsGPT is a multi-modal LLM which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
-If you want to use Azure OpenAI Service, you need to set these environment variables:
-```bash
-export OPENAI_API_TYPE="azure"
-export OPENAI_API_BASE="<Azure OpenAI Service Endpoint>"
-export OPENAI_API_KEY="<Azure OpenAI Service Key>"
-```
+### How does it work
 
-#### Azure Cognitive Service Requirements
+The workflow of CogsGPT consists of three stages:
+1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to first think of the user's request carefully, and then parse it into a sequence of Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
+2. Task Execution Stage: In this stage, CogsGPT will execute the tasks one by one. The execution result will be stored for future reference.
+3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
 
-Next, you need also to deploy an [Azure Cognitive Service](https://azure.microsoft.com/en-us/products/cognitive-services/). Follow the official documents to obtain the deployment key and other resources, and set these environment variables:
-```bash
-export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
-export COGS_KEY="<Azure Cognitive Service Key>"
-export COGS_REGION="<Azure Cognitive Service Region>"
-```
+## Getting Started
 
-#### Platform Requirements
+### Prerequisites
 
-At last, follow the [instruction](https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/quickstarts/setup-platform?tabs=windows%2Cubuntu%2Cdotnet%2Cjre%2Cmaven%2Cnodejs%2Cmac%2Cpypi&pivots=programming-language-python#platform-requirements) here to check your platfrom requirments (which is necessary to use Azure Speech SDK for Python)
+- Python 3.8+
+- OpenAI API key
+- Azure Cognitive Multi-Service deployment ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
+- Set the following environment variables:
+    ```bash
+    # OpenAI
+    export OPENAI_API_TYPE="openai"
+    export OPENAI_API_KEY="<OpenAI API Key>"
+
+    # Azure Cognitive Service
+    export COGS_ENDPOINT="<Azure Cognitive Service Endpoint>"
+    export COGS_KEY="<Azure Cognitive Service Key>"
+    export COGS_REGION="<Azure Cognitive Service Region>"
+    ```
 
 ### Quick Install
 
-You can now install CogsGPT with pip:
 ```bash
 pip install cogsgpt
 ```
 
 ### Usage
 
-You can use CogsGPT in your own application to process image or audio inputs within several lines of codes:
+You can use CogsGPT in your own application to process image or audio inputs within three lines of codes:
 ```python
 from cogsgpt import CogsGPT
 
-if os.environ["OPENAI_API_TYPE"] == "openai":
-    agent = CogsGPT(model_name="gpt-3.5-turbo")
-elif os.environ["OPENAI_API_TYPE"] == "azure":
-    agent = CogsGPT(deployment_name="<YOUR DEPLOYMENT NAME>", openai_api_version="<YOUR DEPLOYMENT VERSION>")
-
+agent = CogsGPT(model_name="gpt-3.5-turbo")
 agent.chat("What's the content in a.jpg?")
 ```
 
-Or you can experience an interactive console application with the following command:
-```bash
-python ./tests/test_awesome_chat.py
-```
+For more details on the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
+
+### Gradio Demo
 
-### Gradio App
+The CogsGPT Gradio demo is now available on [HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
 
-The Gradio demo is now hosted on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT). You can also run the following commands to start the demo locally:
+You can also use the following commands to run the demo locally with your own Azure Cognitive Service (Don't forget to set the environment variables first!):
 ```bash
 pip install gradio
 python app.py
 ```
 
-Now open your favorite browser and ENJOY THE CHAT!
+Now open your favorite browser and ENJOY YOUR CHAT!
+
+## Acknowledgments
+
+This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS), and is built on top of [LangChain](https://github.com/hwchase17/langchain).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
```

### Comparing `cogsgpt-0.0.3.1/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-0.0.4/cogsgpt.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 cogsgpt/__init__.py
 cogsgpt/awesome_chat.py
-cogsgpt/awesome_prompts.py
 cogsgpt/llm.py
+cogsgpt/logger.py
+cogsgpt/schema.py
 cogsgpt/utils.py
 cogsgpt.egg-info/PKG-INFO
 cogsgpt.egg-info/SOURCES.txt
 cogsgpt.egg-info/dependency_links.txt
 cogsgpt.egg-info/requires.txt
 cogsgpt.egg-info/top_level.txt
 cogsgpt/cogsmodel/__init__.py
 cogsgpt/cogsmodel/base_model.py
 cogsgpt/cogsmodel/cv/__init__.py
-cogsgpt/cogsmodel/cv/image_analysis.py
-cogsgpt/cogsmodel/cv/ocr.py
+cogsgpt/cogsmodel/cv/background_remover.py
+cogsgpt/cogsmodel/cv/form_recognizer.py
+cogsgpt/cogsmodel/cv/image_analysis_v3.py
+cogsgpt/cogsmodel/cv/image_analysis_v4.py
+cogsgpt/cogsmodel/cv/utils.py
 cogsgpt/cogsmodel/nlp/__init__.py
 cogsgpt/cogsmodel/nlp/text_analysis.py
 cogsgpt/cogsmodel/nlp/text_generation.py
 cogsgpt/cogsmodel/nlp/text_summarize.py
 cogsgpt/cogsmodel/nlp/text_translation.py
 cogsgpt/cogsmodel/speech/__init__.py
 cogsgpt/cogsmodel/speech/speech.py
 cogsgpt/metas/generate_response_presteps.json
-cogsgpt/metas/parse_task_examples.json
-cogsgpt/metas/task_metas.json
+cogsgpt/metas/parse_task_presteps.json
+cogsgpt/metas/prompts.yaml
+cogsgpt/metas/task_metas.yaml
 tests/test_awesome_chat.py
+tests/test_bg_remove.py
+tests/test_form_recognizer.py
 tests/test_image_analisys.py
-tests/test_ocr.py
 tests/test_speech.py
 tests/test_text_analysis.py
 tests/test_text_generation.py
 tests/test_text_summarize.py
 tests/test_text_translation.py
```

### Comparing `cogsgpt-0.0.3.1/pyproject.toml` & `cogsgpt-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "0.0.3.1"
+version = "0.0.4"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["chatgpt", "cognitive service", "llm"]
 dependencies = [
     "azure-ai-vision",
+    "azure-cognitiveservices-vision-computervision",
     "azure-ai-formrecognizer",
     "azure-ai-textanalytics == 5.3.0b1",
     "azure-cognitiveservices-speech",
+    "colorlog",
+    "jinja2",
     "langchain",
     "openai",
-    "jinja2",
-    "colorlog",
+    "pillow",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/whiskyboy/cogsgpt"
```

### Comparing `cogsgpt-0.0.3.1/tests/test_speech.py` & `cogsgpt-0.0.4/tests/test_speech.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 sys.path.insert(0, "./")
 
-from cogsgpt.utils import ArgsType
+from cogsgpt.schema import ArgsType
 from cogsgpt.cogsmodel.speech import Speech2TextModel, Text2SpeechModel
 
 if __name__ == '__main__':
     # Test text2speech model
     text2speech_model = Text2SpeechModel()
     data = {
         ArgsType.TEXT.value: "I'm your AI assistant. You can call me Tina. How can I help you?"
```

### Comparing `cogsgpt-0.0.3.1/tests/test_text_analysis.py` & `cogsgpt-0.0.4/tests/test_text_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 sys.path.insert(0, "./")
 
-from cogsgpt.utils import ArgsType
+from cogsgpt.schema import ArgsType
 from cogsgpt.cogsmodel.nlp import *
 
 if __name__ == '__main__':
     # Test KeyPhraseModel
     model = KeyPhraseModel()
     data = {
         ArgsType.TEXT.value: "Dr. Smith has a very modern medical office, and she has great staff."
@@ -38,8 +38,15 @@
     print(model.run(**data))
 
     # Test SentimentClassiferModel
     model = SentimentAnalysisModel()
     data = {
         ArgsType.TEXT.value: "The food and service were unacceptable. The concierge was nice, however."
     }
+    print(model.run(**data))
+
+    # Test LanguageDetectionModel
+    model = LanguageDetectionModel()
+    data = {
+        ArgsType.TEXT.value: "Ce document est rédigé en Français."
+    }
     print(model.run(**data))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cogsgpt-0.0.3.1/tests/test_text_summarize.py` & `cogsgpt-0.0.4/tests/test_text_summarize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 sys.path.insert(0, "./")
 
-from cogsgpt.utils import ArgsType
+from cogsgpt.schema import ArgsType
 from cogsgpt.cogsmodel.nlp import *
 
 if __name__ == '__main__':
     # Test ExtractSummarizeModel
     model = ExtractSummarizeModel()
     data = {
         ArgsType.TEXT.value: "The extractive summarization feature uses natural language processing techniques to locate key sentences in an unstructured text document. "
```

### Comparing `cogsgpt-0.0.3.1/tests/test_text_translation.py` & `cogsgpt-0.0.4/tests/test_text_translation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 sys.path.insert(0, "./")
 
-from cogsgpt.utils import ArgsType, LanguageType
+from cogsgpt.schema import ArgsType, LanguageType
 from cogsgpt.cogsmodel.nlp import *
 
 if __name__ == '__main__':
     # Test TextTranslationModel
     model = TextTranslationModel()
     data = {
         ArgsType.TEXT.value: "The extractive summarization feature uses natural language processing techniques to locate key sentences in an unstructured text document. "
         "These sentences collectively convey the main idea of the document. This feature is provided as an API for developers. " 
         "They can use it to build intelligent solutions based on the relevant information extracted to support various use cases. "
         "In the public preview, extractive summarization supports several languages. It is based on pretrained multilingual transformer models, part of our quest for holistic representations. "
         "It draws its strength from transfer learning across monolingual and harness the shared nature of languages to produce models of improved quality and efficiency. ",
-        "from_language": LanguageType.English.value,
-        "to_language": LanguageType.Chinese.value,
+        ArgsType.SRC_LANGUAGE.value: LanguageType.English.value,
+        ArgsType.TGT_LANGUAGE.value: LanguageType.Chinese.value,
     }
     print(model.run(**data))
```

