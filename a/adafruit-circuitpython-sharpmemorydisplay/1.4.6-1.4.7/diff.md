# Comparing `tmp/adafruit-circuitpython-sharpmemorydisplay-1.4.6.tar.gz` & `tmp/adafruit-circuitpython-sharpmemorydisplay-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-sharpmemorydisplay-1.4.6.tar", last modified: Thu Nov 10 18:39:04 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-sharpmemorydisplay-1.4.7.tar", last modified: Fri Apr 28 00:15:03 2023, max compression
```

## Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6.tar` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.623305 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-11-10 18:39:04.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-11-10 18:39:04.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:39:04.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-10 18:39:04.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-10 18:39:04.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-11-10 18:38:57.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_sharpmemorydisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5739 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/font5x8.bin.license
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-10 18:38:57.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/sharpmemorydisplay_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-11-10 18:38:57.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/sharpmemorydisplay_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-11-10 18:38:57.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-10 18:38:48.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:39:04.627306 adafruit-circuitpython-sharpmemorydisplay-1.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.800783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.804783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.804783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_sharpmemorydisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/font5x8.bin.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/setup.cfg
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/.gitignore` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/.pre-commit-config.yaml` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/.pylintrc` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSE` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/MIT.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/PKG-INFO` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sharpmemorydisplay
-Version: 1.4.6
+Version: 1.4.7
 Summary: CircuitPython display control library for Sharp memory displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay
 Keywords: adafruit,sharp,memory,display,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/README.rst` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sharpmemorydisplay
-Version: 1.4.6
+Version: 1.4.7
 Summary: CircuitPython display control library for Sharp memory displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay
 Keywords: adafruit,sharp,memory,display,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/adafruit_sharpmemorydisplay.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_sharpmemorydisplay.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,33 +23,44 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 # pylint: enable=line-too-long
+from __future__ import annotations
+
+
+try:
+    # pylint: disable=unused-import
+    import typing
+    from busio import SPI
+    from digitalio import DigitalInOut
+    from circuitpython_typing.pil import Image
+except ImportError:
+    pass
 
 import adafruit_framebuf
 from adafruit_bus_device.spi_device import SPIDevice
 from micropython import const
 
 try:
     import numpy
 except ImportError:
     numpy = None
 
-__version__ = "1.4.6"
+__version__ = "1.4.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay.git"
 
 _SHARPMEM_BIT_WRITECMD = const(0x80)  # in lsb
 _SHARPMEM_BIT_VCOM = const(0x40)  # in lsb
 _SHARPMEM_BIT_CLEAR = const(0x20)  # in lsb
 
 
-def reverse_bit(num):
+def reverse_bit(num: int) -> int:
     """Turn an LSB byte to an MSB byte, and vice versa. Used for SPI as
     it is LSB for the SHARP, but 99% of SPI implementations are MSB only!"""
     result = 0
     for _ in range(8):
         result <<= 1
         result += num & 1
         num >>= 1
@@ -58,15 +69,23 @@
 
 class SharpMemoryDisplay(adafruit_framebuf.FrameBuffer):
     """A driver for sharp memory displays, you can use any size but the
     full display must be buffered in memory!"""
 
     # pylint: disable=too-many-instance-attributes,abstract-method
 
-    def __init__(self, spi, scs_pin, width, height, *, baudrate=2000000):
+    def __init__(
+        self,
+        spi: SPI,
+        scs_pin: DigitalInOut,
+        width: int,
+        height: int,
+        *,
+        baudrate=2000000,
+    ):
         scs_pin.switch_to_output(value=True)
         self.spi_device = SPIDevice(
             spi, scs_pin, cs_active_value=True, baudrate=baudrate
         )
         # prealloc for when we write the display
         self._buf = bytearray(1)
 
@@ -74,15 +93,15 @@
         # when writing out SPI so lets just do flipping once, in the buffer
         self.buffer = bytearray((width // 8) * height)
         super().__init__(self.buffer, width, height, buf_format=adafruit_framebuf.MHMSB)
 
         # Set the vcom bit to a defined state
         self._vcom = True
 
-    def show(self):
+    def show(self) -> None:
         """write out the frame buffer via SPI, we use MSB SPI only so some
         bit-swapping is required.
         """
 
         with self.spi_device as spi:
 
             image_buffer = bytearray()
@@ -101,15 +120,15 @@
                 image_buffer.extend(self.buffer[slice_from : slice_from + line_len])
                 slice_from += line_len
                 self._buf[0] = 0
                 image_buffer.extend(self._buf)
             image_buffer.extend(self._buf)
             spi.write(image_buffer)
 
-    def image(self, img):
+    def image(self, img: Image) -> None:
         """Set buffer to value of Python Imaging Library image.  The image should
         be in 1 bit mode and a size equal to the display size."""
         # determine our effective width/height, taking rotation into account
         width = self.width
         height = self.height
         if self.rotation in (1, 3):
             width, height = height, width
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/_static/favicon.ico` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/conf.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/docs/index.rst` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/font5x8.bin` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/font5x8.bin`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/sharpmemorydisplay_pillow_demo.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/examples/sharpmemorydisplay_simpletest.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.6/pyproject.toml` & `adafruit-circuitpython-sharpmemorydisplay-1.4.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-sharpmemorydisplay"
 description = "CircuitPython display control library for Sharp memory displays."
-version = "1.4.6"
+version = "1.4.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay"}
 keywords = [
     "adafruit",
```

