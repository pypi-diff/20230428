# Comparing `tmp/loggerml-0.2.7.tar.gz` & `tmp/loggerml-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.2.7.tar", last modified: Fri Apr 28 13:43:14 2023, max compression
+gzip compressed data, was "loggerml-0.2.8.tar", last modified: Fri Apr 28 13:55:39 2023, max compression
```

## Comparing `loggerml-0.2.7.tar` & `loggerml-0.2.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 13:42:57.000000 loggerml-0.2.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.400635 loggerml-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.404635 loggerml-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 13:42:57.000000 loggerml-0.2.7/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 13:42:57.000000 loggerml-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-04-28 13:42:57.000000 loggerml-0.2.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 13:42:57.000000 loggerml-0.2.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 13:42:57.000000 loggerml-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 13:43:14.408635 loggerml-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 13:42:57.000000 loggerml-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 13:42:57.000000 loggerml-0.2.7/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.404635 loggerml-0.2.7/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 13:42:57.000000 loggerml-0.2.7/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 13:42:57.000000 loggerml-0.2.7/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 13:42:57.000000 loggerml-0.2.7/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.404635 loggerml-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.404635 loggerml-0.2.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/source/logml.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.404635 loggerml-0.2.7/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/source/usage/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-28 13:42:57.000000 loggerml-0.2.7/docs/source/usage/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 13:42:57.000000 loggerml-0.2.7/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 13:42:57.000000 loggerml-0.2.7/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 13:42:57.000000 loggerml-0.2.7/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 13:42:57.000000 loggerml-0.2.7/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 13:42:57.000000 loggerml-0.2.7/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 13:42:57.000000 loggerml-0.2.7/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 13:43:14.000000 loggerml-0.2.7/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 13:43:14.000000 loggerml-0.2.7/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:43:14.000000 loggerml-0.2.7/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:43:14.000000 loggerml-0.2.7/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 13:43:14.000000 loggerml-0.2.7/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 13:42:57.000000 loggerml-0.2.7/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:43:14.000000 loggerml-0.2.7/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-28 13:42:57.000000 loggerml-0.2.7/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 13:42:57.000000 loggerml-0.2.7/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 13:42:57.000000 loggerml-0.2.7/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 13:42:57.000000 loggerml-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 13:42:57.000000 loggerml-0.2.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:42:57.000000 loggerml-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:43:14.408635 loggerml-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 13:42:57.000000 loggerml-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.400635 loggerml-0.2.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 13:42:57.000000 loggerml-0.2.7/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 13:42:57.000000 loggerml-0.2.7/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:14.408635 loggerml-0.2.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 13:42:57.000000 loggerml-0.2.7/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 13:42:57.000000 loggerml-0.2.7/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 13:55:23.000000 loggerml-0.2.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.726155 loggerml-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.730155 loggerml-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 13:55:23.000000 loggerml-0.2.8/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 13:55:23.000000 loggerml-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-04-28 13:55:23.000000 loggerml-0.2.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 13:55:23.000000 loggerml-0.2.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 13:55:23.000000 loggerml-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 13:55:39.734156 loggerml-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 13:55:23.000000 loggerml-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 13:55:23.000000 loggerml-0.2.8/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 13:55:23.000000 loggerml-0.2.8/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 13:55:23.000000 loggerml-0.2.8/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 13:55:23.000000 loggerml-0.2.8/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/logml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/usage/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-28 13:55:23.000000 loggerml-0.2.8/docs/source/usage/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 13:55:23.000000 loggerml-0.2.8/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 13:55:23.000000 loggerml-0.2.8/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 13:55:39.000000 loggerml-0.2.8/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 13:55:23.000000 loggerml-0.2.8/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:55:39.000000 loggerml-0.2.8/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-28 13:55:23.000000 loggerml-0.2.8/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 13:55:23.000000 loggerml-0.2.8/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 13:55:23.000000 loggerml-0.2.8/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 13:55:23.000000 loggerml-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 13:55:23.000000 loggerml-0.2.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:55:23.000000 loggerml-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:55:39.734156 loggerml-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 13:55:23.000000 loggerml-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.730155 loggerml-0.2.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:55:39.734156 loggerml-0.2.8/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 13:55:23.000000 loggerml-0.2.8/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.2.7/.github/workflows/pipy_deployment.yaml` & `loggerml-0.2.8/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/.github/workflows/pydocstyle.yaml` & `loggerml-0.2.8/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/.github/workflows/pylint.yaml` & `loggerml-0.2.8/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/.github/workflows/tests.yaml` & `loggerml-0.2.8/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/.pylintrc` & `loggerml-0.2.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/CONTRIBUTING.md` & `loggerml-0.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/LICENSE` & `loggerml-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/PKG-INFO` & `loggerml-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.7
+Version: 0.2.8
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.7/README.md` & `loggerml-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/README_pipy.md` & `loggerml-0.2.8/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/assets/advanced.gif` & `loggerml-0.2.8/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/assets/base.gif` & `loggerml-0.2.8/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/assets/no_n_batches.png` & `loggerml-0.2.8/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/docs/README.rst` & `loggerml-0.2.8/docs/README.rst`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/docs/index.rst` & `loggerml-0.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/docs/source/conf.py` & `loggerml-0.2.8/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# Configuration file for the Sphinx documentation builder.
-#
+"""Configuration file for the Sphinx documentation builder."""
+# pylint: disable=all
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath('../..'))
 
+from logml import __version__  # noqa E402
+
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'LoggerML'
-copyright = '2023, Valentin Goldite'
+copyright = '2023, Valentin Goldite'  # noqa A001
 author = 'Valentin Goldite'
-release = '0.2.6'
+release = __version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 # Add napoleon to the extensions list
-extensions = ['myst_parser', 'sphinx.ext.napoleon']
+extensions = ['sphinx.ext.napoleon']
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 
 # Napoleon settings
 napoleon_google_docstring = True
```

### Comparing `loggerml-0.2.7/docs/source/usage/quickstart.rst` & `loggerml-0.2.8/docs/source/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.2.8/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/github_actions_utils/pylint_manager.py` & `loggerml-0.2.8/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/github_actions_utils/pytest_manager.py` & `loggerml-0.2.8/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/licenses_tier/RICH_LICENSE` & `loggerml-0.2.8/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/loggerml.egg-info/PKG-INFO` & `loggerml-0.2.8/loggerml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.7
+Version: 0.2.8
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.7/loggerml.egg-info/SOURCES.txt` & `loggerml-0.2.8/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/logml/__init__.py` & `loggerml-0.2.8/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/logml/logger.py` & `loggerml-0.2.8/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/logml/time_utils.py` & `loggerml-0.2.8/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/pre-commit-checks.sh` & `loggerml-0.2.8/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/pyproject.toml` & `loggerml-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/tests/integration/inte_logger.py` & `loggerml-0.2.8/tests/integration/inte_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/tests/integration/inte_two_loggers.py` & `loggerml-0.2.8/tests/integration/inte_two_loggers.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/tests/unit/test_logger.py` & `loggerml-0.2.8/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.7/tests/unit/test_time_utils.py` & `loggerml-0.2.8/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

