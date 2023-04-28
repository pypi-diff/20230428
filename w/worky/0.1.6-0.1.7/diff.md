# Comparing `tmp/worky-0.1.6.tar.gz` & `tmp/worky-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worky-0.1.6.tar", max compression
+gzip compressed data, was "worky-0.1.7.tar", max compression
```

## Comparing `worky-0.1.6.tar` & `worky-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.6/LICENSE
--rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.6/README.md
--rw-r--r--   0        0        0      821 2023-04-27 13:58:26.636824 worky-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-27 13:17:33.681261 worky-0.1.6/worky/__init__.py
--rw-r--r--   0        0        0      121 2023-04-27 13:11:32.808745 worky-0.1.6/worky/__main__.py
--rw-r--r--   0        0        0     3618 2023-04-27 13:11:21.488772 worky-0.1.6/worky/main.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.6/worky/models/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.6/worky/models/config_model.py
--rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.6/worky/models/log_level.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.6/worky/utils/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.6/worky/utils/logger.py
--rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.6/worky/utils/util.py
--rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 worky-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.7/LICENSE
+-rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.7/README.md
+-rw-r--r--   0        0        0      838 2023-04-27 14:39:59.065300 worky-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-04-27 14:39:59.061967 worky-0.1.7/worky/__init__.py
+-rw-r--r--   0        0        0      121 2023-04-27 14:33:11.629893 worky-0.1.7/worky/__main__.py
+-rw-r--r--   0        0        0     3618 2023-04-27 13:11:21.488772 worky-0.1.7/worky/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.7/worky/models/__init__.py
+-rw-r--r--   0        0        0     1759 2023-04-27 14:40:49.885173 worky-0.1.7/worky/models/config_model.py
+-rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.7/worky/models/log_level.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.7/worky/utils/__init__.py
+-rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.7/worky/utils/logger.py
+-rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.7/worky/utils/util.py
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 worky-0.1.7/PKG-INFO
```

### Comparing `worky-0.1.6/LICENSE` & `worky-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `worky-0.1.6/README.md` & `worky-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `worky-0.1.6/pyproject.toml` & `worky-0.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "worky"
-version = "0.1.6"
+version = "0.1.7"
 description = "Worky is a tool that helps to define and load project workspaces."
 authors = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 maintainers = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 readme = "README.md"
 packages = [{ include = "worky" }]
 homepage = "https://github.com/ZappaBoy/worky"
 repository = "https://github.com/ZappaBoy/worky"
@@ -12,14 +12,15 @@
 keywords = ["worky", "productivity", "workspace", "initializer"]
 classifiers = [
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 poetry2setup = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `worky-0.1.6/worky/main.py` & `worky-0.1.7/worky/main.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.6/worky/models/config_model.py` & `worky-0.1.7/worky/models/config_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
-import tomllib
 from typing import List
 
+import toml  # replace with tomllib whet python 3.11 become stable
+
 expandable_variables_pattern = re.compile(r"\$\{.*}")
 excluded_steps_entries = ['variables']
 
 
 class Config:
     variables: dict = {}
     steps: List = []
@@ -14,16 +15,15 @@
         self.config_path = config_path
         config_file_content = self.read_config_file(config_path)
         self.read_variables(config_file_content)
         self.read_steps(config_file_content)
 
     @staticmethod
     def read_config_file(config_path: str):
-        with open(config_path, 'rb') as config_file:
-            return tomllib.load(config_file)
+        return toml.load(config_path)
 
     def read_steps(self, config_file_content):
         for key, value in config_file_content.items():
             if key not in excluded_steps_entries:
                 args = value['args'] if 'args' in value else []
                 args = [self.expand_variables(value) for value in args]
                 self.steps.append({
```

### Comparing `worky-0.1.6/worky/utils/logger.py` & `worky-0.1.7/worky/utils/logger.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.6/PKG-INFO` & `worky-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: worky
-Version: 0.1.6
+Version: 0.1.7
 Summary: Worky is a tool that helps to define and load project workspaces.
 Home-page: https://github.com/ZappaBoy/worky
 Keywords: worky,productivity,workspace,initializer
 Author: ZappaBoy
 Author-email: federico.zappone@justanother.cloud
 Maintainer: ZappaBoy
 Maintainer-email: federico.zappone@justanother.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://github.com/ZappaBoy/worky/blob/main/README.md
 Project-URL: Repository, https://github.com/ZappaBoy/worky
 Description-Content-Type: text/markdown
 
 # Worky
 Manage your workspaces and increase your productivity.
```

