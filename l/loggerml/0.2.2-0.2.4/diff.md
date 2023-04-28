# Comparing `tmp/loggerml-0.2.2.tar.gz` & `tmp/loggerml-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.2.2.tar", last modified: Fri Apr 28 00:43:27 2023, max compression
+gzip compressed data, was "loggerml-0.2.4.tar", last modified: Fri Apr 28 01:29:55 2023, max compression
```

## Comparing `loggerml-0.2.2.tar` & `loggerml-0.2.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 00:43:10.000000 loggerml-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.777691 loggerml-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 00:43:10.000000 loggerml-0.2.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 00:43:10.000000 loggerml-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 00:43:10.000000 loggerml-0.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 00:43:10.000000 loggerml-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 00:43:10.000000 loggerml-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-28 00:43:27.781690 loggerml-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-28 00:43:10.000000 loggerml-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-28 00:43:10.000000 loggerml-0.2.2/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 00:43:10.000000 loggerml-0.2.2/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 00:43:10.000000 loggerml-0.2.2/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 00:43:10.000000 loggerml-0.2.2/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 00:43:10.000000 loggerml-0.2.2/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 00:43:10.000000 loggerml-0.2.2/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 00:43:10.000000 loggerml-0.2.2/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 00:43:10.000000 loggerml-0.2.2/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 00:43:10.000000 loggerml-0.2.2/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 00:43:10.000000 loggerml-0.2.2/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-28 00:43:27.000000 loggerml-0.2.2/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 00:43:27.000000 loggerml-0.2.2/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:43:27.000000 loggerml-0.2.2/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 00:43:27.000000 loggerml-0.2.2/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 00:43:27.000000 loggerml-0.2.2/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-28 00:43:10.000000 loggerml-0.2.2/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:10.000000 loggerml-0.2.2/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-28 00:43:10.000000 loggerml-0.2.2/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 00:43:10.000000 loggerml-0.2.2/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 00:43:10.000000 loggerml-0.2.2/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-28 00:43:10.000000 loggerml-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 00:43:10.000000 loggerml-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 00:43:10.000000 loggerml-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:43:27.781690 loggerml-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 00:43:10.000000 loggerml-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.777691 loggerml-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 00:43:10.000000 loggerml-0.2.2/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 00:43:10.000000 loggerml-0.2.2/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:43:27.781690 loggerml-0.2.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 00:43:10.000000 loggerml-0.2.2/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 00:43:10.000000 loggerml-0.2.2/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 01:29:32.000000 loggerml-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.446137 loggerml-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 01:29:32.000000 loggerml-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 01:29:32.000000 loggerml-0.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 01:29:32.000000 loggerml-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 01:29:32.000000 loggerml-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:29:55.458137 loggerml-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 01:29:32.000000 loggerml-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 01:29:32.000000 loggerml-0.2.4/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 01:29:32.000000 loggerml-0.2.4/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 01:29:32.000000 loggerml-0.2.4/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 01:29:32.000000 loggerml-0.2.4/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 01:29:32.000000 loggerml-0.2.4/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 01:29:32.000000 loggerml-0.2.4/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 01:29:55.000000 loggerml-0.2.4/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-28 01:29:32.000000 loggerml-0.2.4/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 01:29:32.000000 loggerml-0.2.4/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 01:29:32.000000 loggerml-0.2.4/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-28 01:29:32.000000 loggerml-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 01:29:32.000000 loggerml-0.2.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:29:32.000000 loggerml-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:29:55.458137 loggerml-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 01:29:32.000000 loggerml-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.450137 loggerml-0.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.2.2/.github/workflows/pipy_deployment.yaml` & `loggerml-0.2.4/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/.github/workflows/pydocstyle.yaml` & `loggerml-0.2.4/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/.github/workflows/pylint.yaml` & `loggerml-0.2.4/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/.github/workflows/tests.yaml` & `loggerml-0.2.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/.pylintrc` & `loggerml-0.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/CONTRIBUTING.md` & `loggerml-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/LICENSE` & `loggerml-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/PKG-INFO` & `loggerml-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.2
+Version: 0.2.4
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way using
 [rich](https://github.com/Textualize/rich)✨ with useful information but with
 minimal code.
 
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
-![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
+![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
@@ -56,15 +56,17 @@
 python -c "print('\x1B')"
 ```
 
 It should print an *empty* line.
 
 ## Quick start
 
-Integrate the LogML logger in your training loop. For instance for 4 epochs,
+### Minimal usage
+
+Integrate the LogML logger in your training loops! For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
 from logml import Logger
 
 logger = Logger(
     n_epochs=4,
@@ -88,21 +90,22 @@
 
 Epoch 2/4, batch 8/20
 [=================>                              ][40%]
 [global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
 loss: 0.5432 | accuracy: 0.8524 |
 ```
 
-Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. For instance:
+### Advanced usage
+
+Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. You can also log the averaged value over the epoch. For instance:
 
 ```python
 logger = Logger(
     n_epochs=4,
     n_batches=20,
-    # (Log interval by default is 1, log every batch)
     styles='yellow',
     digits={'accuracy': 2},
     average=['loss'],  # loss will be averaged over the current epoch
     bold_keys=True,
     show_time=False,  # Remove the time bar
 )
 for _ in range(4):
@@ -130,37 +133,18 @@
 loss: 0.5432 | accuracy: 85 |
 Training is going well?
 Yes!
 ```
 
 With "loss: 0.5432" in italic red, "accuracy: 85" in yellow and both keys in bold.
 
-Finally, if you don't have the number of batches in advance, you can initialize the
-logger with `n_batches=None`. Only the available information will be displayed.
-For instance with the configuration of the first example:
-
-```script
-Epoch 1/4, batch 20/20
-[  *                                             ][ ? %]
-[global 00:00:02 >  ? | epoch 00:00:02 >  ? ]
-loss: 0.5432 | accuracy: 0.8524 |
-
-Epoch 2/4, batch 8/20
-[                           *                     ][ ? %]
-[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-loss: 0.5432 | accuracy: 0.8524 |
-```
-
-The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
-
-## Todo
+### Don't know the number of batches in advance?
 
-- [ ] Manage a validation loop (then multiple loggers)
-- [ ] Enable not using `new_epoch/log()` if log config is minimal
-- [ ] Add color customization for message, epoch/batch number and time
+If you don't have the number of batches in advance, you can initialize the
+logger with `n_batches=None`. The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
 
 ## How to contribute
 
 For **development**, install the package dynamically and dev requirements with:
 
 ```bash
 pip install -e .
```

### Comparing `loggerml-0.2.2/README.md` & `loggerml-0.2.4/loggerml.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+Metadata-Version: 2.1
+Name: loggerml
+Version: 0.2.4
+Summary: Log your ml training in the console in an attractive way.
+Author-email: Valentin Goldite <valentin.goldite@gmail.com>
+Project-URL: Source, https://github.com/valentingol/logml
+Keywords: logging,machine,learning
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way using
 [rich](https://github.com/Textualize/rich)✨ with useful information but with
 minimal code.
 
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
-![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
+![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
@@ -44,44 +56,56 @@
 python -c "print('\x1B')"
 ```
 
 It should print an *empty* line.
 
 ## Quick start
 
-Integrate the LogML logger in your training loop. For instance for 4 epochs,
+### Minimal usage
+
+Integrate the LogML logger in your training loops! For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
 from logml import Logger
 
 logger = Logger(
     n_epochs=4,
     n_batches=20,
     log_interval=2,
 )
 for _ in range(4):
     logger.start_epoch()  # Indicate the start of a new epoch
     for _ in range(20):
         logger.start_batch()  # Indicate the start of a new batch
-        # Log every 2 batches but you should call the log method at every batch
         logger.log({'loss': 0.54321256, 'accuracy': 0.85244777})
 ```
 
 Yields:
 
-![Alt Text](assets/base.gif)
+```script
+Epoch 1/4, batch 20/20
+[================================================][100%]
+[global 00:00:02 > 00:00:06 | epoch 00:00:02 > 00:00:00]
+loss: 0.5432 | accuracy: 0.8524 |
+
+Epoch 2/4, batch 8/20
+[=================>                              ][40%]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 0.8524 |
+```
+
+### Advanced usage
 
-Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. For instance:
+Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. You can also log the averaged value over the epoch. For instance:
 
 ```python
 logger = Logger(
     n_epochs=4,
     n_batches=20,
-    # (Log interval by default is 1, log every batch)
     styles='yellow',
     digits={'accuracy': 2},
     average=['loss'],  # loss will be averaged over the current epoch
     bold_keys=True,
     show_time=False,  # Remove the time bar
 )
 for _ in range(4):
@@ -94,27 +118,33 @@
             styles={'loss': 'italic red'},
             message="Training is going well?\nYes!",
         )
 ```
 
 Yields:
 
-![Alt Text](assets/advanced.gif)
-
-Finally, if you don't have the number of batches in advance, you can initialize the logger with `n_batches=None`. Only the available information will be displayed. For instance with the configuration of the first example:
-
-![Alt Text](assets/no_n_batches.png)
+```script
+Epoch 1/4, batch 20/20
+[================================================][100%]
+loss: 0.5432 | accuracy: 85 |
+
+Epoch 2/4, batch 7/20
+[=================>                              ][35%]
+[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
+loss: 0.5432 | accuracy: 85 |
+Training is going well?
+Yes!
+```
 
-The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
+With "loss: 0.5432" in italic red, "accuracy: 85" in yellow and both keys in bold.
 
-## Todo
+### Don't know the number of batches in advance?
 
-- [ ] Manage a validation loop (then multiple loggers)
-- [ ] Enable not using `new_epoch/log()` if log config is minimal
-- [ ] Add color customization for message, epoch/batch number and time
+If you don't have the number of batches in advance, you can initialize the
+logger with `n_batches=None`. The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
 
 ## How to contribute
 
 For **development**, install the package dynamically and dev requirements with:
 
 ```bash
 pip install -e .
```

### Comparing `loggerml-0.2.2/README_pipy.md` & `loggerml-0.2.4/README_pipy.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way using
 [rich](https://github.com/Textualize/rich)✨ with useful information but with
 minimal code.
 
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
-![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
+![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
@@ -44,15 +44,17 @@
 python -c "print('\x1B')"
 ```
 
 It should print an *empty* line.
 
 ## Quick start
 
-Integrate the LogML logger in your training loop. For instance for 4 epochs,
+### Minimal usage
+
+Integrate the LogML logger in your training loops! For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
 from logml import Logger
 
 logger = Logger(
     n_epochs=4,
@@ -76,21 +78,22 @@
 
 Epoch 2/4, batch 8/20
 [=================>                              ][40%]
 [global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
 loss: 0.5432 | accuracy: 0.8524 |
 ```
 
-Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. For instance:
+### Advanced usage
+
+Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. You can also log the averaged value over the epoch. For instance:
 
 ```python
 logger = Logger(
     n_epochs=4,
     n_batches=20,
-    # (Log interval by default is 1, log every batch)
     styles='yellow',
     digits={'accuracy': 2},
     average=['loss'],  # loss will be averaged over the current epoch
     bold_keys=True,
     show_time=False,  # Remove the time bar
 )
 for _ in range(4):
@@ -118,37 +121,18 @@
 loss: 0.5432 | accuracy: 85 |
 Training is going well?
 Yes!
 ```
 
 With "loss: 0.5432" in italic red, "accuracy: 85" in yellow and both keys in bold.
 
-Finally, if you don't have the number of batches in advance, you can initialize the
-logger with `n_batches=None`. Only the available information will be displayed.
-For instance with the configuration of the first example:
-
-```script
-Epoch 1/4, batch 20/20
-[  *                                             ][ ? %]
-[global 00:00:02 >  ? | epoch 00:00:02 >  ? ]
-loss: 0.5432 | accuracy: 0.8524 |
-
-Epoch 2/4, batch 8/20
-[                           *                     ][ ? %]
-[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-loss: 0.5432 | accuracy: 0.8524 |
-```
-
-The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
-
-## Todo
+### Don't know the number of batches in advance?
 
-- [ ] Manage a validation loop (then multiple loggers)
-- [ ] Enable not using `new_epoch/log()` if log config is minimal
-- [ ] Add color customization for message, epoch/batch number and time
+If you don't have the number of batches in advance, you can initialize the
+logger with `n_batches=None`. The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
 
 ## How to contribute
 
 For **development**, install the package dynamically and dev requirements with:
 
 ```bash
 pip install -e .
```

### Comparing `loggerml-0.2.2/assets/advanced.gif` & `loggerml-0.2.4/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/assets/base.gif` & `loggerml-0.2.4/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/assets/no_n_batches.png` & `loggerml-0.2.4/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.2.4/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/github_actions_utils/pylint_manager.py` & `loggerml-0.2.4/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/github_actions_utils/pytest_manager.py` & `loggerml-0.2.4/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/licenses_tier/RICH_LICENSE` & `loggerml-0.2.4/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/loggerml.egg-info/PKG-INFO` & `loggerml-0.2.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-Metadata-Version: 2.1
-Name: loggerml
-Version: 0.2.2
-Summary: Log your ml training in the console in an attractive way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/logml
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way using
 [rich](https://github.com/Textualize/rich)✨ with useful information but with
 minimal code.
 
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
-![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
+![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/logml/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/ruff.yaml)
 [![Flake8](https://github.com/valentingol/logml/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/flake.yaml)
@@ -56,53 +44,47 @@
 python -c "print('\x1B')"
 ```
 
 It should print an *empty* line.
 
 ## Quick start
 
-Integrate the LogML logger in your training loop. For instance for 4 epochs,
+### Minimal usage
+
+Integrate the LogML logger in your training loops! For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
 from logml import Logger
 
 logger = Logger(
     n_epochs=4,
     n_batches=20,
     log_interval=2,
 )
 for _ in range(4):
     logger.start_epoch()  # Indicate the start of a new epoch
     for _ in range(20):
         logger.start_batch()  # Indicate the start of a new batch
+        # Log every 2 batches but you should call the log method at every batch
         logger.log({'loss': 0.54321256, 'accuracy': 0.85244777})
 ```
 
 Yields:
 
-```script
-Epoch 1/4, batch 20/20
-[================================================][100%]
-[global 00:00:02 > 00:00:06 | epoch 00:00:02 > 00:00:00]
-loss: 0.5432 | accuracy: 0.8524 |
-
-Epoch 2/4, batch 8/20
-[=================>                              ][40%]
-[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-loss: 0.5432 | accuracy: 0.8524 |
-```
+![Alt Text](assets/base.gif)
 
-Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. For instance:
+### Advanced usage
+
+Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. You can also log the averaged value over the epoch. For instance:
 
 ```python
 logger = Logger(
     n_epochs=4,
     n_batches=20,
-    # (Log interval by default is 1, log every batch)
     styles='yellow',
     digits={'accuracy': 2},
     average=['loss'],  # loss will be averaged over the current epoch
     bold_keys=True,
     show_time=False,  # Remove the time bar
 )
 for _ in range(4):
@@ -115,52 +97,41 @@
             styles={'loss': 'italic red'},
             message="Training is going well?\nYes!",
         )
 ```
 
 Yields:
 
-```script
-Epoch 1/4, batch 20/20
-[================================================][100%]
-loss: 0.5432 | accuracy: 85 |
-
-Epoch 2/4, batch 7/20
-[=================>                              ][35%]
-[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-loss: 0.5432 | accuracy: 85 |
-Training is going well?
-Yes!
-```
+![Alt Text](assets/advanced.gif)
 
-With "loss: 0.5432" in italic red, "accuracy: 85" in yellow and both keys in bold.
+### Don't know the number of batches in advance?
 
-Finally, if you don't have the number of batches in advance, you can initialize the
-logger with `n_batches=None`. Only the available information will be displayed.
-For instance with the configuration of the first example:
+If you don't have the number of batches in advance, you can initialize the logger with `n_batches=None`. Only the available information will be displayed. For instance with the configuration of the first example:
 
-```script
-Epoch 1/4, batch 20/20
-[  *                                             ][ ? %]
-[global 00:00:02 >  ? | epoch 00:00:02 >  ? ]
-loss: 0.5432 | accuracy: 0.8524 |
-
-Epoch 2/4, batch 8/20
-[                           *                     ][ ? %]
-[global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-loss: 0.5432 | accuracy: 0.8524 |
-```
+![Alt Text](assets/no_n_batches.png)
 
 The progress bar is replaced by a cyclic animation. The eta times are not know at the first epoch but was estimated after the second epoch.
 
 ## Todo
 
-- [ ] Manage a validation loop (then multiple loggers)
-- [ ] Enable not using `new_epoch/log()` if log config is minimal
-- [ ] Add color customization for message, epoch/batch number and time
+Priority:
+
+- [ ] Doc with Sphinx
+- [ ] Be compatible with Windows and notebooks (with curses and some tricks)
+
+Secondary:
+
+- [ ] Explain how to use a tracker log (wandb for instance) with LogML
+- [ ] Use regex for `styles`, `digits` and `average` keys
+
+Done:
+
+- [x] Manage a validation loop (then multiple loggers)
+- [ ] ~~Enable not using `new_epoch/log()` if log config is minimal~~
+- [x] Add color customization for message, epoch/batch number and time
 
 ## How to contribute
 
 For **development**, install the package dynamically and dev requirements with:
 
 ```bash
 pip install -e .
```

### Comparing `loggerml-0.2.2/loggerml.egg-info/SOURCES.txt` & `loggerml-0.2.4/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/logml/__init__.py` & `loggerml-0.2.4/logml/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     This project is free to use for COMMERCIAL USE, MODIFICATION,
     DISTRIBUTION and PRIVATE USE as long as the original license is
     include as well as this copy right notice.
 """
 from logml.logger import Logger
 
 try:
-    from logml._version import version as __version__
-    from logml._version import version_tuple
+    from logml._version import __version__, __version_tuple__
 except ImportError:
     __version__ = "unknown version"
-    version_tuple = (0, 0, "unknown version")
+    __version_tuple__ = (0, 0, "unknown version")
 
 
-__all__ = ['__version__', 'version_tuple', 'Logger']
+__all__ = ['__version__', '__version_tuple__', 'Logger']
```

### Comparing `loggerml-0.2.2/logml/logger.py` & `loggerml-0.2.4/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/logml/time_utils.py` & `loggerml-0.2.4/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/pre-commit-checks.sh` & `loggerml-0.2.4/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/pyproject.toml` & `loggerml-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 dynamic = ["readme", "dependencies", "version"]
 
 [tool.setuptools]
 packages = ["logml"]
 license-files = ['LICEN[CS]E*', 'COPYING*', 'NOTICE*', 'AUTHORS*']
 
 [tool.setuptools_scm]
+write_to = "logml/_version.py"
 
 [project.urls]
 Source = "https://github.com/valentingol/logml"
 
 [tool.setuptools.dynamic]
 readme = { file = ["README_pipy.md"] , content-type = "text/markdown" }
 dependencies = { file = ["requirements.txt"] }
@@ -77,14 +78,15 @@
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = false
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
+exclude = ['*/_version.py', '*/__init__.py']
 files = '*.py'
 follow_imports = 'skip'
 follow_imports_for_stubs = false
 ignore_missing_imports = true
 no_implicit_optional = true
 no_implicit_reexport = true
 pretty = true
```

### Comparing `loggerml-0.2.2/tests/integration/inte_logger.py` & `loggerml-0.2.4/tests/integration/inte_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/tests/integration/inte_two_loggers.py` & `loggerml-0.2.4/tests/integration/inte_two_loggers.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/tests/unit/test_logger.py` & `loggerml-0.2.4/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.2/tests/unit/test_time_utils.py` & `loggerml-0.2.4/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

