# Comparing `tmp/circuitpython_simnple_dial-0.1.0.tar.gz` & `tmp/circuitpython_simnple_dial-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython_simnple_dial-0.1.0.tar", last modified: Sat Mar 18 18:43:37 2023, max compression
+gzip compressed data, was "circuitpython_simnple_dial-0.2.0.tar", last modified: Fri Apr 28 03:26:17 2023, max compression
```

## Comparing `circuitpython_simnple_dial-0.1.0.tar` & `circuitpython_simnple_dial-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.048007 circuitpython_simnple_dial-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.036007 circuitpython_simnple_dial-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.036007 circuitpython_simnple_dial-0.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.036007 circuitpython_simnple_dial-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.036007 circuitpython_simnple_dial-0.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-18 18:43:37.048007 circuitpython_simnple_dial-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.040007 circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-18 18:43:36.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-18 18:43:37.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 18:43:36.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-18 18:43:36.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-18 18:43:36.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.040007 circuitpython_simnple_dial-0.1.0/circuitpython_simple_dial/
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-03-18 18:43:29.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simple_dial/dial_needle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-03-18 18:43:29.000000 circuitpython_simnple_dial-0.1.0/circuitpython_simple_dial/simple_dial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.048007 circuitpython_simnple_dial-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.048007 circuitpython_simnple_dial-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/dial.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/dial.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/dial.png
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/dial.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)  8781743 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/watchwatch.gif
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/docs/watchwatch.gif.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 18:43:37.048007 circuitpython_simnple_dial-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-18 18:43:29.000000 circuitpython_simnple_dial-0.1.0/examples/simple_dial_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-18 18:43:29.000000 circuitpython_simnple_dial-0.1.0/examples/simple_dial_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-18 18:43:29.000000 circuitpython_simnple_dial-0.1.0/examples/simple_dial_two_needles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-18 18:43:29.000000 circuitpython_simnple_dial-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-18 18:43:17.000000 circuitpython_simnple_dial-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 18:43:37.048007 circuitpython_simnple_dial-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.722245 circuitpython_simnple_dial-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.706245 circuitpython_simnple_dial-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.706245 circuitpython_simnple_dial-0.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-28 03:26:17.722245 circuitpython_simnple_dial-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/dial_needle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/simple_dial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.718245 circuitpython_simnple_dial-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.718245 circuitpython_simnple_dial-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.png
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)  8781743 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/watchwatch.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/watchwatch.gif.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.718245 circuitpython_simnple_dial-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/examples/simple_dial_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/examples/simple_dial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/examples/simple_dial_two_needles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:26:17.722245 circuitpython_simnple_dial-0.2.0/setup.cfg
```

### Comparing `circuitpython_simnple_dial-0.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython_simnple_dial-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/.pre-commit-config.yaml` & `circuitpython_simnple_dial-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/.pylintrc` & `circuitpython_simnple_dial-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/CODE_OF_CONDUCT.md` & `circuitpython_simnple_dial-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/LICENSE` & `circuitpython_simnple_dial-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython_simnple_dial-0.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/LICENSES/MIT.txt` & `circuitpython_simnple_dial-0.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/LICENSES/Unlicense.txt` & `circuitpython_simnple_dial-0.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/PKG-INFO` & `circuitpython_simnple_dial-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython_simnple_dial
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple dial widget
 Author-email: "Jose D. Montoya" <simpledial@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_simple_dial.git
 Keywords: adafruit,blinka,circuitpython,displayio,circuitpython,graphics,dial,library,plotting,clock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -24,26 +24,33 @@
     :target: https://circuitpython-simple_dial.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_simple_dial/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-simnple-dial.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-simnple-dial
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-simnple-dial?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-simnple-dial
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha.
-Main Differences:
-
+A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha. Main Differences:
     * Dial is a complete circle
     * Needle is a line. This line could be full or half
     * Needle size could be shortened using the pad option
-    * Others to come.
+    * Can have more than one needle.
+    * Minor ticks can have their own labels
 
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/dial.png
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython_simnple_dial-0.1.0/README.rst` & `circuitpython_simnple_dial-0.2.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -6,26 +6,33 @@
     :target: https://circuitpython-simple_dial.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_simple_dial/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-simnple-dial.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-simnple-dial
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-simnple-dial?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-simnple-dial
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha.
-Main Differences:
-
+A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha. Main Differences:
     * Dial is a complete circle
     * Needle is a line. This line could be full or half
     * Needle size could be shortened using the pad option
-    * Others to come.
+    * Can have more than one needle.
+    * Minor ticks can have their own labels
 
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/dial.png
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/PKG-INFO` & `circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-simnple-dial
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple dial widget
 Author-email: "Jose D. Montoya" <simpledial@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_simple_dial.git
 Keywords: adafruit,blinka,circuitpython,displayio,circuitpython,graphics,dial,library,plotting,clock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -24,26 +24,33 @@
     :target: https://circuitpython-simple_dial.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_simple_dial/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-simnple-dial.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-simnple-dial
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-simnple-dial?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-simnple-dial
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha.
-Main Differences:
-
+A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha. Main Differences:
     * Dial is a complete circle
     * Needle is a line. This line could be full or half
     * Needle size could be shortened using the pad option
-    * Others to come.
+    * Can have more than one needle.
+    * Minor ticks can have their own labels
 
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/dial.png
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython_simnple_dial-0.1.0/circuitpython_simnple_dial.egg-info/SOURCES.txt` & `circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/circuitpython_simple_dial/dial_needle.py` & `circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/dial_needle.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/circuitpython_simple_dial/simple_dial.py` & `circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/simple_dial.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # pylint: disable=too-many-lines, too-many-instance-attributes, too-many-arguments
 # pylint: disable=too-many-locals, too-many-statements, attribute-defined-outside-init
 # pylint: disable=unused-argument, unsubscriptable-object, undefined-variable, invalid-name
+# pylint: disable=invalid-unary-operand-type
 
 import math
 import displayio
 from terminalio import FONT as terminalio_FONT
 from adafruit_display_text import bitmap_label
 import bitmaptools
 
@@ -72,15 +73,21 @@
         width=100,
         height=100,
         padding=5,  # keepout amount around border, in pixels
         tick_color=0xFFFFFF,
         major_ticks=5,  # if int, the total number of major ticks
         major_tick_stroke=4,
         major_tick_length=10,
-        major_tick_labels=("0", "25", "50", "75", "100"),
+        major_tick_labels=(
+            "0",
+            "25",
+            "50",
+            "75",
+        ),
+        minor_tick_labels=None,
         minor_ticks=3,  # if int, the number of minor ticks per major tick
         minor_tick_stroke=1,
         minor_tick_length=5,
         tick_label_font=None,
         tick_label_color=0xFFFFFF,
         rotate_tick_labels=True,
         tick_label_scale=1.0,
@@ -88,14 +95,15 @@
         **kwargs,
     ):
         super().__init__(x=x, y=y, scale=1)
 
         self._background_color = background_color
 
         self._major_tick_labels = major_tick_labels
+        self._minor_ticks_labels = minor_tick_labels
 
         self._tick_color = tick_color
         self._tick_label_color = tick_label_color
         if tick_label_font is None:
             self._tick_label_font = terminalio_FONT
         else:
             self._tick_label_font = tick_label_font
@@ -126,27 +134,33 @@
         # update the dial dimensions to fit inside the requested width and height
         self._adjust_dimensions(width, height)
         self._bounding_box = [0, 0, self._width, self._height]
 
         # create the dial palette and bitmaps
         self.dial_bitmap = displayio.Bitmap(self._width, self._height, 3)
 
-        self.draw_ticks(
+        self.position_major_ticks = self.draw_ticks(
             tick_count=self._major_ticks,
             tick_stroke=self._major_tick_stroke,
             tick_length=self._major_tick_length,
         )
 
-        self.draw_ticks(
+        temporal_position_minor_ticks = self.draw_ticks(
             tick_count=self._minor_ticks * (self._major_ticks - 1) + 1,
             tick_stroke=self._minor_tick_stroke,
             tick_length=self._minor_tick_length,
         )
-
-        self.draw_labels()
+        self.position_minor_ticks = []
+        for element in temporal_position_minor_ticks:
+            if element not in self.position_major_ticks:
+                self.position_minor_ticks.append(element)
+
+        self.draw_labels(self.position_major_ticks, self._major_tick_labels)
+        if self._minor_ticks_labels:
+            self.draw_labels(self.position_minor_ticks, self._minor_ticks_labels)
 
         self.dial_palette = displayio.Palette(4)
         if self._background_color is None:
             self.dial_palette.make_transparent(0)
             self.dial_palette[0] = 0x000000
         else:
             self.dial_palette[0] = self._background_color
@@ -155,36 +169,38 @@
 
         # create the dial tilegrid and append to the self Widget->Group
         self.dial_tilegrid = displayio.TileGrid(
             self.dial_bitmap, pixel_shader=self.dial_palette
         )
         self.append(self.dial_tilegrid)
 
-        points = []
-        for i in range(0, 361, 1):
-            points.append(
-                (
-                    self._dial_center[0]
-                    + int(self._dial_radius * math.cos(i * math.pi / 180)),
-                    self._dial_center[1]
-                    + int(self._dial_radius * math.sin(i * math.pi / 180)),
-                )
-            )
+        self._draw_circle()
 
-        for index, _ in enumerate(points):
-            if index + 1 >= len(points):
-                break
-            bitmaptools.draw_line(
-                self.dial_bitmap,
-                points[index][0],
-                points[index][1],
-                points[index + 1][0],
-                points[index + 1][1],
-                2,
-            )
+    def _draw_circle(self):
+
+        x = 0
+        y = self._dial_radius
+        d = 3 - 2 * self._dial_radius
+
+        while x <= y:
+            self.dial_bitmap[x + self._dial_center[0], y + self._dial_center[1]] = 1
+            self.dial_bitmap[-x + self._dial_center[0], -y + self._dial_center[1]] = 1
+            self.dial_bitmap[x + self._dial_center[0], -y + self._dial_center[1]] = 1
+            self.dial_bitmap[-x + self._dial_center[0], y + self._dial_center[1]] = 1
+            self.dial_bitmap[y + self._dial_center[0], x + self._dial_center[1]] = 1
+            self.dial_bitmap[-y + self._dial_center[0], x + self._dial_center[1]] = 1
+            self.dial_bitmap[-y + self._dial_center[0], -x + self._dial_center[1]] = 1
+            self.dial_bitmap[y + self._dial_center[0], -x + self._dial_center[1]] = 1
+
+            if d <= 0:
+                d = d + (4 * x) + 6
+            else:
+                d = d + 4 * (x - y) + 10
+                y = y - 1
+            x = x + 1
 
     def _adjust_dimensions(self, width, height):
 
         # calculate the pixel dimension to fit within width/height (including padding)
         if (width - 2 * self._padding < 0) or (height - 2 * self._padding < 0):
             raise ValueError("Width, height, or padding size makes zero sized box")
 
@@ -211,27 +227,28 @@
         """Helper function for drawing ticks on the dial widget.  Can be used to
         customize the dial face.
 
         :param int tick_count: number of ticks to be drawn
         :param int tick_stroke: the pixel width of the line used to draw the tick
 
         """
-
+        angle_positions = []
         if tick_count <= 1:
             pass
         else:
             tick_bitmap = displayio.Bitmap(
                 tick_stroke, tick_length, 3
             )  # make a tick line bitmap for blitting
             tick_bitmap.fill(2)
             for i in range(tick_count):
                 this_angle = round(
                     (-180 + ((i * 360 / (tick_count - 1)))) * (2 * math.pi / 360),
                     4,
                 )  # in radians
+                angle_positions.append(this_angle)
                 target_position_x = self._dial_center[0] + self._dial_radius * math.sin(
                     this_angle
                 )
                 target_position_y = self._dial_center[1] - self._dial_radius * math.cos(
                     this_angle
                 )
 
@@ -240,41 +257,43 @@
                     ox=round(target_position_x),
                     oy=round(target_position_y),
                     source_bitmap=tick_bitmap,
                     px=round(tick_bitmap.width / 2),
                     py=0,
                     angle=this_angle,  # in radians
                 )
+        return angle_positions
 
-    def draw_labels(self):
+    def draw_labels(self, positions, labels):
         """Helper function for drawing text labels on the dial widget.  Can be used
         to customize the dial face.
 
         """
 
-        label_count = len(self._major_tick_labels)
+        label_count = len(positions)
 
-        for i, this_label_text in enumerate(self._major_tick_labels):
-            if i >= label_count - 1:
+        for i, this_label_text in enumerate(labels):
+            if i >= label_count:
                 break
             temp_label = bitmap_label.Label(
                 self._tick_label_font, text=this_label_text
             )  # make a tick line bitmap for blitting
 
-            this_angle = (2 * math.pi / 360) * (
-                -180 + i * 360 / (label_count - 1)
-            )  # in radians
+            this_angle = positions[i]
 
             target_position_x = self._dial_center[0] + (
                 self._dial_radius + self._font_height // 2
             ) * math.sin(this_angle)
             target_position_y = self._dial_center[1] - (
                 self._dial_radius + self._font_height // 2
             ) * math.cos(this_angle)
 
+            if not self._rotate_tick_labels:
+                this_angle = 0
+
             bitmaptools.rotozoom(
                 self.dial_bitmap,
                 ox=round(target_position_x),
                 oy=round(target_position_y),
                 source_bitmap=temp_label.bitmap,
                 px=round(temp_label.bitmap.width // 2),
                 py=round(temp_label.bitmap.height // 2),
```

### Comparing `circuitpython_simnple_dial-0.1.0/docs/_static/favicon.ico` & `circuitpython_simnple_dial-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/docs/conf.py` & `circuitpython_simnple_dial-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/docs/dial.jpg` & `circuitpython_simnple_dial-0.2.0/docs/dial.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/docs/dial.png` & `circuitpython_simnple_dial-0.2.0/docs/dial.png`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/docs/examples.rst` & `circuitpython_simnple_dial-0.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/docs/watchwatch.gif` & `circuitpython_simnple_dial-0.2.0/docs/watchwatch.gif`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/examples/simple_dial_test.py` & `circuitpython_simnple_dial-0.2.0/examples/simple_dial_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/examples/simple_dial_two_needles.py` & `circuitpython_simnple_dial-0.2.0/examples/simple_dial_two_needles.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.1.0/pyproject.toml` & `circuitpython_simnple_dial-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython_simnple_dial"
 description = "Simple dial widget"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "simpledial@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_simple_dial.git"}
 keywords = [
     "adafruit",
```

