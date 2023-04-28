# Comparing `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.4.0.tar.gz` & `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.4.0.tar", last modified: Thu Apr 27 11:22:00 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.4.1.tar", last modified: Fri Apr 28 15:16:56 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0.tar` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.905083 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-27 11:22:00.905083 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.901083 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.905083 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 11:22:00.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:22:00.905083 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:00.905083 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 11:19:57.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:56.400824 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-28 15:16:56.400824 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:56.400824 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:56.400824 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 15:16:56.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:16:56.400824 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:56.400824 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 15:14:23.000000 resoto-plugin-cleanup-aws-loadbalancers-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.4.0
+Version: 3.4.1
 Summary: AWS Loadbalancers Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/README.md` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers/__init__.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers/config.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.4.0
+Version: 3.4.1
 Summary: AWS Loadbalancers Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.4.0/setup.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-aws-loadbalancers",
-    version="3.4.0",
+    version="3.4.1",
     description="AWS Loadbalancers Cleaner Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": [
```

