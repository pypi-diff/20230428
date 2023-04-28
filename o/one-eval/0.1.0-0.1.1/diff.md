# Comparing `tmp/one-eval-0.1.0.tar.gz` & `tmp/one-eval-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-eval-0.1.0.tar", last modified: Fri Apr 28 09:45:52 2023, max compression
+gzip compressed data, was "one-eval-0.1.1.tar", last modified: Fri Apr 28 09:50:23 2023, max compression
```

## Comparing `one-eval-0.1.0.tar` & `one-eval-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:45:52.406643 one-eval-0.1.0/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 one-eval-0.1.0/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2379 2023-04-28 09:45:52.406490 one-eval-0.1.0/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1956 2023-04-28 08:22:23.000000 one-eval-0.1.0/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:45:52.403471 one-eval-0.1.0/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 one-eval-0.1.0/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2463 2023-04-28 09:44:15.000000 one-eval-0.1.0/commands/one_api_eval_file.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2117 2023-04-28 09:43:29.000000 one-eval-0.1.0/commands/one_api_eval_one.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:45:52.404046 one-eval-0.1.0/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)       76 2023-04-28 09:44:10.000000 one-eval-0.1.0/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6728 2023-04-28 09:43:34.000000 one-eval-0.1.0/eval/one_ai_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:45:52.405040 one-eval-0.1.0/one_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2379 2023-04-28 09:45:52.000000 one-eval-0.1.0/one_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      473 2023-04-28 09:45:52.000000 one-eval-0.1.0/one_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-28 09:45:52.000000 one-eval-0.1.0/one_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)      127 2023-04-28 09:45:52.000000 one-eval-0.1.0/one_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       48 2023-04-28 09:45:52.000000 one-eval-0.1.0/one_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-04-28 09:45:52.000000 one-eval-0.1.0/one_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:45:52.405680 one-eval-0.1.0/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-28 09:38:25.000000 one-eval-0.1.0/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      860 2023-04-28 08:33:34.000000 one-eval-0.1.0/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     5526 2023-04-28 09:42:56.000000 one-eval-0.1.0/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-28 09:45:52.406695 one-eval-0.1.0/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1022 2023-04-28 08:54:16.000000 one-eval-0.1.0/setup.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:45:52.406174 one-eval-0.1.0/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 one-eval-0.1.0/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2819 2023-04-28 09:42:03.000000 one-eval-0.1.0/utils/data_utils.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:50:23.425610 one-eval-0.1.1/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 one-eval-0.1.1/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2379 2023-04-28 09:50:23.425465 one-eval-0.1.1/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1956 2023-04-28 08:22:23.000000 one-eval-0.1.1/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:50:23.422028 one-eval-0.1.1/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 one-eval-0.1.1/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2463 2023-04-28 09:44:15.000000 one-eval-0.1.1/commands/one_api_eval_file.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2117 2023-04-28 09:43:29.000000 one-eval-0.1.1/commands/one_api_eval_one.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:50:23.422582 one-eval-0.1.1/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       76 2023-04-28 09:44:10.000000 one-eval-0.1.1/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6728 2023-04-28 09:43:34.000000 one-eval-0.1.1/eval/one_ai_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:50:23.423825 one-eval-0.1.1/one_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2379 2023-04-28 09:50:23.000000 one-eval-0.1.1/one_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      473 2023-04-28 09:50:23.000000 one-eval-0.1.1/one_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-28 09:50:23.000000 one-eval-0.1.1/one_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)      113 2023-04-28 09:50:23.000000 one-eval-0.1.1/one_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       48 2023-04-28 09:50:23.000000 one-eval-0.1.1/one_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-04-28 09:50:23.000000 one-eval-0.1.1/one_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:50:23.424625 one-eval-0.1.1/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-28 09:38:25.000000 one-eval-0.1.1/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      860 2023-04-28 08:33:34.000000 one-eval-0.1.1/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5526 2023-04-28 09:42:56.000000 one-eval-0.1.1/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-28 09:50:23.425652 one-eval-0.1.1/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1008 2023-04-28 09:50:18.000000 one-eval-0.1.1/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-28 09:50:23.425140 one-eval-0.1.1/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 one-eval-0.1.1/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2819 2023-04-28 09:42:03.000000 one-eval-0.1.1/utils/data_utils.py
```

### Comparing `one-eval-0.1.0/LICENSE` & `one-eval-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/PKG-INFO` & `one-eval-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-eval
-Version: 0.1.0
+Version: 0.1.1
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/OneEval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-eval-0.1.0/README.md` & `one-eval-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/commands/one_api_eval_file.py` & `one-eval-0.1.1/commands/one_api_eval_file.py`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/commands/one_api_eval_one.py` & `one-eval-0.1.1/commands/one_api_eval_one.py`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/eval/one_ai_eval.py` & `one-eval-0.1.1/eval/one_ai_eval.py`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/one_eval.egg-info/PKG-INFO` & `one-eval-0.1.1/one_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-eval
-Version: 0.1.0
+Version: 0.1.1
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/OneEval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-eval-0.1.0/prompt_template/eval_prompt_template.json` & `one-eval-0.1.1/prompt_template/eval_prompt_template.json`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/prompt_template/prompter.py` & `one-eval-0.1.1/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `one-eval-0.1.0/setup.py` & `one-eval-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-eval",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     package_data={
       "prompt_template":["eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool"
         "pandas",
         "openpyxl",
         "tabulate",
         "XlsxWriter"
     ],
     entry_points={
         "console_scripts": [
-            "one-eval-file=oneapi.commands.one_api_eval_file:main",
-            "one-eval-line=oneapi.commands.one_api_eval_one:main",
+            "one-eval-file=commands.one_api_eval_file:main",
+            "one-eval-line=commands.one_api_eval_one:main",
         ]
     },
     description="Using only one line of commmands to evaluate multiple models",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/muximus3/OneEval",
     classifiers=[
```

### Comparing `one-eval-0.1.0/utils/data_utils.py` & `one-eval-0.1.1/utils/data_utils.py`

 * *Files identical despite different names*

