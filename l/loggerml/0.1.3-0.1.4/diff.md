# Comparing `tmp/loggerml-0.1.3.tar.gz` & `tmp/loggerml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.1.3.tar", last modified: Thu Apr 27 03:27:42 2023, max compression
+gzip compressed data, was "loggerml-0.1.4.tar", last modified: Thu Apr 27 11:17:32 2023, max compression
```

## Comparing `loggerml-0.1.3.tar` & `loggerml-0.1.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 03:27:24.000000 loggerml-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.179008 loggerml-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.183008 loggerml-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-27 03:27:24.000000 loggerml-0.1.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 03:27:24.000000 loggerml-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-27 03:27:24.000000 loggerml-0.1.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-27 03:27:24.000000 loggerml-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 03:27:24.000000 loggerml-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 03:27:42.187008 loggerml-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-27 03:27:24.000000 loggerml-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-27 03:27:24.000000 loggerml-0.1.3/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.183008 loggerml-0.1.3/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-27 03:27:24.000000 loggerml-0.1.3/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-27 03:27:24.000000 loggerml-0.1.3/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-27 03:27:24.000000 loggerml-0.1.3/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.183008 loggerml-0.1.3/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 03:27:24.000000 loggerml-0.1.3/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 03:27:42.000000 loggerml-0.1.3/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 03:27:24.000000 loggerml-0.1.3/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-27 03:27:24.000000 loggerml-0.1.3/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 03:27:24.000000 loggerml-0.1.3/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 03:27:24.000000 loggerml-0.1.3/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-27 03:27:24.000000 loggerml-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 03:27:24.000000 loggerml-0.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 03:27:24.000000 loggerml-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:27:42.187008 loggerml-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 03:27:24.000000 loggerml-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.179008 loggerml-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-27 03:27:24.000000 loggerml-0.1.3/tests/integration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:27:42.187008 loggerml-0.1.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 03:27:24.000000 loggerml-0.1.3/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 03:27:24.000000 loggerml-0.1.3/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 11:17:13.000000 loggerml-0.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.171786 loggerml-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-27 11:17:13.000000 loggerml-0.1.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 11:17:13.000000 loggerml-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-27 11:17:13.000000 loggerml-0.1.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-27 11:17:13.000000 loggerml-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 11:17:13.000000 loggerml-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 11:17:32.175786 loggerml-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-27 11:17:13.000000 loggerml-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-27 11:17:13.000000 loggerml-0.1.4/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-27 11:17:13.000000 loggerml-0.1.4/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-27 11:17:13.000000 loggerml-0.1.4/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-27 11:17:13.000000 loggerml-0.1.4/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 11:17:13.000000 loggerml-0.1.4/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 11:17:13.000000 loggerml-0.1.4/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 11:17:13.000000 loggerml-0.1.4/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 11:17:13.000000 loggerml-0.1.4/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 11:17:13.000000 loggerml-0.1.4/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-27 11:17:32.000000 loggerml-0.1.4/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 11:17:32.000000 loggerml-0.1.4/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:17:32.000000 loggerml-0.1.4/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 11:17:32.000000 loggerml-0.1.4/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 11:17:32.000000 loggerml-0.1.4/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 11:17:13.000000 loggerml-0.1.4/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-27 11:17:13.000000 loggerml-0.1.4/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-27 11:17:13.000000 loggerml-0.1.4/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 11:17:13.000000 loggerml-0.1.4/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-27 11:17:13.000000 loggerml-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 11:17:13.000000 loggerml-0.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 11:17:13.000000 loggerml-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:17:32.175786 loggerml-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 11:17:13.000000 loggerml-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.171786 loggerml-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-27 11:17:13.000000 loggerml-0.1.4/tests/integration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:17:32.175786 loggerml-0.1.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 11:17:13.000000 loggerml-0.1.4/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 11:17:13.000000 loggerml-0.1.4/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.1.3/.github/workflows/pipy_deployment.yaml` & `loggerml-0.1.4/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/.github/workflows/pydocstyle.yaml` & `loggerml-0.1.4/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/.github/workflows/pylint.yaml` & `loggerml-0.1.4/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/.github/workflows/tests.yaml` & `loggerml-0.1.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/.pylintrc` & `loggerml-0.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/CONTRIBUTING.md` & `loggerml-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/LICENSE` & `loggerml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/PKG-INFO` & `loggerml-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.1.3/README.md` & `loggerml-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/README_pipy.md` & `loggerml-0.1.4/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/assets/advanced.gif` & `loggerml-0.1.4/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/assets/base.gif` & `loggerml-0.1.4/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/assets/no_n_batches.png` & `loggerml-0.1.4/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.1.4/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/github_actions_utils/pylint_manager.py` & `loggerml-0.1.4/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/github_actions_utils/pytest_manager.py` & `loggerml-0.1.4/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/loggerml.egg-info/PKG-INFO` & `loggerml-0.1.4/loggerml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.1.3/loggerml.egg-info/SOURCES.txt` & `loggerml-0.1.4/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/logml/__init__.py` & `loggerml-0.1.4/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/logml/logger.py` & `loggerml-0.1.4/logml/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/logml/time_utils.py` & `loggerml-0.1.4/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/pre-commit-checks.sh` & `loggerml-0.1.4/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/pyproject.toml` & `loggerml-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 keywords = ["logging", "machine", "learning"]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["readme", "dependencies", "version"]
 
 [tool.setuptools]
-py-modules = ["logml"]
+packages = ["logml"]
 license-files = ['LICEN[CS]E*', 'COPYING*', 'NOTICE*', 'AUTHORS*']
 
 [tool.setuptools_scm]
 
 [project.urls]
 Source = "https://github.com/valentingol/logml"
```

### Comparing `loggerml-0.1.3/tests/integration/logger.py` & `loggerml-0.1.4/tests/integration/logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/tests/unit/test_logger.py` & `loggerml-0.1.4/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.1.3/tests/unit/test_time_utils.py` & `loggerml-0.1.4/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

