# Comparing `tmp/loggerml-0.2.8.tar.gz` & `tmp/loggerml-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.2.8.tar", last modified: Fri Apr 28 13:55:39 2023, max compression
+gzip compressed data, was "loggerml-0.2.9.tar", last modified: Fri Apr 28 15:31:45 2023, max compression
```

## Comparing `loggerml-0.2.8.tar` & `loggerml-0.2.9.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 13:55:23.000000 loggerml-0.2.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.726155 loggerml-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.730155 loggerml-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 13:55:23.000000 loggerml-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-04-28 13:55:23.000000 loggerml-0.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 13:55:23.000000 loggerml-0.2.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 13:55:23.000000 loggerml-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 13:55:39.734156 loggerml-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 13:55:23.000000 loggerml-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 13:55:23.000000 loggerml-0.2.8/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 13:55:23.000000 loggerml-0.2.8/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 13:55:23.000000 loggerml-0.2.8/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 13:55:23.000000 loggerml-0.2.8/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/logml.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/usage/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/usage/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 13:55:23.000000 loggerml-0.2.8/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 13:55:23.000000 loggerml-0.2.8/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:55:39.000000 loggerml-0.2.8/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-28 13:55:23.000000 loggerml-0.2.8/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 13:55:23.000000 loggerml-0.2.8/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 13:55:23.000000 loggerml-0.2.8/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 13:55:23.000000 loggerml-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 13:55:23.000000 loggerml-0.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:55:23.000000 loggerml-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:55:39.734156 loggerml-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 13:55:23.000000 loggerml-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.730155 loggerml-0.2.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.674543 loggerml-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 15:31:23.000000 loggerml-0.2.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.662542 loggerml-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.666543 loggerml-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 15:31:23.000000 loggerml-0.2.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 15:31:23.000000 loggerml-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-04-28 15:31:23.000000 loggerml-0.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 15:31:23.000000 loggerml-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 15:31:23.000000 loggerml-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 15:31:45.674543 loggerml-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 15:31:23.000000 loggerml-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 15:31:23.000000 loggerml-0.2.9/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.670543 loggerml-0.2.9/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 15:31:23.000000 loggerml-0.2.9/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 15:31:23.000000 loggerml-0.2.9/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 15:31:23.000000 loggerml-0.2.9/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.670543 loggerml-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 15:31:23.000000 loggerml-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.670543 loggerml-0.2.9/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 15:31:23.000000 loggerml-0.2.9/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 15:31:23.000000 loggerml-0.2.9/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 15:31:23.000000 loggerml-0.2.9/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 15:31:23.000000 loggerml-0.2.9/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 15:31:23.000000 loggerml-0.2.9/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.670543 loggerml-0.2.9/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 15:31:23.000000 loggerml-0.2.9/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.670543 loggerml-0.2.9/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 15:31:45.000000 loggerml-0.2.9/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 15:31:45.000000 loggerml-0.2.9/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:31:45.000000 loggerml-0.2.9/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 15:31:45.000000 loggerml-0.2.9/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 15:31:45.000000 loggerml-0.2.9/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.674543 loggerml-0.2.9/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 15:31:23.000000 loggerml-0.2.9/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 15:31:45.000000 loggerml-0.2.9/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-28 15:31:23.000000 loggerml-0.2.9/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 15:31:23.000000 loggerml-0.2.9/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 15:31:23.000000 loggerml-0.2.9/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 15:31:23.000000 loggerml-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 15:31:23.000000 loggerml-0.2.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 15:31:23.000000 loggerml-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:31:45.674543 loggerml-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 15:31:23.000000 loggerml-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.666543 loggerml-0.2.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.674543 loggerml-0.2.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 15:31:23.000000 loggerml-0.2.9/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 15:31:23.000000 loggerml-0.2.9/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:45.674543 loggerml-0.2.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 15:31:23.000000 loggerml-0.2.9/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 15:31:23.000000 loggerml-0.2.9/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.2.8/.github/workflows/pipy_deployment.yaml` & `loggerml-0.2.9/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/.github/workflows/pydocstyle.yaml` & `loggerml-0.2.9/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/.github/workflows/pylint.yaml` & `loggerml-0.2.9/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/.github/workflows/tests.yaml` & `loggerml-0.2.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/.pylintrc` & `loggerml-0.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/CONTRIBUTING.md` & `loggerml-0.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/LICENSE` & `loggerml-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/PKG-INFO` & `loggerml-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.8
+Version: 0.2.9
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.8/README.md` & `loggerml-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/README_pipy.md` & `loggerml-0.2.9/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/assets/advanced.gif` & `loggerml-0.2.9/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/assets/base.gif` & `loggerml-0.2.9/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/assets/no_n_batches.png` & `loggerml-0.2.9/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/docs/README.rst` & `loggerml-0.2.9/docs/README.rst`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/docs/source/usage/quickstart.rst` & `loggerml-0.2.9/docs/quickstart.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,81 @@
-***********
-Quick start
-***********
-
-#############
-Minimal usage
-#############
+# Quick start
+
+## Minimal usage
 
 Integrate the LogML logger in your training loops! For instance for 4 epochs,
-20 batches per epoch and a log interval of 2 n_batches:
-::
+20 batches per epoch and a log interval of 2 batches:
 
-    from logml import Logger
+```python
+from logml import Logger
 
-    logger = Logger(
-        n_epochs=4,
-        n_batches=20,
-        log_interval=2,
-    )
-    for _ in range(4):
-        logger.start_epoch()  # Indicate the start of a new epoch
-        for _ in range(20):
-            logger.start_batch()  # Indicate the start of a new batch
-            logger.log({'loss': 0.54321256, 'accuracy': 0.85244777})
+logger = Logger(
+    n_epochs=4,
+    n_batches=20,
+    log_interval=2,
+)
+for _ in range(4):
+    logger.start_epoch()  # Indicate the start of a new epoch
+    for _ in range(20):
+        logger.start_batch()  # Indicate the start of a new batch
+        logger.log({'loss': 0.54321256, 'accuracy': 0.85244777})
+```
 
 Yields:
-::
 
-    Epoch 1/4, batch 20/20
-    [================================================][100%]
-    [global 00:00:02 > 00:00:06 | epoch 00:00:02 > 00:00:00]
-    loss: 0.5432 | accuracy: 0.8524 |
-
-    Epoch 2/4, batch 8/20
-    [=================>                              ][40%]
-    [global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-    loss: 0.5432 | accuracy: 0.8524 |
-
-##############
-Advanced usage
-##############
-
-Now you can customize the logger with your own styles and colors.
-You can set the default configuration at the initialization of the logger and then
-you can override it during log. You can also log the averaged value over the epoch.
-For instance:
-::
-
-    logger = Logger(
-        n_epochs=4,
-        n_batches=20,
-        styles='yellow',
-        digits={'accuracy': 2},
-        average=['loss'],  # loss will be averaged over the current epoch
-        bold_keys=True,
-        show_time=False,  # Remove the time bar
-    )
-    for _ in range(4):
-        logger.start_epoch()
-        for _ in range(20):
-            logger.start_batch()
-            # Overwrite the default style for "loss" and add a message
-            logger.log(
-                {'loss': 0.54321256, 'accuracy': 85.244777},
-                styles={'loss': 'italic red'},
-                message="Training is going well?\nYes!",
-            )
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
+## Advanced usage
+
+Now you can customize the logger with your own styles and colors. You can set the default configuration at the initialization of the logger and then you can override it during log. You can also log the averaged value over the epoch. For instance:
+
+```python
+logger = Logger(
+    n_epochs=4,
+    n_batches=20,
+    styles='yellow',
+    digits={'accuracy': 2},
+    average=['loss'],  # loss will be averaged over the current epoch
+    bold_keys=True,
+    show_time=False,  # Remove the time bar
+)
+for _ in range(4):
+    logger.start_epoch()
+    for _ in range(20):
+        logger.start_batch()
+        # Overwrite the default style for "loss" and add a message
+        logger.log(
+            {'loss': 0.54321256, 'accuracy': 85.244777},
+            styles={'loss': 'italic red'},
+            message="Training is going well?\nYes!",
+        )
+```
 
 Yields:
-::
 
-    Epoch 1/4, batch 20/20
-    [================================================][100%]
-    loss: 0.5432 | accuracy: 85 |
-
-    Epoch 2/4, batch 7/20
-    [=================>                              ][35%]
-    [global 00:00:03 > 00:00:05 | epoch 00:00:01 > 00:00:01]
-    loss: 0.5432 | accuracy: 85 |
-    Training is going well?
-    Yes!
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
+
+But with this style:
 
-With "loss: 0.5432" in italic red, "accuracy: 85" in yellow and both keys in bold.
+<span style="color:red">***loss*** *: 0.5432*</span> |
+<span style="color:yellow">**accuracy**: 85</span> |
```

### Comparing `loggerml-0.2.8/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.2.9/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/github_actions_utils/pylint_manager.py` & `loggerml-0.2.9/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/github_actions_utils/pytest_manager.py` & `loggerml-0.2.9/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/licenses_tier/RICH_LICENSE` & `loggerml-0.2.9/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/loggerml.egg-info/PKG-INFO` & `loggerml-0.2.9/loggerml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.8
+Version: 0.2.9
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.8/logml/__init__.py` & `loggerml-0.2.9/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/logml/logger.py` & `loggerml-0.2.9/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/logml/time_utils.py` & `loggerml-0.2.9/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/pre-commit-checks.sh` & `loggerml-0.2.9/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/pyproject.toml` & `loggerml-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/tests/integration/inte_logger.py` & `loggerml-0.2.9/tests/integration/inte_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/tests/integration/inte_two_loggers.py` & `loggerml-0.2.9/tests/integration/inte_two_loggers.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/tests/unit/test_logger.py` & `loggerml-0.2.9/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.8/tests/unit/test_time_utils.py` & `loggerml-0.2.9/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

