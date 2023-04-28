# Comparing `tmp/resotometrics-3.4.0.tar.gz` & `tmp/resotometrics-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.4.0.tar", last modified: Thu Apr 27 11:22:11 2023, max compression
+gzip compressed data, was "resotometrics-3.4.1.tar", last modified: Fri Apr 28 15:13:22 2023, max compression
```

## Comparing `resotometrics-3.4.0.tar` & `resotometrics-3.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:11.037708 resotometrics-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 11:20:00.000000 resotometrics-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-27 11:22:11.037708 resotometrics-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-27 11:20:00.000000 resotometrics-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:20:00.000000 resotometrics-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:11.029708 resotometrics-3.4.0/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 11:20:00.000000 resotometrics-3.4.0/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-27 11:20:00.000000 resotometrics-3.4.0/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-27 11:20:00.000000 resotometrics-3.4.0/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-27 11:20:00.000000 resotometrics-3.4.0/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 11:20:00.000000 resotometrics-3.4.0/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-27 11:20:00.000000 resotometrics-3.4.0/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:11.033708 resotometrics-3.4.0/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 11:22:11.000000 resotometrics-3.4.0/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:22:11.037708 resotometrics-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-27 11:20:00.000000 resotometrics-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:11.037708 resotometrics-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-27 11:20:00.000000 resotometrics-3.4.0/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:22.130953 resotometrics-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 15:11:42.000000 resotometrics-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-28 15:13:22.130953 resotometrics-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-28 15:11:42.000000 resotometrics-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:11:42.000000 resotometrics-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:22.130953 resotometrics-3.4.1/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 15:11:42.000000 resotometrics-3.4.1/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-28 15:11:42.000000 resotometrics-3.4.1/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-28 15:11:42.000000 resotometrics-3.4.1/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-28 15:11:42.000000 resotometrics-3.4.1/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 15:11:42.000000 resotometrics-3.4.1/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-28 15:11:42.000000 resotometrics-3.4.1/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:22.130953 resotometrics-3.4.1/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 15:13:22.000000 resotometrics-3.4.1/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:13:22.130953 resotometrics-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-28 15:11:42.000000 resotometrics-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:22.130953 resotometrics-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 15:11:42.000000 resotometrics-3.4.1/test/test_args.py
```

### Comparing `resotometrics-3.4.0/PKG-INFO` & `resotometrics-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.4.0
+Version: 3.4.1
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -204,15 +204,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotometrics-3.4.0/README.md` & `resotometrics-3.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotometrics-3.4.0/resotometrics/__main__.py` & `resotometrics-3.4.1/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.0/resotometrics/config.py` & `resotometrics-3.4.1/resotometrics/config.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.0/resotometrics/default_metrics.yaml` & `resotometrics-3.4.1/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.0/resotometrics/metrics.py` & `resotometrics-3.4.1/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.0/resotometrics/search.py` & `resotometrics-3.4.1/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.0/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.4.1/resotometrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.4.0
+Version: 3.4.1
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -204,15 +204,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotometrics-3.4.0/setup.py` & `resotometrics-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.0/test/test_args.py` & `resotometrics-3.4.1/test/test_args.py`

 * *Files identical despite different names*

