# Comparing `tmp/circuitpython-isl29125-0.2.1.tar.gz` & `tmp/circuitpython-isl29125-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-isl29125-0.2.1.tar", last modified: Thu Mar 30 15:35:47 2023, max compression
+gzip compressed data, was "circuitpython-isl29125-0.2.3.tar", last modified: Fri Apr 28 18:19:35 2023, max compression
```

## Comparing `circuitpython-isl29125-0.2.1.tar` & `circuitpython-isl29125-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.498556 circuitpython-isl29125-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.502556 circuitpython-isl29125-0.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.502556 circuitpython-isl29125-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-30 15:35:47.000000 circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-30 15:35:47.000000 circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:35:47.000000 circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-30 15:35:47.000000 circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 15:35:47.000000 circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/examples/isl29125_ADC_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/examples/isl29125_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/examples/isl29125_rgb_sensing_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/examples/isl29125_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/examples/isl29125_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/isl29125.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-30 15:35:38.000000 circuitpython-isl29125-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-30 15:35:26.000000 circuitpython-isl29125-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 15:35:47.506556 circuitpython-isl29125-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.592719 circuitpython-isl29125-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.572719 circuitpython-isl29125-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.580719 circuitpython-isl29125-0.2.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.580719 circuitpython-isl29125-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.580719 circuitpython-isl29125-0.2.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-28 18:19:35.592719 circuitpython-isl29125-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.584719 circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-28 18:19:35.000000 circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-28 18:19:35.000000 circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:19:35.000000 circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 18:19:35.000000 circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 18:19:35.000000 circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.588719 circuitpython-isl29125-0.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.588719 circuitpython-isl29125-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:19:35.592719 circuitpython-isl29125-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/examples/isl29125_ADC_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/examples/isl29125_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/examples/isl29125_rgb_sensing_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/examples/isl29125_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/examples/isl29125_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/isl29125.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-28 18:19:26.000000 circuitpython-isl29125-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 18:19:14.000000 circuitpython-isl29125-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:19:35.592719 circuitpython-isl29125-0.2.3/setup.cfg
```

### Comparing `circuitpython-isl29125-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-isl29125-0.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/.github/workflows/release_gh.yml` & `circuitpython-isl29125-0.2.3/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/.gitignore` & `circuitpython-isl29125-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/.pre-commit-config.yaml` & `circuitpython-isl29125-0.2.3/.pre-commit-config.yaml`

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

### Comparing `circuitpython-isl29125-0.2.1/.pylintrc` & `circuitpython-isl29125-0.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/CODE_OF_CONDUCT.md` & `circuitpython-isl29125-0.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/LICENSE` & `circuitpython-isl29125-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-isl29125-0.2.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/LICENSES/MIT.txt` & `circuitpython-isl29125-0.2.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/LICENSES/Unlicense.txt` & `circuitpython-isl29125-0.2.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/PKG-INFO` & `circuitpython-isl29125-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-isl29125
-Version: 0.2.1
+Version: 0.2.3
 Summary: driver for the isl29125 light sensor
 Author-email: "Jose D. Montoya" <isl@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_isl29125
 Keywords: adafruit,blinka,circuitpython,micropython,isl29125,light,lux,sensor,isl29125,circuitpython,red,green,blue,color
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -25,14 +25,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_isl29125/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_isl29125/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-isl29125.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-isl29125
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-isl29125?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-isl29125
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Driver for the isl29125 light sensor.
```

### Comparing `circuitpython-isl29125-0.2.1/README.rst` & `circuitpython-isl29125-0.2.3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_isl29125/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_isl29125/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-isl29125.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-isl29125
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-isl29125?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-isl29125
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Driver for the isl29125 light sensor.
```

### Comparing `circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/PKG-INFO` & `circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-isl29125
-Version: 0.2.1
+Version: 0.2.3
 Summary: driver for the isl29125 light sensor
 Author-email: "Jose D. Montoya" <isl@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_isl29125
 Keywords: adafruit,blinka,circuitpython,micropython,isl29125,light,lux,sensor,isl29125,circuitpython,red,green,blue,color
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -25,14 +25,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_isl29125/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_isl29125/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-isl29125.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-isl29125
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-isl29125?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-isl29125
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Driver for the isl29125 light sensor.
```

### Comparing `circuitpython-isl29125-0.2.1/circuitpython_isl29125.egg-info/SOURCES.txt` & `circuitpython-isl29125-0.2.3/circuitpython_isl29125.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
+docs/_static/Logo.png
+docs/_static/Logo.png.license
+docs/_static/extra_css.css
+docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/isl29125_ADC_resolution.py
 examples/isl29125_operation_mode.py
 examples/isl29125_rgb_sensing_range.py
 examples/isl29125_simpletest.py
 examples/isl29125_threshold.py
```

### Comparing `circuitpython-isl29125-0.2.1/docs/examples.rst` & `circuitpython-isl29125-0.2.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/examples/isl29125_ADC_resolution.py` & `circuitpython-isl29125-0.2.3/examples/isl29125_ADC_resolution.py`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/examples/isl29125_rgb_sensing_range.py` & `circuitpython-isl29125-0.2.3/examples/isl29125_rgb_sensing_range.py`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/examples/isl29125_threshold.py` & `circuitpython-isl29125-0.2.3/examples/isl29125_threshold.py`

 * *Files identical despite different names*

### Comparing `circuitpython-isl29125-0.2.1/isl29125.py` & `circuitpython-isl29125-0.2.3/isl29125.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,19 +22,18 @@
 from micropython import const
 from adafruit_bus_device import i2c_device
 from adafruit_register.i2c_struct import ROUnaryStruct, UnaryStruct
 from adafruit_register.i2c_bits import RWBits
 
 try:
     from busio import I2C
-    from typing_extensions import NoReturn
 except ImportError:
     pass
 
-__version__ = "0.2.1"
+__version__ = "0.2.3"
 __repo__ = "https://github.com/jposada202020/CircuitPython_isl29125.git"
 
 _I2C_ADDR = const(0x44)
 _REG_WHOAMI = const(0x00)
 _CONFIG1 = const(0x01)
 _CONFIG2 = const(0x02)
 _CONFIG3 = const(0x03)
@@ -45,34 +44,47 @@
 GREEN_ONLY = const(0b001)
 RED_ONLY = const(0b010)
 BLUE_ONLY = const(0b11)
 STANDBY = const(0b100)  # No ADC Conversion
 RED_GREEN_BLUE = const(0b101)
 GREEN_RED = const(0b110)
 GREEN_BLUE = const(0b111)
+operation_values = (
+    POWERDOWN,
+    GREEN_ONLY,
+    RED_ONLY,
+    BLUE_ONLY,
+    STANDBY,
+    RED_GREEN_BLUE,
+    GREEN_RED,
+    GREEN_BLUE,
+)
 
 # Sensing Range
 LUX_375 = const(0b0)
 LUX_10K = const(0b1)
+sensing_range_values = (LUX_375, LUX_10K)
 
 # ADC Resolution
 RES_16BITS = const(0b0)
 RES_12BITS = const(0b1)
 
 # Interrupt
 NO_INTERRUPT = const(0b00)
 GREEN_INTERRUPT = const(0b01)
 RED_INTERRUPT = const(0b10)
 BLUE_INTERRUPT = const(0b11)
+interrupt_values = (NO_INTERRUPT, GREEN_INTERRUPT, RED_INTERRUPT, BLUE_INTERRUPT)
 
 # Persistent Control
 IC1 = const(0b00)
 IC2 = const(0b01)
 IC4 = const(0b10)
 IC8 = const(0b11)
+persistent_control_values = (IC1, IC2, IC4, IC8)
 
 # pylint: disable= invalid-name, too-many-instance-attributes, missing-function-docstring
 
 
 class ISL29125:
     """Driver for the ISL29125 Light Sensor connected over I2C.
 
@@ -107,26 +119,21 @@
 
     """
 
     _device_id = ROUnaryStruct(_REG_WHOAMI, "B")
     _conf_reg = UnaryStruct(_CONFIG1, "B")
     _conf_reg2 = UnaryStruct(_CONFIG2, "B")
     _conf_reg3 = UnaryStruct(_CONFIG3, "B")
-    _low_threshold_LSB = UnaryStruct(0x04, "B")
-    _low_threshold_MSB = UnaryStruct(0x05, "B")
-    _high_threshold_LSB = UnaryStruct(0x06, "B")
-    _high_threshold_MSB = UnaryStruct(0x07, "B")
+    _low_threshold = UnaryStruct(0x04, "h")
+    _high_threshold = UnaryStruct(0x06, "h")
     _flag_register = UnaryStruct(0x08, "B")
 
-    _g_LSB = ROUnaryStruct(0x09, "B")
-    _g_MSB = ROUnaryStruct(0x0A, "B")
-    _r_LSB = ROUnaryStruct(0x0B, "B")
-    _r_MSB = ROUnaryStruct(0x0C, "B")
-    _b_LSB = ROUnaryStruct(0x0D, "B")
-    _b_MSB = ROUnaryStruct(0x0E, "B")
+    _green = ROUnaryStruct(0x09, "h")
+    _red = ROUnaryStruct(0x0B, "h")
+    _blue = ROUnaryStruct(0x0D, "h")
 
     _operation_mode = RWBits(3, _CONFIG1, 0)
     _rgb_sensing_range = RWBits(1, _CONFIG1, 3)
     _adc_resolution = RWBits(1, _CONFIG1, 3)
     _ir_compensation = RWBits(1, _CONFIG2, 7)
     _ir_compensation_value = RWBits(6, _CONFIG2, 0)
     _interrupt_threshold_status = RWBits(2, _CONFIG3, 0)
@@ -134,50 +141,50 @@
     _interrupt_triggered_status = RWBits(1, _FLAG_REGISTER, 0)
     _brown_out = RWBits(1, _FLAG_REGISTER, 2)
 
     def __init__(self, i2c_bus: I2C, address: int = _I2C_ADDR) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
 
         if self._device_id != 0x7D:
-            raise RuntimeError("Failed to find ISL29125")
+            raise RuntimeError("Failed to find the ISL29125")
 
         self._conf_reg = 0x0D
         # 0xBF Datasheet recommendation to max out IR compensation value.
         # It makes High range reach more than 10,000lux.
         self._conf_reg2 = 0xBF
         self.clear_register_flag()
         # Setting the brownout to 0 according to datasheet recommendation
         self._brown_out = 0
 
     @property
     def green(self):
         """Green property"""
 
-        return self._g_MSB * 256 + self._g_LSB
+        return self._green
 
     @property
     def red(self):
         """red property"""
 
-        return self._r_MSB * 256 + self._r_LSB
+        return self._red
 
     @property
     def blue(self):
         """blue property"""
 
-        return self._b_MSB * 256 + self._b_LSB
+        return self._blue
 
     @property
     def colors(self):
         """colors property"""
 
-        return self.red, self.green, self.blue
+        return self._red, self._green, self._blue
 
     @property
-    def operation_mode(self) -> int:
+    def operation_mode(self) -> str:
         """The device has various RGB operating modes. The device powers up on
         a disable mode. All operating modes are in continuous ADC
         conversion. The following bits are used to enable the operating mode
 
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
@@ -209,24 +216,35 @@
             isl = isl29125.ISL29125(i2c)
 
 
             isl.operation_mode = isl29125.BLUE_ONLY
 
 
         """
+        values = (
+            "POWERDOWN",
+            "GREEN_ONLY",
+            "RED_ONLY",
+            "BLUE_ONLY",
+            "STANDBY",
+            "RED_GREEN_BLUE",
+            "GREEN_RED",
+            "GREEN_BLUE",
+        )
 
-        return self._operation_mode
+        return values[self._operation_mode]
 
     @operation_mode.setter
-    def operation_mode(self, value: int) -> NoReturn:
-
+    def operation_mode(self, value: int) -> None:
+        if value not in operation_values:
+            raise ValueError("Value must be a valid operation mode setting")
         self._operation_mode = value
 
     @property
-    def sensing_range(self) -> int:
+    def sensing_range(self) -> str:
         """The Full Scale RGB Range has two different selectable ranges at bit 3.
          The range determines the ADC resolution (12 bits and 16 bits).
          Each range has a maximum allowable lux value. Higher range values offer
          better resolution and wider lux value
 
 
         +----------------------------------------+----------------------------------+
@@ -247,24 +265,26 @@
             isl = isl29125.ISL29125(i2c)
 
 
             isl.operation_mode = isl29125.LUX_375
 
 
         """
+        values = ("LUX_375", "LUX_10K")
 
-        return self._rgb_sensing_range
+        return values[self._rgb_sensing_range]
 
     @sensing_range.setter
-    def sensing_range(self, value: int) -> NoReturn:
-
+    def sensing_range(self, value: int) -> None:
+        if value not in sensing_range_values:
+            raise ValueError("Value must be a valid sensing range setting")
         self._rgb_sensing_range = value
 
     @property
-    def adc_resolution(self) -> int:
+    def adc_resolution(self) -> str:
         """ADC’s resolution and the number of clock cycles per conversion is
         determined by this bit. Changing the resolution of the ADC, changes the
         number of clock cycles of the ADC which in turn changes the integration time.
         Integration time is the period the ADC samples the photodiode current signal
         for a measurement
 
 
@@ -286,20 +306,21 @@
             isl = isl29125.ISL29125(i2c)
 
 
             isl.operation_mode = isl29125.RES_12BITS
 
 
         """
-
-        return self._adc_resolution
+        values = ("RES_12BITS", "RES_16BITS")
+        return values[self._adc_resolution]
 
     @adc_resolution.setter
-    def adc_resolution(self, value: int) -> NoReturn:
-
+    def adc_resolution(self, value: int) -> None:
+        if value not in (0, 1):
+            raise ValueError("Value must be a valid adc resolution setting")
         self._adc_resolution = value
 
     @property
     def ir_compensation(self) -> int:
         """The device provides a programmable active IR compensation which allows fine-tuning
          of residual infrared components from the output which allows optimizing the measurement
           variation between differing IR-content light sources.
@@ -326,16 +347,17 @@
 
 
         """
 
         return self._ir_compensation
 
     @ir_compensation.setter
-    def ir_compensation(self, value: int) -> NoReturn:
-
+    def ir_compensation(self, value: int) -> None:
+        if value not in (0, 1):
+            raise ValueError("Value must be a valid ir compensation setting")
         self._ir_compensation = value
 
     @property
     def ir_compensation_value(self) -> int:
         """The effective IR compensation is from 106 to 169 in the CONF2 register.
         Consult datasheet for detailed IR filtering calibration
 
@@ -362,20 +384,21 @@
 
 
         """
 
         return self._ir_compensation_value
 
     @ir_compensation_value.setter
-    def ir_compensation_value(self, value: int) -> NoReturn:
-
+    def ir_compensation_value(self, value: int) -> None:
+        if value not in (1, 2, 4, 8, 16, 32):
+            raise ValueError("Value must be a valid ir compensation setting")
         self._ir_compensation_value = value
 
     @property
-    def interrupt_threshold(self) -> int:
+    def interrupt_threshold(self) -> str:
         """The interrupt_threshold is the status bits for light intensity detection.
         The property:`interrupt_triggered` is set to logic HIGH when the light intensity
         crosses the interrupt thresholds window (register address 0x04 - 0x07)
 
         +----------------------------------------+----------------------------------+
         | Value                                  | Value                            |
         +========================================+==================================+
@@ -397,51 +420,51 @@
             isl = isl29125.ISL29125(i2c)
 
 
             isl.interrupt_threshold = isl29125.BLUE_INTERRUPT
 
 
         """
-
-        return self._interrupt_threshold_status
+        values = ("No Interrupt", "Green Interrupt", "Red Interrupt", "Blue Interrupt")
+        return values[self._interrupt_threshold_status]
 
     @interrupt_threshold.setter
-    def interrupt_threshold(self, value) -> NoReturn:
+    def interrupt_threshold(self, value) -> None:
+        if value not in interrupt_values:
+            raise ValueError("Value must be a valid interrupt threshold Value")
         self._interrupt_threshold_status = value
 
     @property
     def high_threshold(self) -> int:
         """
         The interrupt threshold level is a 16-bit number (Low Threshold-1 and Low Threshold-2).
         The lower interrupt threshold registers are used to set the lower trigger point for
         interrupt generation. If the ALS value crosses below or is equal to the lower
         threshold, an interrupt is asserted on the interrupt pin (LOW) and the interrupt
         status bit (HIGH).
 
         """
 
-        return self._high_threshold_MSB * 256 + self._high_threshold_LSB
+        return self._high_threshold
 
     @high_threshold.setter
-    def high_threshold(self, value: int) -> NoReturn:
-        self._high_threshold_LSB = value & 0xFF
-        self._high_threshold_MSB = value >> 8
+    def high_threshold(self, value: int) -> None:
+        self._high_threshold = value
 
     @property
     def low_threshold(self) -> int:
-        return self._low_threshold_MSB * 256 + self._low_threshold_LSB
+        return self._low_threshold
 
     @low_threshold.setter
-    def low_threshold(self, value: int) -> NoReturn:
-        self._low_threshold_LSB = value & 0xFF
-        self._low_threshold_MSB = value >> 8
+    def low_threshold(self, value: int) -> None:
+        self._low_threshold = value
 
     @property
     def interrupt_triggered(self) -> int:
-        """Is set to high when the interrupt thresholds have been triggered (out of
+        """Is set to high when the interrupt threshold have been triggered (out of
         threshold window) and logic low when not yet triggered.
 
         +----------------------------------------+----------------------------------+
         | Value                                  | Value                            |
         +========================================+==================================+
         | :py:const:`0b0`                        | Interrupt is cleared or          |
         |                                        | not triggered yet                |
@@ -497,19 +520,21 @@
             isl = isl29125.ISL29125(i2c)
 
 
             isl.persistent_control = isl29125.IC4
 
 
         """
+        values = ("IC1", "IC2", "IC4", "IC8")
 
-        return self._interrupt_persistent_control
+        return values[self._interrupt_persistent_control]
 
     @persistent_control.setter
-    def persistent_control(self, value: int) -> NoReturn:
-
+    def persistent_control(self, value: int) -> None:
+        if value not in persistent_control_values:
+            raise ValueError("Value must be a valid persistent control value")
         self._interrupt_persistent_control = value
 
     def clear_register_flag(self):
         """Clears the flag register performing a read action"""
 
         return self._flag_register
```

### Comparing `circuitpython-isl29125-0.2.1/pyproject.toml` & `circuitpython-isl29125-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-isl29125"
 description = "driver for the isl29125 light sensor"
-version = "0.2.1"
+version = "0.2.3"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "isl@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_isl29125"}
 keywords = [
     "adafruit",
```

