# Comparing `tmp/skeletonkey-0.0.10.tar.gz` & `tmp/skeletonkey-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.0.10.tar", last modified: Fri Apr 28 01:45:56 2023, max compression
+gzip compressed data, was "skeletonkey-0.0.11.tar", last modified: Fri Apr 28 02:06:21 2023, max compression
```

## Comparing `skeletonkey-0.0.10.tar` & `skeletonkey-0.0.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 01:45:56.006215 skeletonkey-0.0.10/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-04-27 04:50:50.000000 skeletonkey-0.0.10/LICENSE
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1627 2023-04-28 01:45:55.994215 skeletonkey-0.0.10/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1142 2023-04-27 16:49:28.000000 skeletonkey-0.0.10/README.md
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-04-28 01:45:56.018216 skeletonkey-0.0.10/setup.cfg
--rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)      710 2023-04-28 01:44:47.000000 skeletonkey-0.0.10/setup.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 01:45:55.758203 skeletonkey-0.0.10/skeletonkey/
--rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)     5036 2023-04-28 00:03:50.000000 skeletonkey-0.0.10/skeletonkey/__init__.py
--rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)     6367 2023-04-28 00:17:00.000000 skeletonkey-0.0.10/skeletonkey/utils.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 01:45:55.930212 skeletonkey-0.0.10/skeletonkey.egg-info/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1627 2023-04-28 01:45:55.000000 skeletonkey-0.0.10/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      211 2023-04-28 01:45:55.000000 skeletonkey-0.0.10/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-04-28 01:45:55.000000 skeletonkey-0.0.10/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-04-28 01:45:55.000000 skeletonkey-0.0.10/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 02:06:21.565911 skeletonkey-0.0.11/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-04-27 04:50:50.000000 skeletonkey-0.0.11/LICENSE
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1667 2023-04-28 02:06:21.553910 skeletonkey-0.0.11/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1176 2023-04-28 01:59:03.000000 skeletonkey-0.0.11/README.md
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-04-28 02:06:21.593912 skeletonkey-0.0.11/setup.cfg
+-rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)      718 2023-04-28 02:05:55.000000 skeletonkey-0.0.11/setup.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 02:06:21.045885 skeletonkey-0.0.11/skeletonkey/
+-rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)     5043 2023-04-28 01:55:09.000000 skeletonkey-0.0.11/skeletonkey/__init__.py
+-rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)     6367 2023-04-28 00:17:00.000000 skeletonkey-0.0.11/skeletonkey/utils.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 02:06:21.393902 skeletonkey-0.0.11/skeletonkey.egg-info/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1667 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      211 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.0.10/LICENSE` & `skeletonkey-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.0.10/PKG-INFO` & `skeletonkey-0.0.11/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.0.10
+Version: 0.0.11
 Summary: A bare-bones configuration managment tool.
-Home-page: https://github.com/sizemore0125/bones
+Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bones: A Bare-bones Configuration Management Tool
+# SkeletonKey: A Bare-bones Configuration Management Tool
 
-Bones is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
+`skeletonkey` is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
 
 ### Usage
 
-Below is an example of how to use Bones in your project:
+Below is an example of how to use `skeletonkey` in your project:
 
 ```python
-import bones
+import skeletonkey
 
 class MyModel:
     def __init__(self, layer_size: int, activation: str) -> None:
         self.layer_size = layer_size
         self.activation = activation
 
-@bones.skeleton_key("config.yaml")
+@skeletonkey.unlock("config.yaml")
 def main(args):
-    model = bones.instantiate(args.model)
+    model = skeletonkey.instantiate(args.model)
     print("Model layer size: ", model.layer_size)
     print("Model activation: ", model.activation)
     print("Number of Epochs: ", args.epochs)
 
 if __name__ == "__main__":  
     main()
 ```
```

### Comparing `skeletonkey-0.0.10/README.md` & `skeletonkey-0.0.11/skeletonkey.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-# bones: A Bare-bones Configuration Management Tool
+Metadata-Version: 2.1
+Name: skeletonkey
+Version: 0.0.11
+Summary: A bare-bones configuration managment tool.
+Home-page: https://github.com/sizemore0125/skeletonkey
+Author: Logan Sizemore
+Author-email: sizemore0125@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Bones is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
+# SkeletonKey: A Bare-bones Configuration Management Tool
+
+`skeletonkey` is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
 
 ### Usage
 
-Below is an example of how to use Bones in your project:
+Below is an example of how to use `skeletonkey` in your project:
 
 ```python
-import bones
+import skeletonkey
 
 class MyModel:
     def __init__(self, layer_size: int, activation: str) -> None:
         self.layer_size = layer_size
         self.activation = activation
 
-@bones.skeleton_key("config.yaml")
+@skeletonkey.unlock("config.yaml")
 def main(args):
-    model = bones.instantiate(args.model)
+    model = skeletonkey.instantiate(args.model)
     print("Model layer size: ", model.layer_size)
     print("Model activation: ", model.activation)
     print("Number of Epochs: ", args.epochs)
 
 if __name__ == "__main__":  
     main()
 ```
@@ -33,7 +49,9 @@
   layer_size: 128
   activation: relu
 ```
 To run the script and overwrite default arguments, use the command:
 ```bash
 python project.py --epochs 256
 ```
+
+
```

### Comparing `skeletonkey-0.0.10/setup.py` & `skeletonkey-0.0.11/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.0.10",
+    version="0.0.11",
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/sizemore0125/bones",
+    url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
-)
+)
```

### Comparing `skeletonkey-0.0.10/skeletonkey/__init__.py` & `skeletonkey-0.0.11/skeletonkey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,44 +13,47 @@
 import inspect
 import os
 import sys
 from typing import Callable, Optional, Type, Any, Dict
 
 from .utils import open_yaml, load_yaml_config, add_args_from_dict, add_yaml_extension
 
+
 def get_config_dir_path(config_path: str) -> str:
     """
     Convert a given relative or absolute config file path to its absolute directory path.
 
     Args:
         config_path (str): The path to the configuration file. Can be either relative or absolute.
 
     Returns:
         str: The absolute directory path containing the configuration file.
     """
-     # Check if the given config_path is a relative path
+    # Check if the given config_path is a relative path
     if not os.path.isabs(config_path):
         # Get the directory of the main script file (entry point) in absolute form
-        path_from_main = os.path.dirname(os.path.abspath(str(sys.modules['__main__'].__file__)))
+        path_from_main = os.path.dirname(
+            os.path.abspath(str(sys.modules["__main__"].__file__))
+        )
 
         if config_path.startswith("./"):
-            config_path = config_path[len("./"):]
+            config_path = config_path[len("./") :]
 
         # Traverse up the directory structure for each "../" in config_path
         # Remove the "../" string from the path, and remove a directory from main.
         while config_path.startswith("../"):
-            config_path = config_path[len("../"):]
+            config_path = config_path[len("../") :]
             path_from_main = os.path.dirname(path_from_main)
 
         # Create absolute path.
         config_path = os.path.join(path_from_main, config_path)
     return config_path
 
 
-def skeleton_key(config_name: str, config_path: Optional[str]=None) -> Callable:
+def unlock(config_name: str, config_path: Optional[str] = None) -> Callable:
     """
     Create a decorator for parsing and injecting configuration arguments into a
     main function from a YAML file.
 
     Args:
         config_name (str): The name of the YAML configuration file.
         config_path (str): The path to the directory containing the configuration
@@ -77,14 +80,15 @@
             args = parser.parse_args()
             main(args)
 
         return _inner_function
 
     return _parse_config
 
+
 def import_class(class_string: str) -> Type[Any]:
     """
     Dynamically import a class using its full module path and class name.
 
     Args:
         class_string (str): A string representing the full path to the class,
                             including the module name and class name, separated
@@ -96,14 +100,15 @@
     parts = class_string.split(".")
     module_name = ".".join(parts[:-1])
     class_name = parts[-1]
     module = __import__(module_name, fromlist=[class_name])
     class_obj = getattr(module, class_name)
     return class_obj
 
+
 def instantiate(kwargs: Dict[str, Any]) -> Any:
     """
     Instantiate a class object using a dictionary of keyword arguments.
     The dictionary should contain the keys "_kwargs_" and "_target_" to
     specify the class to instantiate and its arguments.
 
     Args:
@@ -117,18 +122,16 @@
 
     Raises:
         AssertionError: If the class is missing specific parameters.
     """
     target_keyword = "_target_"
     class_obj = import_class(kwargs[target_keyword])
     del kwargs[target_keyword]
-    
+
     obj_parameters = list(inspect.signature(class_obj).parameters)
     valid_parameters = {k: v for k, v in kwargs.items() if k in obj_parameters}
-    missing_parameters = [
-        k for k in obj_parameters if k not in valid_parameters.keys()
-    ]
+    missing_parameters = [k for k in obj_parameters if k not in valid_parameters.keys()]
     assert (
         len(missing_parameters) == 0
     ), f"Object mssing specific parameters. ({missing_parameters})"
 
     return class_obj(**kwargs)
```

### Comparing `skeletonkey-0.0.10/skeletonkey/utils.py` & `skeletonkey-0.0.11/skeletonkey/utils.py`

 * *Files identical despite different names*

