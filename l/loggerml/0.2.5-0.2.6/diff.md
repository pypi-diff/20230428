# Comparing `tmp/loggerml-0.2.5.tar.gz` & `tmp/loggerml-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-0.2.5.tar", last modified: Fri Apr 28 01:38:37 2023, max compression
+gzip compressed data, was "loggerml-0.2.6.tar", last modified: Fri Apr 28 01:55:15 2023, max compression
```

## Comparing `loggerml-0.2.5.tar` & `loggerml-0.2.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 01:38:13.000000 loggerml-0.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.601664 loggerml-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.605664 loggerml-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 01:38:13.000000 loggerml-0.2.5/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 01:38:13.000000 loggerml-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 01:38:13.000000 loggerml-0.2.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 01:38:13.000000 loggerml-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 01:38:13.000000 loggerml-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:38:37.613664 loggerml-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 01:38:13.000000 loggerml-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 01:38:13.000000 loggerml-0.2.5/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.609664 loggerml-0.2.5/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 01:38:13.000000 loggerml-0.2.5/assets/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 01:38:13.000000 loggerml-0.2.5/assets/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 01:38:13.000000 loggerml-0.2.5/assets/no_n_batches.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.609664 loggerml-0.2.5/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 01:38:13.000000 loggerml-0.2.5/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.609664 loggerml-0.2.5/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 01:38:13.000000 loggerml-0.2.5/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 01:38:37.000000 loggerml-0.2.5/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 01:38:13.000000 loggerml-0.2.5/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 01:38:37.000000 loggerml-0.2.5/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-28 01:38:13.000000 loggerml-0.2.5/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 01:38:13.000000 loggerml-0.2.5/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 01:38:13.000000 loggerml-0.2.5/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 01:38:13.000000 loggerml-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 01:38:13.000000 loggerml-0.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:38:13.000000 loggerml-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:38:37.613664 loggerml-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 01:38:13.000000 loggerml-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.601664 loggerml-0.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:38:37.613664 loggerml-0.2.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 01:38:13.000000 loggerml-0.2.5/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.563723 loggerml-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 01:54:52.000000 loggerml-0.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.555723 loggerml-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.559723 loggerml-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-28 01:54:52.000000 loggerml-0.2.6/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 01:54:52.000000 loggerml-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-04-28 01:54:52.000000 loggerml-0.2.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-28 01:54:52.000000 loggerml-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 01:54:52.000000 loggerml-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:55:15.563723 loggerml-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-28 01:54:52.000000 loggerml-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-28 01:54:52.000000 loggerml-0.2.6/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.559723 loggerml-0.2.6/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   233850 2023-04-28 01:54:52.000000 loggerml-0.2.6/assets/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   373300 2023-04-28 01:54:52.000000 loggerml-0.2.6/assets/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-04-28 01:54:52.000000 loggerml-0.2.6/assets/no_n_batches.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.559723 loggerml-0.2.6/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 01:54:52.000000 loggerml-0.2.6/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 01:54:52.000000 loggerml-0.2.6/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 01:54:52.000000 loggerml-0.2.6/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 01:54:52.000000 loggerml-0.2.6/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 01:54:52.000000 loggerml-0.2.6/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.559723 loggerml-0.2.6/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 01:54:52.000000 loggerml-0.2.6/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.559723 loggerml-0.2.6/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-28 01:55:15.000000 loggerml-0.2.6/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 01:55:15.000000 loggerml-0.2.6/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:55:15.000000 loggerml-0.2.6/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:55:15.000000 loggerml-0.2.6/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 01:55:15.000000 loggerml-0.2.6/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.563723 loggerml-0.2.6/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-28 01:54:52.000000 loggerml-0.2.6/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 01:55:15.000000 loggerml-0.2.6/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-28 01:54:52.000000 loggerml-0.2.6/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-28 01:54:52.000000 loggerml-0.2.6/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 01:54:52.000000 loggerml-0.2.6/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 01:54:52.000000 loggerml-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 01:54:52.000000 loggerml-0.2.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 01:54:52.000000 loggerml-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:55:15.563723 loggerml-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 01:54:52.000000 loggerml-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.555723 loggerml-0.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.563723 loggerml-0.2.6/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 01:54:52.000000 loggerml-0.2.6/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 01:54:52.000000 loggerml-0.2.6/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:55:15.563723 loggerml-0.2.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 01:54:52.000000 loggerml-0.2.6/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 01:54:52.000000 loggerml-0.2.6/tests/unit/test_time_utils.py
```

### Comparing `loggerml-0.2.5/.github/workflows/pipy_deployment.yaml` & `loggerml-0.2.6/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/.github/workflows/pydocstyle.yaml` & `loggerml-0.2.6/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/.github/workflows/pylint.yaml` & `loggerml-0.2.6/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/.github/workflows/tests.yaml` & `loggerml-0.2.6/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/.pylintrc` & `loggerml-0.2.6/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 fail-under=10
 
 # Interpret the stdin as a python script, whose filename needs to be passed as
 # the module_or_package argument.
 #from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
-ignore=CVS
+ignore=CVS,_version.py
 
 # Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against paths and can be in Posix or Windows format.
 ignore-paths=
 
 # Files or directories matching the regex patterns are skipped. The regex
 # matches against base names, not paths. The default value ignores Emacs file
```

### Comparing `loggerml-0.2.5/CONTRIBUTING.md` & `loggerml-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/LICENSE` & `loggerml-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/PKG-INFO` & `loggerml-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.5
+Version: 0.2.6
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.5/README.md` & `loggerml-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/README_pipy.md` & `loggerml-0.2.6/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/assets/advanced.gif` & `loggerml-0.2.6/assets/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/assets/base.gif` & `loggerml-0.2.6/assets/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/assets/no_n_batches.png` & `loggerml-0.2.6/assets/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/github_actions_utils/pydocstyle_manager.py` & `loggerml-0.2.6/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/github_actions_utils/pylint_manager.py` & `loggerml-0.2.6/github_actions_utils/pylint_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     """
     args = sys.argv[1:]
     score = -10000.0  # A default value
     for arg in args:
         if arg.startswith("--score="):
             score = float(arg.split("=")[1])
     if score == -10000.0:
-        raise ValueError(
-            "Please specify the score of Pylint using the flag --score=N."
-        )
+        raise ValueError("Please specify the score of Pylint using the flag --score=N.")
     if score < PYLINT_SCORE_MIN:
         raise ValueError(
             f"Pylint score {score} is lower than minimum ({PYLINT_SCORE_MIN})"
         )
 
     return score
```

### Comparing `loggerml-0.2.5/github_actions_utils/pytest_manager.py` & `loggerml-0.2.6/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/licenses_tier/RICH_LICENSE` & `loggerml-0.2.6/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/loggerml.egg-info/PKG-INFO` & `loggerml-0.2.6/loggerml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 0.2.5
+Version: 0.2.6
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-0.2.5/loggerml.egg-info/SOURCES.txt` & `loggerml-0.2.6/loggerml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/logml/__init__.py` & `loggerml-0.2.6/logml/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     This project is free to use for COMMERCIAL USE, MODIFICATION,
     DISTRIBUTION and PRIVATE USE as long as the original license is
     include as well as this copy right notice.
 """
 from logml._version import __version__, __version_tuple__
 from logml.logger import Logger
 
-__all__ = ['__version__', '__version_tuple__', 'Logger']
+__all__ = ["__version__", "__version_tuple__", "Logger"]
```

### Comparing `loggerml-0.2.5/logml/logger.py` & `loggerml-0.2.6/logml/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from logml.time_utils import get_time_range, sec_to_timestr
 
 VarType = Union[int, float, str, bool]
 DictVarType = Union[Dict[str, int], Dict[str, float], Dict[str, str], Dict[str, bool]]
 
 
-class Logger():
+class Logger:
     """Logger class. Handles int, float, str and bool values.
 
     Parameters
     ----------
     n_epochs : int
         Number of epochs.
     n_batches : Optional[int]
@@ -62,15 +62,15 @@
     def __init__(
         self,
         n_epochs: int,
         n_batches: Optional[int],
         log_interval: int = 1,
         name: Optional[str] = None,
         *,
-        styles: Union[Dict, str] = 'white',
+        styles: Union[Dict, str] = "white",
         digits: Union[Dict, int] = 6,
         average: Optional[List[str]] = None,
         highlight: bool = False,
         silent: bool = False,
         show_bar: bool = True,
         show_time: bool = True,
         bold_keys: bool = False,
@@ -145,19 +145,23 @@
         self.step += 1
         self.current_batch += 1
 
     def _prelog_check(self) -> None:
         """Check if the logger is ready to log."""
         err_message = ""
         if self.current_epoch == 0:
-            err_message += ("You must indicate a new epoch before logging "
-                            "with `logger.new_epoch()` at start of the epoch.\n")
+            err_message += (
+                "You must indicate a new epoch before logging "
+                "with `logger.new_epoch()` at start of the epoch.\n"
+            )
         if self.current_batch == 0:
-            err_message += ("You must indicate a new batch before logging "
-                            "with `logger.new_batch()` just after batch loading.\n")
+            err_message += (
+                "You must indicate a new batch before logging "
+                "with `logger.new_batch()` just after batch loading.\n"
+            )
         if err_message:
             raise ValueError(err_message)
 
     def log(
         self,
         values: Dict[str, VarType],
         *,
@@ -190,19 +194,19 @@
             None to not average. By default None.
         """
         self._prelog_check()
         # Update internal values
         for key, val in values.items():
             self._update_val(key, val)
         # No log if it is not the moment
-        if (self.silent  # Never log if silent
-            or (self.current_batch % self.log_interval != 0
-                and self.current_batch != 1  # Log the first batch
-                and (self.n_batches is None
-                     or self.current_batch != self.n_batches))):  # Log the last batch
+        if self.silent or (  # Never log if silent
+            self.current_batch % self.log_interval != 0
+            and self.current_batch != 1  # Log the first batch
+            and (self.n_batches is None or self.current_batch != self.n_batches)
+        ):  # Log the last batch
             return
 
         # Here we log
 
         cursor.hide()  # Prevent cursor to blinking
         # Move cursor to the beginning of the previous log
         if self.log_lines > 0:
@@ -219,75 +223,89 @@
         self._print_time_info()
         average_dict = {key: True for key in average} if average else {}
         # Print keys and values
         self._print_keys_vals(
             values,
             styles=styles,  # type: ignore
             digits=digits,  # type: ignore
-            average=average_dict
+            average=average_dict,
         )
         # Print message (if available)
         self._print_message(message)
         cursor.show()  # Restore cursor
 
     def _update_val(self, key: str, val: VarType) -> None:
         """Update the internal values."""
         if key not in self.counts:
             self.counts[key] = 0
         if key not in self.mean_vals:
             self.mean_vals[key] = 0
         self.counts[key] += 1
         if isinstance(val, (int, float)):
-            mean = ((self.mean_vals[key] * (self.counts[key]-1) + val)
-                    / self.counts[key])
+            mean = (self.mean_vals[key] * (self.counts[key] - 1) + val) / self.counts[
+                key
+            ]
             self.mean_vals[key] = mean
         self.vals[key] = val
 
     def _print_name(self) -> None:
         """Print the name of the logger."""
         if self.name:
-            self._print(self.name, end='', style=self.name_style)
+            self._print(self.name, end="", style=self.name_style)
             # NOTE: Add clear line escape token to avoid overlapping
-            print('\x1B[0K')
+            print("\x1B[0K")
             self.log_lines += 1
 
     def _print_epoch_batch(self) -> None:
         """Print epoch and batch info."""
         if self.n_batches is not None:
-            self._print(f"Epoch {self.current_epoch}/{self.n_epochs}, "
-                        f"batch {self.current_batch}/{self.n_batches}", end='')
+            self._print(
+                f"Epoch {self.current_epoch}/{self.n_epochs}, "
+                f"batch {self.current_batch}/{self.n_batches}",
+                end="",
+            )
         else:
-            self._print(f"Epoch {self.current_epoch}/{self.n_epochs}, "
-                        f"batch {self.current_batch}", end='')
+            self._print(
+                f"Epoch {self.current_epoch}/{self.n_epochs}, "
+                f"batch {self.current_batch}",
+                end="",
+            )
         # NOTE: Add clear line escape token to avoid overlapping
-        print('\x1B[0K')
+        print("\x1B[0K")
         self.log_lines += 1
 
     def _print_bar(self) -> None:
         """Print progress bar."""
         if self.show_bar:
             if self.n_batches is not None:
                 progress = min(100, int(100 * self.current_batch / self.n_batches))
                 arrow_len = int(47 * progress / 100)
-                arrowhead = '>' if arrow_len < 47 else '='
-                in_progress = '*' if progress < 100 else ''
-                self._print(f"[{'=' * arrow_len}{arrowhead}{'·' * (47-arrow_len)}]"
-                            f"[{progress}%{in_progress}]",
-                            sep='', end='', overflow='ellipsis')
+                arrowhead = ">" if arrow_len < 47 else "="
+                in_progress = "*" if progress < 100 else ""
+                self._print(
+                    f"[{'=' * arrow_len}{arrowhead}{'·' * (47-arrow_len)}]"
+                    f"[{progress}%{in_progress}]",
+                    sep="",
+                    end="",
+                    overflow="ellipsis",
+                )
             else:
                 # NOTE: We don't know the number of batches, so we just print
                 # a bar that cycles every 20 log intervals
                 progress = (self.step // self.log_interval) % 20
                 arrow_len = int(53 * progress / 19)
-                arrowhead = '●'
-                self._print(f"[{'·' * arrow_len}{arrowhead}{'·' * (53-arrow_len)}]",
-                            end='', overflow='ellipsis')
+                arrowhead = "●"
+                self._print(
+                    f"[{'·' * arrow_len}{arrowhead}{'·' * (53-arrow_len)}]",
+                    end="",
+                    overflow="ellipsis",
+                )
 
             # NOTE: Add clear line escape token to avoid overlapping
-            print('\x1B[0K')
+            print("\x1B[0K")
             self.log_lines += 1
 
     def _print_time_info(self) -> None:
         """Print time info."""
         if self.show_time:
             (delta_glob, delta_epoch, eta_glob, eta_epoch) = get_time_range(
                 current_time=time.time(),
@@ -296,22 +314,26 @@
                 current_epoch=self.current_epoch,
                 current_batch=self.current_batch,
                 n_epochs=self.n_epochs,
                 n_batches=self.n_batches,
             )
             delta_glob_str = sec_to_timestr(delta_glob)
             delta_epoch_str = sec_to_timestr(delta_epoch)
-            eta_glob_str = sec_to_timestr(eta_glob) if eta_glob is not None else ' ? '
-            eta_epoch_str = sec_to_timestr(eta_epoch)if eta_epoch is not None else ' ? '
-            time_str = (f"\\[global {delta_glob_str} < {eta_glob_str} | "
-                        f"epoch {delta_epoch_str} < {eta_epoch_str}]")
+            eta_glob_str = sec_to_timestr(eta_glob) if eta_glob is not None else " ? "
+            eta_epoch_str = (
+                sec_to_timestr(eta_epoch) if eta_epoch is not None else " ? "
+            )
+            time_str = (
+                f"\\[global {delta_glob_str} < {eta_glob_str} | "
+                f"epoch {delta_epoch_str} < {eta_epoch_str}]"
+            )
 
-            self._print(time_str, sep='', end='', overflow='ellipsis')
+            self._print(time_str, sep="", end="", overflow="ellipsis")
             # NOTE: Add clear line escape token to avoid overlapping
-            print('\x1B[0K')
+            print("\x1B[0K")
             # Add the extra number of lines printed due to overflow
             self.log_lines += 1 + len(time_str) // self._console.width
 
     def _print_keys_vals(
         self,
         values: Dict[str, VarType],
         *,
@@ -322,67 +344,56 @@
         """Print the key and value."""
         count = 0
         line_len = 0
         for key, val in values.items():
             count += 1
             # Get style, digits and average
             style = self._get_param(
-                key,
-                styles,
-                self.default_styles,
-                default_value='white'
-            )
-            n_digit = self._get_param(
-                key,
-                digits,
-                self.default_digits,
-                default_value=6
+                key, styles, self.default_styles, default_value="white"
             )
+            n_digit = self._get_param(key, digits, self.default_digits, default_value=6)
             avg = self._get_param(
-                key,
-                average,
-                self.default_average,
-                default_value=False
+                key, average, self.default_average, default_value=False
             )
             # Modify value
             if isinstance(val, (int, float)):
                 if avg:
                     val = self.mean_vals[key]
-                val = str(val)[:int(n_digit)].ljust(int(n_digit))
+                val = str(val)[: int(n_digit)].ljust(int(n_digit))
             # str_len: expected length of the string to be printed
             str_len = len(key) + 2 + len(val)
             if line_len + str_len > self._console.width:
                 # Go to next line
                 # NOTE: Add clear line escape token to avoid overlapping
-                print('\x1B[0K')
+                print("\x1B[0K")
                 line_len = 0
                 self.log_lines += 1
             if line_len != 0:
                 # Exists previous key-value pair in the line: add separator
-                self._print(' | ', end='')
+                self._print(" | ", end="")
                 str_len += 2
             # Print key
             if self.bold_keys:
-                self._print(key, style='bold ' + str(style), end=': ', highlight=False)
+                self._print(key, style="bold " + str(style), end=": ", highlight=False)
             else:
-                self._print(key, style=style, end=': ', highlight=False)
+                self._print(key, style=style, end=": ", highlight=False)
             # Print value
-            self._print(val, style=style, end='', highlight=False)
+            self._print(val, style=style, end="", highlight=False)
             line_len += str_len
         # NOTE: Add clear line escape token to avoid overlapping
-        print('\x1B[0K')
+        print("\x1B[0K")
         self.log_lines += 1
 
     @staticmethod
     def _get_param(
         key: str,
         log_configs: Union[DictVarType, VarType, None],
         default_configs: Union[VarType, Dict[str, VarType]],
         *,
-        default_value: VarType
+        default_value: VarType,
     ) -> VarType:
         """Get the parameter for the key on log_configs or default_configs."""
         if isinstance(log_configs, (int, float, str, bool)):
             config = log_configs
         elif log_configs and key in log_configs:
             config = log_configs[key]
         elif not isinstance(default_configs, Dict):
@@ -392,12 +403,12 @@
         else:
             config = default_value
         return config
 
     def _print_message(self, message: Optional[str]) -> None:
         """Print message."""
         if message:
-            for line in message.split('\n'):
-                self._print(line, end='', highlight=False)
+            for line in message.split("\n"):
+                self._print(line, end="", highlight=False)
                 # NOTE: Add clear line escape token to avoid overlapping
-                print('\x1B[0K')
-            self.log_lines += 1 + message.count('\n')
+                print("\x1B[0K")
+            self.log_lines += 1 + message.count("\n")
```

### Comparing `loggerml-0.2.5/logml/time_utils.py` & `loggerml-0.2.6/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/pre-commit-checks.sh` & `loggerml-0.2.6/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/pyproject.toml` & `loggerml-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loggerml-0.2.5/tests/integration/inte_two_loggers.py` & `loggerml-0.2.6/tests/integration/inte_logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,53 @@
-"""Integration tests for 2 loggers."""
+"""Integration tests for Logger."""
 
 import time
 
 from logml.logger import Logger
 
 
 def main() -> None:
     """Integration test for Logger."""
-    n_epochs = 2
-    n_batches_train = 20
-    n_batches_val = 5
-    train_logger = Logger(n_epochs, n_batches_train, name='Training',
-                          name_style='bold dark_orange', styles='red')
-    val_logger = Logger(n_epochs, n_batches_val, name='Validation',
-                        name_style='bold cyan', styles='blue')
-    for _ in range(n_epochs):
-        train_logger.new_epoch()
-        for _ in range(n_batches_train):
-            train_logger.new_batch()
-            time.sleep(0.03)
-            train_logger.log({'train loss': 0.1})
-        val_logger.new_epoch()
-        for _ in range(n_batches_val):
-            val_logger.new_batch()
-            time.sleep(0.06)
-            val_logger.log({'val loss': 0.1})
+    n_epochs = 5
+    n_batches = 10
+    logger = Logger(
+        n_epochs=n_epochs,
+        n_batches=n_batches,
+        log_interval=2,
+        digits={"train acc": 2},
+        styles="yellow",
+        average=["train loss"],
+        bold_keys=True,
+        highlight=True,
+    )
+    logger.start()
+    for i in range(2):
+        for epoch in range(n_epochs):
+            logger.new_epoch()
+            for batch in range(n_batches):
+                logger.new_batch()
+                time.sleep(0.02)
+                styles = {"train loss": "green", "train acc": "blue"}
+                logger.log(
+                    {
+                        "train loss": 1 - epoch / n_epochs,
+                        "train acc": 100 * batch / n_batches,
+                        "mse": 0.2,
+                    },
+                    message="This is...\nok?",
+                    styles=styles,
+                    average=["mse"],
+                )
+        if i == 0:
+            logger.reset()
+            logger.bold_keys = False
+            logger.n_batches = None
+    logger.log(
+        {f"new loss{i}": 0.3 for i in range(1, 13)},
+        styles="red",
+        digits=3,
+        message="\n",
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `loggerml-0.2.5/tests/unit/test_time_utils.py` & `loggerml-0.2.6/tests/unit/test_time_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from logml.time_utils import get_time_range, sec_to_timestr
 
 
 def test_get_time_range() -> None:
     """Test get_time_range."""
     params: Mapping[str, Any] = {
-        'current_time': 4.0,
-        'start_glob': 1.0,
-        'start_epoch': 3.0,
-        'current_epoch': 2,
-        'current_batch': 5,
-        'n_epochs': 4,
-        'n_batches': 10,
+        "current_time": 4.0,
+        "start_glob": 1.0,
+        "start_epoch": 3.0,
+        "current_epoch": 2,
+        "current_batch": 5,
+        "n_epochs": 4,
+        "n_batches": 10,
     }
     (delta_glob, delta_epoch, eta_glob, eta_epoch) = get_time_range(
         current_time=4.0,
         start_glob=1.0,
         start_epoch=3.0,
         current_epoch=2,
         current_batch=5,
@@ -55,15 +55,15 @@
         n_batches=None,
     )
     check.equal(delta_glob, 3.0)
     check.equal(delta_epoch, 1.0)
     check.is_none(eta_glob)
     check.is_none(eta_epoch)
 
-    for key in ['current_batch', 'current_epoch', 'n_epochs', 'n_batches']:
+    for key in ["current_batch", "current_epoch", "n_epochs", "n_batches"]:
         with check.raises(ValueError):
             get_time_range(**{**params, key: 0})
 
 
 def test_sec_to_timestr() -> None:
     """Test sec_to_timestr."""
     timestr = sec_to_timestr(499985.1)
```

