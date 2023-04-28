# Comparing `tmp/resoto-plugin-k8s-3.4.0.tar.gz` & `tmp/resoto-plugin-k8s-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.4.0.tar", last modified: Thu Apr 27 11:22:39 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.4.1.tar", last modified: Fri Apr 28 15:17:05 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.4.0.tar` & `resoto-plugin-k8s-3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:39.566432 resoto-plugin-k8s-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-27 11:22:39.566432 resoto-plugin-k8s-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:39.562432 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   104090 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:39.566432 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 11:22:39.000000 resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 11:22:39.566432 resoto-plugin-k8s-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-27 11:20:00.000000 resoto-plugin-k8s-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:05.184461 resoto-plugin-k8s-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-28 15:17:05.184461 resoto-plugin-k8s-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:05.184461 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104090 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:05.184461 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 15:17:05.000000 resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 15:17:05.188461 resoto-plugin-k8s-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-28 15:14:00.000000 resoto-plugin-k8s-3.4.1/setup.py
```

### Comparing `resoto-plugin-k8s-3.4.0/PKG-INFO` & `resoto-plugin-k8s-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Kubernetes Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.4.0/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.4.1/resoto_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.4.0/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.4.1/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Kubernetes Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.4.0/setup.py` & `resoto-plugin-k8s-3.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-k8s",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto Kubernetes Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["k8s_collector = resoto_plugin_k8s:KubernetesCollectorPlugin"]},
     include_package_data=True,
```

