# Comparing `tmp/resoto-plugin-slack-3.4.0.tar.gz` & `tmp/resoto-plugin-slack-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-slack-3.4.0.tar", last modified: Thu Apr 27 11:23:55 2023, max compression
+gzip compressed data, was "resoto-plugin-slack-3.4.1.tar", last modified: Fri Apr 28 15:16:38 2023, max compression
```

## Comparing `resoto-plugin-slack-3.4.0.tar` & `resoto-plugin-slack-3.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:23:55.070667 resoto-plugin-slack-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 11:23:55.070667 resoto-plugin-slack-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:23:55.066667 resoto-plugin-slack-3.4.0/resoto_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:23:55.070667 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 11:23:55.000000 resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:23:55.070667 resoto-plugin-slack-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:23:55.070667 resoto-plugin-slack-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 11:22:13.000000 resoto-plugin-slack-3.4.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:38.894437 resoto-plugin-slack-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 15:16:38.894437 resoto-plugin-slack-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:38.890437 resoto-plugin-slack-3.4.1/resoto_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:38.890437 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 15:16:38.000000 resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:16:38.894437 resoto-plugin-slack-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:38.894437 resoto-plugin-slack-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-28 15:14:36.000000 resoto-plugin-slack-3.4.1/test/test_config.py
```

### Comparing `resoto-plugin-slack-3.4.0/PKG-INFO` & `resoto-plugin-slack-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Slack Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/slack
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-slack-3.4.0/resoto_plugin_slack/__init__.py` & `resoto-plugin-slack-3.4.1/resoto_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.4.0/resoto_plugin_slack/resources.py` & `resoto-plugin-slack-3.4.1/resoto_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.4.0/resoto_plugin_slack.egg-info/PKG-INFO` & `resoto-plugin-slack-3.4.1/resoto_plugin_slack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto Slack Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/slack
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-slack-3.4.0/setup.py` & `resoto-plugin-slack-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-slack",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto Slack Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": [
```

