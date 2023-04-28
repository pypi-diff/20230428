# Comparing `tmp/pyproject-generator-0.0.5.tar.gz` & `tmp/pyproject-generator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.5.tar", last modified: Fri Apr 28 19:23:36 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.6.tar", last modified: Fri Apr 28 19:30:56 2023, max compression
```

## Comparing `pyproject-generator-0.0.5.tar` & `pyproject-generator-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.015025 pyproject-generator-0.0.5/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:23:36.015286 pyproject-generator-0.0.5/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.5/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.5/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-28 19:23:36.016563 pyproject-generator-0.0.5/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:35.992215 pyproject-generator-0.0.5/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:35.997430 pyproject-generator-0.0.5/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.5/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-28 19:23:26.000000 pyproject-generator-0.0.5/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2570 2023-04-28 19:13:46.000000 pyproject-generator-0.0.5/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.000311 pyproject-generator-0.0.5/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.5/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.5/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     7486 2023-04-28 19:20:05.000000 pyproject-generator-0.0.5/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.008211 pyproject-generator-0.0.5/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.5/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.5/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.5/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.5/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.5/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.5/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.013286 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      720 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.014449 pyproject-generator-0.0.5/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.5/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.416182 pyproject-generator-0.0.6/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:30:56.416361 pyproject-generator-0.0.6/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.6/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.6/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-28 19:30:56.417212 pyproject-generator-0.0.6/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.394662 pyproject-generator-0.0.6/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.399744 pyproject-generator-0.0.6/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.6/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-28 19:30:35.000000 pyproject-generator-0.0.6/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2570 2023-04-28 19:13:46.000000 pyproject-generator-0.0.6/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.402617 pyproject-generator-0.0.6/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.6/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.6/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     7502 2023-04-28 19:30:05.000000 pyproject-generator-0.0.6/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.411728 pyproject-generator-0.0.6/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.6/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.6/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.6/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.6/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.6/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.6/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.415347 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      720 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.415897 pyproject-generator-0.0.6/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.6/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.5/PKG-INFO` & `pyproject-generator-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.5/README.md` & `pyproject-generator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.5/setup.cfg` & `pyproject-generator-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.5/src/pyproject/cli.py` & `pyproject-generator-0.0.6/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.5/src/pyproject/project_builder.py` & `pyproject-generator-0.0.6/src/pyproject/project_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                 merged_config[k] = config[k]
 
         return merged_config
 
     def config(self):
         config = self._config
         config["dependencies"] = list(config["dependencies"])
-        with open(self._config_path, "w") as f:
+        with open(self._config_path / "config.json", "w") as f:
             json.dump(config, f, indent=4)
 
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
 
         env = Env()
```

### Comparing `pyproject-generator-0.0.5/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.6/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.5/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.6/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.5/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.6/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.5/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.0.6/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.5/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.6/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

