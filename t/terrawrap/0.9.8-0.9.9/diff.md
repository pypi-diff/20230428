# Comparing `tmp/terrawrap-0.9.8.tar.gz` & `tmp/terrawrap-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/terrawrap-0.9.8.tar", last modified: Fri Jun 17 16:33:48 2022, max compression
+gzip compressed data, was "dist/terrawrap-0.9.9.tar", last modified: Tue Jun 28 19:00:05 2022, max compression
```

## Comparing `terrawrap-0.9.8.tar` & `terrawrap-0.9.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:48.000000 terrawrap-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (116)     3334 2022-06-17 16:33:47.000000 terrawrap-0.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)       93 2022-06-17 16:33:47.000000 terrawrap-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    14578 2022-06-17 16:33:48.000000 terrawrap-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    11558 2022-06-17 16:33:47.000000 terrawrap-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:48.000000 terrawrap-0.9.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)     2437 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/backend_check
--rwxr-xr-x   0 runner    (1001) docker     (116)     4758 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/graph_apply
--rwxr-xr-x   0 runner    (1001) docker     (116)     4635 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/pipeline_check
--rwxr-xr-x   0 runner    (1001) docker     (116)    16919 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/plan_check
--rwxr-xr-x   0 runner    (1001) docker     (116)     9784 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/tf
--rwxr-xr-x   0 runner    (1001) docker     (116)     1984 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/tf_apply
--rwxr-xr-x   0 runner    (1001) docker     (116)     2447 2022-06-17 16:33:47.000000 terrawrap-0.9.8/bin/visualize
--rw-r--r--   0 runner    (1001) docker     (116)      403 2022-06-17 16:33:47.000000 terrawrap-0.9.8/requirements.pip
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-17 16:33:48.000000 terrawrap-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2580 2022-06-17 16:33:47.000000 terrawrap-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap/
--rw-r--r--   0 runner    (1001) docker     (116)       92 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      321 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap/models/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7756 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/models/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     4262 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/models/graph_entry.py
--rw-r--r--   0 runner    (1001) docker     (116)     5621 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/models/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     4106 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/models/pipeline_entry.py
--rw-r--r--   0 runner    (1001) docker     (116)     3084 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/models/wrapper_config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7842 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    15883 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (116)      920 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5149 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     2336 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (116)     4001 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     5352 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/plugin_download.py
--rw-r--r--   0 runner    (1001) docker     (116)     5187 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/tf_variables.py
--rw-r--r--   0 runner    (1001) docker     (116)     1915 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-06-17 16:33:47.000000 terrawrap-0.9.8/terrawrap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    14578 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      972 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      200 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2022-06-17 16:33:48.000000 terrawrap-0.9.8/terrawrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      305 2022-06-17 16:33:47.000000 terrawrap-0.9.8/test-requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:05.000000 terrawrap-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     3334 2022-06-28 19:00:04.000000 terrawrap-0.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)       93 2022-06-28 19:00:04.000000 terrawrap-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    14578 2022-06-28 19:00:05.000000 terrawrap-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    11558 2022-06-28 19:00:04.000000 terrawrap-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:05.000000 terrawrap-0.9.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2437 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/backend_check
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4758 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/graph_apply
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4635 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/pipeline_check
+-rwxr-xr-x   0 runner    (1001) docker     (116)    16919 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/plan_check
+-rwxr-xr-x   0 runner    (1001) docker     (116)     9784 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/tf
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1984 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/tf_apply
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2447 2022-06-28 19:00:04.000000 terrawrap-0.9.9/bin/visualize
+-rw-r--r--   0 runner    (1001) docker     (116)      428 2022-06-28 19:00:04.000000 terrawrap-0.9.9/requirements.pip
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-28 19:00:05.000000 terrawrap-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2580 2022-06-28 19:00:04.000000 terrawrap-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap/
+-rw-r--r--   0 runner    (1001) docker     (116)       92 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap/models/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7756 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/models/graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4262 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/models/graph_entry.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5621 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/models/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4106 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/models/pipeline_entry.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3084 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/models/wrapper_config.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8115 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15883 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (116)      920 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5149 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2336 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4001 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5352 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/plugin_download.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5187 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/tf_variables.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1915 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2022-06-28 19:00:04.000000 terrawrap-0.9.9/terrawrap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    14578 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      972 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      225 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2022-06-28 19:00:05.000000 terrawrap-0.9.9/terrawrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      305 2022-06-28 19:00:04.000000 terrawrap-0.9.9/test-requirements.pip
```

### Comparing `terrawrap-0.9.8/CHANGELOG.md` & `terrawrap-0.9.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/PKG-INFO` & `terrawrap-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrawrap
-Version: 0.9.8
+Version: 0.9.9
 Summary: Set of Python-based CLI tools for working with Terraform configurations
 Home-page: https://github.com/amplify-education/terrawrap
 Author: Amplify Education
 Author-email: github@amplify.com
 License: MIT
 Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/e8bf52c80edf4070a18d8725b1f5f166)](https://app.codacy.com/app/amplify-education/terrawrap?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/terrawrap&utm_campaign=Badge_Grade_Settings)
         [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/ceeb459250dd429f9ca5a497c0e45051)](https://www.codacy.com/app/amplify-education/terrawrap?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/terrawrap&utm_campaign=Badge_Coverage)
```

### Comparing `terrawrap-0.9.8/README.md` & `terrawrap-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/backend_check` & `terrawrap-0.9.9/bin/backend_check`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/graph_apply` & `terrawrap-0.9.9/bin/graph_apply`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/pipeline_check` & `terrawrap-0.9.9/bin/pipeline_check`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/plan_check` & `terrawrap-0.9.9/bin/plan_check`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/tf` & `terrawrap-0.9.9/bin/tf`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/tf_apply` & `terrawrap-0.9.9/bin/tf_apply`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/bin/visualize` & `terrawrap-0.9.9/bin/visualize`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/setup.py` & `terrawrap-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/models/graph.py` & `terrawrap-0.9.9/terrawrap/models/graph.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/models/graph_entry.py` & `terrawrap-0.9.9/terrawrap/models/graph_entry.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/models/pipeline.py` & `terrawrap-0.9.9/terrawrap/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/models/pipeline_entry.py` & `terrawrap-0.9.9/terrawrap/models/pipeline_entry.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/models/wrapper_config.py` & `terrawrap-0.9.9/terrawrap/models/wrapper_config.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/cli.py` & `terrawrap-0.9.9/terrawrap/utils/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from enum import Enum
 
 from typing import List, Tuple, Union
 
 import requests
 
 from amplify_aws_utils.resource_helper import Jitter
+from aws_requests_auth.boto_utils import BotoAWSRequestsAuth
 
 from terrawrap.utils.git_utils import get_git_root
 
 logger = logging.getLogger(__name__)
 
 MAX_RETRIES = 5
 RETRIABLE_ERRORS = [
@@ -225,19 +226,28 @@
     except Exception:
         user = 'System'
 
     logger.info('Attempting to send data to Audit API: %s run by %s(%s)', path, user, status)
 
     url = (audit_api_url + AUDIT_UPDATE_PATH) if update else (audit_api_url + AUDIT_POST_PATH)
 
+    auth = BotoAWSRequestsAuth(
+        aws_host='terraform-audit-api.devops.amplify.com',
+        aws_region='us-west-2',
+        aws_service='execute-api'
+    )
+
     try:
         requests.post(
-            url, json={
+            url=url,
+            auth=auth,
+            json={
                 'directory': path,
                 'start_time': start_time,
                 'status': status,
                 'run_by': user,
                 'output': stdout
-            })
+            }
+        )
         logger.info('Successfully posted data to provided url: %s', audit_api_url)
     except requests.exceptions.RequestException:
         logger.error("Unable to post data to provided url: %s", audit_api_url)
```

### Comparing `terrawrap-0.9.8/terrawrap/utils/collection_utils.py` & `terrawrap-0.9.9/terrawrap/utils/collection_utils.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/config.py` & `terrawrap-0.9.9/terrawrap/utils/config.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/dynamodb.py` & `terrawrap-0.9.9/terrawrap/utils/dynamodb.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/git_utils.py` & `terrawrap-0.9.9/terrawrap/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/graph.py` & `terrawrap-0.9.9/terrawrap/utils/graph.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/module.py` & `terrawrap-0.9.9/terrawrap/utils/module.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/path.py` & `terrawrap-0.9.9/terrawrap/utils/path.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/plugin_download.py` & `terrawrap-0.9.9/terrawrap/utils/plugin_download.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/tf_variables.py` & `terrawrap-0.9.9/terrawrap/utils/tf_variables.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap/utils/version.py` & `terrawrap-0.9.9/terrawrap/utils/version.py`

 * *Files identical despite different names*

### Comparing `terrawrap-0.9.8/terrawrap.egg-info/PKG-INFO` & `terrawrap-0.9.9/terrawrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrawrap
-Version: 0.9.8
+Version: 0.9.9
 Summary: Set of Python-based CLI tools for working with Terraform configurations
 Home-page: https://github.com/amplify-education/terrawrap
 Author: Amplify Education
 Author-email: github@amplify.com
 License: MIT
 Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/e8bf52c80edf4070a18d8725b1f5f166)](https://app.codacy.com/app/amplify-education/terrawrap?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/terrawrap&utm_campaign=Badge_Grade_Settings)
         [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/ceeb459250dd429f9ca5a497c0e45051)](https://www.codacy.com/app/amplify-education/terrawrap?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/terrawrap&utm_campaign=Badge_Coverage)
```

### Comparing `terrawrap-0.9.8/terrawrap.egg-info/SOURCES.txt` & `terrawrap-0.9.9/terrawrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

