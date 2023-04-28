# Comparing `tmp/adafruit-circuitpython-monsterm4sk-0.3.8.tar.gz` & `tmp/adafruit-circuitpython-monsterm4sk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-monsterm4sk-0.3.8.tar", last modified: Fri Jul 22 19:25:52 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-monsterm4sk-0.3.9.tar", last modified: Mon Jul 25 16:42:43 2022, max compression
```

## Comparing `adafruit-circuitpython-monsterm4sk-0.3.8.tar` & `adafruit-circuitpython-monsterm4sk-0.3.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.018943 adafruit-circuitpython-monsterm4sk-0.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.006942 adafruit-circuitpython-monsterm4sk-0.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.010942 adafruit-circuitpython-monsterm4sk-0.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.010942 adafruit-circuitpython-monsterm4sk-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.014943 adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-07-22 19:25:52.018943 adafruit-circuitpython-monsterm4sk-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.014943 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-07-22 19:25:51.000000 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-07-22 19:25:51.000000 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 19:25:51.000000 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-22 19:25:51.000000 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-22 19:25:51.000000 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6627 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_monsterm4sk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.014943 adafruit-circuitpython-monsterm4sk-0.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.014943 adafruit-circuitpython-monsterm4sk-0.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 19:25:52.018943 adafruit-circuitpython-monsterm4sk-0.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/monsterm4sk_pumpkin_shifting_eyes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/monsterm4sk_rainbow_stars.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/monsterm4sk_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)    25722 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/rainbow_star.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/rainbow_star.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    31526 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/small_triangle_eye.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/examples/small_triangle_eye.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-22 19:25:52.018943 adafruit-circuitpython-monsterm4sk-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-07-22 19:25:31.000000 adafruit-circuitpython-monsterm4sk-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.112699 adafruit-circuitpython-monsterm4sk-0.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-07-25 16:42:42.000000 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-07-25 16:42:43.000000 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 16:42:42.000000 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-25 16:42:42.000000 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-25 16:42:42.000000 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6620 2022-07-25 16:42:35.000000 adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_monsterm4sk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-07-25 16:42:35.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/monsterm4sk_pumpkin_shifting_eyes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-07-25 16:42:35.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/monsterm4sk_rainbow_stars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-07-25 16:42:35.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/monsterm4sk_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25722 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/rainbow_star.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/rainbow_star.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    31526 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/small_triangle_eye.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/examples/small_triangle_eye.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-25 16:42:15.000000 adafruit-circuitpython-monsterm4sk-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-25 16:42:43.116699 adafruit-circuitpython-monsterm4sk-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-07-25 16:42:35.000000 adafruit-circuitpython-monsterm4sk-0.3.9/setup.py
```

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-monsterm4sk-0.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-monsterm4sk-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-monsterm4sk-0.3.9/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -77,9 +77,12 @@
         pip install setuptools wheel twine
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
+        for file in $(find -not -path "./.*" -not -path "./docs*" -name "*.py"); do
+            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+        done;
         python setup.py sdist
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/.gitignore` & `adafruit-circuitpython-monsterm4sk-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-monsterm4sk-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/.pylintrc` & `adafruit-circuitpython-monsterm4sk-0.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-monsterm4sk-0.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/LICENSE` & `adafruit-circuitpython-monsterm4sk-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-monsterm4sk-0.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/PKG-INFO` & `adafruit-circuitpython-monsterm4sk-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-monsterm4sk
-Version: 0.3.8
+Version: 0.3.9
 Summary: Helper library for the MONSTER M4SK device. Allows usage of screens and other built-in hardware.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MONSTERM4SK
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit monsterm4sk microcontroller display breakout hardwaremicropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/README.rst` & `adafruit-circuitpython-monsterm4sk-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/PKG-INFO` & `adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-monsterm4sk
-Version: 0.3.8
+Version: 0.3.9
 Summary: Helper library for the MONSTER M4SK device. Allows usage of screens and other built-in hardware.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MONSTERM4SK
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit monsterm4sk microcontroller display breakout hardwaremicropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_circuitpython_monsterm4sk.egg-info/SOURCES.txt` & `adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_circuitpython_monsterm4sk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/adafruit_monsterm4sk.py` & `adafruit-circuitpython-monsterm4sk-0.3.9/adafruit_monsterm4sk.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import digitalio
 from adafruit_seesaw.seesaw import Seesaw
 import displayio
 import touchio
 from adafruit_st7789 import ST7789
 import adafruit_lis3dh
 
-__version__ = "0.0.0-auto.0"
+__version__ = "0.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MONSTERM4SK.git"
 
 # Seesaw pin numbers
 SS_LIGHTSENSOR_PIN = 2  # "through-hole" light sensor near left eye
 SS_VCCSENSOR_PIN = 3
 SS_BACKLIGHT_PIN = 5  # left screen backlight
 SS_TFTRESET_PIN = 8  # left screen reset
```

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-monsterm4sk-0.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/docs/conf.py` & `adafruit-circuitpython-monsterm4sk-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/docs/examples.rst` & `adafruit-circuitpython-monsterm4sk-0.3.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/docs/index.rst` & `adafruit-circuitpython-monsterm4sk-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/examples/monsterm4sk_pumpkin_shifting_eyes.py` & `adafruit-circuitpython-monsterm4sk-0.3.9/examples/monsterm4sk_pumpkin_shifting_eyes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/examples/monsterm4sk_rainbow_stars.py` & `adafruit-circuitpython-monsterm4sk-0.3.9/examples/monsterm4sk_rainbow_stars.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/examples/monsterm4sk_simpletest.py` & `adafruit-circuitpython-monsterm4sk-0.3.9/examples/monsterm4sk_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/examples/rainbow_star.bmp` & `adafruit-circuitpython-monsterm4sk-0.3.9/examples/rainbow_star.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/examples/small_triangle_eye.bmp` & `adafruit-circuitpython-monsterm4sk-0.3.9/examples/small_triangle_eye.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-monsterm4sk-0.3.8/setup.py` & `adafruit-circuitpython-monsterm4sk-0.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="adafruit-circuitpython-monsterm4sk",
-    use_scm_version=True,
+    use_scm_version={
+        # This is needed for the PyPI version munging in the Github Actions release.yml
+        "git_describe_command": "git describe --tags --long",
+        "local_scheme": "no-local-version",
+    },
     setup_requires=["setuptools_scm"],
     description="Helper library for the MONSTER M4SK device. Allows usage of"
     " screens and other built-in hardware.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     # The project's main homepage.
     url="https://github.com/adafruit/Adafruit_CircuitPython_MONSTERM4SK",
```

