# Comparing `tmp/efficiency-1.2.tar.gz` & `tmp/efficiency-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficiency-1.2.tar", last modified: Wed Apr 19 16:43:12 2023, max compression
+gzip compressed data, was "efficiency-1.2.1.tar", last modified: Fri Apr 28 16:20:32 2023, max compression
```

## Comparing `efficiency-1.2.tar` & `efficiency-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/
--rw-r--r--   0 zjin      (7600) is        (1040)     1079 2023-04-19 16:43:03.000000 efficiency-1.2/LICENSE.txt
--rw-r--r--   0 zjin      (7600) is        (1040)     1862 2023-04-19 16:43:12.649815 efficiency-1.2/PKG-INFO
--rw-r--r--   0 zjin      (7600) is        (1040)     1612 2023-04-19 16:43:03.000000 efficiency-1.2/README.md
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/efficiency/
--rw-r--r--   0 zjin      (7600) is        (1040)      201 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/__init__.py
--rw-r--r--   0 zjin      (7600) is        (1040)     1011 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/file_manager.py
--rw-r--r--   0 zjin      (7600) is        (1040)     6584 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/function.py
--rw-r--r--   0 zjin      (7600) is        (1040)    12306 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/log.py
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/efficiency/mt/
--rw-r--r--   0 zjin      (7600) is        (1040)       55 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/mt/__init__.py
--rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/mt/loss_plot.py
--rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/mt/tensorboard_logging.py
--rw-r--r--   0 zjin      (7600) is        (1040)     8294 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/nlp.py
--rw-r--r--   0 zjin      (7600) is        (1040)     9206 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/plotter.py
--rw-r--r--   0 zjin      (7600) is        (1040)      520 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/record.py
--rw-r--r--   0 zjin      (7600) is        (1040)    11694 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/text.py
--rw-r--r--   0 zjin      (7600) is        (1040)      573 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/web.py
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/efficiency.egg-info/
--rw-r--r--   0 zjin      (7600) is        (1040)     1862 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/PKG-INFO
--rw-r--r--   0 zjin      (7600) is        (1040)      488 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/SOURCES.txt
--rw-r--r--   0 zjin      (7600) is        (1040)        1 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/dependency_links.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       24 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/requires.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       11 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/top_level.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       79 2023-04-19 16:43:12.649815 efficiency-1.2/setup.cfg
--rw-r--r--   0 zjin      (7600) is        (1040)      507 2023-04-19 16:43:03.000000 efficiency-1.2/setup.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-28 16:20:32.797467 efficiency-1.2.1/
+-rw-r--r--   0 zjin      (7600) is        (1040)     1079 2023-04-28 16:20:12.000000 efficiency-1.2.1/LICENSE.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)     1864 2023-04-28 16:20:32.797467 efficiency-1.2.1/PKG-INFO
+-rw-r--r--   0 zjin      (7600) is        (1040)     1612 2023-04-28 16:20:12.000000 efficiency-1.2.1/README.md
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-28 16:20:32.797467 efficiency-1.2.1/efficiency/
+-rw-r--r--   0 zjin      (7600) is        (1040)      201 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/__init__.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     6788 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/bib.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     1011 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/file_manager.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     6584 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/function.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    12306 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/log.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-28 16:20:32.797467 efficiency-1.2.1/efficiency/mt/
+-rw-r--r--   0 zjin      (7600) is        (1040)       55 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/mt/__init__.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/mt/loss_plot.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/mt/tensorboard_logging.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     8364 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/nlp.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     9206 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/plotter.py
+-rw-r--r--   0 zjin      (7600) is        (1040)      520 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/record.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    11694 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/text.py
+-rw-r--r--   0 zjin      (7600) is        (1040)      573 2023-04-28 16:20:12.000000 efficiency-1.2.1/efficiency/web.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-28 16:20:32.797467 efficiency-1.2.1/efficiency.egg-info/
+-rw-r--r--   0 zjin      (7600) is        (1040)     1864 2023-04-28 16:20:32.000000 efficiency-1.2.1/efficiency.egg-info/PKG-INFO
+-rw-r--r--   0 zjin      (7600) is        (1040)      506 2023-04-28 16:20:32.000000 efficiency-1.2.1/efficiency.egg-info/SOURCES.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)        1 2023-04-28 16:20:32.000000 efficiency-1.2.1/efficiency.egg-info/dependency_links.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       24 2023-04-28 16:20:32.000000 efficiency-1.2.1/efficiency.egg-info/requires.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       11 2023-04-28 16:20:32.000000 efficiency-1.2.1/efficiency.egg-info/top_level.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       79 2023-04-28 16:20:32.797467 efficiency-1.2.1/setup.cfg
+-rw-r--r--   0 zjin      (7600) is        (1040)      509 2023-04-28 16:20:12.000000 efficiency-1.2.1/setup.py
```

### Comparing `efficiency-1.2/LICENSE.txt` & `efficiency-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/PKG-INFO` & `efficiency-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficiency
-Version: 1.2
+Version: 1.2.1
 Summary: A package for efficient programming
 Home-page: https://github.com/zhijing-jin/efficiency
 Author: Zhijing Jin
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `efficiency-1.2/README.md` & `efficiency-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/file_manager.py` & `efficiency-1.2.1/efficiency/file_manager.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/function.py` & `efficiency-1.2.1/efficiency/function.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/log.py` & `efficiency-1.2.1/efficiency/log.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/mt/loss_plot.py` & `efficiency-1.2.1/efficiency/mt/loss_plot.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/mt/tensorboard_logging.py` & `efficiency-1.2.1/efficiency/mt/tensorboard_logging.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/nlp.py` & `efficiency-1.2.1/efficiency/nlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,18 @@
         "gpt-3.5-turbo": 0.002,
         "gpt-4-32k": 0.12,
         "gpt-4": 0.06,
         "text-davinci-003": 0.0200,
     }
 
     def __init__(self, model_version='gpt3.5', max_tokens=100, output_file='.cache_gpt_responses.csv',
-                 system_prompt="You are a helpful assistant."):
+                 system_prompt="You are a helpful assistant.",
+                 openai_key_alias='OPENAI_API_KEY', ):
         import os
-        openai_api_key = os.environ['OPENAI_API_KEY']
+        openai_api_key = os.environ[openai_key_alias]
 
         self.model_version = model_version
         self.max_tokens = max_tokens
         self.system_prompt = system_prompt
         self.output_file = output_file
         self.gpt_files = [output_file]
 
@@ -110,18 +111,18 @@
         for file in self.gpt_files:
             data = fread(file, verbose=False)
             cache.update({i[f'query{q_i}']: i[f'pred{q_i}'] for i in data
                           for q_i in list(range(10)) + ['']
                           if f'query{q_i}' in i})
         return cache
 
-    def query_with_patience(self, *args, **kwargs):
+    def ask(self, *args, **kwargs):
         import openai
         try:
-            return self.query(*args, **kwargs)
+            return self.raw_query(*args, **kwargs)
         except openai.error.InvalidRequestError:
             import pdb;
             pdb.set_trace()
             if len(self.dialog_history) > 10:
                 import pdb;
                 pdb.set_trace()
             for turn_i, turn in enumerate(self.dialog_history):
@@ -135,22 +136,24 @@
             '''
             Default rate limits for gpt-4/gpt-4-0314 are 40k TPM and 200 RPM. Default rate limits for gpt-4-32k/gpt-4-32k-0314 are 80k PRM and 400 RPM. 
             https://platform.openai.com/docs/guides/rate-limits/overview
             '''
 
             import time
             time.sleep(sec)
-            return self.query_with_patience(*args, **kwargs)
+            return self.ask(*args, **kwargs)
 
-    def query(self, question, turn_off_cache=False, stop_sign="\nQ: ",
-              continued_questions=False, max_tokens=None, verbose=True, only_response=True,
-              model_version=[None, 'gpt3', 'gpt3.5', 'gpt4'][0],
-              engine=[None, "text-davinci-003", "gpt-3.5-turbo", "gpt-4-32k-0314", "gpt-4-0314", "gpt-4"][0],
-              enable_pdb=False,
-              ):
+    def raw_query(self, question,
+                  turn_off_cache=False,
+                  continued_questions=False,
+                  max_tokens=None, stop_sign="\nQ: ",
+                  model_version=[None, 'gpt3', 'gpt3.5', 'gpt4'][0],
+                  engine=[None, "text-davinci-003", "gpt-3.5-turbo", "gpt-4-32k-0314", "gpt-4-0314", "gpt-4"][0],
+                  enable_pdb=False, verbose=True, only_response=True,
+                  ):
         if model_version is not None:
             engine = self.model_version2engine[model_version]
         elif engine is not None:
             engine = engine
         else:
             engine = self.model_version2engine[self.model_version]
 
@@ -221,12 +224,12 @@
     nlp = NLP()
     sentences = nlp.sent_tokenize(raw_text)
     words = nlp.word_tokenize(sentences[0], lower=True)
     show_var(['sentences', 'words'])
 
     chat = Chatbot()
     query = 'What is the best way to learn Machine Learning?'
-    response = chat.query_with_patience(query)
+    response = chat.ask(query)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `efficiency-1.2/efficiency/plotter.py` & `efficiency-1.2.1/efficiency/plotter.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/record.py` & `efficiency-1.2.1/efficiency/record.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/text.py` & `efficiency-1.2.1/efficiency/text.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency/web.py` & `efficiency-1.2.1/efficiency/web.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.2/efficiency.egg-info/PKG-INFO` & `efficiency-1.2.1/efficiency.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficiency
-Version: 1.2
+Version: 1.2.1
 Summary: A package for efficient programming
 Home-page: https://github.com/zhijing-jin/efficiency
 Author: Zhijing Jin
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

