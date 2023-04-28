# Comparing `tmp/loggerml-0.2.4.tar.gz` & `tmp/loggerml-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.2.4.tar", last modified: Fri Apr 28 01:29:55 2023, max compression
+gzip compressed data, was "loggerml-0.2.5.tar", last modified: Fri Apr 28 01:38:37 2023, max compression
```

## Comparing `loggerml-0.2.4.tar` & `loggerml-0.2.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 01:29:32.000000 loggerml-0.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.446137 loggerml-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 01:29:32.000000 loggerml-0.2.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 01:29:32.000000 loggerml-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 01:29:32.000000 loggerml-0.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 01:29:32.000000 loggerml-0.2.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 01:29:32.000000 loggerml-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:29:55.458137 loggerml-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 01:29:32.000000 loggerml-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 01:29:32.000000 loggerml-0.2.4/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 01:29:32.000000 loggerml-0.2.4/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 01:29:32.000000 loggerml-0.2.4/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 01:29:32.000000 loggerml-0.2.4/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 01:29:32.000000 loggerml-0.2.4/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 01:29:32.000000 loggerml-0.2.4/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.454137 loggerml-0.2.4/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 01:29:55.000000 loggerml-0.2.4/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 01:29:32.000000 loggerml-0.2.4/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 01:29:55.000000 loggerml-0.2.4/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-28 01:29:32.000000 loggerml-0.2.4/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 01:29:32.000000 loggerml-0.2.4/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 01:29:32.000000 loggerml-0.2.4/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-28 01:29:32.000000 loggerml-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 01:29:32.000000 loggerml-0.2.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:29:32.000000 loggerml-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:29:55.458137 loggerml-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 01:29:32.000000 loggerml-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.450137 loggerml-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:29:55.458137 loggerml-0.2.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 01:29:32.000000 loggerml-0.2.4/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 01:38:13.000000 loggerml-0.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.601664 loggerml-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.605664 loggerml-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 01:38:13.000000 loggerml-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 01:38:13.000000 loggerml-0.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 01:38:13.000000 loggerml-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 01:38:13.000000 loggerml-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:38:37.613664 loggerml-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 01:38:13.000000 loggerml-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 01:38:13.000000 loggerml-0.2.5/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.609664 loggerml-0.2.5/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 01:38:13.000000 loggerml-0.2.5/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 01:38:13.000000 loggerml-0.2.5/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 01:38:13.000000 loggerml-0.2.5/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.609664 loggerml-0.2.5/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.609664 loggerml-0.2.5/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 01:38:13.000000 loggerml-0.2.5/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 01:38:13.000000 loggerml-0.2.5/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 01:38:37.000000 loggerml-0.2.5/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-28 01:38:13.000000 loggerml-0.2.5/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 01:38:13.000000 loggerml-0.2.5/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 01:38:13.000000 loggerml-0.2.5/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 01:38:13.000000 loggerml-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 01:38:13.000000 loggerml-0.2.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:38:13.000000 loggerml-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:38:37.613664 loggerml-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 01:38:13.000000 loggerml-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.601664 loggerml-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.2.4/.github/workflows/pipy_deployment.yaml` & `loggerml-0.2.5/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/.github/workflows/pydocstyle.yaml` & `loggerml-0.2.5/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/.github/workflows/pylint.yaml` & `loggerml-0.2.5/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/.github/workflows/tests.yaml` & `loggerml-0.2.5/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/.pylintrc` & `loggerml-0.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/CONTRIBUTING.md` & `loggerml-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/LICENSE` & `loggerml-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/PKG-INFO` & `loggerml-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.4
+Version: 0.2.5
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.4/README.md` & `loggerml-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/README_pipy.md` & `loggerml-0.2.5/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/assets/advanced.gif` & `loggerml-0.2.5/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/assets/base.gif` & `loggerml-0.2.5/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/assets/no_n_batches.png` & `loggerml-0.2.5/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.2.5/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/github_actions_utils/pylint_manager.py` & `loggerml-0.2.5/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/github_actions_utils/pytest_manager.py` & `loggerml-0.2.5/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/licenses_tier/RICH_LICENSE` & `loggerml-0.2.5/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/loggerml.egg-info/PKG-INFO` & `loggerml-0.2.5/loggerml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.4
+Version: 0.2.5
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.4/loggerml.egg-info/SOURCES.txt` & `loggerml-0.2.5/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/logml/logger.py` & `loggerml-0.2.5/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/logml/time_utils.py` & `loggerml-0.2.5/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/pre-commit-checks.sh` & `loggerml-0.2.5/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/pyproject.toml` & `loggerml-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = false
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
-exclude = ['*/_version.py', '*/__init__.py']
 files = '*.py'
 follow_imports = 'skip'
 follow_imports_for_stubs = false
 ignore_missing_imports = true
 no_implicit_optional = true
 no_implicit_reexport = true
 pretty = true
```

### Comparing `loggerml-0.2.4/tests/integration/inte_logger.py` & `loggerml-0.2.5/tests/integration/inte_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/tests/integration/inte_two_loggers.py` & `loggerml-0.2.5/tests/integration/inte_two_loggers.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/tests/unit/test_logger.py` & `loggerml-0.2.5/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.4/tests/unit/test_time_utils.py` & `loggerml-0.2.5/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

