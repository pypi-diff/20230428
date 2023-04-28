# Comparing `tmp/adafruit-circuitpython-ov7670-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-ov7670-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ov7670-1.0.8.tar", last modified: Tue Aug  9 19:33:36 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ov7670-1.0.9.tar", last modified: Mon Aug 22 18:45:18 2022, max compression
```

## Comparing `adafruit-circuitpython-ov7670-1.0.8.tar` & `adafruit-circuitpython-ov7670-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.807380 adafruit-circuitpython-ov7670-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.807380 adafruit-circuitpython-ov7670-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.807380 adafruit-circuitpython-ov7670-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.807380 adafruit-circuitpython-ov7670-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-08-09 19:33:36.000000 adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-08-09 19:33:36.000000 adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:33:36.000000 adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-09 19:33:36.000000 adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:33:36.000000 adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    28248 2022-08-09 19:33:27.000000 adafruit-circuitpython-ov7670-1.0.8/adafruit_ov7670.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-08-09 19:33:27.000000 adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_displayio_gcm4_tftshield18.py
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-08-09 19:33:27.000000 adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_displayio_kaluga1_3_ili9341.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-08-09 19:33:27.000000 adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_displayio_pico_st7789_2in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-08-09 19:33:27.000000 adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-08-09 19:33:27.000000 adafruit-circuitpython-ov7670-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-09 19:33:18.000000 adafruit-circuitpython-ov7670-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:33:36.811380 adafruit-circuitpython-ov7670-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.952817 adafruit-circuitpython-ov7670-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-08-22 18:45:18.952817 adafruit-circuitpython-ov7670-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-08-22 18:45:18.000000 adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-08-22 18:45:18.000000 adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:45:18.000000 adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 18:45:18.000000 adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:45:18.000000 adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    28248 2022-08-22 18:45:11.000000 adafruit-circuitpython-ov7670-1.0.9/adafruit_ov7670.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.948817 adafruit-circuitpython-ov7670-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:18.952817 adafruit-circuitpython-ov7670-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-08-22 18:45:11.000000 adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_displayio_gcm4_tftshield18.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-08-22 18:45:11.000000 adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_displayio_kaluga1_3_ili9341.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-08-22 18:45:11.000000 adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_displayio_pico_st7789_2in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-08-22 18:45:11.000000 adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-08-22 18:45:11.000000 adafruit-circuitpython-ov7670-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:45:03.000000 adafruit-circuitpython-ov7670-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:45:18.952817 adafruit-circuitpython-ov7670-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ov7670-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ov7670-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-ov7670-1.0.9/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
       run: |
         echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         pip install --upgrade build twine
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+            sed -i -e "s/0.0.0+auto.0/1.2.3/" $file;
         done;
         python -m build
         twine check dist/*
```

### Comparing `adafruit-circuitpython-ov7670-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-ov7670-1.0.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,11 @@
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+            sed -i -e "s/0.0.0+auto.0/${{github.event.release.tag_name}}/" $file;
         done;
         python -m build
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-ov7670-1.0.8/.gitignore` & `adafruit-circuitpython-ov7670-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ov7670-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/.pylintrc` & `adafruit-circuitpython-ov7670-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ov7670-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/LICENSE` & `adafruit-circuitpython-ov7670-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ov7670-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ov7670-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ov7670-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/PKG-INFO` & `adafruit-circuitpython-ov7670-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ov7670
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for OV7670 cameras
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,ov7670,camera,breakout,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ov7670-1.0.8/README.rst` & `adafruit-circuitpython-ov7670-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/PKG-INFO` & `adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ov7670
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for OV7670 cameras
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,ov7670,camera,breakout,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ov7670-1.0.8/adafruit_circuitpython_ov7670.egg-info/SOURCES.txt` & `adafruit-circuitpython-ov7670-1.0.9/adafruit_circuitpython_ov7670.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/adafruit_ov7670.py` & `adafruit-circuitpython-ov7670-1.0.9/adafruit_ov7670.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   https://github.com/adafruit/circuitpython/releases
 * The CircuitPython build for your board must support the ``imagecapture`` module.
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 # imports
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_OV7670.git"
 
 import time
 
 import digitalio
 import imagecapture
 import pwmio
```

### Comparing `adafruit-circuitpython-ov7670-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ov7670-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/docs/conf.py` & `adafruit-circuitpython-ov7670-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/docs/index.rst` & `adafruit-circuitpython-ov7670-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_displayio_gcm4_tftshield18.py` & `adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_displayio_gcm4_tftshield18.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_displayio_kaluga1_3_ili9341.py` & `adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_displayio_kaluga1_3_ili9341.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_displayio_pico_st7789_2in.py` & `adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_displayio_pico_st7789_2in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/examples/ov7670_simpletest.py` & `adafruit-circuitpython-ov7670-1.0.9/examples/ov7670_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov7670-1.0.8/pyproject.toml` & `adafruit-circuitpython-ov7670-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ov7670"
 description = "CircuitPython driver for OV7670 cameras"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_REPLACE"}
 keywords = [
     "adafruit",
```

