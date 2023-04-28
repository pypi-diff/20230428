# Comparing `tmp/frigate-0.7.0a0.post0.dev38.tar.gz` & `tmp/frigate-0.8.0a0.post0.dev39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frigate-0.7.0a0.post0.dev38.tar", last modified: Thu Mar 30 12:55:13 2023, max compression
+gzip compressed data, was "frigate-0.8.0a0.post0.dev39.tar", last modified: Fri Apr 28 19:15:24 2023, max compression
```

## Comparing `frigate-0.7.0a0.post0.dev38.tar` & `frigate-0.8.0a0.post0.dev39.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/frigate/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/frigate/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/pre_commit_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/frigate/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/sphinx/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/frigate/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/templates/base.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/templates/html.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/templates/markdown.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/templates/rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/frigate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/frigate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 12:55:13.000000 frigate-0.7.0a0.post0.dev38/frigate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-30 12:55:13.626857 frigate-0.7.0a0.post0.dev38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68767 2023-03-30 12:55:00.000000 frigate-0.7.0a0.post0.dev38/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/frigate/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/frigate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/pre_commit_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/frigate/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/sphinx/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/frigate/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/templates/base.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/templates/html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/templates/markdown.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/templates/rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/frigate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/frigate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 19:15:23.000000 frigate-0.8.0a0.post0.dev39/frigate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 19:15:24.030055 frigate-0.8.0a0.post0.dev39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68767 2023-04-28 19:15:11.000000 frigate-0.8.0a0.post0.dev39/versioneer.py
```

### Comparing `frigate-0.7.0a0.post0.dev38/LICENSE` & `frigate-0.8.0a0.post0.dev39/LICENSE`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/PKG-INFO` & `frigate-0.8.0a0.post0.dev39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigate
-Version: 0.7.0a0.post0.dev38
+Version: 0.8.0a0.post0.dev39
 Summary: A tool for autogenerating helm documentation.
 Home-page: 
 Download-URL: 
 Author: Jacob Tomlinson
 Author-email: jtomlinson@nvidia.com
 License: Apache License 2.0
 Platform: any
```

### Comparing `frigate-0.7.0a0.post0.dev38/README.md` & `frigate-0.8.0a0.post0.dev39/README.md`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/cli.py` & `frigate-0.8.0a0.post0.dev39/frigate/cli.py`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/gen.py` & `frigate-0.8.0a0.post0.dev39/frigate/gen.py`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/pre_commit_hook.py` & `frigate-0.8.0a0.post0.dev39/frigate/pre_commit_hook.py`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/sphinx/ext.py` & `frigate-0.8.0a0.post0.dev39/frigate/sphinx/ext.py`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/templates/html.jinja2` & `frigate-0.8.0a0.post0.dev39/frigate/templates/html.jinja2`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/templates/markdown.jinja2` & `frigate-0.8.0a0.post0.dev39/frigate/templates/markdown.jinja2`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/templates/rst.jinja2` & `frigate-0.8.0a0.post0.dev39/frigate/templates/rst.jinja2`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate/utils.py` & `frigate-0.8.0a0.post0.dev39/frigate/utils.py`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/frigate.egg-info/PKG-INFO` & `frigate-0.8.0a0.post0.dev39/frigate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigate
-Version: 0.7.0a0.post0.dev38
+Version: 0.8.0a0.post0.dev39
 Summary: A tool for autogenerating helm documentation.
 Home-page: 
 Download-URL: 
 Author: Jacob Tomlinson
 Author-email: jtomlinson@nvidia.com
 License: Apache License 2.0
 Platform: any
```

### Comparing `frigate-0.7.0a0.post0.dev38/frigate.egg-info/SOURCES.txt` & `frigate-0.8.0a0.post0.dev39/frigate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/setup.py` & `frigate-0.8.0a0.post0.dev39/setup.py`

 * *Files identical despite different names*

### Comparing `frigate-0.7.0a0.post0.dev38/versioneer.py` & `frigate-0.8.0a0.post0.dev39/versioneer.py`

 * *Files identical despite different names*

