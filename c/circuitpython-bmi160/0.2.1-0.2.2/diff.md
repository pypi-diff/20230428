# Comparing `tmp/circuitpython-bmi160-0.2.1.tar.gz` & `tmp/circuitpython-bmi160-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bmi160-0.2.1.tar", last modified: Sat Apr  1 17:50:03 2023, max compression
+gzip compressed data, was "circuitpython-bmi160-0.2.2.tar", last modified: Fri Apr 28 12:34:37 2023, max compression
```

## Comparing `circuitpython-bmi160-0.2.1.tar` & `circuitpython-bmi160-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.421603 circuitpython-bmi160-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.421603 circuitpython-bmi160-0.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.421603 circuitpython-bmi160-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.421603 circuitpython-bmi160-0.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/bmi160.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-01 17:50:03.000000 circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-01 17:50:03.000000 circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 17:50:03.000000 circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-01 17:50:03.000000 circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 17:50:03.000000 circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_acc_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_acce_datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_gyro_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_gyro_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_gyro_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/examples/bmi160_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-01 17:49:55.000000 circuitpython-bmi160-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-01 17:49:46.000000 circuitpython-bmi160-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 17:50:03.425603 circuitpython-bmi160-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.844716 circuitpython-bmi160-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.844716 circuitpython-bmi160-0.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.844716 circuitpython-bmi160-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    27325 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/bmi160.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-28 12:34:37.000000 circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-28 12:34:37.000000 circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:34:37.000000 circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 12:34:37.000000 circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 12:34:37.000000 circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_acc_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_acce_datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_gyro_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_gyro_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_gyro_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/examples/bmi160_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-28 12:34:30.000000 circuitpython-bmi160-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 12:34:17.000000 circuitpython-bmi160-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:34:37.848716 circuitpython-bmi160-0.2.2/setup.cfg
```

### Comparing `circuitpython-bmi160-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-bmi160-0.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/.github/workflows/release_gh.yml` & `circuitpython-bmi160-0.2.2/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/.gitignore` & `circuitpython-bmi160-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/.pre-commit-config.yaml` & `circuitpython-bmi160-0.2.2/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
```

### Comparing `circuitpython-bmi160-0.2.1/.pylintrc` & `circuitpython-bmi160-0.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/CODE_OF_CONDUCT.md` & `circuitpython-bmi160-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/LICENSE` & `circuitpython-bmi160-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-bmi160-0.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/LICENSES/MIT.txt` & `circuitpython-bmi160-0.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/LICENSES/Unlicense.txt` & `circuitpython-bmi160-0.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/PKG-INFO` & `circuitpython-bmi160-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmi160
-Version: 0.2.1
+Version: 0.2.2
 Summary: Driver for the BMI160 sensor
 Author-email: "Jose D. Montoya" <bmi160@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMI160
 Keywords: adafruit,blinka,circuitpython,micropython,bmi160,acceleration,gyro,magnetic,BMI160,python,step,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -25,14 +25,22 @@
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_BMI160/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_BMI160/actions
     :alt: Build Status
 
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-bmi160.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-bmi160
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-bmi160?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-bmi160
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Driver for the BMI160 sensor
```

### Comparing `circuitpython-bmi160-0.2.1/README.rst` & `circuitpython-bmi160-0.2.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,22 @@
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_BMI160/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_BMI160/actions
     :alt: Build Status
 
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-bmi160.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-bmi160
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-bmi160?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-bmi160
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Driver for the BMI160 sensor
```

### Comparing `circuitpython-bmi160-0.2.1/bmi160.py` & `circuitpython-bmi160-0.2.2/bmi160.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 """
-`bmi160`
+`BMI160`
 ================================================================================
 
 Driver for the BMI160 sensor
 
 
 * Author(s): Jose D. Montoya
 
@@ -16,32 +16,32 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
+
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
 import time
 from micropython import const
 from adafruit_bus_device import i2c_device
 from adafruit_register.i2c_struct import ROUnaryStruct, UnaryStruct
 from adafruit_register.i2c_bits import RWBits
 
 try:
     from busio import I2C
-    from typing_extensions import NoReturn
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMI160.git"
 
 
 _I2C_ADDR = const(0x69)
 _REG_WHOAMI = const(0x00)
 _ERROR_CODE = const(0x02)
 _COMMAND = const(0x7E)
@@ -63,70 +63,101 @@
 BANDWIDTH_50 = const(0b0111)  # 50 Hz
 BANDWIDTH_100 = const(0b1000)  # 100 Hz
 BANDWIDTH_200 = const(0b1001)  # 200 Hz
 BANDWIDTH_400 = const(0b1010)  # 400 Hz
 BANDWIDTH_800 = const(0b1011)  # 800 Hz
 BANDWIDTH_1600 = const(0b1100)  # 1600 Hz
 BANDWIDTH_3200 = const(0b1101)  # 3200 Hz
+bandwidth_values = (
+    BANDWIDTH_25_32,
+    BANDWIDTH_25_16,
+    BANDWIDTH_25_8,
+    BANDWIDTH_25_4,
+    BANDWIDTH_25_2,
+    BANDWIDTH_25,
+    BANDWIDTH_50,
+    BANDWIDTH_100,
+    BANDWIDTH_200,
+    BANDWIDTH_400,
+    BANDWIDTH_800,
+    BANDWIDTH_1600,
+    BANDWIDTH_3200,
+)
+gyro_bandwidth_values = (
+    BANDWIDTH_25,
+    BANDWIDTH_50,
+    BANDWIDTH_100,
+    BANDWIDTH_200,
+    BANDWIDTH_400,
+    BANDWIDTH_800,
+    BANDWIDTH_1600,
+    BANDWIDTH_3200,
+)
 
 # Acceleration Range
 ACCEL_RANGE_2G = const(0b0011)
 ACCEL_RANGE_4G = const(0b0101)
 ACCEL_RANGE_8G = const(0b1000)
 ACCEL_RANGE_16G = const(0b1100)
+acc_range_values = (ACCEL_RANGE_2G, ACCEL_RANGE_4G, ACCEL_RANGE_8G, ACCEL_RANGE_16G)
 
 # UNDERSAMPLE
 NO_UNDERSAMPLE = const(0)
 UNDERSAMPLE = const(1)
+acc_sample_values = (NO_UNDERSAMPLE, UNDERSAMPLE)
 
-# Bandwith Parameter
+# Bandwidth Parameter
 FILTER = const(0)
 AVERAGING = const(1)
+acc_bandwidth_values = (FILTER, AVERAGING)
 
 # Acceleration Data
 ACC_X_LSB = const(0x12)
-ACC_X_MSB = const(0x13)
 ACC_Y_LSB = const(0x14)
-ACC_Y_MSB = const(0x15)
 ACC_Z_LSB = const(0x16)
-ACC_Z_MSB = const(0x17)
 
 # Acc Power Modes
 ACC_POWER_SUSPEND = const(0x10)
 ACC_POWER_NORMAL = const(0x11)
 ACC_POWER_LOWPOWER = const(0x12)
+acc_power_mode_values = (ACC_POWER_LOWPOWER, ACC_POWER_NORMAL, ACC_POWER_SUSPEND)
 
 # Temperature
 TEMP_LSB = const(0x20)
-TEMP_MSB = const(0x21)
 
 # Gyro Data
 GYRO_X_LSB = const(0x0C)
-GYRO_X_MSB = const(0x0D)
 GYRO_Y_LSB = const(0x0E)
-GYRO_Y_MSB = const(0x0F)
 GYRO_Z_LSB = const(0x10)
-GYRO_Z_MSB = const(0x11)
 
 # Gyro Cutoffs
 GYRO_NORMAL = const(0b10)
 GYRO_OSR2 = const(0b01)
 GYRO_OSR4 = const(0b00)
+gyro_cutoffs_values = (GYRO_OSR4, GYRO_OSR2, GYRO_NORMAL)
 
 # Gyro Power Modes
 GYRO_POWER_SUSPEND = const(0x14)
 GYRO_POWER_NORMAL = const(0x15)
 GYRO_POWER_FASTSTARTUP = const(0x17)
+gyro_power_modes = (GYRO_POWER_SUSPEND, GYRO_POWER_NORMAL, GYRO_POWER_FASTSTARTUP)
 
 # Gyro Ranges
 GYRO_RANGE_2000 = const(0b000)
 GYRO_RANGE_1000 = const(0b001)
 GYRO_RANGE_500 = const(0b010)
 GYRO_RANGE_250 = const(0b011)
 GYRO_RANGE_125 = const(0b100)
+gyro_values = (
+    GYRO_RANGE_125,
+    GYRO_RANGE_250,
+    GYRO_RANGE_500,
+    GYRO_RANGE_1000,
+    GYRO_RANGE_2000,
+)
 
 # pylint: disable= invalid-name, too-many-instance-attributes, missing-function-docstring
 
 
 class BMI160:
     """Driver for the BMI160 Sensor connected over I2C.
 
@@ -136,76 +167,80 @@
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`BMI160` class.
     First you will need to import the libraries to use the sensor
 
-        .. code-block:: python
+    .. code-block:: python
 
-            import board
-            import bmi160 as BMI160
+        import board
+        import bmi160 as BMI160
 
     Once this is done you can define your `board.I2C` object and define your sensor object
 
-        .. code-block:: python
+    .. code-block:: python
 
-            i2c = board.I2C()  # uses board.SCL and board.SDA
-            bmi = BMI160.BMI160(i2c)
+        i2c = board.I2C()  # uses board.SCL and board.SDA
+        bmi = BMI160.BMI160(i2c)
 
     Now you have access to the attributes
 
-        .. code-block:: python
+    .. code-block:: python
 
-            accx, accy, accz = bmi.acceleration
-            gyrox, gyroy, gyroz = bmi.gyro
+        accx, accy, accz = bmi.acceleration
+        gyrox, gyroy, gyroz = bmi.gyro
 
 
     """
 
     _device_id = ROUnaryStruct(_REG_WHOAMI, "B")
     _soft_reset = UnaryStruct(_COMMAND, "B")
     _error_code = UnaryStruct(_ERROR_CODE, "B")
     _acc_config = UnaryStruct(_ACCEL_CONFIG, "B")
     _power_mode = UnaryStruct(0x03, "B")
     _gyro_config = UnaryStruct(_GYRO_CONFIG, "B")
 
     # Acceleration Data
-    _acc_data_x_msb = UnaryStruct(ACC_X_MSB, "B")
-    _acc_data_x_lsb = UnaryStruct(ACC_X_LSB, "B")
-    _acc_data_y_msb = UnaryStruct(ACC_Y_MSB, "B")
-    _acc_data_y_lsb = UnaryStruct(ACC_Y_LSB, "B")
-    _acc_data_z_msb = UnaryStruct(ACC_Z_MSB, "B")
-    _acc_data_z_lsb = UnaryStruct(ACC_Z_LSB, "B")
+    _acc_data_x = UnaryStruct(ACC_X_LSB, "<h")
+    _acc_data_y = UnaryStruct(ACC_Y_LSB, "<h")
+    _acc_data_z = UnaryStruct(ACC_Z_LSB, "<h")
     _read = UnaryStruct(_COMMAND, "B")
 
     # ACC_CONF Register (0x40)
     # Sets the output data rate, the bandwidth, and the read mode of the acceleration
     # sensor
     _acc_us = RWBits(1, _ACCEL_CONFIG, 7)
     _acc_bwp = RWBits(1, _ACCEL_CONFIG, 6)
     _acc_odr = RWBits(4, _ACCEL_CONFIG, 0)
 
     # ACC_RANGE Register (0x41)
     # The register allows the selection of the accelerometer g-range
     _acc_range = RWBits(4, _ACC_RANGE, 0)
-    acceleration_scale = {3: 16384, 5: 8192, 8: 4096, 12: 2048}
-    gyro_scale = {0: 16.4, 1: 32.8, 2: 65.6, 3: 131.2, 4: 262.4}
+    acceleration_scale = {
+        "ACCEL_RANGE_2G": 16384,
+        "ACCEL_RANGE_4G": 8192,
+        "ACCEL_RANGE_8G": 4096,
+        "ACCEL_RANGE_16G": 2048,
+    }
+    gyro_scale = {
+        "GYRO_RANGE_125": 16.4,
+        "GYRO_RANGE_250": 32.8,
+        "GYRO_RANGE_500": 65.6,
+        "GYRO_RANGE_1000": 131.2,
+        "GYRO_RANGE_2000": 262.4,
+    }
 
     # Temperature
-    _temp_data_msb = UnaryStruct(TEMP_MSB, "B")
-    _temp_data_lsb = UnaryStruct(TEMP_LSB, "B")
+    _temp_data = UnaryStruct(TEMP_LSB, "<h")
 
     # Gyro Data
-    _gyro_data_x_msb = UnaryStruct(GYRO_X_MSB, "B")
-    _gyro_data_x_lsb = UnaryStruct(GYRO_X_LSB, "B")
-    _gyro_data_y_msb = UnaryStruct(GYRO_Y_MSB, "B")
-    _gyro_data_y_lsb = UnaryStruct(GYRO_Y_LSB, "B")
-    _gyro_data_z_msb = UnaryStruct(GYRO_Z_MSB, "B")
-    _gyro_data_z_lsb = UnaryStruct(GYRO_Z_LSB, "B")
+    _gyro_data_x = UnaryStruct(GYRO_X_LSB, "<h")
+    _gyro_data_y = UnaryStruct(GYRO_Y_LSB, "<h")
+    _gyro_data_z = UnaryStruct(GYRO_Z_LSB, "<h")
 
     # GYRO_CONF Register (0x41)
     # Sets the output data rate, the bandwidth, and the read mode of the gyro
     # sensor
     _gyro_bwp = RWBits(2, _GYRO_CONFIG, 4)
     _gyro_odr = RWBits(4, _GYRO_CONFIG, 0)
 
@@ -223,25 +258,25 @@
         self._read = 0x03
         time.sleep(0.1)
         self._read = ACC_POWER_NORMAL
         time.sleep(0.1)
         self._read = GYRO_POWER_NORMAL
         time.sleep(0.1)
 
-    def soft_reset(self) -> NoReturn:
+    def soft_reset(self) -> None:
         """
         Performs a Soft Reset
 
-        :return: NoReturn
+        :return: None
 
         """
         self._soft_reset = RESET_COMMAND
         time.sleep(0.015)
 
-    def error_code(self) -> NoReturn:
+    def error_code(self) -> None:
         """
         The register is meant for debug purposes, not for regular verification
         if an operation completed successfully.
 
         Fatal Error: Error during bootup. Broken hardware(e.g.NVM error, see
         ASIC spec for details).This flag will not be cleared after reading the
         register.The only way to clear the flag is a POR.
@@ -266,15 +301,15 @@
             print("Drop Command Error")
         if code_errors[error_codes] != "No Error":
             print(code_errors[error_codes])
         if fatal_error:
             print("Fatal Error")
 
     @property
-    def acceleration_undersample(self) -> int:
+    def acceleration_undersample(self) -> str:
         """
         The undersampling parameter is typically used in low power mode.
         When acc_us is set to ‘0’ and the accelerometer is in low-power mode,
         it will change to normal mode. If the acc_us is set to ‘0’ and a
         command to enter low-power mode is sent to the Register (0x7E) CMD,
         this command is ignored.
 
@@ -283,43 +318,49 @@
         +========================================+=========================+
         | :py:const:`BMI160.NO_UNDERSAMPLE`      | :py:const:`0`           |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.UNDERSAMPLE`         | :py:const:`1`           |
         +----------------------------------------+-------------------------+
 
         """
-        return self._acc_us
+        sample_values = ("NO_UNDERSAMPLE", "UNDERSAMPLE")
+        return sample_values[self._acc_us]
 
     @acceleration_undersample.setter
-    def acceleration_undersample(self, value: int) -> NoReturn:
+    def acceleration_undersample(self, value: int) -> None:
+        if value not in acc_sample_values:
+            raise ValueError("Value must be a valid acceleration undersample value")
         self._acc_us = value
 
     @property
-    def acceleration_bandwidth_parameter(self) -> int:
+    def acceleration_bandwidth_parameter(self) -> str:
         """
         Determines filter configuration (acc_us=0) and averaging for
         undersampling mode (acc_us=1).
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
         | :py:const:`BMI160.FILTER`              | :py:const:`0`           |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.AVERAGING`           | :py:const:`1`           |
         +----------------------------------------+-------------------------+
 
         """
-        return self._acc_bwp
+        values = ("FILTER", "AVERAGING")
+        return values[self._acc_bwp]
 
     @acceleration_bandwidth_parameter.setter
-    def acceleration_bandwidth_parameter(self, value: int) -> NoReturn:
+    def acceleration_bandwidth_parameter(self, value: int) -> None:
+        if value not in acc_bandwidth_values:
+            raise ValueError("Value must a be a valid Acceleration bandwidth setting")
         self._acc_bwp = value
 
     @property
-    def acceleration_output_data_rate(self) -> int:
+    def acceleration_output_data_rate(self) -> str:
         """
         Define the output data rate in Hz is given by :math:`100/2^(8-accodr)`
         The output data rate is independent of the power mode setting for the sensor
 
         Configurations without a bandwidth number are illegal settings and will
         result in an error code in the Register (0x02) ERR_REG.
 
@@ -350,22 +391,39 @@
         +----------------------------------------+---------------------------------+
         | :py:const:`BMI160.BANDWIDTH_800`       | :py:const:`0b1011` 800 Hz       |
         +----------------------------------------+---------------------------------+
         | :py:const:`BMI160.BANDWIDTH_1600`      | :py:const:`0b1100` 1600 Hz      |
         +----------------------------------------+---------------------------------+
 
         """
-        return self._acc_odr
+        values = (
+            "BANDWIDTH_25_32",
+            "BANDWIDTH_25_16",
+            "BANDWIDTH_25_8",
+            "BANDWIDTH_25_4",
+            "BANDWIDTH_25_2",
+            "BANDWIDTH_25",
+            "BANDWIDTH_50",
+            "BANDWIDTH_100",
+            "BANDWIDTH_200",
+            "BANDWIDTH_400",
+            "BANDWIDTH_800",
+            "BANDWIDTH_1600",
+            "BANDWIDTH_3200",
+        )
+        return values[self._acc_odr]
 
     @acceleration_output_data_rate.setter
-    def acceleration_output_data_rate(self, value: int) -> NoReturn:
+    def acceleration_output_data_rate(self, value: int) -> None:
+        if value not in bandwidth_values:
+            raise ValueError("Value must be a valid Acceleration Data Rate setting")
         self._acc_odr = value
 
     @property
-    def acceleration_range(self) -> int:
+    def acceleration_range(self) -> str:
         """
         The register allows the selection of the accelerometer g-range.
         Changing the range of the accelerometer does not clear the data
         ready bit in the Register (0x1B) STATUS. It is recommended to
         read the Register (0x04-0x17) DATA after the range change to
         remove a stall data ready bit from before the range change.
 
@@ -378,58 +436,68 @@
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.ACCEL_RANGE_8G`      | :py:const:`0b1000`      |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.ACCEL_RANGE_16G`     | :py:const:`0b1100`      |
         +----------------------------------------+-------------------------+
 
         """
-        return self._acc_range
+        values = {
+            3: "ACCEL_RANGE_2G",
+            5: "ACCEL_RANGE_4G",
+            8: "ACCEL_RANGE_8G",
+            12: "ACCEL_RANGE_16G",
+        }
+        return values[self._acc_range]
 
     @acceleration_range.setter
-    def acceleration_range(self, value: int) -> NoReturn:
+    def acceleration_range(self, value: int) -> None:
+        if value not in acc_range_values:
+            raise ValueError("Value must be a valid Acceleration Range setting")
         self._acc_range = value
 
     @property
     def acceleration(self) -> Tuple[int, int, int]:
 
         factor = self.acceleration_scale[self.acceleration_range]
 
-        x = (self._acc_data_x_msb * 256 + self._acc_data_x_lsb) / factor
-        y = (self._acc_data_y_msb * 256 + self._acc_data_y_lsb) / factor
-        z = (self._acc_data_z_msb * 256 + self._acc_data_z_lsb) / factor
+        x = self._acc_data_x / factor
+        y = self._acc_data_y / factor
+        z = self._acc_data_z / factor
         return x, y, z
 
-    def power_mode_status(self) -> NoReturn:
+    def power_mode_status(self) -> None:
         values = self._power_mode
 
         acc_pmu_status = (values & 0x18) >> 4
         gyr_pmu_status = (values & 0xC) >> 2
         mag_pmu_status = values & 0x03
 
         acc_pmu_codes = {0: "Suspend", 1: "Normal", 2: "Low Power"}
         gyr_pmu_codes = {0: "Suspend", 1: "Normal", 3: "Fast Start - Up"}
         mag_pmu_codes = {0: "Suspend", 1: "Normal", 2: "Low Power"}
 
         print("Acceleration Power Mode: ", acc_pmu_codes[acc_pmu_status])
         print("Gyro Power Mode", gyr_pmu_codes[gyr_pmu_status])
         print("Mag Power Mode", mag_pmu_codes[mag_pmu_status])
 
-    def acc_power_mode(self, value: int) -> NoReturn:
+    def acc_power_mode(self, value: int) -> None:
         """
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
         | :py:const:`BMI160.ACC_POWER_SUSPEND`   | :py:const:`0x10`        |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.ACC_POWER_NORMAL`    | :py:const:`0x11`        |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.POWER_LOWPOWER`      | :py:const:`0x12`        |
         +----------------------------------------+-------------------------+
 
         """
+        if value not in acc_power_mode_values:
+            raise ValueError("Value must be a valid Acceleration Power Mode Setting")
         self._read = value
         time.sleep(0.1)
 
     @property
     def temperature(self) -> int:
         """
         The temperature is disabled when all sensors are in suspend mode. The output
@@ -438,28 +506,28 @@
 
         If the gyroscope is in normal mode (see Register (0x03) PMU_STATUS),
         the temperature is updated every 10 ms (+-12%). If the gyroscope is in suspend
         mode or fast-power up mode, the temperature is updated every 1.28 s aligned
         :return: int
         """
 
-        return ((self._temp_data_msb * 256 + self._temp_data_lsb) * 1 / 2**9) + 23
+        return (self._temp_data * 1 / 2**9) + 23
 
     @property
     def gyro(self) -> Tuple[int, int, int]:
 
         factor = self.gyro_scale[self.gyro_range]
 
-        x = (self._gyro_data_x_msb * 256 + self._gyro_data_x_lsb) / factor
-        y = (self._gyro_data_y_msb * 256 + self._gyro_data_y_lsb) / factor
-        z = (self._gyro_data_z_msb * 256 + self._gyro_data_z_lsb) / factor
+        x = self._gyro_data_x / factor
+        y = self._gyro_data_y / factor
+        z = self._gyro_data_z / factor
         return x, y, z
 
     @property
-    def gyro_output_data_rate(self) -> int:
+    def gyro_output_data_rate(self) -> str:
         """
         Define the output data rate in Hz is given by :math:`100/2^(8-gyroodr)`
         The output data rate is independent of the power mode setting for the sensor
 
         Configurations without a bandwidth number are illegal settings and will
         result in an error code in the Register (0x02) ERR_REG.
 
@@ -486,22 +554,35 @@
         +----------------------------------------+---------------------------------+
         | :py:const:`BMI160.BANDWIDTH_1600`      | :py:const:`0b1100` 1600 Hz      |
         +----------------------------------------+---------------------------------+
         | :py:const:`BMI160.BANDWIDTH_3200`      | :py:const:`0b1101` 3200 Hz      |
         +----------------------------------------+---------------------------------+
 
         """
-        return self._gyro_odr
+        values = (
+            "BANDWIDTH_25",
+            "BANDWIDTH_50",
+            "BANDWIDTH_100",
+            "BANDWIDTH_200",
+            "BANDWIDTH_400",
+            "BANDWIDTH_800",
+            "BANDWIDTH_1600",
+            "BANDWIDTH_3200",
+        )
+
+        return values[self._gyro_odr]
 
     @gyro_output_data_rate.setter
-    def gyro_output_data_rate(self, value: int) -> NoReturn:
+    def gyro_output_data_rate(self, value: int) -> None:
+        if value not in gyro_bandwidth_values:
+            raise ValueError("Value must be a valid Gyro Data Rate setting")
         self._gyro_odr = value
 
     @property
-    def gyro_bandwidth_parameter(self) -> int:
+    def gyro_bandwidth_parameter(self) -> str:
         """
         The gyroscope bandwidth coefficient defines the 3 dB cutoff frequency
          of the low pass filter for the sensor data.
 
         When the filter mode is set to normal (gyr_bwp=0b10), the gyroscope
         data is sampled at equidistant points in the time, defined by the
         gyroscope output data rate parameter (gyr_odr). The output data rate
@@ -533,38 +614,55 @@
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.GYRO_OSR2`           | :py:const:`0b01`        |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.GYRO_OSR4`           | :py:const:`0b00`        |
         +----------------------------------------+-------------------------+
 
         """
-        return self._gyro_bwp
+        values = ("GYRO_OSR4", "GYRO_OSR2", "GYRO_NORMAL")
+        return values[self._gyro_bwp]
 
     @gyro_bandwidth_parameter.setter
-    def gyro_bandwidth_parameter(self, value: int) -> NoReturn:
+    def gyro_bandwidth_parameter(self, value: int) -> None:
+        if value not in gyro_cutoffs_values:
+            raise ValueError("Value must be a valid Gyro Bandwidth setting")
         self._gyro_bwp = value
 
-    def gyro_power_mode(self, value: int) -> NoReturn:
+    @property
+    def gyro_power_mode(self) -> str:
         """
         +-------------------------------------------+-------------------------+
         | Mode                                      | Value                   |
         +===========================================+=========================+
         | :py:const:`BMI160.GYRO_POWER_SUSPEND`     | :py:const:`0x14`        |
         +-------------------------------------------+-------------------------+
         | :py:const:`BMI160.GYRO_POWER_NORMAL`      | :py:const:`0x15`        |
         +-------------------------------------------+-------------------------+
         | :py:const:`BMI160.GYRO_POWER_FASTSTARTUP` | :py:const:`0x17`        |
         +-------------------------------------------+-------------------------+
 
         """
+        g_power_modes = {
+            0x14: "GYRO_POWER_SUSPEND",
+            0x15: "GYRO_POWER_NORMAL",
+            0x17: "GYRO_POWER_FASTSTARTUP",
+        }
+
+        return g_power_modes[self._read]
+
+    @gyro_power_mode.setter
+    def gyro_power_mode(self, value: int) -> None:
+        if value not in gyro_power_modes:
+            raise ValueError("Value must be a valid Gyro Power Mode")
+
         self._read = value
         time.sleep(0.1)
 
     @property
-    def gyro_range(self) -> int:
+    def gyro_range(self) -> str:
         """
         The register allows the selection of the gyro g-range.
         Changing the range of the accelerometer does not clear the data
         ready bit in the Register (0x1B) STATUS. It is recommended to
         read the Register (0x04-0x17) DATA after the range change to
         remove a stall data ready bit from before the range change.
 
@@ -579,12 +677,22 @@
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.GYRO_RANGE_250`      | :py:const:`0b011`       |
         +----------------------------------------+-------------------------+
         | :py:const:`BMI160.GYRO_RANGE_125`      | :py:const:`0b100`       |
         +----------------------------------------+-------------------------+
 
         """
-        return self._gyro_range
+        g_values = (
+            "GYRO_RANGE_125",
+            "GYRO_RANGE_250",
+            "GYRO_RANGE_500",
+            "GYRO_RANGE_1000",
+            "GYRO_RANGE_2000",
+        )
+
+        return g_values[self._gyro_range]
 
     @gyro_range.setter
-    def gyro_range(self, value: int) -> NoReturn:
+    def gyro_range(self, value: int) -> None:
+        if value not in gyro_values:
+            raise ValueError("Value must be a valid Gyro range")
         self._gyro_range = value
```

### Comparing `circuitpython-bmi160-0.2.1/circuitpython_bmi160.egg-info/PKG-INFO` & `circuitpython-bmi160-0.2.2/circuitpython_bmi160.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmi160
-Version: 0.2.1
+Version: 0.2.2
 Summary: Driver for the BMI160 sensor
 Author-email: "Jose D. Montoya" <bmi160@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMI160
 Keywords: adafruit,blinka,circuitpython,micropython,bmi160,acceleration,gyro,magnetic,BMI160,python,step,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -25,14 +25,22 @@
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_BMI160/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_BMI160/actions
     :alt: Build Status
 
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-bmi160.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-bmi160
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-bmi160?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-bmi160
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Driver for the BMI160 sensor
```

### Comparing `circuitpython-bmi160-0.2.1/docs/examples.rst` & `circuitpython-bmi160-0.2.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/docs/index.rst` & `circuitpython-bmi160-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmi160-0.2.1/pyproject.toml` & `circuitpython-bmi160-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bmi160"
 description = "Driver for the BMI160 sensor"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "bmi160@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMI160"}
 keywords = [
     "adafruit",
```

