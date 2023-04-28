# Comparing `tmp/circuitpython-mag-cal-1.0.3.tar.gz` & `tmp/circuitpython-mag-cal-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mag-cal-1.0.3.tar", last modified: Sun Apr 23 00:59:18 2023, max compression
+gzip compressed data, was "circuitpython-mag-cal-1.1.0.tar", last modified: Fri Apr 28 20:11:11 2023, max compression
```

## Comparing `circuitpython-mag-cal-1.0.3.tar` & `circuitpython-mag-cal-1.1.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.978024 circuitpython-mag-cal-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.970024 circuitpython-mag-cal-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-23 00:59:18.978024 circuitpython-mag-cal-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-23 00:59:18.000000 circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-23 00:59:18.000000 circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:59:18.000000 circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 00:59:18.000000 circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 00:59:18.000000 circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/howto.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/examples/mag_cal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.974024 circuitpython-mag-cal-1.0.3/mag_cal/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/nm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/rbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/mag_cal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:59:18.978024 circuitpython-mag-cal-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.978024 circuitpython-mag-cal-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.970024 circuitpython-mag-cal-1.0.3/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:59:18.978024 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ab.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ai.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ai.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/bh.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/bh.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/bi.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/bi.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ee.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ee.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/fb.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/fb.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/hj.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/hj.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/hj2.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/hj2.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/jd.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:59:02.000000 circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/jd.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-23 00:59:11.000000 circuitpython-mag-cal-1.0.3/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.573021 circuitpython-mag-cal-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 20:11:11.000000 circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/howto.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/examples/mag_cal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/mag_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24919 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/mag_cal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.581021 circuitpython-mag-cal-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.577021 circuitpython-mag-cal-1.1.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:11:11.585021 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ab.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ai.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ai.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bh.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bh.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bi.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ee.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/fb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/fb.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj2.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/jd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 20:10:54.000000 circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/jd.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-28 20:11:04.000000 circuitpython-mag-cal-1.1.0/tests/test_sensor.py
```

### Comparing `circuitpython-mag-cal-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mag-cal-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/.gitignore` & `circuitpython-mag-cal-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/.pre-commit-config.yaml` & `circuitpython-mag-cal-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/.pylintrc` & `circuitpython-mag-cal-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/CODE_OF_CONDUCT.md` & `circuitpython-mag-cal-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/LICENSE` & `circuitpython-mag-cal-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/LICENSES/CC-BY-4.0.txt` & `circuitpython-mag-cal-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/LICENSES/MIT.txt` & `circuitpython-mag-cal-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/LICENSES/Unlicense.txt` & `circuitpython-mag-cal-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/PKG-INFO` & `circuitpython-mag-cal-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.0.3
+Version: 1.1.0
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.0.3/README.rst` & `circuitpython-mag-cal-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/PKG-INFO` & `circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.0.3
+Version: 1.1.0
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.0.3/circuitpython_mag_cal.egg-info/SOURCES.txt` & `circuitpython-mag-cal-1.1.0/circuitpython_mag_cal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/docs/_static/favicon.ico` & `circuitpython-mag-cal-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/docs/conf.py` & `circuitpython-mag-cal-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/docs/howto.rst` & `circuitpython-mag-cal-1.1.0/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/docs/index.rst` & `circuitpython-mag-cal-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/examples/mag_cal_simpletest.py` & `circuitpython-mag-cal-1.1.0/examples/mag_cal_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/__init__.py` & `circuitpython-mag-cal-1.1.0/mag_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/axes.py` & `circuitpython-mag-cal-1.1.0/mag_cal/axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/calibration.py` & `circuitpython-mag-cal-1.1.0/mag_cal/calibration.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     # work with normal numpy
     import numpy as np
 except ImportError:
     # or work with ulab if we are in CircuitPython
     from ulab import numpy as np
 
-__version__ = "1.0.3"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/furbrain/CircuitPython_mag_cal.git"
 
 
 def _vector_from_matrices(matrix: np.ndarray, i: int, j: int):
     return np.array([x[i, j] for x in matrix])
 
 
@@ -35,14 +35,23 @@
     Object representing a magnetometer and accelerometer calibration
     """
 
     MAGNETOMETER = 1
     ACCELEROMETER = 2
     BOTH = MAGNETOMETER | ACCELEROMETER
 
+    ELLIPSOID = 0  #: Fit to Ellipsoid
+    AXIS_CORRECTION = 1  #: Fit to ellipsoid then correct any axis misalignment
+    NON_LINEAR = (
+        2  #: as per `AXIS_CORRECTION` and then do correction for non-linear effects
+    )
+    FAST_NON_LINEAR = (
+        3  #: as per `AXIS_CORRECTION` and then do quick non-linear correction
+    )
+
     def __init__(self, mag_axes: str = "+X+Y+Z", grav_axes: str = None):
         """
         Create an object representing the calibration coefficients for a combined
         magnetometer and accelerometer
 
         :param str mag_axes: A string representing how your magnetometer is mounted with respect to
           your device. For each axis XYZ of your device (see above for axis descriptions), state the
@@ -83,14 +92,59 @@
         """
         instance = cls()
         instance.mag = Sensor.from_dict(dct["mag"])
         instance.grav = Sensor.from_dict(dct["grav"])
         instance.ready = dct["ready"]
         return instance
 
+    def calibrate(
+        self,
+        mag_data: np.ndarray,
+        grav_data: np.ndarray,
+        routine: int = FAST_NON_LINEAR,
+    ):
+        """
+        Perform a full calibration, with an algorithm depending on the value of ``routine``. If
+        you select a routine other than `ELLIPSOID` you must provide at least one run
+        of at least four shots in the same direction with varying amonts of roll. Ideally two sets
+        of eight readings, but this is not vital.
+        :param np.ndarray mag_data: Numpy array of magnetic readings of shape (N,3)
+        :param np.ndarray grav_data: Numpy array of gravity readings of shape (M,3)
+        :param routine: what level of calibration to perform:
+
+          * `ELLIPSOID`: Simplest form of calibration, very fast, does not require any sets of
+            readings to be aligned. Does not correct for misalignment between pointer and sensors.
+          * `AXIS_CORRECTION`: This routine performs the `ELLIPSOID` and then applies a
+            rotation to offset any misalignment between the pointer and sensors (and also
+            misalignment between accelrometer and magnetometer if relevant). This process will
+            automatically identify which shots have been taken in the same direction
+          * `NON_LINEAR`: Performs calibration as per `AXIS_CORRECTION`, then uses an
+            optimisation process to account for non-linear sensor response. See `fit_non_linear`
+            for details.
+          * `FAST_NON_LINEAR`: Performs calibration as per `AXIS_CORRECTION`, then uses a
+            least-squares process to account for non-linear sensor response. A lot faster than
+            `NON_LINEAR`, but slightly less accurate. See `fit_non_linear_quick` for details
+
+        :return: Measure of error: percentage error of fit for `ELLIPSOID`,
+          standard deviation of error in degrees for other methods. Normally <1 degree is
+          acceptable, <0.5 degrees is good.
+        """
+        self.fit_ellipsoid(mag_data, grav_data)
+        if routine >= self.AXIS_CORRECTION:
+            runs = self.find_similar_shots(mag_data, grav_data)
+            paired_data = [(mag_data[a:b], grav_data[a:b]) for a, b in runs]
+            self.fit_to_axis(paired_data)
+            if routine == self.NON_LINEAR:
+                self.fit_non_linear(paired_data)
+            elif routine == self.FAST_NON_LINEAR:
+                self.fit_non_linear_quick(paired_data)
+            return self.accuracy(paired_data)
+        # just ellipsod fit done, so use uniformity measure
+        return np.mean(self.uniformity(mag_data, grav_data))
+
     def fit_ellipsoid(
         self, mag_data: np.ndarray, grav_data: np.ndarray
     ) -> Tuple[float, float]:
         """
         Take multiple sets of readings in various directions. You can then use this function
         to determine an ideal set of calibration coefficients
 
@@ -435,7 +489,50 @@
                     [c1 * c3 - s1 * s2 * s3, -c2 * s1, c1 * s3 + c3 * s1 * s2],
                     [c3 * s1 + c1 * s2 * s3, c1 * c2, s1 * s3 - c1 * c3 * s2],
                     [-c2 * s3, s2, c2 * c3],
                 ]
             )
             return matrix
         return [cls.angles_to_matrix(*args) for args in zip(azimuth, inclination, roll)]
+
+    def find_similar_shots(
+        self, mag: np.ndarray, grav: np.ndarray, precision=30, min_run=4
+    ):
+        """
+        Find runs of shots that are within precision degrees of each other
+        :param mag: numpy array of magnetic data
+        :param grav: numpy array of accelerometer data
+        :param precision: number of degrees shots should be within
+        :param min_run: minimum length of run to find
+        :return: list of start and finish indices for each run
+        """
+        azimuths, inclinations, _ = self.get_angles(mag, grav)
+        groups = []
+        i = 0
+        while i < len(azimuths) - min_run:
+            for j in reversed(range(i + min_run, len(azimuths) + 1)):
+                if self._is_a_run(azimuths[i:j], inclinations[i:j], precision):
+                    groups.append([i, j])
+                    i = j
+                    break
+            else:
+                i += 1
+        return groups
+
+    @staticmethod
+    def _is_a_run(azimuths: np.ndarray, inclinations: np.ndarray, precision: float):
+        """
+        Given a list of azimuths and inclinations, return true if they are all near each other
+        :param azimuths: list of azimuths
+        :param inclinations: list of inclinations
+        :param precision: maximum allowed degrees of difference
+        :return:
+        """
+        if max(inclinations) - min(inclinations) > precision:
+            return False
+        if max(azimuths) > 360 - precision:
+            azimuths = (
+                azimuths + 180
+            ) % 360  # rotate by 180 degs if shots near 359/0 degs
+        if max(azimuths) - min(azimuths) > precision:
+            return False
+        return True
```

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/lstsq.py` & `circuitpython-mag-cal-1.1.0/mag_cal/lstsq.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/nm.py` & `circuitpython-mag-cal-1.1.0/mag_cal/nm.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/rbf.py` & `circuitpython-mag-cal-1.1.0/mag_cal/rbf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/sensor.py` & `circuitpython-mag-cal-1.1.0/mag_cal/sensor.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/mag_cal/utils.py` & `circuitpython-mag-cal-1.1.0/mag_cal/utils.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/pyproject.toml` & `circuitpython-mag-cal-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mag-cal"
 description = "Calibrate magnetometer and accelerometer readings"
-version = "1.0.3"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_mag_cal"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ab.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ab.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ai.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ai.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/bh.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bh.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/bi.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/bi.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/ee.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/ee.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/fb.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/fb.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/hj.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/hj2.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/hj2.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/fixtures/cal_data/jd.json` & `circuitpython-mag-cal-1.1.0/tests/fixtures/cal_data/jd.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/test_axes.py` & `circuitpython-mag-cal-1.1.0/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.0.3/tests/test_calibration.py` & `circuitpython-mag-cal-1.1.0/tests/test_calibration.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,28 @@
         matrices = Calibration.angles_to_matrix(azimuths, inclinations, rolls)
         new_az, new_inc, new_roll = Calibration.matrix_to_angles(matrices)
 
         np.testing.assert_array_almost_equal(azimuths, new_az)
         np.testing.assert_array_almost_equal(inclinations, new_inc)
         np.testing.assert_array_almost_equal(rolls, new_roll)
 
+    def test_find_runs(self):
+        for mag, grav, _ in self.fixtures.values():
+            calib = Calibration()
+            calib.fit_ellipsoid(mag, grav)
+            self.assertListEqual(
+                [[8, 16], [16, 24]], calib.find_similar_shots(mag, grav)
+            )
+
+    def test_integration_calibrate(self):
+        for mag, grav, _ in self.fixtures.values():
+            calib = Calibration()
+            accuracy = calib.calibrate(mag, grav)
+            self.assertGreater(0.5, accuracy)
+
     @unittest.skip
     def test_display_non_linear_maps(self):
         # pylint: disable=invalid-name,import-outside-toplevel,cell-var-from-loop
         import matplotlib.pyplot as plt
 
         mag, grav, aligned_data = list(self.fixtures.values())[3]
         calib = Calibration()
```

### Comparing `circuitpython-mag-cal-1.0.3/tests/test_sensor.py` & `circuitpython-mag-cal-1.1.0/tests/test_sensor.py`

 * *Files identical despite different names*

