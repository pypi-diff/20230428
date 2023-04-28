# Comparing `tmp/yaecs-3.1.0.tar.gz` & `tmp/yaecs-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.1.0.tar", last modified: Thu Apr 27 13:52:45 2023, max compression
+gzip compressed data, was "yaecs-3.1.1.tar", last modified: Fri Apr 28 10:42:20 2023, max compression
```

## Comparing `yaecs-3.1.0.tar` & `yaecs-3.1.1.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.626813 yaecs-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 13:52:28.000000 yaecs-3.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.618813 yaecs-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 13:52:28.000000 yaecs-3.1.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-27 13:52:28.000000 yaecs-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-04-27 13:52:28.000000 yaecs-3.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-27 13:52:28.000000 yaecs-3.1.0/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-27 13:52:28.000000 yaecs-3.1.0/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-04-27 13:52:28.000000 yaecs-3.1.0/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-27 13:52:28.000000 yaecs-3.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 13:52:28.000000 yaecs-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-27 13:52:45.626813 yaecs-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-27 13:52:28.000000 yaecs-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 13:52:28.000000 yaecs-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 13:52:28.000000 yaecs-3.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-04-27 13:52:28.000000 yaecs-3.1.0/resources/yaecs_constructor_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:52:45.626813 yaecs-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 13:52:28.000000 yaecs-3.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-27 13:52:28.000000 yaecs-3.1.0/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.618813 yaecs-3.1.0/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-27 13:52:28.000000 yaecs-3.1.0/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34035 2023-04-27 13:52:28.000000 yaecs-3.1.0/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-27 13:52:28.000000 yaecs-3.1.0/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-27 13:52:28.000000 yaecs-3.1.0/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.626813 yaecs-3.1.0/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43910 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17162 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-27 13:52:28.000000 yaecs-3.1.0/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:45.622813 yaecs-3.1.0/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-27 13:52:45.000000 yaecs-3.1.0/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-27 13:52:45.000000 yaecs-3.1.0/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:52:45.000000 yaecs-3.1.0/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 13:52:45.000000 yaecs-3.1.0/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 13:52:45.000000 yaecs-3.1.0/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.654179 yaecs-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 10:42:04.000000 yaecs-3.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.634178 yaecs-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.642178 yaecs-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 10:42:04.000000 yaecs-3.1.1/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-28 10:42:04.000000 yaecs-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-04-28 10:42:04.000000 yaecs-3.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-28 10:42:04.000000 yaecs-3.1.1/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-28 10:42:04.000000 yaecs-3.1.1/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-04-28 10:42:04.000000 yaecs-3.1.1/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-28 10:42:04.000000 yaecs-3.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 10:42:04.000000 yaecs-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-28 10:42:20.654179 yaecs-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-28 10:42:04.000000 yaecs-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-28 10:42:04.000000 yaecs-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 10:42:04.000000 yaecs-3.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.642178 yaecs-3.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-04-28 10:42:04.000000 yaecs-3.1.1/resources/yaecs_constructor_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:42:20.654179 yaecs-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 10:42:04.000000 yaecs-3.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-28 10:42:04.000000 yaecs-3.1.1/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.638178 yaecs-3.1.1/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-28 10:42:04.000000 yaecs-3.1.1/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34035 2023-04-28 10:42:04.000000 yaecs-3.1.1/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 10:42:04.000000 yaecs-3.1.1/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.650179 yaecs-3.1.1/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.650179 yaecs-3.1.1/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.654179 yaecs-3.1.1/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43910 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17162 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.654179 yaecs-3.1.1/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.1.0/.github/workflows/pipy_deployment.yaml` & `yaecs-3.1.1/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/.gitignore` & `yaecs-3.1.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -146,8 +146,11 @@
 
 # PyCharm
 #  JetBrains specific template is maintainted in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
-.vscode/
+.vscode/
+
+# Setuptools SCM
+yaecs/_version.py
```

### Comparing `yaecs-3.1.0/.pylintrc` & `yaecs-3.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/COPYING.LESSER.md` & `yaecs-3.1.1/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/COPYING.md` & `yaecs-3.1.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/DOCUMENTATION_WIP.md` & `yaecs-3.1.1/DOCUMENTATION_WIP.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/LICENSE.md` & `yaecs-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/PKG-INFO` & `yaecs-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.1.0/README.md` & `yaecs-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/pyproject.toml` & `yaecs-3.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
-build-backend = "setuptools.build_meta"
 
 [project]
 name = "yaecs"
 authors = [
     {name="Reactive Reality AG"},
 ]
 description = """A Config System designed for experimental purposes"""
@@ -13,15 +12,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["readme", "version"]
 dependencies = ["pyyaml==6.0", "mock==4.0.3"]
 
 [tool.setuptools]
-py-modules = ["yaecs"]
+packages = ["yaecs"]
 license-files = ['LICEN[CS]E*', 'COPYING*', 'NOTICE*', 'AUTHORS*']
 
 [tool.setuptools_scm]
 write_to = "yaecs/_version.py"
 
 [project.urls]
 Source = "https://gitlab.com/reactivereality/public/yaecs"
```

### Comparing `yaecs-3.1.0/resources/yaecs_constructor_overview.png` & `yaecs-3.1.1/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/setup.py` & `yaecs-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/short-readme.md` & `yaecs-3.1.1/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/unittests/config/conftest.py` & `yaecs-3.1.1/unittests/config/conftest.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/unittests/config/test_config.py` & `yaecs-3.1.1/unittests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/unittests/config/utils.py` & `yaecs-3.1.1/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/usage_example/configs/project_config.py` & `yaecs-3.1.1/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/usage_example/main.py` & `yaecs-3.1.1/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/usage_example/project_utils/utils.py` & `yaecs-3.1.1/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/__init__.py` & `yaecs-3.1.1/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config.py` & `yaecs-3.1.1/yaecs/config/config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config_base.py` & `yaecs-3.1.1/yaecs/config/config_base.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config_convenience.py` & `yaecs-3.1.1/yaecs/config/config_convenience.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config_getters.py` & `yaecs-3.1.1/yaecs/config/config_getters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config_hooks.py` & `yaecs-3.1.1/yaecs/config/config_hooks.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config_processing_functions.py` & `yaecs-3.1.1/yaecs/config/config_processing_functions.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config/config_setters.py` & `yaecs-3.1.1/yaecs/config/config_setters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/config_history.py` & `yaecs-3.1.1/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/experiment.py` & `yaecs-3.1.1/yaecs/experiment.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/pytorch_lightning_utils.py` & `yaecs-3.1.1/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/user_utils.py` & `yaecs-3.1.1/yaecs/user_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs/yaecs_utils.py` & `yaecs-3.1.1/yaecs/yaecs_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.0/yaecs.egg-info/PKG-INFO` & `yaecs-3.1.1/yaecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.1.0/yaecs.egg-info/SOURCES.txt` & `yaecs-3.1.1/yaecs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 usage_example/configs/default/main_config.yaml
 usage_example/configs/default/model_config.yaml
 usage_example/configs/experiment/dummy_test.yaml
 usage_example/configs/experiment/grid_search.yaml
 usage_example/configs/experiment/random_search.yaml
 usage_example/project_utils/utils.py
 yaecs/__init__.py
+yaecs/_version.py
 yaecs/config_history.py
 yaecs/experiment.py
 yaecs/pytorch_lightning_utils.py
 yaecs/user_utils.py
 yaecs/yaecs_utils.py
 yaecs.egg-info/PKG-INFO
 yaecs.egg-info/SOURCES.txt
```

