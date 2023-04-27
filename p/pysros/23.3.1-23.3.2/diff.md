# Comparing `tmp/pysros-23.3.1.tar.gz` & `tmp/pysros-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysros-23.3.1.tar", last modified: Fri Mar 17 22:30:59 2023, max compression
+gzip compressed data, was "pysros-23.3.2.tar", last modified: Thu Apr 27 23:30:05 2023, max compression
```

## Comparing `pysros-23.3.1.tar` & `pysros-23.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:30:59.166184 pysros-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-03-17 22:30:50.000000 pysros-23.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-17 22:30:59.166184 pysros-23.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-17 22:30:50.000000 pysros-23.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:30:59.166184 pysros-23.3.1/pysros/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    58667 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/management.py
--rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/model_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26080 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    46775 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/request_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-03-17 22:30:50.000000 pysros-23.3.1/pysros/yang_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:30:59.166184 pysros-23.3.1/pysros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 22:30:59.000000 pysros-23.3.1/pysros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 22:30:59.166184 pysros-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-17 22:30:50.000000 pysros-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:30:05.853163 pysros-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-04-27 23:29:55.000000 pysros-23.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-27 23:30:05.853163 pysros-23.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-27 23:29:55.000000 pysros-23.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:30:05.849163 pysros-23.3.2/pysros/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58667 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/model_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26080 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46775 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/request_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-04-27 23:29:55.000000 pysros-23.3.2/pysros/yang_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:30:05.853163 pysros-23.3.2/pysros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 23:30:05.000000 pysros-23.3.2/pysros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:30:05.853163 pysros-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 23:29:55.000000 pysros-23.3.2/setup.py
```

### Comparing `pysros-23.3.1/LICENSE.md` & `pysros-23.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/PKG-INFO` & `pysros-23.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.3.1
+Version: 23.3.2
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
```

### Comparing `pysros-23.3.1/README.md` & `pysros-23.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/errors.py` & `pysros-23.3.2/pysros/errors.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/exceptions.py` & `pysros-23.3.2/pysros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/identifier.py` & `pysros-23.3.2/pysros/identifier.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/management.py` & `pysros-23.3.2/pysros/management.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/model.py` & `pysros-23.3.2/pysros/model.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/model_builder.py` & `pysros-23.3.2/pysros/model_builder.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/model_path.py` & `pysros-23.3.2/pysros/model_path.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/model_walker.py` & `pysros-23.3.2/pysros/model_walker.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/pprint.py` & `pysros-23.3.2/pysros/pprint.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/request_data.py` & `pysros-23.3.2/pysros/request_data.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/singleton.py` & `pysros-23.3.2/pysros/singleton.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/tokenizer.py` & `pysros-23.3.2/pysros/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/wrappers.py` & `pysros-23.3.2/pysros/wrappers.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros/yang_type.py` & `pysros-23.3.2/pysros/yang_type.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.1/pysros.egg-info/PKG-INFO` & `pysros-23.3.2/pysros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.3.1
+Version: 23.3.2
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
```

### Comparing `pysros-23.3.1/setup.py` & `pysros-23.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pysros',
-    version='23.3.1',
+    version='23.3.2',
     packages=['pysros'],
     url='https://www.nokia.com',
     license='Copyright 2021 Nokia.  License available in the LICENSE.md file.',
     author='Nokia',
     author_email='',
     description='Python for the Nokia Service Router Operating Systems (pySROS)',
     project_urls={
```

