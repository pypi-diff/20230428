# Comparing `tmp/spec_pilot-0.2.0.tar.gz` & `tmp/spec_pilot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec_pilot-0.2.0.tar", last modified: Wed Apr 26 16:41:34 2023, max compression
+gzip compressed data, was "spec_pilot-0.2.1.tar", last modified: Fri Apr 28 02:17:45 2023, max compression
```

## Comparing `spec_pilot-0.2.0.tar` & `spec_pilot-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/spec_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/spec_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/spec_pilot.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/spec_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/spec_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/spec_pilot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/validator.py
```

### Comparing `spec_pilot-0.2.0/LICENSE` & `spec_pilot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spec_pilot-0.2.0/PKG-INFO` & `spec_pilot-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec_pilot
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to generate OpenAPI specifications using natural language
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -74,14 +74,15 @@
 ```
 
 - Create a new OpenAPI asset from a template:
 
 ```bash
 spec_pilot --create template asset_name output_path
 ```
+## Generate and save your OpenAPI components using the corresponding functions
 
 ## Python Package Usage
 
 You can also use Spec-Pilot as a Python package in your projects. Here's an example of how to use it:
 
 ```python
 from spec_pilot import init_project, generate_openapi_spec, process_natural_language_input, vacuum, render_template
```

### Comparing `spec_pilot-0.2.0/README.md` & `spec_pilot-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ```
 
 - Create a new OpenAPI asset from a template:
 
 ```bash
 spec_pilot --create template asset_name output_path
 ```
+## Generate and save your OpenAPI components using the corresponding functions
 
 ## Python Package Usage
 
 You can also use Spec-Pilot as a Python package in your projects. Here's an example of how to use it:
 
 ```python
 from spec_pilot import init_project, generate_openapi_spec, process_natural_language_input, vacuum, render_template
```

### Comparing `spec_pilot-0.2.0/setup.py` & `spec_pilot-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         os.system("python -m spacy download en_core_web_sm")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="spec_pilot",
-    version="0.2.0",
+    version="0.2.1",
     author="jmfwolf",
     author_email="jmfwolf@hacksomniac.com",
     description="A tool to generate OpenAPI specifications using natural language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jmfwolf/spec-pilot",
     packages=find_packages(),
```

### Comparing `spec_pilot-0.2.0/spec_pilot.egg-info/PKG-INFO` & `spec_pilot-0.2.1/spec_pilot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to generate OpenAPI specifications using natural language
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -74,14 +74,15 @@
 ```
 
 - Create a new OpenAPI asset from a template:
 
 ```bash
 spec_pilot --create template asset_name output_path
 ```
+## Generate and save your OpenAPI components using the corresponding functions
 
 ## Python Package Usage
 
 You can also use Spec-Pilot as a Python package in your projects. Here's an example of how to use it:
 
 ```python
 from spec_pilot import init_project, generate_openapi_spec, process_natural_language_input, vacuum, render_template
```

### Comparing `spec_pilot-0.2.0/src/spec_parser.py` & `spec_pilot-0.2.1/src/spec_parser.py`

 * *Files identical despite different names*

### Comparing `spec_pilot-0.2.0/src/spec_pilot.py` & `spec_pilot-0.2.1/src/spec_pilot.py`

 * *Files identical despite different names*

### Comparing `spec_pilot-0.2.0/src/validator.py` & `spec_pilot-0.2.1/src/validator.py`

 * *Files identical despite different names*

