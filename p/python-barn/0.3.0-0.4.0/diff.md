# Comparing `tmp/python-barn-0.3.0.tar.gz` & `tmp/python-barn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barn-0.3.0.tar", last modified: Fri Apr  7 19:37:21 2023, max compression
+gzip compressed data, was "python-barn-0.4.0.tar", last modified: Fri Apr 28 10:38:31 2023, max compression
```

## Comparing `python-barn-0.3.0.tar` & `python-barn-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:37:21.866259 python-barn-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-07 19:37:21.866259 python-barn-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 19:37:12.000000 python-barn-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:37:21.862259 python-barn-0.3.0/python_barn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-07 19:37:21.000000 python-barn-0.3.0/python_barn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-07 19:37:21.000000 python-barn-0.3.0/python_barn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:37:21.000000 python-barn-0.3.0/python_barn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:37:21.000000 python-barn-0.3.0/python_barn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-07 19:37:21.000000 python-barn-0.3.0/python_barn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:37:21.866259 python-barn-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-07 19:37:12.000000 python-barn-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:37:21.862259 python-barn-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:37:21.866259 python-barn-0.3.0/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/actions/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/actions/execute_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/actions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:37:21.866259 python-barn-0.3.0/src/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/console/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-07 19:37:12.000000 python-barn-0.3.0/src/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.974480 python-barn-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 10:38:31.974480 python-barn-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 10:38:19.000000 python-barn-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.970480 python-barn-0.4.0/python_barn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:38:31.974480 python-barn-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-28 10:38:19.000000 python-barn-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.970480 python-barn-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.974480 python-barn-0.4.0/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/execute_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/core.py
```

### Comparing `python-barn-0.3.0/PKG-INFO` & `python-barn-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.3.0
+Version: 0.4.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.3.0/python_barn.egg-info/PKG-INFO` & `python-barn-0.4.0/python_barn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.3.0
+Version: 0.4.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.3.0/setup.py` & `python-barn-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-barn",
-    version="0.3.0",
+    version="0.4.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "barn=src.cli:main",
         ],
     },
     package_data={
```

### Comparing `python-barn-0.3.0/src/actions/init.py` & `python-barn-0.4.0/src/actions/init.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.3.0/src/cli.py` & `python-barn-0.4.0/src/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
-from src.actions import install, add, init, execute_script, remove
+from src.actions import install, add, init, execute_script, remove, show
 from src.core import barn_action, Context
 
 def main():
 
     title = r"""
 _________                   
 ______/ /_  ____ __________ 
@@ -33,45 +33,48 @@
     # Add 'add' command
     add_parser = subparsers.add_parser('add')
     add_parser.add_argument("requirement", help="The name of package to add, versioning is also supported")
     
     remove_parser = subparsers.add_parser('remove')
     remove_parser.add_argument("package_name", help="The name of package to add, versioning is also supported")
 
+    show_parser = subparsers.add_parser('show')
+    show_parser.add_argument("-v", "--verbose", help="extra text", action='store_true')
+    show_parser.add_argument("package_name", help="The name of package to show")
+    show_parser.add_argument("-f", "--files", help="Show the full list of files", action='store_true')
 
     subparsers.add_parser('test')
 
-
     # Parse the arguments
  
     args, unknown_args = parser.parse_known_args()
 
     if len(unknown_args) > 0:
         """
         Script time
         """
         execute_script(unknown_args[0])
 
     # If no command is given, print help and exit
     elif args.command is None:
         install()
-
-    elif args.command == 'test':
-        @barn_action
-        def test_action(context: Context=None):
-            # Do whatever here
-            context.add_dependency_to_project_yaml("test", "1.0.0")
-        test_action()
-
+    elif args.command == 'show':
+        show(args.package_name, verbose=args.verbose, files=args.files)
     elif args.command == 'install':
         install()
     elif args.command == 'remove':
         remove(args.package_name)
     elif args.command == 'add':
         add(args.requirement)
     elif args.command == 'init':
         init()
+    elif args.command == 'test':
+        @barn_action
+        def test_action(context: Context=None):
+            # Do whatever here
+            context.add_dependency_to_project_yaml("test", "1.0.0")
+        test_action()
     else:
         print("Unknown command: " + args.command)
 
 # if __name__ == "__main__":
 #     main()
```

### Comparing `python-barn-0.3.0/src/core.py` & `python-barn-0.4.0/src/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,15 +93,18 @@
     def get_dependencies_from_project_yaml(self):
         dependencies = self.get_project_dependencies()
 
         requirements = []
         for dependency in dependencies:
             package_name = list(dependency.keys())[0]
             version = dependency[package_name]
-            requirements.append(f"{package_name}{version}")
+            if version == "N/A":
+                requirements.append(package_name)
+            else:
+                requirements.append(f"{package_name}{version}")
         return requirements
 
     def freeze_lock(self):
         stdout, exit_code = self.run_command_in_context(
             "pip freeze > ./barn.lock"
         )
 
@@ -114,20 +117,25 @@
     def get_project_config(self):
         # Load the YAML file
         with open(self.project_yaml_path, 'r') as yaml_file:
             yaml_content = yaml.safe_load(yaml_file)
 
         return yaml_content
     
-    def add_dependency_to_project_yaml(self, package, version):
+    def add_dependency_to_project_yaml(self, package, version=None, is_url=False):
         yaml_content = self.get_project_config()
-        new_entry = {
-            package: version
-        }
-
+        if is_url:
+            new_entry = {
+                package: f"N/A"
+            }
+        else:
+            new_entry = {
+                package: version
+            }
+            
         if "dependencies" not in yaml_content:
             yaml_content["dependencies"] = []
 
         dependencies: list[any] = yaml_content["dependencies"]
         if new_entry not in dependencies:
             yaml_content["dependencies"].append(new_entry)
             with open(self.project_yaml_path, 'w') as yaml_file:
```

