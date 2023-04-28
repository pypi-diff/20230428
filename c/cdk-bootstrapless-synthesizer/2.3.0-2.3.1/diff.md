# Comparing `tmp/cdk-bootstrapless-synthesizer-2.3.0.tar.gz` & `tmp/cdk-bootstrapless-synthesizer-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-bootstrapless-synthesizer-2.3.0.tar", last modified: Wed Mar 22 02:20:55 2023, max compression
+gzip compressed data, was "cdk-bootstrapless-synthesizer-2.3.1.tar", last modified: Fri Apr 28 01:59:59 2023, max compression
```

## Comparing `cdk-bootstrapless-synthesizer-2.3.0.tar` & `cdk-bootstrapless-synthesizer-2.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:20:55.591617 cdk-bootstrapless-synthesizer-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-22 02:20:55.591617 cdk-bootstrapless-synthesizer-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 02:20:55.591617 cdk-bootstrapless-synthesizer-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:20:55.587617 cdk-bootstrapless-synthesizer-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:20:55.591617 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/
--rw-r--r--   0 runner    (1001) docker     (123)    89880 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:20:55.591617 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   160852 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/_jsii/cdk-bootstrapless-synthesizer@2.3.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 02:20:37.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 02:20:55.591617 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-22 02:20:54.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-22 02:20:55.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 02:20:55.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-22 02:20:55.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-22 02:20:55.000000 cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:59:59.975927 cdk-bootstrapless-synthesizer-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-28 01:59:59.975927 cdk-bootstrapless-synthesizer-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:59:59.975927 cdk-bootstrapless-synthesizer-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:59:59.971927 cdk-bootstrapless-synthesizer-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:59:59.971927 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    89880 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:59:59.975927 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160863 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/_jsii/cdk-bootstrapless-synthesizer@2.3.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:59:46.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:59:59.971927 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-28 01:59:59.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 01:59:59.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:59:59.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-28 01:59:59.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 01:59:59.000000 cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/top_level.txt
```

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/LICENSE` & `cdk-bootstrapless-synthesizer-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/PKG-INFO` & `cdk-bootstrapless-synthesizer-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-bootstrapless-synthesizer
-Version: 2.3.0
+Version: 2.3.1
 Summary: Generate directly usable AWS CloudFormation template with aws-cdk v2.
 Home-page: https://github.com/aws-samples/cdk-bootstrapless-synthesizer.git
 Author: wchaws
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-bootstrapless-synthesizer.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/README.md` & `cdk-bootstrapless-synthesizer-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/setup.py` & `cdk-bootstrapless-synthesizer-2.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-bootstrapless-synthesizer",
-    "version": "2.3.0",
+    "version": "2.3.1",
     "description": "Generate directly usable AWS CloudFormation template with aws-cdk v2.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-bootstrapless-synthesizer.git",
     "long_description_content_type": "text/markdown",
     "author": "wchaws",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_bootstrapless_synthesizer",
         "cdk_bootstrapless_synthesizer._jsii"
     ],
     "package_data": {
         "cdk_bootstrapless_synthesizer._jsii": [
-            "cdk-bootstrapless-synthesizer@2.3.0.jsii.tgz"
+            "cdk-bootstrapless-synthesizer@2.3.1.jsii.tgz"
         ],
         "cdk_bootstrapless_synthesizer": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer/__init__.py` & `cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/PKG-INFO` & `cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-bootstrapless-synthesizer
-Version: 2.3.0
+Version: 2.3.1
 Summary: Generate directly usable AWS CloudFormation template with aws-cdk v2.
 Home-page: https://github.com/aws-samples/cdk-bootstrapless-synthesizer.git
 Author: wchaws
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-bootstrapless-synthesizer.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-bootstrapless-synthesizer-2.3.0/src/cdk_bootstrapless_synthesizer.egg-info/SOURCES.txt` & `cdk-bootstrapless-synthesizer-2.3.1/src/cdk_bootstrapless_synthesizer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_bootstrapless_synthesizer/py.typed
 src/cdk_bootstrapless_synthesizer.egg-info/PKG-INFO
 src/cdk_bootstrapless_synthesizer.egg-info/SOURCES.txt
 src/cdk_bootstrapless_synthesizer.egg-info/dependency_links.txt
 src/cdk_bootstrapless_synthesizer.egg-info/requires.txt
 src/cdk_bootstrapless_synthesizer.egg-info/top_level.txt
 src/cdk_bootstrapless_synthesizer/_jsii/__init__.py
-src/cdk_bootstrapless_synthesizer/_jsii/cdk-bootstrapless-synthesizer@2.3.0.jsii.tgz
+src/cdk_bootstrapless_synthesizer/_jsii/cdk-bootstrapless-synthesizer@2.3.1.jsii.tgz
```

