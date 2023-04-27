# Comparing `tmp/loggerml-0.2.0.tar.gz` & `tmp/loggerml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.2.0.tar", last modified: Thu Apr 27 22:21:36 2023, max compression
+gzip compressed data, was "loggerml-0.2.1.tar", last modified: Thu Apr 27 23:06:04 2023, max compression
```

## Comparing `loggerml-0.2.0.tar` & `loggerml-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.474956 loggerml-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 22:21:18.000000 loggerml-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.466956 loggerml-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.470956 loggerml-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-27 22:21:18.000000 loggerml-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 22:21:18.000000 loggerml-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-27 22:21:18.000000 loggerml-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-27 22:21:18.000000 loggerml-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 22:21:18.000000 loggerml-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 22:21:36.474956 loggerml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-27 22:21:18.000000 loggerml-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-27 22:21:18.000000 loggerml-0.2.0/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.470956 loggerml-0.2.0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-27 22:21:18.000000 loggerml-0.2.0/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-27 22:21:18.000000 loggerml-0.2.0/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-27 22:21:18.000000 loggerml-0.2.0/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.470956 loggerml-0.2.0/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 22:21:18.000000 loggerml-0.2.0/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 22:21:18.000000 loggerml-0.2.0/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 22:21:18.000000 loggerml-0.2.0/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 22:21:18.000000 loggerml-0.2.0/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 22:21:18.000000 loggerml-0.2.0/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.470956 loggerml-0.2.0/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 22:21:36.000000 loggerml-0.2.0/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 22:21:36.000000 loggerml-0.2.0/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:21:36.000000 loggerml-0.2.0/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 22:21:36.000000 loggerml-0.2.0/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 22:21:36.000000 loggerml-0.2.0/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.474956 loggerml-0.2.0/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:21:18.000000 loggerml-0.2.0/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-27 22:21:18.000000 loggerml-0.2.0/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 22:21:18.000000 loggerml-0.2.0/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 22:21:18.000000 loggerml-0.2.0/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-27 22:21:18.000000 loggerml-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 22:21:18.000000 loggerml-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 22:21:18.000000 loggerml-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:21:36.474956 loggerml-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 22:21:18.000000 loggerml-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.466956 loggerml-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.474956 loggerml-0.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-27 22:21:18.000000 loggerml-0.2.0/tests/integration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:21:36.474956 loggerml-0.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-27 22:21:18.000000 loggerml-0.2.0/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 22:21:18.000000 loggerml-0.2.0/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 23:05:41.000000 loggerml-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.978687 loggerml-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-27 23:05:41.000000 loggerml-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 23:05:41.000000 loggerml-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-27 23:05:41.000000 loggerml-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-27 23:05:41.000000 loggerml-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 23:05:41.000000 loggerml-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-27 23:06:04.982687 loggerml-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-27 23:05:41.000000 loggerml-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-27 23:05:41.000000 loggerml-0.2.1/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-27 23:05:41.000000 loggerml-0.2.1/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-27 23:05:41.000000 loggerml-0.2.1/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-27 23:05:41.000000 loggerml-0.2.1/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 23:05:41.000000 loggerml-0.2.1/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 23:05:41.000000 loggerml-0.2.1/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 23:05:41.000000 loggerml-0.2.1/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 23:05:41.000000 loggerml-0.2.1/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 23:05:41.000000 loggerml-0.2.1/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-27 23:06:04.000000 loggerml-0.2.1/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 23:06:04.000000 loggerml-0.2.1/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:06:04.000000 loggerml-0.2.1/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 23:06:04.000000 loggerml-0.2.1/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 23:06:04.000000 loggerml-0.2.1/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 23:05:41.000000 loggerml-0.2.1/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-27 23:05:41.000000 loggerml-0.2.1/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 23:05:41.000000 loggerml-0.2.1/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 23:05:41.000000 loggerml-0.2.1/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-27 23:05:41.000000 loggerml-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-27 23:05:41.000000 loggerml-0.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 23:05:41.000000 loggerml-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:06:04.982687 loggerml-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 23:05:41.000000 loggerml-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.978687 loggerml-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-27 23:05:41.000000 loggerml-0.2.1/tests/integration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:06:04.982687 loggerml-0.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-27 23:05:41.000000 loggerml-0.2.1/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 23:05:41.000000 loggerml-0.2.1/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.2.0/.github/workflows/pipy_deployment.yaml` & `loggerml-0.2.1/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/.github/workflows/pydocstyle.yaml` & `loggerml-0.2.1/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/.github/workflows/pylint.yaml` & `loggerml-0.2.1/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/.github/workflows/tests.yaml` & `loggerml-0.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/.pylintrc` & `loggerml-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/CONTRIBUTING.md` & `loggerml-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/LICENSE` & `loggerml-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/PKG-INFO` & `loggerml-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.0
+Version: 0.2.1
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
-Support all Unix and Emacs distribution as well as Windows 11.
-
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -32,21 +30,36 @@
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 
 ## Installation
 
-In a new virtual environment, install simply the package via pipy:
+In a new virtual environment, install simply the package via
+[pipy](https://pypi.org/project/loggerml/):
 
 ```bash
 pip install loggerml
 ```
 
-**Be careful, Windows 10 is not supported (but Windows 11 yes).**
+## Supported platforms
+
+This package assume that you are using a terminal that support ANSI escape sequences.
+See [here](https://en.wikipedia.org/wiki/ANSI_escape_code#Platform_support) for
+supported platforms. All Unix and Emacs distribution are supported as well as Windows
+but only on some machine (Windows 11 seems to work but not Windows 10).
+
+The quick test to know if your terminal support ANSI escape sequence is to run the
+following command in your terminal:
+
+```script
+python -c "print('\x1B')"
+```
+
+It should print an *empty* line.
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
```

### Comparing `loggerml-0.2.0/README.md` & `loggerml-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
-Support all Unix and Emacs distribution and Windows 11.
-
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -20,21 +18,36 @@
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 
 ## Installation
 
-In a new virtual environment, install simply the package via pipy:
+In a new virtual environment, install simply the package via
+[pipy](https://pypi.org/project/loggerml/):
 
 ```bash
 pip install loggerml
 ```
 
-**Be careful, Windows 10 is not supported (but Windows 11 yes).**
+## Supported platforms
+
+This package assume that you are using a terminal that support ANSI escape sequences.
+See [here](https://en.wikipedia.org/wiki/ANSI_escape_code#Platform_support) for
+supported platforms. All Unix and Emacs distribution are supported as well as Windows
+but only on some machine (Windows 11 seems to work but not Windows 10).
+
+The quick test to know if your terminal support ANSI escape sequence is to run the
+following command in your terminal:
+
+```script
+python -c "print('\x1B')"
+```
+
+It should print an *empty* line.
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
```

### Comparing `loggerml-0.2.0/README_pipy.md` & `loggerml-0.2.1/loggerml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+Metadata-Version: 2.1
+Name: loggerml
+Version: 0.2.1
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
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
-Support all Unix and Emacs distribution as well as Windows 11.
-
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -20,21 +30,36 @@
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 
 ## Installation
 
-In a new virtual environment, install simply the package via pipy:
+In a new virtual environment, install simply the package via
+[pipy](https://pypi.org/project/loggerml/):
 
 ```bash
 pip install loggerml
 ```
 
-**Be careful, Windows 10 is not supported (but Windows 11 yes).**
+## Supported platforms
+
+This package assume that you are using a terminal that support ANSI escape sequences.
+See [here](https://en.wikipedia.org/wiki/ANSI_escape_code#Platform_support) for
+supported platforms. All Unix and Emacs distribution are supported as well as Windows
+but only on some machine (Windows 11 seems to work but not Windows 10).
+
+The quick test to know if your terminal support ANSI escape sequence is to run the
+following command in your terminal:
+
+```script
+python -c "print('\x1B')"
+```
+
+It should print an *empty* line.
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
```

### Comparing `loggerml-0.2.0/assets/advanced.gif` & `loggerml-0.2.1/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/assets/base.gif` & `loggerml-0.2.1/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/assets/no_n_batches.png` & `loggerml-0.2.1/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.2.1/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/github_actions_utils/pylint_manager.py` & `loggerml-0.2.1/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/github_actions_utils/pytest_manager.py` & `loggerml-0.2.1/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/loggerml.egg-info/PKG-INFO` & `loggerml-0.2.1/README_pipy.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-Metadata-Version: 2.1
-Name: loggerml
-Version: 0.2.0
-Summary: Log your ml training in the console in an attractive way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/logml
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # LoggerML - Machine Learning Logger in the console
 
 Log your Machine Learning training in the console in a beautiful way ✨
 and with minimal code.
 
-Support all Unix and Emacs distribution as well as Windows 11.
-
 [![Release](https://img.shields.io/github/v/release/valentingol/logml?include_prereleases)](https://github.com/valentingol/logml/releases)
 ![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/logml?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -32,21 +18,36 @@
 [![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_pylint.json)](https://github.com/valentingol/logml/actions/workflows/pylint.yaml)
 
 [![Tests](https://github.com/valentingol/logml/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/451f91cece4478ebc81377e27e432f8b/raw/logml_tests.json)](https://github.com/valentingol/logml/actions/workflows/tests.yaml)
 
 ## Installation
 
-In a new virtual environment, install simply the package via pipy:
+In a new virtual environment, install simply the package via
+[pipy](https://pypi.org/project/loggerml/):
 
 ```bash
 pip install loggerml
 ```
 
-**Be careful, Windows 10 is not supported (but Windows 11 yes).**
+## Supported platforms
+
+This package assume that you are using a terminal that support ANSI escape sequences.
+See [here](https://en.wikipedia.org/wiki/ANSI_escape_code#Platform_support) for
+supported platforms. All Unix and Emacs distribution are supported as well as Windows
+but only on some machine (Windows 11 seems to work but not Windows 10).
+
+The quick test to know if your terminal support ANSI escape sequence is to run the
+following command in your terminal:
+
+```script
+python -c "print('\x1B')"
+```
+
+It should print an *empty* line.
 
 ## Quick start
 
 Integrate the LogML logger in your training loop. For instance for 4 epochs,
 20 batches per epoch and a log interval of 2 batches:
 
 ```python
```

### Comparing `loggerml-0.2.0/loggerml.egg-info/SOURCES.txt` & `loggerml-0.2.1/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/logml/__init__.py` & `loggerml-0.2.1/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/logml/logger.py` & `loggerml-0.2.1/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/logml/time_utils.py` & `loggerml-0.2.1/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/pre-commit-checks.sh` & `loggerml-0.2.1/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/pyproject.toml` & `loggerml-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [project]
 name = "loggerml"
 authors = [
     {name="Valentin Goldite", email="valentin.goldite@gmail.com"},
 ]
 description = """Log your ml training in the console in an attractive way."""
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 keywords = ["logging", "machine", "learning"]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["readme", "dependencies", "version"]
 
 [tool.setuptools]
```

### Comparing `loggerml-0.2.0/tests/integration/logger.py` & `loggerml-0.2.1/tests/integration/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/tests/unit/test_logger.py` & `loggerml-0.2.1/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.0/tests/unit/test_time_utils.py` & `loggerml-0.2.1/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

