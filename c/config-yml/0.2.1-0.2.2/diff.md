# Comparing `tmp/config_yml-0.2.1.tar.gz` & `tmp/config_yml-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_yml-0.2.1.tar", last modified: Wed Apr 26 06:12:07 2023, max compression
+gzip compressed data, was "config_yml-0.2.2.tar", last modified: Fri Apr 28 10:56:10 2023, max compression
```

## Comparing `config_yml-0.2.1.tar` & `config_yml-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 06:12:07.398057 config_yml-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 06:11:57.000000 config_yml-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.394057 config_yml-0.2.1/config_yml/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 06:11:57.000000 config_yml-0.2.1/config_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-04-26 06:11:57.000000 config_yml-0.2.1/config_yml/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/config_yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 06:12:07.000000 config_yml-0.2.1/config_yml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:12:07.398057 config_yml-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 06:11:57.000000 config_yml-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:12:07.398057 config_yml-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/data/config_existing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/data/config_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-26 06:11:57.000000 config_yml-0.2.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 10:56:10.775020 config_yml-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-28 10:55:58.000000 config_yml-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/config_yml/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 10:55:58.000000 config_yml-0.2.2/config_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-28 10:55:58.000000 config_yml-0.2.2/config_yml/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/config_yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:56:10.775020 config_yml-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-28 10:55:58.000000 config_yml-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/data/config_existing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/data/config_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/test_config.py
```

### Comparing `config_yml-0.2.1/PKG-INFO` & `config_yml-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_yml
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `config_yml-0.2.1/config_yml/config.py` & `config_yml-0.2.2/config_yml/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,72 @@
 """ Config class """
 import os
 import copy
 from pathlib import Path
 import logging
 import yaml
+import shutil
 
 log = logging.getLogger(__name__)
 
 
 class Config:
     """ Manages a config file that will be generated in the /var/ folder
     """
 
-    def __init__(self, package_name: str, template_path: str, config_file_name: str):
+    def __init__(self, package_name: str, template_path: str, config_file_name: str, dry_run_abs_path: str = None):
         """_summary_
 
         Args:
             package_name (str): Name of the package owner of the config file
             template_path (str): Path of the template file
             config_path (str): Name of config file (will be placed in home/var/{modulename} folder)
+            dry_run_abs_path (str): None if no dry run selected
+                                    "" if dry run selected, with empsty config file
+                                    "{absolute-path}" if dry run selected, starting with an initial file
         """
         self._template_path = template_path
         self._config_file_name = config_file_name
         self.homevar = os.path.join(str(Path.home()), 'var', package_name)
 
         if not os.path.exists(self.homevar):
             os.makedirs(self.homevar)
 
+        if dry_run_abs_path is not None:
+            self.dry_run = True
+            self.homevar = os.path.join(self.homevar, 'dryrun_config')
+            if os.path.exists(self.homevar):
+                shutil.rmtree(self.homevar)
+            os.makedirs(self.homevar)
+            if  dry_run_abs_path != "":
+                shutil.copy(dry_run_abs_path,  os.path.join(self.homevar, self._config_file_name))           
+        else:
+            self.dry_run = False
+
         self.config = {}
 
         self.read_config()
 
+    def __del__(self):
+        if self.dry_run:
+            shutil.rmtree(self.homevar)
+
     def __getitem__(self, key):
         return self.config.get(key, None)
 
-    @staticmethod
-    def get_config_path(package_name: str, config_file_name: str) -> str:
+    def get_config_path(self) -> str:
         """Get the path for the config, inside the homevar path
         Args:
             package_name (str): The name of the package... will be joined after the homevar
             config_file_name (str): Name of the config file itself (without folder... just the file name)
 
         Returns:
             str: The path of the config file
         """
-        return os.path.join(str(Path.home()), 'var', package_name, config_file_name)
+        return os.path.join(self.homevar, self._config_file_name)
 
     def get_dict(self) -> dict:
         """Returns the config  dictionary
         Returns:
             dict: Config
         """
         return self.config
```

### Comparing `config_yml-0.2.1/config_yml.egg-info/PKG-INFO` & `config_yml-0.2.2/config_yml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-yml
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `config_yml-0.2.1/setup.py` & `config_yml-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="config_yml",
-    version="0.2.1",
+    version="0.2.2",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility modules for Class management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/config_yml",
     packages=setuptools.find_packages(),
```

### Comparing `config_yml-0.2.1/tests/test_config.py` & `config_yml-0.2.2/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,56 +83,49 @@
                 "singlemerge": "template",
                 "fruits": ["orange", "apple", "banana"],
             },
         ]
         self.assertEqual(config_template, expected_merge)
 
     def test_002_from_scrath(self):
-        """ Remove config file, to start from scratch """
-        var_config_path = Config.get_config_path("baseutils_tests", "config_new.yml")
-        if os.path.exists(var_config_path):
-            os.remove(Config.getConfigPath("baseutils_tests", "config_new.yml"))
-
+        """ Test config initialization from scratch
+        """
         # Instatiate a config file from scratch, based only on template
         # Will be automatically writen to file
         template_path = f'{Path(__file__).parent}/data/config_template.yml'
-        _ = Config(
-                    package_name="baseutils_tests",
+        config = Config(
+                    package_name="config_yml",
                     template_path=template_path,
                     config_file_name="config_new.yml",
+                    dry_run_abs_path=""
                   )
 
         try:
             # Check that resulting config file equals the template file
-            with open(var_config_path, "r", encoding="utf-8") as config_file:
+            with open(config.get_config_path(), "r", encoding="utf-8") as config_file:
                 config_read = yaml.load(config_file, Loader=yaml.FullLoader)
                 with open(template_path, "r", encoding="utf-8") as template_config_file:
                     template_config_read = yaml.load(template_config_file, Loader=yaml.FullLoader)
                     self.assertEqual(config_read, template_config_read)
         except IOError as ex:
             self.assertFalse(f"File not found: {ex}")
-        finally:
-            os.remove(Config.get_config_path("baseutils_tests", "config_new.yml"))
 
     def test_003_update_config(self):
         """Test updating a config
         """
         # Copy already-made config to var destination
         existing_path = f"{Path(__file__).parent}/data/config_existing.yml"
-        var_config_path = Config.get_config_path(
-            "baseutils_tests", "config_existing.yml"
-        )
-        shutil.copy(existing_path, var_config_path)
 
         # Instatiate a config file from scratch, with an updated template, with an existing config
         template_path = f'{Path(__file__).parent}/data/config_template.yml'
         config = Config(
-                        package_name="baseutils_tests",
+                        package_name="config_yml",
                         template_path=template_path,
                         config_file_name="config_existing.yml",
+                        dry_run_abs_path=existing_path
                        )
 
         expected_merged = {
                             "key_template1": "template",
                             "key_template2": "changed",
                             "key_template3": "new in config",
                           }
@@ -140,23 +133,20 @@
         # Check memory matches
         self.assertEqual(config.get_dict(), expected_merged)
 
         config.write()
 
         try:
             # Check that resulting config file equals the template file
-            with open(var_config_path, "r", encoding="utf-8") as config_file:
+            with open(config.get_config_path(), "r", encoding="utf-8") as config_file:
                 config_read = yaml.load(config_file, Loader=yaml.FullLoader)
                 expected_merged = {
                                     "key_template1": "template",
                                     "key_template2": "changed",
                                     "key_template3": "new in config",
                                   }
                 self.assertEqual(config_read, expected_merged)
         except IOError as ex:
             self.assertFalse(f"File not found: {ex}")
-        finally:
-            os.remove(Config.get_config_path("baseutils_tests", "config_existing.yml"))
-
 
 if __name__ == "__main__":
     unittest.main()
```

