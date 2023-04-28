# Comparing `tmp/scpkit-0.1.3.tar.gz` & `tmp/scpkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.1.3.tar", last modified: Wed Apr 26 20:54:30 2023, max compression
+gzip compressed data, was "scpkit-0.2.0.tar", last modified: Fri Apr 28 19:53:59 2023, max compression
```

## Comparing `scpkit-0.1.3.tar` & `scpkit-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.232133 scpkit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 20:54:05.000000 scpkit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-26 20:54:30.232133 scpkit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-26 20:54:05.000000 scpkit-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 20:54:05.000000 scpkit-0.1.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.228132 scpkit-0.1.3/scpkit/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.232133 scpkit-0.1.3/scpkit/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-26 20:54:05.000000 scpkit-0.1.3/scpkit/src/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.228132 scpkit-0.1.3/scpkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 20:54:30.000000 scpkit-0.1.3/scpkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 20:54:30.232133 scpkit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:54:05.000000 scpkit-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:54:30.232133 scpkit-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-26 20:54:05.000000 scpkit-0.1.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.817956 scpkit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 19:53:48.000000 scpkit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-28 19:53:59.817956 scpkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-28 19:53:48.000000 scpkit-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 19:53:48.000000 scpkit-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.813955 scpkit-0.2.0/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.817956 scpkit-0.2.0/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.813955 scpkit-0.2.0/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 19:53:59.817956 scpkit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:53:48.000000 scpkit-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.817956 scpkit-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-28 19:53:48.000000 scpkit-0.2.0/tests/test.py
```

### Comparing `scpkit-0.1.3/LICENSE` & `scpkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.3/PKG-INFO` & `scpkit-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.1.3
+Version: 0.2.0
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
-This project provides a python module to aid in Service Control Policy management in AWS accounts. See our release [blog](https://blog.aquia.us/blog/) for additional details.
+This project provides a python module to aid in Service Control Policy management in AWS accounts.
 
 SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
```

### Comparing `scpkit-0.1.3/README.md` & `scpkit-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
-This project provides a python module to aid in Service Control Policy management in AWS accounts. See our release [blog](https://blog.aquia.us/blog/) for additional details.
+This project provides a python module to aid in Service Control Policy management in AWS accounts.
 
 SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
```

### Comparing `scpkit-0.1.3/scpkit/main.py` & `scpkit-0.2.0/scpkit/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """SCPkit
 Usage:
     main.py (validate | merge) [--sourcefiles sourcefiles] [--profile profile] [ --outdir outdir] [--validate-after-merge] [--readable]
 
 Options:
     -h --help                   Show this screen.
     --version                   Show version.
-    --sourcefiles sourcefiles   Directory path to SCP files in json format
+    --sourcefiles sourcefiles   Directory path to SCP files in json format or a single SCP file
     --outdir outdir             Directory to write new SCP files [Default: ./]
     --profile profile           AWS profile name
     --validate-after-merge      Validate the policies after merging them
     --readable                  Leave indentation and some whitespace to make the SCPs readable
 """
 from docopt import docopt
 from .src.validate import validate_policies
-from .src.merge import scp_merge, get_files_in_dir
+from .src.merge import scp_merge
+from .src.util import get_files_in_dir
 
 def main():
     arguments = {
         k.lstrip('-'): v for k, v in docopt(__doc__).items()
     }
 
     arguments['scps'] = get_files_in_dir(arguments["sourcefiles"])
```

### Comparing `scpkit-0.1.3/scpkit/src/merge.py` & `scpkit-0.2.0/scpkit/src/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .util import write_json, find_key_in_json, load_json, make_actions_and_resources_lists, dump_json
+from .util import write_json, find_key_in_json, load_json, make_actions_and_resources_lists, dump_json, get_files_in_dir
 from copy import deepcopy
 from pathlib import Path
 from .model import SCP
 from .validate import validate_policies
 from itertools import groupby
 
 def sort_list_of_dicts(content):
@@ -82,27 +82,14 @@
     write_json(new_policies, kwargs['outdir'], readable=kwargs.get("readable"))
 
     if kwargs.get("validate-after-merge"):
         scps = [ SCP(name=i, content=scp) for i, scp in enumerate(new_policies, 1) ]
         validate_policies(scps, kwargs['profile'], kwargs['outdir'])
 
 
-def get_files_in_dir(folder):
-    """Loads all JSON files from a directory
-    Args:
-        folder (str): Folder that contains JSON files
-    Returns:
-        [list]: list of JSON content from all files
-    """
-
-    p = Path(folder)
-    all_content = [ SCP(name=file.name, content=load_json(file)) for file in list(p.glob('**/*.json')) ]
-    return all_content
-
-
 def combine_similar_sids(content):
     """Combines SIDs that have the same Resource, Effect, and Condition (if exists)
 
     Args:
         content (list): List of SCP dictionaries
 
     Returns:
```

### Comparing `scpkit-0.1.3/scpkit/src/model.py` & `scpkit-0.2.0/scpkit/src/model.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.3/scpkit/src/util.py` & `scpkit-0.2.0/scpkit/src/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from pathlib import Path
+from .model import SCP
 
 
 def load_json(filepath):
     """Loads json content from files
     Args:
         filepath (str): Path to a file containing json
     Returns:
@@ -45,24 +46,35 @@
     """
     if readable:
         return json.dumps(content, indent=2)
     else:
         return json.dumps(content)
 
 
-def get_filepaths_in_dir(folder):
-    """Loads all JSON filepaths from a directory
+def get_files_in_dir(filepath):
+    """Loads all JSON files from a directory
     Args:
-        folder (str): Folder that contains JSON files
+        filepath (str): Folder that contains JSON files or an individual json file
     Returns:
-        [list]: list of JSON files in a directory
+        [list]: list of JSON content from all files
     """
 
-    p = Path(folder)
-    all_content = [ file for file in list(p.glob('**/*.json')) ]
+    p = Path(filepath)
+
+    if not p.exists():
+        raise FileNotFoundError(f"The file {p} does not exist.")
+
+    if p.is_dir(): 
+        p = list(p.glob('**/*.json'))
+    elif p.is_file():
+        p = [p]
+    else:
+        raise Exception
+
+    all_content = [ SCP(name=file.name, content=load_json(file)) for file in p ]
     return all_content
 
 
 def find_key_in_json(content, key_to_find):
     """Recursive function to find a key 
     Args:
         content ([dict]): IAM Policy document
```

### Comparing `scpkit-0.1.3/scpkit/src/validate.py` & `scpkit-0.2.0/scpkit/src/validate.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.3/scpkit.egg-info/PKG-INFO` & `scpkit-0.2.0/scpkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.1.3
+Version: 0.2.0
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # SCPkit
 [![GitHub Super-Linter](https://github.com/aquia-inc/scpkit/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/aquia-inc/scpkit/actions/workflows/linter.yaml)
 
 ## Overview
 
-This project provides a python module to aid in Service Control Policy management in AWS accounts. See our release [blog](https://blog.aquia.us/blog/) for additional details.
+This project provides a python module to aid in Service Control Policy management in AWS accounts.
 
 SCPs have a current limit of 5 total per entity, and a size limit on each of 5120 bytes. This tool will merge selected SCPs into the fewest amount of policies, and optionally remove whitespace characters as they count toward the byte limit.
 
 
 ```mermaid
   stateDiagram-v2
       [SCPTool] --> Validate
```

### Comparing `scpkit-0.1.3/setup.cfg` & `scpkit-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aquia-inc/scpkit/issues
 	Source = https://github.com/aquia-inc/scpkit
 description = This package helps consolidate service control policies in AWS
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.1.3
+version = 0.2.0
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `scpkit-0.1.3/tests/test.py` & `scpkit-0.2.0/tests/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Unit tests
 """
 
 import pytest #pylint: disable=import-errors
 
-from scpkit.src.util import find_key_in_json
+from scpkit.src.util import find_key_in_json, get_files_in_dir, load_json
 from scpkit.src.merge import sort_list_of_dicts, merge_json, combine_similar_sids
 
 
 test_scp_1 = {
     "Version": "2012-10-17",
     "Statement": [
         {
@@ -150,7 +150,16 @@
                         "organizations:LeaveOrganization"],
                     "Resource": ["*"],
                     "Effect": "Deny"
                 }
                 ]
     scps = combine_similar_sids(test_data)
     assert result == scps
+
+
+def test_get_files_in_dir():
+    f = get_files_in_dir("./tests/testfiles")
+    assert len(f) == 2
+
+def test_get_file_in_dir():
+    f = get_files_in_dir("./tests/testfiles/test-scp-1.json")
+    assert len(f) == 1
```

