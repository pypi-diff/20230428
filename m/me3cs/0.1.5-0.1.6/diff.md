# Comparing `tmp/me3cs-0.1.5.tar.gz` & `tmp/me3cs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me3cs-0.1.5.tar", last modified: Wed Apr 26 12:31:12 2023, max compression
+gzip compressed data, was "me3cs-0.1.6.tar", last modified: Fri Apr 28 11:31:55 2023, max compression
```

## Comparing `me3cs-0.1.5.tar` & `me3cs-0.1.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.484894 me3cs-0.1.5/
--rw-------   0 mac        (501) staff       (20)     1665 2023-03-08 16:03:54.000000 me3cs-0.1.5/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)      237 2023-04-26 12:31:12.484541 me3cs-0.1.5/PKG-INFO
--rw-------   0 mac        (501) staff       (20)     5017 2023-03-24 15:14:56.000000 me3cs-0.1.5/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.431039 me3cs-0.1.5/me3cs/
--rw-------   0 mac        (501) staff       (20)       35 2023-04-25 14:12:58.000000 me3cs-0.1.5/me3cs/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.443414 me3cs-0.1.5/me3cs/cross_validation/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-07 13:23:52.000000 me3cs-0.1.5/me3cs/cross_validation/__init__.py
--rw-------   0 mac        (501) staff       (20)     3883 2023-03-06 14:16:47.000000 me3cs-0.1.5/me3cs/cross_validation/cross_validation.py
--rw-------   0 mac        (501) staff       (20)     1131 2023-03-06 14:16:47.000000 me3cs-0.1.5/me3cs/cross_validation/cross_validation_model.py
--rw-------   0 mac        (501) staff       (20)      658 2023-03-01 09:15:56.000000 me3cs-0.1.5/me3cs/cross_validation/cross_validation_predictor.py
--rw-------   0 mac        (501) staff       (20)     3904 2023-04-25 10:55:20.000000 me3cs-0.1.5/me3cs/cross_validation/cross_validation_preprocessing.py
--rw-------   0 mac        (501) staff       (20)     1492 2023-03-06 14:16:47.000000 me3cs-0.1.5/me3cs/cross_validation/cross_validation_split.py
--rw-------   0 mac        (501) staff       (20)     1541 2023-03-06 14:16:47.000000 me3cs-0.1.5/me3cs/cross_validation/cross_validation_types.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.456014 me3cs-0.1.5/me3cs/framework/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-07 13:23:52.000000 me3cs-0.1.5/me3cs/framework/__init__.py
--rw-------   0 mac        (501) staff       (20)     1787 2023-04-25 20:56:47.000000 me3cs-0.1.5/me3cs/framework/base_model.py
--rw-r--r--   0 mac        (501) staff       (20)     1101 2023-04-25 14:21:34.000000 me3cs-0.1.5/me3cs/framework/branch.py
--rw-r--r--   0 mac        (501) staff       (20)     6619 2023-04-25 16:41:34.000000 me3cs-0.1.5/me3cs/framework/data.py
--rw-------   0 mac        (501) staff       (20)     1560 2023-03-06 16:41:15.000000 me3cs-0.1.5/me3cs/framework/decomposition_model.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.459082 me3cs-0.1.5/me3cs/framework/helper_classes/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-15 13:47:36.000000 me3cs-0.1.5/me3cs/framework/helper_classes/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1054 2023-04-25 11:32:24.000000 me3cs-0.1.5/me3cs/framework/helper_classes/handle_input.py
--rw-r--r--   0 mac        (501) staff       (20)      830 2023-04-25 20:52:31.000000 me3cs-0.1.5/me3cs/framework/helper_classes/link.py
--rw-------   0 mac        (501) staff       (20)     1884 2023-04-12 14:35:10.000000 me3cs-0.1.5/me3cs/framework/helper_classes/options.py
--rw-r--r--   0 mac        (501) staff       (20)     7587 2023-04-25 15:22:20.000000 me3cs-0.1.5/me3cs/framework/log.py
--rw-------   0 mac        (501) staff       (20)      209 2023-03-07 12:24:36.000000 me3cs-0.1.5/me3cs/framework/model.py
--rw-r--r--   0 mac        (501) staff       (20)     5519 2023-04-25 21:29:56.000000 me3cs-0.1.5/me3cs/framework/outlier_detection.py
--rw-------   0 mac        (501) staff       (20)     3906 2023-04-25 15:25:02.000000 me3cs-0.1.5/me3cs/framework/regression_model.py
--rw-------   0 mac        (501) staff       (20)      825 2023-04-25 12:10:56.000000 me3cs-0.1.5/me3cs/framework/results.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.460047 me3cs-0.1.5/me3cs/metrics/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-08 14:14:27.000000 me3cs-0.1.5/me3cs/metrics/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.462793 me3cs-0.1.5/me3cs/metrics/regression/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-08 14:15:17.000000 me3cs-0.1.5/me3cs/metrics/regression/__init__.py
--rw-------   0 mac        (501) staff       (20)      732 2023-04-14 15:26:07.000000 me3cs-0.1.5/me3cs/metrics/regression/diagnostics.py
--rw-------   0 mac        (501) staff       (20)      451 2023-04-14 15:28:19.000000 me3cs-0.1.5/me3cs/metrics/regression/metrics.py
--rw-------   0 mac        (501) staff       (20)     2225 2023-04-14 15:20:26.000000 me3cs-0.1.5/me3cs/metrics/regression/results.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.466290 me3cs-0.1.5/me3cs/misc/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-08 11:17:11.000000 me3cs-0.1.5/me3cs/misc/__init__.py
--rw-------   0 mac        (501) staff       (20)     1930 2023-03-07 11:32:53.000000 me3cs-0.1.5/me3cs/misc/handle_data.py
--rw-r--r--   0 mac        (501) staff       (20)     9552 2023-04-21 09:04:27.000000 me3cs-0.1.5/me3cs/misc/metrics.py
--rw-------   0 mac        (501) staff       (20)     2674 2023-03-07 12:46:26.000000 me3cs-0.1.5/me3cs/misc/preprocessing.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.469581 me3cs-0.1.5/me3cs/missing_data/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-15 14:02:29.000000 me3cs-0.1.5/me3cs/missing_data/__init__.py
--rw-------   0 mac        (501) staff       (20)        0 2022-11-15 14:05:27.000000 me3cs-0.1.5/me3cs/missing_data/bootstrapping.py
--rw-------   0 mac        (501) staff       (20)     2042 2023-03-06 11:57:03.000000 me3cs-0.1.5/me3cs/missing_data/imputation.py
--rw-------   0 mac        (501) staff       (20)      309 2023-02-23 10:43:40.000000 me3cs-0.1.5/me3cs/missing_data/interpolation.py
--rw-------   0 mac        (501) staff       (20)     6861 2023-04-25 14:25:50.000000 me3cs-0.1.5/me3cs/missing_data/missing_data.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.470486 me3cs-0.1.5/me3cs/models/
--rw-------   0 mac        (501) staff       (20)        0 2022-11-07 13:23:25.000000 me3cs-0.1.5/me3cs/models/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.472966 me3cs-0.1.5/me3cs/models/decomposition/
--rw-------   0 mac        (501) staff       (20)        0 2022-10-05 13:52:15.000000 me3cs-0.1.5/me3cs/models/decomposition/__init__.py
--rw-------   0 mac        (501) staff       (20)      636 2023-03-06 16:41:15.000000 me3cs-0.1.5/me3cs/models/decomposition/decomposition_diagnostics.py
--rw-------   0 mac        (501) staff       (20)      676 2023-03-06 16:41:15.000000 me3cs-0.1.5/me3cs/models/decomposition/decomposition_results.py
--rw-------   0 mac        (501) staff       (20)     3223 2023-03-06 11:57:03.000000 me3cs-0.1.5/me3cs/models/decomposition/pca.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.476945 me3cs-0.1.5/me3cs/models/regression/
--rw-------   0 mac        (501) staff       (20)        0 2022-10-05 10:10:26.000000 me3cs-0.1.5/me3cs/models/regression/__init__.py
--rw-------   0 mac        (501) staff       (20)       57 2022-11-15 15:12:29.000000 me3cs-0.1.5/me3cs/models/regression/cls.py
--rw-------   0 mac        (501) staff       (20)      404 2023-03-06 11:57:04.000000 me3cs-0.1.5/me3cs/models/regression/mlr.py
--rw-------   0 mac        (501) staff       (20)      778 2023-03-06 16:41:15.000000 me3cs-0.1.5/me3cs/models/regression/pcr.py
--rw-------   0 mac        (501) staff       (20)     8636 2023-03-07 14:11:40.000000 me3cs-0.1.5/me3cs/models/regression/pls.py
--rw-------   0 mac        (501) staff       (20)       54 2022-11-15 15:12:30.000000 me3cs-0.1.5/me3cs/models/regression/svm.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.483673 me3cs-0.1.5/me3cs/preprocessing/
--rw-------   0 mac        (501) staff       (20)       28 2022-11-08 20:04:04.000000 me3cs-0.1.5/me3cs/preprocessing/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4417 2023-04-25 15:59:41.000000 me3cs-0.1.5/me3cs/preprocessing/base.py
--rw-------   0 mac        (501) staff       (20)     1891 2023-04-14 18:44:05.000000 me3cs-0.1.5/me3cs/preprocessing/called.py
--rw-------   0 mac        (501) staff       (20)     3885 2023-03-07 16:29:10.000000 me3cs-0.1.5/me3cs/preprocessing/filtering.py
--rw-------   0 mac        (501) staff       (20)     1760 2023-04-25 11:04:15.000000 me3cs-0.1.5/me3cs/preprocessing/normalisation.py
--rw-------   0 mac        (501) staff       (20)      934 2023-04-25 11:58:31.000000 me3cs-0.1.5/me3cs/preprocessing/preprocessing.py
--rw-------   0 mac        (501) staff       (20)     4058 2023-04-25 11:46:34.000000 me3cs-0.1.5/me3cs/preprocessing/scaling.py
--rw-------   0 mac        (501) staff       (20)     3198 2023-03-07 13:29:33.000000 me3cs-0.1.5/me3cs/preprocessing/standardisation.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-26 12:31:12.435411 me3cs-0.1.5/me3cs.egg-info/
--rw-------   0 mac        (501) staff       (20)      237 2023-04-26 12:31:12.000000 me3cs-0.1.5/me3cs.egg-info/PKG-INFO
--rw-------   0 mac        (501) staff       (20)     2102 2023-04-26 12:31:12.000000 me3cs-0.1.5/me3cs.egg-info/SOURCES.txt
--rw-------   0 mac        (501) staff       (20)        1 2023-04-26 12:31:12.000000 me3cs-0.1.5/me3cs.egg-info/dependency_links.txt
--rw-------   0 mac        (501) staff       (20)       19 2023-04-26 12:31:12.000000 me3cs-0.1.5/me3cs.egg-info/requires.txt
--rw-------   0 mac        (501) staff       (20)        6 2023-04-26 12:31:12.000000 me3cs-0.1.5/me3cs.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-26 12:31:12.485019 me3cs-0.1.5/setup.cfg
--rw-------   0 mac        (501) staff       (20)      407 2023-04-26 12:31:10.000000 me3cs-0.1.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.534608 me3cs-0.1.6/
+-rw-------   0 mac        (501) staff       (20)     1665 2023-03-08 16:03:54.000000 me3cs-0.1.6/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)      237 2023-04-28 11:31:55.533797 me3cs-0.1.6/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)     5017 2023-03-24 15:14:56.000000 me3cs-0.1.6/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.478936 me3cs-0.1.6/me3cs/
+-rw-------   0 mac        (501) staff       (20)       35 2023-04-25 14:12:58.000000 me3cs-0.1.6/me3cs/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.488734 me3cs-0.1.6/me3cs/cross_validation/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-07 13:23:52.000000 me3cs-0.1.6/me3cs/cross_validation/__init__.py
+-rw-------   0 mac        (501) staff       (20)     3883 2023-03-06 14:16:47.000000 me3cs-0.1.6/me3cs/cross_validation/cross_validation.py
+-rw-------   0 mac        (501) staff       (20)     1131 2023-03-06 14:16:47.000000 me3cs-0.1.6/me3cs/cross_validation/cross_validation_model.py
+-rw-------   0 mac        (501) staff       (20)      658 2023-03-01 09:15:56.000000 me3cs-0.1.6/me3cs/cross_validation/cross_validation_predictor.py
+-rw-------   0 mac        (501) staff       (20)     3904 2023-04-25 10:55:20.000000 me3cs-0.1.6/me3cs/cross_validation/cross_validation_preprocessing.py
+-rw-------   0 mac        (501) staff       (20)     1492 2023-03-06 14:16:47.000000 me3cs-0.1.6/me3cs/cross_validation/cross_validation_split.py
+-rw-------   0 mac        (501) staff       (20)     1541 2023-03-06 14:16:47.000000 me3cs-0.1.6/me3cs/cross_validation/cross_validation_types.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.499229 me3cs-0.1.6/me3cs/framework/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-07 13:23:52.000000 me3cs-0.1.6/me3cs/framework/__init__.py
+-rw-------   0 mac        (501) staff       (20)     1787 2023-04-25 20:56:47.000000 me3cs-0.1.6/me3cs/framework/base_model.py
+-rw-r--r--   0 mac        (501) staff       (20)     1101 2023-04-25 14:21:34.000000 me3cs-0.1.6/me3cs/framework/branch.py
+-rw-r--r--   0 mac        (501) staff       (20)     6619 2023-04-25 16:41:34.000000 me3cs-0.1.6/me3cs/framework/data.py
+-rw-------   0 mac        (501) staff       (20)     1560 2023-03-06 16:41:15.000000 me3cs-0.1.6/me3cs/framework/decomposition_model.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.503221 me3cs-0.1.6/me3cs/framework/helper_classes/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-15 13:47:36.000000 me3cs-0.1.6/me3cs/framework/helper_classes/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1054 2023-04-25 11:32:24.000000 me3cs-0.1.6/me3cs/framework/helper_classes/handle_input.py
+-rw-r--r--   0 mac        (501) staff       (20)      830 2023-04-25 20:52:31.000000 me3cs-0.1.6/me3cs/framework/helper_classes/link.py
+-rw-------   0 mac        (501) staff       (20)     1884 2023-04-12 14:35:10.000000 me3cs-0.1.6/me3cs/framework/helper_classes/options.py
+-rw-r--r--   0 mac        (501) staff       (20)     7587 2023-04-25 15:22:20.000000 me3cs-0.1.6/me3cs/framework/log.py
+-rw-------   0 mac        (501) staff       (20)      209 2023-03-07 12:24:36.000000 me3cs-0.1.6/me3cs/framework/model.py
+-rw-r--r--   0 mac        (501) staff       (20)     5519 2023-04-25 21:29:56.000000 me3cs-0.1.6/me3cs/framework/outlier_detection.py
+-rw-------   0 mac        (501) staff       (20)     3906 2023-04-25 15:25:02.000000 me3cs-0.1.6/me3cs/framework/regression_model.py
+-rw-------   0 mac        (501) staff       (20)      825 2023-04-25 12:10:56.000000 me3cs-0.1.6/me3cs/framework/results.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.504934 me3cs-0.1.6/me3cs/metrics/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-08 14:14:27.000000 me3cs-0.1.6/me3cs/metrics/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.508119 me3cs-0.1.6/me3cs/metrics/regression/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-08 14:15:17.000000 me3cs-0.1.6/me3cs/metrics/regression/__init__.py
+-rw-------   0 mac        (501) staff       (20)      732 2023-04-14 15:26:07.000000 me3cs-0.1.6/me3cs/metrics/regression/diagnostics.py
+-rw-------   0 mac        (501) staff       (20)      451 2023-04-14 15:28:19.000000 me3cs-0.1.6/me3cs/metrics/regression/metrics.py
+-rw-------   0 mac        (501) staff       (20)     2225 2023-04-14 15:20:26.000000 me3cs-0.1.6/me3cs/metrics/regression/results.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.511643 me3cs-0.1.6/me3cs/misc/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-08 11:17:11.000000 me3cs-0.1.6/me3cs/misc/__init__.py
+-rw-------   0 mac        (501) staff       (20)     1930 2023-03-07 11:32:53.000000 me3cs-0.1.6/me3cs/misc/handle_data.py
+-rw-r--r--   0 mac        (501) staff       (20)     9552 2023-04-21 09:04:27.000000 me3cs-0.1.6/me3cs/misc/metrics.py
+-rw-------   0 mac        (501) staff       (20)     2674 2023-03-07 12:46:26.000000 me3cs-0.1.6/me3cs/misc/preprocessing.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.517349 me3cs-0.1.6/me3cs/missing_data/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-15 14:02:29.000000 me3cs-0.1.6/me3cs/missing_data/__init__.py
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-15 14:05:27.000000 me3cs-0.1.6/me3cs/missing_data/bootstrapping.py
+-rw-------   0 mac        (501) staff       (20)     2042 2023-03-06 11:57:03.000000 me3cs-0.1.6/me3cs/missing_data/imputation.py
+-rw-------   0 mac        (501) staff       (20)      309 2023-02-23 10:43:40.000000 me3cs-0.1.6/me3cs/missing_data/interpolation.py
+-rw-------   0 mac        (501) staff       (20)     6861 2023-04-25 14:25:50.000000 me3cs-0.1.6/me3cs/missing_data/missing_data.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.518630 me3cs-0.1.6/me3cs/models/
+-rw-------   0 mac        (501) staff       (20)        0 2022-11-07 13:23:25.000000 me3cs-0.1.6/me3cs/models/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.521975 me3cs-0.1.6/me3cs/models/decomposition/
+-rw-------   0 mac        (501) staff       (20)        0 2022-10-05 13:52:15.000000 me3cs-0.1.6/me3cs/models/decomposition/__init__.py
+-rw-------   0 mac        (501) staff       (20)      636 2023-03-06 16:41:15.000000 me3cs-0.1.6/me3cs/models/decomposition/decomposition_diagnostics.py
+-rw-------   0 mac        (501) staff       (20)      676 2023-03-06 16:41:15.000000 me3cs-0.1.6/me3cs/models/decomposition/decomposition_results.py
+-rw-------   0 mac        (501) staff       (20)     3223 2023-03-06 11:57:03.000000 me3cs-0.1.6/me3cs/models/decomposition/pca.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.526588 me3cs-0.1.6/me3cs/models/regression/
+-rw-------   0 mac        (501) staff       (20)        0 2022-10-05 10:10:26.000000 me3cs-0.1.6/me3cs/models/regression/__init__.py
+-rw-------   0 mac        (501) staff       (20)       57 2022-11-15 15:12:29.000000 me3cs-0.1.6/me3cs/models/regression/cls.py
+-rw-------   0 mac        (501) staff       (20)      404 2023-03-06 11:57:04.000000 me3cs-0.1.6/me3cs/models/regression/mlr.py
+-rw-------   0 mac        (501) staff       (20)      778 2023-03-06 16:41:15.000000 me3cs-0.1.6/me3cs/models/regression/pcr.py
+-rw-------   0 mac        (501) staff       (20)     8636 2023-03-07 14:11:40.000000 me3cs-0.1.6/me3cs/models/regression/pls.py
+-rw-------   0 mac        (501) staff       (20)       54 2022-11-15 15:12:30.000000 me3cs-0.1.6/me3cs/models/regression/svm.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.532831 me3cs-0.1.6/me3cs/preprocessing/
+-rw-------   0 mac        (501) staff       (20)       28 2022-11-08 20:04:04.000000 me3cs-0.1.6/me3cs/preprocessing/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4417 2023-04-25 15:59:41.000000 me3cs-0.1.6/me3cs/preprocessing/base.py
+-rw-------   0 mac        (501) staff       (20)     1891 2023-04-14 18:44:05.000000 me3cs-0.1.6/me3cs/preprocessing/called.py
+-rw-------   0 mac        (501) staff       (20)     3885 2023-03-07 16:29:10.000000 me3cs-0.1.6/me3cs/preprocessing/filtering.py
+-rw-------   0 mac        (501) staff       (20)     1760 2023-04-25 11:04:15.000000 me3cs-0.1.6/me3cs/preprocessing/normalisation.py
+-rw-------   0 mac        (501) staff       (20)      934 2023-04-25 11:58:31.000000 me3cs-0.1.6/me3cs/preprocessing/preprocessing.py
+-rw-------   0 mac        (501) staff       (20)     4058 2023-04-25 11:46:34.000000 me3cs-0.1.6/me3cs/preprocessing/scaling.py
+-rw-------   0 mac        (501) staff       (20)     3198 2023-03-07 13:29:33.000000 me3cs-0.1.6/me3cs/preprocessing/standardisation.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-28 11:31:55.481637 me3cs-0.1.6/me3cs.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      237 2023-04-28 11:31:55.000000 me3cs-0.1.6/me3cs.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2102 2023-04-28 11:31:55.000000 me3cs-0.1.6/me3cs.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-28 11:31:55.000000 me3cs-0.1.6/me3cs.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-04-28 11:31:55.000000 me3cs-0.1.6/me3cs.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-04-28 11:31:55.000000 me3cs-0.1.6/me3cs.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-28 11:31:55.534826 me3cs-0.1.6/setup.cfg
+-rw-------   0 mac        (501) staff       (20)      407 2023-04-28 11:31:43.000000 me3cs-0.1.6/setup.py
```

### Comparing `me3cs-0.1.5/LICENSE.txt` & `me3cs-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/README.md` & `me3cs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/cross_validation/cross_validation.py` & `me3cs-0.1.6/me3cs/cross_validation/cross_validation.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/cross_validation/cross_validation_model.py` & `me3cs-0.1.6/me3cs/cross_validation/cross_validation_model.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/cross_validation/cross_validation_predictor.py` & `me3cs-0.1.6/me3cs/cross_validation/cross_validation_predictor.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/cross_validation/cross_validation_preprocessing.py` & `me3cs-0.1.6/me3cs/cross_validation/cross_validation_preprocessing.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/cross_validation/cross_validation_split.py` & `me3cs-0.1.6/me3cs/cross_validation/cross_validation_split.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/cross_validation/cross_validation_types.py` & `me3cs-0.1.6/me3cs/cross_validation/cross_validation_types.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/base_model.py` & `me3cs-0.1.6/me3cs/framework/base_model.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/branch.py` & `me3cs-0.1.6/me3cs/framework/branch.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/data.py` & `me3cs-0.1.6/me3cs/framework/data.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/decomposition_model.py` & `me3cs-0.1.6/me3cs/framework/decomposition_model.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/helper_classes/handle_input.py` & `me3cs-0.1.6/me3cs/framework/helper_classes/handle_input.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/helper_classes/link.py` & `me3cs-0.1.6/me3cs/framework/helper_classes/link.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/helper_classes/options.py` & `me3cs-0.1.6/me3cs/framework/helper_classes/options.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/log.py` & `me3cs-0.1.6/me3cs/framework/log.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/outlier_detection.py` & `me3cs-0.1.6/me3cs/framework/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/regression_model.py` & `me3cs-0.1.6/me3cs/framework/regression_model.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/framework/results.py` & `me3cs-0.1.6/me3cs/framework/results.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/metrics/regression/diagnostics.py` & `me3cs-0.1.6/me3cs/metrics/regression/diagnostics.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/metrics/regression/results.py` & `me3cs-0.1.6/me3cs/metrics/regression/results.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/misc/handle_data.py` & `me3cs-0.1.6/me3cs/misc/handle_data.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/misc/metrics.py` & `me3cs-0.1.6/me3cs/misc/metrics.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/misc/preprocessing.py` & `me3cs-0.1.6/me3cs/misc/preprocessing.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/missing_data/imputation.py` & `me3cs-0.1.6/me3cs/missing_data/imputation.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/missing_data/missing_data.py` & `me3cs-0.1.6/me3cs/missing_data/missing_data.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/models/decomposition/decomposition_diagnostics.py` & `me3cs-0.1.6/me3cs/models/decomposition/decomposition_diagnostics.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/models/decomposition/decomposition_results.py` & `me3cs-0.1.6/me3cs/models/decomposition/decomposition_results.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/models/decomposition/pca.py` & `me3cs-0.1.6/me3cs/models/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/models/regression/pcr.py` & `me3cs-0.1.6/me3cs/models/regression/pcr.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/models/regression/pls.py` & `me3cs-0.1.6/me3cs/models/regression/pls.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/base.py` & `me3cs-0.1.6/me3cs/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/called.py` & `me3cs-0.1.6/me3cs/preprocessing/called.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/filtering.py` & `me3cs-0.1.6/me3cs/preprocessing/filtering.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/normalisation.py` & `me3cs-0.1.6/me3cs/preprocessing/normalisation.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/preprocessing.py` & `me3cs-0.1.6/me3cs/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/scaling.py` & `me3cs-0.1.6/me3cs/preprocessing/scaling.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs/preprocessing/standardisation.py` & `me3cs-0.1.6/me3cs/preprocessing/standardisation.py`

 * *Files identical despite different names*

### Comparing `me3cs-0.1.5/me3cs.egg-info/SOURCES.txt` & `me3cs-0.1.6/me3cs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

