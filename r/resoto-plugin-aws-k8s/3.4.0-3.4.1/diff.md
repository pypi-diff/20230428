# Comparing `tmp/resoto-plugin-aws-k8s-3.4.0.tar.gz` & `tmp/resoto-plugin-aws-k8s-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-k8s-3.4.0.tar", last modified: Thu Apr 27 11:22:15 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-k8s-3.4.1.tar", last modified: Fri Apr 28 15:15:17 2023, max compression
```

## Comparing `resoto-plugin-aws-k8s-3.4.0.tar` & `resoto-plugin-aws-k8s-3.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:15.862218 resoto-plugin-aws-k8s-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-27 11:22:15.862218 resoto-plugin-aws-k8s-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:15.858219 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:15.862218 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 11:22:15.000000 resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:22:15.866219 resoto-plugin-aws-k8s-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:15.862218 resoto-plugin-aws-k8s-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-27 11:19:57.000000 resoto-plugin-aws-k8s-3.4.0/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:17.840756 resoto-plugin-aws-k8s-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-28 15:15:17.840756 resoto-plugin-aws-k8s-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:17.836756 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:17.840756 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 15:15:17.000000 resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:15:17.840756 resoto-plugin-aws-k8s-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:17.840756 resoto-plugin-aws-k8s-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 15:13:00.000000 resoto-plugin-aws-k8s-3.4.1/test/test_collector.py
```

### Comparing `resoto-plugin-aws-k8s-3.4.0/PKG-INFO` & `resoto-plugin-aws-k8s-3.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto AWS-K8s Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s/__init__.py` & `resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-k8s-3.4.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO` & `resoto-plugin-aws-k8s-3.4.1/resoto_plugin_aws_k8s.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto AWS-K8s Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-k8s-3.4.0/setup.py` & `resoto-plugin-aws-k8s-3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-aws-k8s",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto AWS-K8s Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["aws_k8s_collector = resoto_plugin_aws_k8s:AWSK8sCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-aws-k8s-3.4.0/test/test_collector.py` & `resoto-plugin-aws-k8s-3.4.1/test/test_collector.py`

 * *Files identical despite different names*

