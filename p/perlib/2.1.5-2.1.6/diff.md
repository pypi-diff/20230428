# Comparing `tmp/perlib-2.1.5.tar.gz` & `tmp/perlib-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perlib-2.1.5.tar", last modified: Mon Apr 17 14:49:02 2023, max compression
+gzip compressed data, was "perlib-2.1.6.tar", last modified: Fri Apr 28 16:59:45 2023, max compression
```

## Comparing `perlib-2.1.5.tar` & `perlib-2.1.6.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.987751 perlib-2.1.5/
--rw-rw-rw-   0        0        0    11558 2023-04-04 21:29:00.000000 perlib-2.1.5/LICENSE.md
--rw-rw-rw-   0        0        0    10622 2023-04-17 14:49:02.987751 perlib-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    10025 2023-04-04 21:32:21.000000 perlib-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.712430 perlib-2.1.5/perlib/
--rw-rw-rw-   0        0        0      922 2023-04-17 14:48:53.000000 perlib-2.1.5/perlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.750130 perlib-2.1.5/perlib/analysis/
--rw-rw-rw-   0        0        0      131 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/__init__.py
--rw-rw-rw-   0        0        0      863 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/exceptions.py
--rw-rw-rw-   0        0        0     5664 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/multivariate.py
--rw-rw-rw-   0        0        0    10432 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/plotting.py
--rw-rw-rw-   0        0        0     8015 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/univariate.py
--rw-rw-rw-   0        0        0     3208 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/validate.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.750130 perlib-2.1.5/perlib/api/
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/api/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/api/api.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.765920 perlib-2.1.5/perlib/core/
--rw-rw-rw-   0        0        0      454 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/core/__init__.py
--rw-rw-rw-   0        0        0     3740 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/_requests.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.802855 perlib-2.1.5/perlib/core/metrics/
--rw-rw-rw-   0        0        0       56 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/metrics/__init__.py
--rw-rw-rw-   0        0        0    90017 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/metrics/classification.py
--rw-rw-rw-   0        0        0    21214 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/metrics/regression.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.821182 perlib-2.1.5/perlib/core/models/
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/models/__init__.py
--rw-rw-rw-   0        0        0     4843 2023-04-04 22:12:52.000000 perlib-2.1.5/perlib/core/models/dmodels.py
--rw-rw-rw-   0        0        0     7819 2023-04-04 22:13:07.000000 perlib-2.1.5/perlib/core/models/lstnet.py
--rw-rw-rw-   0        0        0     2581 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/models/mmodels.py
--rw-rw-rw-   0        0        0     2302 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/models/smodels.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.836801 perlib-2.1.5/perlib/core/optimizers/
--rw-rw-rw-   0        0        0    32659 2023-04-04 21:52:50.000000 perlib-2.1.5/perlib/core/optimizers/Optimizers.py
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/optimizers/__init__.py
--rw-rw-rw-   0        0        0    11942 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/req_utils.py
--rw-rw-rw-   0        0        0    13165 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/tester.py
--rw-rw-rw-   0        0        0    20024 2023-04-17 14:45:58.000000 perlib-2.1.5/perlib/core/train.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.887350 perlib-2.1.5/perlib/datasets/
--rw-rw-rw-   0        0        0      273 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/__init__.py
--rw-rw-rw-   0        0        0     3158 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/airpassengers.py
--rw-rw-rw-   0        0        0     5263 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/ausbeer.py
--rw-rw-rw-   0        0        0     3337 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/austres.py
--rw-rw-rw-   0        0        0     4709 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/heartrate.py
--rw-rw-rw-   0        0        0     3515 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/lynx.py
--rw-rw-rw-   0        0        0    36115 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/taylor.py
--rw-rw-rw-   0        0        0     4820 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/wineind.py
--rw-rw-rw-   0        0        0     3645 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/woolyrnq.py
--rw-rw-rw-   0        0        0    11981 2023-04-05 07:46:38.000000 perlib-2.1.5/perlib/forecaster.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.906883 perlib-2.1.5/perlib/piplines/
--rw-rw-rw-   0        0        0        0 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/piplines/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-04 22:58:03.000000 perlib-2.1.5/perlib/piplines/dpipline.py
--rw-rw-rw-   0        0        0    21347 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/piplines/mpipline.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.947866 perlib-2.1.5/perlib/preprocessing/
--rw-rw-rw-   0        0        0     5447 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/Normalizing.py
--rw-rw-rw-   0        0        0      241 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     9738 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_split.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.987751 perlib-2.1.5/perlib/preprocessing/_utils/
--rw-rw-rw-   0        0        0      111 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/__init__.py
--rw-rw-rw-   0        0        0     8551 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/dataframe.py
--rw-rw-rw-   0        0        0    27299 2023-04-12 17:23:29.000000 perlib-2.1.5/perlib/preprocessing/_utils/dataset_utils.py
--rw-rw-rw-   0        0        0     9766 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/timeseries_dataset.py
--rw-rw-rw-   0        0        0    12153 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/tools.py
--rw-rw-rw-   0        0        0    13496 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/autopreprocess.py
--rw-rw-rw-   0        0        0     4491 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/encode.py
--rw-rw-rw-   0        0        0    13956 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/imputer.py
--rw-rw-rw-   0        0        0     3446 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/outliers.py
--rw-rw-rw-   0        0        0    19319 2023-04-13 12:15:50.000000 perlib-2.1.5/perlib/preprocessing/preparate.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.728283 perlib-2.1.5/perlib.egg-info/
--rw-rw-rw-   0        0        0    10622 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1693 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:49:02.987751 perlib-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-04 21:29:01.000000 perlib-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.566769 perlib-2.1.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 21:29:00.000000 perlib-2.1.6/LICENSE.md
+-rw-rw-rw-   0        0        0    10622 2023-04-28 16:59:45.566769 perlib-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10025 2023-04-04 21:32:21.000000 perlib-2.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.451923 perlib-2.1.6/perlib/
+-rw-rw-rw-   0        0        0      922 2023-04-28 16:57:08.000000 perlib-2.1.6/perlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.466502 perlib-2.1.6/perlib/analysis/
+-rw-rw-rw-   0        0        0      131 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/__init__.py
+-rw-rw-rw-   0        0        0      863 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/exceptions.py
+-rw-rw-rw-   0        0        0     5664 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/multivariate.py
+-rw-rw-rw-   0        0        0    10432 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/plotting.py
+-rw-rw-rw-   0        0        0     8015 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/univariate.py
+-rw-rw-rw-   0        0        0     3208 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/validate.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.472019 perlib-2.1.6/perlib/api/
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/api/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/api/api.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.482055 perlib-2.1.6/perlib/core/
+-rw-rw-rw-   0        0        0      454 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/core/__init__.py
+-rw-rw-rw-   0        0        0     3740 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/_requests.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.489653 perlib-2.1.6/perlib/core/metrics/
+-rw-rw-rw-   0        0        0       56 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/metrics/__init__.py
+-rw-rw-rw-   0        0        0    90017 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/metrics/classification.py
+-rw-rw-rw-   0        0        0    21214 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/metrics/regression.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.501964 perlib-2.1.6/perlib/core/models/
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/models/__init__.py
+-rw-rw-rw-   0        0        0     4843 2023-04-04 22:12:52.000000 perlib-2.1.6/perlib/core/models/dmodels.py
+-rw-rw-rw-   0        0        0     2601 2023-04-27 08:45:32.000000 perlib-2.1.6/perlib/core/models/elm.py
+-rw-rw-rw-   0        0        0     7819 2023-04-04 22:13:07.000000 perlib-2.1.6/perlib/core/models/lstnet.py
+-rw-rw-rw-   0        0        0     2581 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/models/mmodels.py
+-rw-rw-rw-   0        0        0     2302 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/models/smodels.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.505483 perlib-2.1.6/perlib/core/optimizers/
+-rw-rw-rw-   0        0        0    32659 2023-04-04 21:52:50.000000 perlib-2.1.6/perlib/core/optimizers/Optimizers.py
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/optimizers/__init__.py
+-rw-rw-rw-   0        0        0    11950 2023-04-26 13:57:44.000000 perlib-2.1.6/perlib/core/req_utils.py
+-rw-rw-rw-   0        0        0    13165 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/tester.py
+-rw-rw-rw-   0        0        0    20205 2023-04-28 16:52:41.000000 perlib-2.1.6/perlib/core/train.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.522002 perlib-2.1.6/perlib/datasets/
+-rw-rw-rw-   0        0        0      273 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3158 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/airpassengers.py
+-rw-rw-rw-   0        0        0     5263 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/ausbeer.py
+-rw-rw-rw-   0        0        0     3337 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/austres.py
+-rw-rw-rw-   0        0        0     4709 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/heartrate.py
+-rw-rw-rw-   0        0        0     3515 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/lynx.py
+-rw-rw-rw-   0        0        0    36115 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/taylor.py
+-rw-rw-rw-   0        0        0     4820 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/wineind.py
+-rw-rw-rw-   0        0        0     3645 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/woolyrnq.py
+-rw-rw-rw-   0        0        0    11981 2023-04-05 07:46:38.000000 perlib-2.1.6/perlib/forecaster.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.531943 perlib-2.1.6/perlib/piplines/
+-rw-rw-rw-   0        0        0        0 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/piplines/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-04 22:58:03.000000 perlib-2.1.6/perlib/piplines/dpipline.py
+-rw-rw-rw-   0        0        0    21347 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/piplines/mpipline.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.552153 perlib-2.1.6/perlib/preprocessing/
+-rw-rw-rw-   0        0        0     5447 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/Normalizing.py
+-rw-rw-rw-   0        0        0      241 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     9739 2023-04-28 16:40:53.000000 perlib-2.1.6/perlib/preprocessing/_split.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.566769 perlib-2.1.6/perlib/preprocessing/_utils/
+-rw-rw-rw-   0        0        0      111 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/__init__.py
+-rw-rw-rw-   0        0        0     8551 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/dataframe.py
+-rw-rw-rw-   0        0        0    27299 2023-04-12 17:23:29.000000 perlib-2.1.6/perlib/preprocessing/_utils/dataset_utils.py
+-rw-rw-rw-   0        0        0     9766 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/timeseries_dataset.py
+-rw-rw-rw-   0        0        0    12153 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/tools.py
+-rw-rw-rw-   0        0        0    13496 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/autopreprocess.py
+-rw-rw-rw-   0        0        0     4491 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/encode.py
+-rw-rw-rw-   0        0        0    13956 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/imputer.py
+-rw-rw-rw-   0        0        0     3446 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/outliers.py
+-rw-rw-rw-   0        0        0    19319 2023-04-13 12:15:50.000000 perlib-2.1.6/perlib/preprocessing/preparate.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.457435 perlib-2.1.6/perlib.egg-info/
+-rw-rw-rw-   0        0        0    10622 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1719 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 16:59:45.566769 perlib-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-04 21:29:01.000000 perlib-2.1.6/setup.py
```

### Comparing `perlib-2.1.5/LICENSE.md` & `perlib-2.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/PKG-INFO` & `perlib-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perlib
-Version: 2.1.5
+Version: 2.1.6
 Summary: Deep learning, Machine learning and Statistical learning for humans.
 Home-page: https://github.com/Ruzzg/perlib
 Author: Rüzgar Ersin Kanar
 Author-email: ruzgarknr@gmail.com
 License: Apache Software License
 Keywords: perlib,tensorflow,machine learning,deep learning
 Platform: UNKNOWN
```

### Comparing `perlib-2.1.5/README.md` & `perlib-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/__init__.py` & `perlib-2.1.6/perlib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Bu projenin tüm hakları Rüzgar Ersin Kanar'a aittir. Harici kimse ticari amaçlı kullanamaz.
-__version__ = "2.1.5"
+__version__ = "2.1.6"
 from .forecaster import *
 from .core._requests import req_info,aR_info,m_info
 from .core.models.dmodels import models as dmodels
 from .core.models.mmodels import models as mmodels
 from .core.models.smodels import models as smodels
 from .core.train import dTrain,sTrain,mTrain
 from .core.tester import dTester,sTester
```

### Comparing `perlib-2.1.5/perlib/analysis/exceptions.py` & `perlib-2.1.6/perlib/analysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/analysis/multivariate.py` & `perlib-2.1.6/perlib/analysis/multivariate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/analysis/plotting.py` & `perlib-2.1.6/perlib/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/analysis/univariate.py` & `perlib-2.1.6/perlib/analysis/univariate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/analysis/validate.py` & `perlib-2.1.6/perlib/analysis/validate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/_requests.py` & `perlib-2.1.6/perlib/core/_requests.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/metrics/classification.py` & `perlib-2.1.6/perlib/core/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/metrics/regression.py` & `perlib-2.1.6/perlib/core/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/models/dmodels.py` & `perlib-2.1.6/perlib/core/models/dmodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/models/lstnet.py` & `perlib-2.1.6/perlib/core/models/lstnet.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/models/mmodels.py` & `perlib-2.1.6/perlib/core/models/mmodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/models/smodels.py` & `perlib-2.1.6/perlib/core/models/smodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/optimizers/Optimizers.py` & `perlib-2.1.6/perlib/core/optimizers/Optimizers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/req_utils.py` & `perlib-2.1.6/perlib/core/req_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 "GaussianProcessRegressor",
 "OrthogonalMatchingPursuit",
 "ExtraTreeRegressor",
 "DummyRegressor",
 "LassoLars",
 "KernelRidge",
 "CatBoostRegressor",
-"MLPRegressor"]
+"MLPRegressor",
+"ELM"]
 
 cls = ["LinearSVC",
 "SGDClassifier",
 "MLPClassifier",
 "XGBClassifier",
 "Perceptron",
 "LogisticRegression",
```

### Comparing `perlib-2.1.5/perlib/core/tester.py` & `perlib-2.1.6/perlib/core/tester.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/core/train.py` & `perlib-2.1.6/perlib/core/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 import joblib
 from .models.smodels import *
 from ..preprocessing.preparate import dataPrepration
 import tensorflow as tf
 from datetime import datetime
 from .models.lstnet import LSTNetModel
+from .models.elm import ELM
 import json
 from .req_utils import *
 from itertools import product
 import numpy as np
 from statsmodels.tsa.statespace.sarimax import SARIMAX
 from statsmodels.tsa.arima.model import ARIMA
 from ..piplines.mpipline import Regressor,Classifier
@@ -112,16 +113,16 @@
             if self.dataFrame.shape[0] == 0:
                 raise ValueError('Data is empty.')
             return True
         else:
             raise TypeError("must be datafarame")
 
     def data_split_(self):
-        X = self.dataFrame.loc[:, self.dataFrame.columns != self.object.m_info.y]
-        y = self.dataFrame[[self.object.m_info.y]]
+        X = self.dataFrame.loc[:, self.dataFrame.columns != self.object.m_info.y].values
+        y = self.dataFrame[[self.object.m_info.y]].values
         return X,y
 
     def _scaler(self,X,y):
         self.scalerX = self.pr.get_scaler(self.object.m_info.scaler)
         self.scalery = self.pr.get_scaler(self.object.m_info.scaler)
         self.X = self.scalerX.fit_transform(X)
         if self.check_mod().__name__ == "Regressor":
@@ -156,15 +157,18 @@
             X_train, X_test, y_train, y_test  = self._test_size(X,y)
             m = eval(self.object.m_info.modelname)
             return m,scalerX,scalery,X_train,X_test, y_train, y_test
 
     def fit(self):
         m,scalerX,scalery,X_train,X_test, y_train, y_test = self.tr()
         if self.object.m_info.modelparams:
-            model = m(**self.object.m_info.modelparams)
+            try:
+                model = m(**self.object.m_info.modelparams)
+            except:
+                model = ELM(self.object.m_info.modelparams)
         else:
             model = m()
         model.fit(X_train, y_train)
         return model,scalery,scalerX,X_test, y_test
 
     def predict(self,metric= "mape"):
         """
@@ -173,15 +177,15 @@
         "matthews_corrcoef": "mc", "zero_one_loss": "zol", "f1_score": "fs", "hinge_loss": "hl",
         "hamming_loss": "hml", "classification_report": "cr", "precision_score": "ps", "recall_score": "rs",
         "balanced_accuracy_score": "bac", "precision_recall_fscore_support": "prfs", "fbeta_score": "fbs"}" or
         Regression metrics : {"max_error": "ma", "mean_absolute_error": "mae", "mean_squared_error": "mse",
         "mean_squared_log_error": "msle", "median_absolute_error": "meae", "mean_absolute_percentage_error": "mape"}
         :return:
         """
-        model_fit,scalery,scalerX,X_test,y_test = self.fit()
+        model_fit,scalery,scalerX,X_test, y_test= self.fit()
         if X_test is not None and y_test is not None:
             if self.check_mod().__name__ == "Regressor":
                 preds = scalery.inverse_transform(model_fit.predict(X_test).reshape(-1, 1))
                 y_test = scalery.inverse_transform(y_test)
             else:
                 preds = model_fit.predict(X_test)
             preds = to_df(preds, columns=["Predicts"])
@@ -293,14 +297,15 @@
         self.pr = dataPrepration()
         self.dataFrame = dataFrame
         self.object = object
         self.model = self.model()
 
     def model(self):
 
+        global model
         if type(self.dataFrame) is pd.DataFrame or isinstance(self.dataFrame, pd.DataFrame):
             if self.dataFrame.shape[0] == 0:
                 raise ValueError('Data is empty.')
         else:
             raise TypeError("must be datafarame")
         check_forecast_date(
             dataFrame=self.dataFrame,
@@ -327,17 +332,17 @@
                                         lookback=self.object.req_info.lookback,
                                         CNNFilters=self.object.req_info.layers["Layer"]["CNNFilters"],
                                         CNNKernel=self.object.req_info.layers["Layer"]["CNNKernel"],
                                         GRUUnits=self.object.req_info.layers["Layer"]["GRUUnits"],
                                         SkipGRUUnits=self.object.req_info.layers["Layer"]["SkipGRUUnits"],
                                         skip=self.object.req_info.layers["Layer"]["Skip"],
                                         highway=self.object.req_info.layers["Layer"]["Highway"])
-            else:
-                model = LSTNetModel(input_shape=X.shape,
-                                    lookback=self.object.req_info.lookback)
+                else:
+                    model = LSTNetModel(input_shape=X.shape,
+                                        lookback=self.object.req_info.lookback)
         else:
             self.object.set_inputShape((X.shape[-2:]))
             self.object.build_model()
             model = self.object.model_multi
         self.train_data_multi = train_data_multi
         self.val_data_multi   = val_data_multi
         try:
```

### Comparing `perlib-2.1.5/perlib/datasets/airpassengers.py` & `perlib-2.1.6/perlib/datasets/airpassengers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/ausbeer.py` & `perlib-2.1.6/perlib/datasets/ausbeer.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/austres.py` & `perlib-2.1.6/perlib/datasets/austres.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/heartrate.py` & `perlib-2.1.6/perlib/datasets/heartrate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/lynx.py` & `perlib-2.1.6/perlib/datasets/lynx.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/taylor.py` & `perlib-2.1.6/perlib/datasets/taylor.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/wineind.py` & `perlib-2.1.6/perlib/datasets/wineind.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/datasets/woolyrnq.py` & `perlib-2.1.6/perlib/datasets/woolyrnq.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/forecaster.py` & `perlib-2.1.6/perlib/forecaster.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/piplines/dpipline.py` & `perlib-2.1.6/perlib/piplines/dpipline.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/piplines/mpipline.py` & `perlib-2.1.6/perlib/piplines/mpipline.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/Normalizing.py` & `perlib-2.1.6/perlib/preprocessing/Normalizing.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/_split.py` & `perlib-2.1.6/perlib/preprocessing/_split.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'SlidingWindowForecastCV'
 ]
 
 
 def train_test_split(*arrays,
                      test_size=None,
                      train_size=None,
-                     random_state=123,
+                     random_state=None,
                      shuffle=False,
                      stratify=None
                      ):
     """Split arrays or matrices into sequential train and test subsets
     Creates train/test splits over endogenous arrays an optional exogenous
     arrays. This is a wrapper of scikit-learn's ``train_test_split`` that
     does not shuffle.
@@ -45,16 +45,16 @@
     splitting : list, length=2 * len(arrays)
         List containing train-test split of inputs.
     Examples
     --------
     """
     return tts(
         *arrays,
-        random_state=123,
-        shuffle=False,
+        random_state=None,
+        shuffle=True,
         stratify=None,
         test_size=test_size,
         train_size=train_size)
 
 
 class BaseTSCrossValidator(BaseEstimator, metaclass=abc.ABCMeta):
     """Base class for time series cross validators
```

### Comparing `perlib-2.1.5/perlib/preprocessing/_utils/dataframe.py` & `perlib-2.1.6/perlib/preprocessing/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/_utils/dataset_utils.py` & `perlib-2.1.6/perlib/preprocessing/_utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/_utils/timeseries_dataset.py` & `perlib-2.1.6/perlib/preprocessing/_utils/timeseries_dataset.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/_utils/tools.py` & `perlib-2.1.6/perlib/preprocessing/_utils/tools.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/autopreprocess.py` & `perlib-2.1.6/perlib/preprocessing/autopreprocess.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/encode.py` & `perlib-2.1.6/perlib/preprocessing/encode.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/imputer.py` & `perlib-2.1.6/perlib/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/outliers.py` & `perlib-2.1.6/perlib/preprocessing/outliers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib/preprocessing/preparate.py` & `perlib-2.1.6/perlib/preprocessing/preparate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.5/perlib.egg-info/PKG-INFO` & `perlib-2.1.6/perlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perlib
-Version: 2.1.5
+Version: 2.1.6
 Summary: Deep learning, Machine learning and Statistical learning for humans.
 Home-page: https://github.com/Ruzzg/perlib
 Author: Rüzgar Ersin Kanar
 Author-email: ruzgarknr@gmail.com
 License: Apache Software License
 Keywords: perlib,tensorflow,machine learning,deep learning
 Platform: UNKNOWN
```

### Comparing `perlib-2.1.5/perlib.egg-info/SOURCES.txt` & `perlib-2.1.6/perlib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 perlib/core/tester.py
 perlib/core/train.py
 perlib/core/metrics/__init__.py
 perlib/core/metrics/classification.py
 perlib/core/metrics/regression.py
 perlib/core/models/__init__.py
 perlib/core/models/dmodels.py
+perlib/core/models/elm.py
 perlib/core/models/lstnet.py
 perlib/core/models/mmodels.py
 perlib/core/models/smodels.py
 perlib/core/optimizers/Optimizers.py
 perlib/core/optimizers/__init__.py
 perlib/datasets/__init__.py
 perlib/datasets/airpassengers.py
```

### Comparing `perlib-2.1.5/setup.py` & `perlib-2.1.6/setup.py`

 * *Files identical despite different names*

