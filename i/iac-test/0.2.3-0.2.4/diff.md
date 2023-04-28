# Comparing `tmp/iac_test-0.2.3.tar.gz` & `tmp/iac_test-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_test-0.2.3.tar", max compression
+gzip compressed data, was "iac_test-0.2.4.tar", max compression
```

## Comparing `iac_test-0.2.3.tar` & `iac_test-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    16295 2023-04-23 20:17:04.012029 iac_test-0.2.3/LICENSE
--rw-r--r--   0        0        0     7337 2023-04-23 20:17:04.012029 iac_test-0.2.3/README.md
--rw-r--r--   0        0        0      394 2023-04-23 20:17:04.012029 iac_test-0.2.3/iac_test/__init__.py
--rw-r--r--   0        0        0      167 2023-04-23 20:17:04.012029 iac_test-0.2.3/iac_test/__main__.py
--rw-r--r--   0        0        0      218 2023-04-23 20:17:04.012029 iac_test-0.2.3/iac_test/ansible_vault.py
--rw-r--r--   0        0        0        0 2023-04-23 20:17:04.012029 iac_test-0.2.3/iac_test/cli/__init__.py
--rw-r--r--   0        0        0     1994 2023-04-23 20:17:04.016029 iac_test-0.2.3/iac_test/cli/main.py
--rw-r--r--   0        0        0     1832 2023-04-23 20:17:04.016029 iac_test-0.2.3/iac_test/cli/options.py
--rw-r--r--   0        0        0      512 2023-04-23 20:17:04.016029 iac_test-0.2.3/iac_test/pabot.py
--rw-r--r--   0        0        0     7976 2023-04-23 20:17:04.016029 iac_test-0.2.3/iac_test/robot_writer.py
--rw-r--r--   0        0        0     4943 2023-04-23 20:17:04.016029 iac_test-0.2.3/iac_test/yaml.py
--rw-r--r--   0        0        0     2004 2023-04-23 20:17:04.016029 iac_test-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8745 1970-01-01 00:00:00.000000 iac_test-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    16295 2023-04-28 20:00:39.495573 iac_test-0.2.4/LICENSE
+-rw-r--r--   0        0        0     7337 2023-04-28 20:00:39.495573 iac_test-0.2.4/README.md
+-rw-r--r--   0        0        0      394 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/__main__.py
+-rw-r--r--   0        0        0      218 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/ansible_vault.py
+-rw-r--r--   0        0        0        0 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/cli/__init__.py
+-rw-r--r--   0        0        0     1994 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/cli/main.py
+-rw-r--r--   0        0        0     1832 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/cli/options.py
+-rw-r--r--   0        0        0      512 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/pabot.py
+-rw-r--r--   0        0        0     8262 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/robot_writer.py
+-rw-r--r--   0        0        0     4943 2023-04-28 20:00:39.495573 iac_test-0.2.4/iac_test/yaml.py
+-rw-r--r--   0        0        0     2004 2023-04-28 20:00:39.495573 iac_test-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     8745 1970-01-01 00:00:00.000000 iac_test-0.2.4/PKG-INFO
```

### Comparing `iac_test-0.2.3/LICENSE` & `iac_test-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_test-0.2.3/README.md` & `iac_test-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `iac_test-0.2.3/iac_test/cli/main.py` & `iac_test-0.2.4/iac_test/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_test-0.2.3/iac_test/cli/options.py` & `iac_test-0.2.4/iac_test/cli/options.py`

 * *Files identical despite different names*

### Comparing `iac_test-0.2.3/iac_test/pabot.py` & `iac_test-0.2.4/iac_test/pabot.py`

 * *Files identical despite different names*

### Comparing `iac_test-0.2.3/iac_test/robot_writer.py` & `iac_test-0.2.4/iac_test/robot_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import importlib.util
 import json
 import logging
 import os
 import pathlib
 import re
+import shutil
 import sys
 from typing import Any, Dict, List
 
 from jinja2 import ChainableUndefined, Environment, FileSystemLoader  # type: ignore
 
 from iac_test import yaml
 
@@ -115,18 +116,23 @@
         for dir, _, files in os.walk(templates_path):
             for filename in files:
                 if (
                     ".robot" not in filename
                     and ".j2" not in filename
                     and ".resource" not in filename
                 ):
-                    logger.warning(
+                    logger.info(
                         "Skip file with unknown file extension (not one of .robot, .resource or .j2): %s",
                         os.path.join(dir, filename),
                     )
+                    out = os.path.join(
+                        output_path, os.path.relpath(dir, templates_path)
+                    )
+                    pathlib.Path(out).mkdir(parents=True, exist_ok=True)
+                    shutil.copy(os.path.join(dir, filename), out)
                     continue
                 rel = os.path.relpath(dir, templates_path)
                 t_path = os.path.join(rel, filename)
 
                 # search for directives
                 pattern = re.compile("{#(.+?)#}")
                 content = ""
```

### Comparing `iac_test-0.2.3/iac_test/yaml.py` & `iac_test-0.2.4/iac_test/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_test-0.2.3/pyproject.toml` & `iac_test-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://github.com/netascode/iac-test"
 homepage = "https://github.com/netascode/iac-test"
 license = "LICENSE"
 maintainers = ["Daniel Schmidt <danischm@cisco.com>"]
 name = "iac-test"
 readme = "README.md"
 repository = "https://github.com/netascode/iac-test"
-version = "0.2.3"
+version = "0.2.4"
 
 [tool.poetry.scripts]
 iac-test = "iac_test.cli.main:main"
 
 [tool.poetry.dependencies]
 Jinja2 = "^3.0.3"
 RESTinstance = "^1.3.0"
```

### Comparing `iac_test-0.2.3/PKG-INFO` & `iac_test-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-test
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI tool to render and execute Robot Framework tests using Jinja templating.
 Home-page: https://github.com/netascode/iac-test
 License: LICENSE
 Author: Daniel Schmidt
 Author-email: danischm@cisco.com
 Maintainer: Daniel Schmidt
 Maintainer-email: danischm@cisco.com
```

