# Comparing `tmp/adafruit-circuitpython-hashlib-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-hashlib-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-hashlib-1.4.8.tar", last modified: Mon Aug 22 18:59:21 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-hashlib-1.4.9.tar", last modified: Fri Aug 26 02:44:03 2022, max compression
```

## Comparing `adafruit-circuitpython-hashlib-1.4.8.tar` & `adafruit-circuitpython-hashlib-1.4.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.471222 adafruit-circuitpython-hashlib-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.467222 adafruit-circuitpython-hashlib-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.467222 adafruit-circuitpython-hashlib-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.467222 adafruit-circuitpython-hashlib-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.467222 adafruit-circuitpython-hashlib-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/LICENSES/RSA-MD.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-08-22 18:59:21.471222 adafruit-circuitpython-hashlib-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.467222 adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-08-22 18:59:21.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-08-22 18:59:21.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:59:21.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 18:59:21.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 18:59:21.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.467222 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9535 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_md5.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5696 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha1.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha224.py
--rw-r--r--   0 runner    (1001) docker     (121)    14134 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha256.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha384.py
--rw-r--r--   0 runner    (1001) docker     (121)    17493 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha512.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.471222 adafruit-circuitpython-hashlib-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.471222 adafruit-circuitpython-hashlib-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:59:21.471222 adafruit-circuitpython-hashlib-1.4.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3267 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/examples/hashlib_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-08-22 18:59:14.000000 adafruit-circuitpython-hashlib-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:59:06.000000 adafruit-circuitpython-hashlib-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:59:21.471222 adafruit-circuitpython-hashlib-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.027606 adafruit-circuitpython-hashlib-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.027606 adafruit-circuitpython-hashlib-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/LICENSES/RSA-MD.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-08-26 02:44:03.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-08-26 02:44:03.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:44:03.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:44:03.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:44:03.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9535 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_md5.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5696 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14134 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17493 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha512.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5650 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3267 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/examples/hashlib_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-08-26 02:43:55.000000 adafruit-circuitpython-hashlib-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:43:47.000000 adafruit-circuitpython-hashlib-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:44:03.031606 adafruit-circuitpython-hashlib-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-hashlib-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-hashlib-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-hashlib-1.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-hashlib-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/.gitignore` & `adafruit-circuitpython-hashlib-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-hashlib-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/.pylintrc` & `adafruit-circuitpython-hashlib-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-hashlib-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/LICENSE` & `adafruit-circuitpython-hashlib-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-hashlib-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-hashlib-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/LICENSES/RSA-MD.txt` & `adafruit-circuitpython-hashlib-1.4.9/LICENSES/RSA-MD.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-hashlib-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/PKG-INFO` & `adafruit-circuitpython-hashlib-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hashlib
-Version: 1.4.8
+Version: 1.4.9
 Summary: Secure hashes and message digests
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_hashlib
 Keywords: adafruit,blinka,circuitpython,micropython,hashlib,hashes,,sha1,,sha224,,sha384,,sha512
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hashlib-1.4.8/README.rst` & `adafruit-circuitpython-hashlib-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/PKG-INFO` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hashlib
-Version: 1.4.8
+Version: 1.4.9
 Summary: Secure hashes and message digests
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_hashlib
 Keywords: adafruit,blinka,circuitpython,micropython,hashlib,hashes,,sha1,,sha224,,sha384,,sha512
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_circuitpython_hashlib.egg-info/SOURCES.txt` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_circuitpython_hashlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/__init__.py` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from hashlib import sha3_384 as sha384
 except ImportError:
     from adafruit_hashlib._sha256 import sha224, sha256
     from adafruit_hashlib._sha512 import sha384, sha512
     from adafruit_hashlib._sha1 import sha1
     from adafruit_hashlib._md5 import md5
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_hashlib.git"
 
 # FIPS secure hash algorithms supported by this library
 ALGOS_AVAIL = ["sha1", "md5", "sha224", "sha256", "sha384", "sha512"]
 
 
 def new(algo, data=b""):
```

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_md5.py` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_md5.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha1.py` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha1.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha256.py` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha256.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/adafruit_hashlib/_sha512.py` & `adafruit-circuitpython-hashlib-1.4.9/adafruit_hashlib/_sha512.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-hashlib-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/docs/conf.py` & `adafruit-circuitpython-hashlib-1.4.9/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -39,15 +40,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit hashlib Library"
-copyright = "2019 Brent Rubell"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Brent Rubell"
 author = "Brent Rubell"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-hashlib-1.4.8/docs/index.rst` & `adafruit-circuitpython-hashlib-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/examples/hashlib_simpletest.py` & `adafruit-circuitpython-hashlib-1.4.9/examples/hashlib_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hashlib-1.4.8/pyproject.toml` & `adafruit-circuitpython-hashlib-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-hashlib"
 description = "Secure hashes and message digests"
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_hashlib"}
 keywords = [
     "adafruit",
```

