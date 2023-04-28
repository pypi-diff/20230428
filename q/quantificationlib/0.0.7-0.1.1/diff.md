# Comparing `tmp/quantificationlib-0.0.7.tar.gz` & `tmp/quantificationlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantificationlib-0.0.7.tar", last modified: Thu Apr 13 14:19:29 2023, max compression
+gzip compressed data, was "quantificationlib-0.1.1.tar", last modified: Fri Apr 28 12:13:39 2023, max compression
```

## Comparing `quantificationlib-0.0.7.tar` & `quantificationlib-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-03-31 08:18:56.000000 quantificationlib-0.0.7/LICENCE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2108 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      955 2023-04-13 14:17:52.000000 quantificationlib-0.0.7/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.897383 quantificationlib-0.0.7/quantificationlib/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      821 2023-04-13 14:18:10.000000 quantificationlib-0.0.7/quantificationlib/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    21959 2023-03-31 11:16:32.000000 quantificationlib-0.0.7/quantificationlib/bag_generator.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    14309 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/base.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.897383 quantificationlib-0.0.7/quantificationlib/baselines/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/baselines/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    23752 2023-04-13 13:54:42.000000 quantificationlib-0.0.7/quantificationlib/baselines/ac.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9902 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/baselines/cc.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/binary/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/binary/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7489 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/binary/debias.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    10493 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/binary/emd.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11269 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/binary/quantiles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       86 2023-03-29 12:43:43.000000 quantificationlib-0.0.7/quantificationlib/cvxpy_installed_solvers.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      626 2023-03-31 08:24:16.000000 quantificationlib-0.0.7/quantificationlib/data_utils.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/decomposition/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/decomposition/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9147 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/decomposition/multiclass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    15664 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/decomposition/ordinal.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/ensembles/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/ensembles/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    28508 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/ensembles/eoq.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.901383 quantificationlib-0.0.7/quantificationlib/estimators/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/estimators/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    12799 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/estimators/cross_validation.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6707 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/estimators/ensembles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    42851 2023-03-31 11:31:31.000000 quantificationlib-0.0.7/quantificationlib/estimators/frank_and_hall.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    16148 2023-03-31 11:31:29.000000 quantificationlib-0.0.7/quantificationlib/estimators/ordinal_ddag.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6239 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/estimators/weighted_knn.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.905383 quantificationlib-0.0.7/quantificationlib/metrics/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/metrics/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5832 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/metrics/binary.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    11844 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/metrics/multiclass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2684 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/metrics/ordinal.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.905383 quantificationlib-0.0.7/quantificationlib/multiclass/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/multiclass/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    34737 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/df.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9077 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/multiclass/em.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    25478 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/energy.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    12964 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/friedman.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7483 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/multiclass/knn.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    29130 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/multiclass/regression.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    19390 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/optimization.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/quantificationlib/ordinal/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.0.7/quantificationlib/ordinal/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     9803 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/ordinal/ac_ordinal.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    13836 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/ordinal/pdf.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1972 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/ordinal/trees.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/quantificationlib/plot/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-13 13:54:42.000000 quantificationlib-0.0.7/quantificationlib/plot/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2832 2023-04-13 13:54:42.000000 quantificationlib-0.0.7/quantificationlib/plot/qlplot.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    15685 2023-03-31 11:16:33.000000 quantificationlib-0.0.7/quantificationlib/search.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.897383 quantificationlib-0.0.7/quantificationlib.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2108 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2029 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       75 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       18 2023-04-13 14:19:29.000000 quantificationlib-0.0.7/quantificationlib.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6550 2023-04-13 14:18:04.000000 quantificationlib-0.0.7/setup.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-13 14:19:29.909383 quantificationlib-0.0.7/tests/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3038 2023-03-31 12:04:50.000000 quantificationlib-0.0.7/tests/test_bag_generators.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7575 2023-04-10 13:16:55.000000 quantificationlib-0.0.7/tests/test_binary_quantifiers.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3041 2023-03-31 11:37:23.000000 quantificationlib-0.0.7/tests/test_cv_estimator.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5084 2023-04-10 13:38:50.000000 quantificationlib-0.0.7/tests/test_decomposition.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3372 2023-04-10 13:34:32.000000 quantificationlib-0.0.7/tests/test_ensembles.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1953 2023-03-31 10:26:42.000000 quantificationlib-0.0.7/tests/test_metrics.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5896 2023-03-31 11:04:10.000000 quantificationlib-0.0.7/tests/test_ordinal_quantifiers.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.173838 quantificationlib-0.1.1/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-03-31 08:18:56.000000 quantificationlib-0.1.1/LICENCE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2015 2023-04-28 12:13:39.173838 quantificationlib-0.1.1/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      862 2023-04-28 11:59:23.000000 quantificationlib-0.1.1/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.161838 quantificationlib-0.1.1/quantificationlib/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      821 2023-04-28 12:12:00.000000 quantificationlib-0.1.1/quantificationlib/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    21992 2023-04-25 08:53:24.000000 quantificationlib-0.1.1/quantificationlib/bag_generator.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    14313 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/base.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.165838 quantificationlib-0.1.1/quantificationlib/baselines/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/baselines/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    23732 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/baselines/ac.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9901 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/baselines/cc.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.165838 quantificationlib-0.1.1/quantificationlib/binary/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/binary/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7494 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/binary/debias.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    10505 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/binary/emd.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11274 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/binary/quantiles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       86 2023-03-29 12:43:43.000000 quantificationlib-0.1.1/quantificationlib/cvxpy_installed_solvers.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      626 2023-03-31 08:24:16.000000 quantificationlib-0.1.1/quantificationlib/data_utils.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.165838 quantificationlib-0.1.1/quantificationlib/decomposition/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/decomposition/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9140 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/decomposition/multiclass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    15704 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/decomposition/ordinal.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.165838 quantificationlib-0.1.1/quantificationlib/ensembles/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/ensembles/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    28592 2023-04-25 08:53:24.000000 quantificationlib-0.1.1/quantificationlib/ensembles/eoq.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.165838 quantificationlib-0.1.1/quantificationlib/estimators/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/estimators/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    12623 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/estimators/cross_validation.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6648 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/estimators/ensembles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    42793 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/estimators/frank_and_hall.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    16422 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/estimators/ordinal_ddag.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6225 2023-04-25 08:53:24.000000 quantificationlib-0.1.1/quantificationlib/estimators/weighted_knn.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.165838 quantificationlib-0.1.1/quantificationlib/metrics/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/metrics/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5833 2023-04-25 08:53:24.000000 quantificationlib-0.1.1/quantificationlib/metrics/binary.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    11875 2023-04-25 08:53:24.000000 quantificationlib-0.1.1/quantificationlib/metrics/multiclass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3274 2023-04-25 08:53:24.000000 quantificationlib-0.1.1/quantificationlib/metrics/ordinal.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.169838 quantificationlib-0.1.1/quantificationlib/multiclass/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/multiclass/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35101 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/multiclass/df.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9082 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/multiclass/em.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    25500 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/multiclass/energy.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    12972 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/multiclass/friedman.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7483 2023-03-31 11:16:33.000000 quantificationlib-0.1.1/quantificationlib/multiclass/knn.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    29506 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/multiclass/regression.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    19900 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/optimization.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.169838 quantificationlib-0.1.1/quantificationlib/ordinal/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-02-02 09:15:27.000000 quantificationlib-0.1.1/quantificationlib/ordinal/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     9773 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/ordinal/ac_ordinal.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    13832 2023-04-28 11:49:09.000000 quantificationlib-0.1.1/quantificationlib/ordinal/pdf.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1972 2023-03-31 11:16:33.000000 quantificationlib-0.1.1/quantificationlib/ordinal/trees.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.169838 quantificationlib-0.1.1/quantificationlib/plot/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-13 13:54:42.000000 quantificationlib-0.1.1/quantificationlib/plot/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4271 2023-04-28 12:00:21.000000 quantificationlib-0.1.1/quantificationlib/plot/qlplot.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    15685 2023-03-31 11:16:33.000000 quantificationlib-0.1.1/quantificationlib/search.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.161838 quantificationlib-0.1.1/quantificationlib.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2015 2023-04-28 12:13:39.000000 quantificationlib-0.1.1/quantificationlib.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2085 2023-04-28 12:13:39.000000 quantificationlib-0.1.1/quantificationlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-04-28 12:13:39.000000 quantificationlib-0.1.1/quantificationlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       75 2023-04-28 12:13:39.000000 quantificationlib-0.1.1/quantificationlib.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       18 2023-04-28 12:13:39.000000 quantificationlib-0.1.1/quantificationlib.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2023-04-28 12:13:39.173838 quantificationlib-0.1.1/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6550 2023-04-28 12:12:52.000000 quantificationlib-0.1.1/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 12:13:39.173838 quantificationlib-0.1.1/tests/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3038 2023-03-31 12:04:50.000000 quantificationlib-0.1.1/tests/test_bag_generators.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     8611 2023-04-25 08:23:13.000000 quantificationlib-0.1.1/tests/test_binary_quantifiers.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3041 2023-03-31 11:37:23.000000 quantificationlib-0.1.1/tests/test_cv_estimator.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5720 2023-04-25 08:52:02.000000 quantificationlib-0.1.1/tests/test_decomposition.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3411 2023-04-25 08:43:26.000000 quantificationlib-0.1.1/tests/test_ensembles.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1953 2023-03-31 10:26:42.000000 quantificationlib-0.1.1/tests/test_metrics.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7689 2023-04-25 09:33:40.000000 quantificationlib-0.1.1/tests/test_multiclass_quantifiers.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6006 2023-04-25 09:06:19.000000 quantificationlib-0.1.1/tests/test_ordinal_quantifiers.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1165 2023-04-28 11:55:49.000000 quantificationlib-0.1.1/tests/test_plot.py
```

### Comparing `quantificationlib-0.0.7/LICENCE` & `quantificationlib-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/PKG-INFO` & `quantificationlib-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quantificationlib
-Version: 0.0.7
+Version: 0.1.1
 Summary: quantificationlib: A library for Quantification Learning
 Home-page: https://github.com/AICGijon/quantificationlib
-Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.8.tar.gz
 Author: Alberto Castaño, Pablo González, Jaime Alonso, Pablo Pérez, Juan José del Coz
 Author-email: bertocast@gmail.com, gonzalezgpablo@uniovi.es, jalonso@uniovi.es, pabloperez@uniovi.es, juanjo@uniovi.es
 Keywords: quantification,label shift,prevalence estimation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -27,14 +27,10 @@
 [![Downloads PyPI](https://static.pepy.tech/personalized-badge/quantificationlib?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=pypi)](https://pypi.org/project/quantificationlib/)
 
 
 # QuantificationLib
 
 QuantificationLib is an open-source library for quantification learning. 
 
-### Last updates:
-- Adding plots [0.0.7]
-- Initial version of the library released [0.0.6].
-
 ### Installation and documentation
 
 The installation, quick-start guide and documentation are available [here](https://aicgijon.github.io/quantificationlib/).
```

### Comparing `quantificationlib-0.0.7/README.md` & `quantificationlib-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,10 @@
 [![Downloads PyPI](https://static.pepy.tech/personalized-badge/quantificationlib?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=pypi)](https://pypi.org/project/quantificationlib/)
 
 
 # QuantificationLib
 
 QuantificationLib is an open-source library for quantification learning. 
 
-### Last updates:
-- Adding plots [0.0.7]
-- Initial version of the library released [0.0.6].
-
 ### Installation and documentation
 
 The installation, quick-start guide and documentation are available [here](https://aicgijon.github.io/quantificationlib/).
```

### Comparing `quantificationlib-0.0.7/quantificationlib/__init__.py` & `quantificationlib-0.1.1/quantificationlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # from quantificationlib import ensembles
 # from quantificationlib import estimators
 # from quantificationlib import examples
 # from quantificationlib import metrics
 # from quantificationlib import multiclass
 # from quantificationlib import ordinal
 #
-__version__ = '0.0.7'
+__version__ = '0.1.1'
 
 # __all__ = [
 #     'baselines',
 #     'binary',
 #     'datasets',
 #     'decomposition',
 #     'ensembles',
```

### Comparing `quantificationlib-0.0.7/quantificationlib/bag_generator.py` & `quantificationlib-0.1.1/quantificationlib/bag_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,29 +34,30 @@
         ----------
         n_bags : int, (default=1000)
             Number of bags
 
         bag_size : int, (default=None)
             Number of examples in each bag
 
-        method : str, (default='Uniform')
+        method : str, (default='Uniform') 
             Method used to generate the distributions. Two methods available:
+            
             - 'Uniform' : the prevalences are uniformly distributed
-            - 'Dirichlet : the prevalences are generated using the Dirichlet distribution
+            - 'Dirichlet' : the prevalences are generated using the Dirichlet distribution
 
         alphas : None, float or array-like, (default=None), shape (n_classes, ) when it is an array
             The parameters for the Dirichlet distribution when the selected method is 'Dirichlet'
 
         min_prevalence : None, float or array-like, (default=None)
             The min prevalence for each class. If None the min prevalence will be 0. If just a single value is passed
             all classes have the same min_prevalence value. This parameter is only used when 'Uniform' method
             is selected
 
         random_state : int, RandomState instance, (default=2032)
-            To generate random numbers
+            To generate random numbers.
             If type(random_state) is int, random_state is the seed used by the random number generator;
             If random_state is a RandomState instance, random_state is the own random number generator;
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
         Attributes
@@ -104,15 +105,15 @@
         self.indexes_ = None
 
     def generate_bags(self, X, y):
         """ Create bags of examples simulating prior probability shift
 
             Two different methods are implemented:
             - 'Uniform' : the prevalences are uniformly distributed
-            - 'Dirichlet : the prevalences are generated using the Dirichlet distribution
+            - 'Dirichlet' : the prevalences are generated using the Dirichlet distribution
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Data
 
             y : array-like, shape (n_examples, )
@@ -322,15 +323,15 @@
         n_bags : int, (default=1000)
             Number of bags
 
         bag_size : int, (default=None)
             Number of examples in each bag
 
         random_state : int, RandomState instance, (default=2032)
-            To generate random numbers
+            To generate random numbers.
             If type(random_state) is int, random_state is the seed used by the random number generator;
             If random_state is a RandomState instance, random_state is the own random number generator;
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
         Attributes
@@ -438,27 +439,28 @@
             Number of bags
 
         bag_size : int, (default=None)
             Number of examples in each bag
 
         method : str, (default='Uniform')
             Method used to generate the distributions. Two methods available:
+            
             - 'Uniform' : the prevalences are uniformly distributed
-            - 'Dirichlet : the prevalences are generated using the Dirichlet distribution
+            - 'Dirichlet' : the prevalences are generated using the Dirichlet distribution
 
         alphas : None, float or array-like, (default=None), shape (n_classes, ) when it is an array
             The parameters for the Dirichlet distribution when the selected method is 'Dirichlet'
 
         min_prevalence : None, float or array-like, (default=None)
             The min prevalence for each class. If None the min prevalence will be 0. If just a single value is passed
             all classes have the same min_prevalence value. This parameter is only used when 'Uniform' method
             is selected
 
         random_state : int, RandomState instance, (default=2032)
-            To generate random numbers
+            To generate random numbers.
             If type(random_state) is int, random_state is the seed used by the random number generator;
             If random_state is a RandomState instance, random_state is the own random number generator;
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
         Attributes
```

### Comparing `quantificationlib-0.0.7/quantificationlib/base.py` & `quantificationlib-0.1.1/quantificationlib/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         Examples of this type of quantifiers are HDX and EDX, for instance
 
         Parameters
         ----------
          verbose : int, optional, (default=0)
              The verbosity level. The default value, zero, means silent mode
 
-         Attributes
-         ----------
+        Attributes
+        ----------
          verbose : int
              The verbosity level
 
          classes_ : ndarray, shape (n_classes, )
              Class labels
      """
     def __init__(self, verbose=0, **kwargs):
@@ -86,27 +86,27 @@
         ----------
         estimator_train : estimator object, optional, (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is used to classify
             the examples of the training set and to obtain their distribution
 
         estimator_test : estimator object, optional, (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is used to classify
-            the examples of the testing bag and to obtain their distribution
+            the examples of the testing bag and to obtain their distribution.
+            For some experiments both estimators could be the same
 
         needs_predictions_train : bool, (default=True)
             True if the quantifier needs to estimate the training distribution
 
         probabilistic_predictions : bool, optional, (default=True)
             Whether the estimators return probabilistic predictions or not. This depends on the specific quantifier,
             some need crisp predictions (e.g. CC) and other methods require probabilistic predictions (PAC, HDy, ...)
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
@@ -269,15 +269,15 @@
 
             First, the method checks if at least one between estimator_test and prediction_test is not None,
             otherwise a ValueError exception is raised.
 
             Then, it computes predictions_test_. If predictions_test is not None, predictions_test_ is copied from
             predictions_test (and converted to crisp values, using `__probs2crisp` method when
             probabilistic_predictions attribute is False). If predictions_test is None, predictions_test_ is computed
-            calling the `predict`/`predict_proba method (depending on the value of the attribute
+            calling the `predict`/`predict_proba` method (depending on the value of the attribute
             probabilistic_predictions) of estimator_test.
 
             Parameters
             ----------
             X : (sparse) array-like, shape (n_examples, n_features)
                 Data
```

### Comparing `quantificationlib-0.0.7/quantificationlib/baselines/ac.py` & `quantificationlib-0.1.1/quantificationlib/baselines/ac.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """ Multiclass Adjusted Count method
 
         This class works in two different ways:
 
         1) Two estimators are used to classify the examples of the training set and the testing set in order to
            compute the confusion matrix of both sets. Estimators can be already trained
 
-        2) You can directly provide the predictions for the examples in the `fit`/`predict methods. This is useful
+        2) You can directly provide the predictions for the examples in the `fit`/`predict` methods. This is useful
            for synthetic/artificial experiments
 
         The idea in both cases is to guarantee that all methods based on distribution matching are using **exactly**
         the same predictions when you compare this kind of quantifiers (and others that also employ an underlying
         classifier, for instance, CC/PCC). In the first case, estimators are only trained once and can be shared
         for several quantifiers of this kind
 
@@ -39,25 +39,24 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict`. It is used to classify the examples of the training
             set and to compute the confusion matrix
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict`. It is used to classify the examples of the testing
-            set and to obtain their predictions
+            set and to obtain their predictions. For some experiments both estimators could be the same
 
         distance : str, representing the distance function (default='HD')
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution. Only used in multiclass problems.
             Distances supported: 'HD', 'L2' and 'L1'
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
@@ -141,15 +140,15 @@
                 Data
 
             y : array-like, shape (n_examples, )
                 True classes
 
             predictions_train : ndarray, shape (n_examples, ) or (n_examples, n_classes)
                 Predictions of the examples in the training set. If shape is (n_examples, n_classes) predictions are
-                converted to crisp values by `super().fit()
+                converted to crisp values by `super().fit()`
 
             Raises
             ------
             ValueError
                 When estimator_train and predictions_train are both None
         """
         super().fit(X, y, predictions_train=predictions_train)
@@ -187,27 +186,26 @@
             For binary problems the system is directly solved using the original AC algorithm proposed by Forman
 
                         p = (p_0 - fpr ) / ( tpr - fpr)
 
             For multiclass problems, the system may not have a solution. Thus, instead we propose to solve an
             optimization problem of this kind:
 
-                      Min   distance ( cm_.T * prevalences, CC(X) )
-                      s.t.  sum(prevalences) = 1
-                            prevalecences_i >= 0
+                      Min   distance ( cm_.T * prevalences, CC(X) )                \n
+                      s.t.  sum(prevalences) = 1 , prevalecences_i >= 0
 
             in which distance can be 'HD' (defect value), 'L1' or 'L2'
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Testing bag
 
             predictions_test : ndarray, shape (n_examples, n_classes) (default=None)
-                They must be probabilities (the estimator used must have a `predict_proba method)
+                They must be probabilities (the estimator used must have a `predict_proba` method)
 
                 If predictions_test is not None they are copied on predictions_test_ and used.
                 If predictions_test is None, predictions for the testing examples are computed using the `predict`
                 method of estimator_test (it must be an actual estimator)
 
             Raises
             ------
@@ -279,15 +277,15 @@
     """ Multiclass Probabilistic Adjusted Count method
 
         This class works in two different ways:
 
         1) Two estimators are used to classify the examples of the training set and the testing set in order to
            compute the (probabilistic) confusion matrix of both sets. Estimators can be already trained
 
-        2) You can directly provide the predictions for the examples in the `fit`/`predict methods. This is useful
+        2) You can directly provide the predictions for the examples in the `fit`/`predict` methods. This is useful
            for synthetic/artificial experiments
 
         The idea in both cases is to guarantee that all methods based on distribution matching are using **exactly**
         the same predictions when you compare this kind of quantifiers (and others that also employ an underlying
         classifier, for instance, CC/PCC). In the first case, estimators are only trained once and can be shared
         for several quantifiers of this kind
 
@@ -295,25 +293,25 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the confusion matrix
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to obtain the confusion matrix of the testing set
+            testing set and to obtain the confusion matrix of the testing set. 
+            For some experiments both estimators could be the same
 
         distance : str, representing the distance function (default='L2')
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution. Only used in multiclass problems.
             Distances supported: 'HD', 'L2' and 'L1'
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
@@ -384,15 +382,15 @@
         self.C_ = None
         self.b_ = None
         self.problem_ = None
 
     def fit(self, X, y, predictions_train=None):
         """ This method performs the following operations: 1) fits the estimators for the training set and the
             testing set (if needed), and 2) computes predictions_train_ (probabilities) if needed. Both operations are
-            performed by the `fit method of its superclass.
+            performed by the `fit` method of its superclass.
             Finally the method computes the (probabilistic) confusion matrix using predictions_train
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Data
 
@@ -430,32 +428,31 @@
 
         return self
 
     def predict(self, X, predictions_test=None):
         """ Predict the class distribution of a testing bag
 
             First, predictions_test_ are computed (if needed, when predictions_test parameter is None) by
-            `super().predict() method.
+            `super().predict()` method.
 
             After that, the prevalences are computed solving a system of linear scalar equations:
 
                          cm_.T * prevalences = PCC(X)
 
             For binary problems the system is directly solved using the original PAC algorithm proposed by Bella et al.
 
                         p = (p_0 - PA(negatives) ) / ( PA(positives) - PA(negatives) )
 
             in which PA stands for probability average.
 
             For multiclass problems, the system may not have a solution. Thus, instead we propose to solve an
             optimization problem of this kind:
 
-                      Min   distance ( cm_.T * prevalences, PCC(X) )
-                      s.t.  sum(prevalences) = 1
-                            prevalecences_i >= 0
+                      Min   distance ( cm_.T * prevalences, PCC(X) )        \n
+                      s.t.  sum(prevalences) = 1, prevalecences_i >= 0
 
             in which distance can be 'HD', 'L1' or 'L2' (defect value)
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Testing bag
```

### Comparing `quantificationlib-0.0.7/quantificationlib/baselines/cc.py` & `quantificationlib-0.1.1/quantificationlib/baselines/cc.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         if self.verbose > 0:
             print('done')
 
         return np.squeeze(prevalences)
 
 
 class PCC(UsingClassifiers):
-    """ Multiclass Probabilistic Classify And Count method.
+    """ Multiclass Probabilistic Classify And Count method
 
         prevalence (class_i) = sum_{x in T} P( h(x) == class_i | x )
 
         This class works in two different ways:
 
         1) An estimator is used to classify the examples of the testing bag (the estimator can be already trained)
```

### Comparing `quantificationlib-0.0.7/quantificationlib/binary/debias.py` & `quantificationlib-0.1.1/quantificationlib/binary/debias.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,21 +34,20 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the confusion matrix
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to obtain the confusion matrix of the testing set
+            testing set and to obtain the confusion matrix of the testing set.
+            For some experiments both estimators could be the same
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
-
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set.
 
         estimator_test : estimator
             Estimator used to classify the examples of the testing bag
@@ -100,15 +99,15 @@
         self.train_prevs_ = None
         # Vt value
         self.Vt_ = None
 
     def fit(self, X, y, predictions_train=None):
         """ This method performs the following operations: 1) fits the estimators for the training set and the
             testing set (if needed), and 2) computes predictions_train_ (probabilities) if needed. Both operations are
-            performed by the `fit method of its superclass.
+            performed by the `fit` method of its superclass.
 
             Finally the method computes the value of Vt
 
             Vt =[ 1/|T| sum_{x in D} (P(h(x)==+1|x) - prior(positives) )^2 ] / (prior(positives) * prior(negatives))
 
             Parameters
             ----------
```

### Comparing `quantificationlib-0.0.7/quantificationlib/binary/emd.py` & `quantificationlib-0.1.1/quantificationlib/binary/emd.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,24 +30,23 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         tol : float, (default=1e-05)
             The precision of the solution when search is used to compute the prevalence
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimator_train and estimator_test could be the same
-
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
             Estimator used to classify the examples of the testing bag
@@ -67,15 +66,15 @@
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         y_ext_ : ndarray, shape(len(predictions_train_, 1)
             Repmat of true labels of the training set. When CV_estimator is used with averaged_predictions=False,
             predictions_train_ will have a larger dimension (factor=n_repetitions * n_folds of the underlying CV)
             than y. In other cases, y_ext_ == y.
-            y_ext_ i used in `fit`/`predict` method whenever the true labels of the training set are needed,
+            y_ext_ is used in `fit`/`predict` method whenever the true labels of the training set are needed,
             instead of y
 
         tol : float
             The precision of the solution when search is used to compute the solution
 
         train_distrib_ : ndarray, shape (n_examples_train, 1) binary quantification
             Contains predictions_train_ in ascending order
@@ -164,16 +163,17 @@
             First, predictions_test_ are computed (if needed, when predictions_test parameter is None) by
             `super().predict()` method.
 
             After that, the method computes the union distribution, merging training and testing distributions. This
             union is sorted based on the posterior probability of each example.
 
             Finally, the prevalences are computed using golden section search using two functions:
-                -compute_sord_weights: to obtain the mixture depending on the estimated prevalence
-                -sord: distance funtion to measure how similar the mixture and the testing distributions are
+            
+            - compute_sord_weights: to obtain the mixture depending on the estimated prevalence
+            - sord: distance funtion to measure how similar the mixture and the testing distributions are
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Testing bag
 
             predictions_test : ndarray, shape (n_examples, n_classes) (default=None)
```

### Comparing `quantificationlib-0.0.7/quantificationlib/binary/quantiles.py` & `quantificationlib-0.1.1/quantificationlib/binary/quantiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,31 +45,30 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         n_quantiles : int
             Number of quantiles
 
         distance : distance function (default=l2)
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution
 
         tol : float, (default=1e-05)
             The precision of the solution when search is used to compute the prevalence
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimator_train and estimator_test could be the same
-
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
             Estimator used to classify the examples of the testing bag
@@ -89,15 +88,15 @@
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         y_ext_ : ndarray, shape(len(predictions_train_, 1)
             Repmat of true labels of the training set. When CV_estimator is used with averaged_predictions=False,
             predictions_train_ will have a larger dimension (factor=n_repetitions * n_folds of the underlying CV)
             than y. In other cases, y_ext_ == y.
-            y_ext_ i used in `fit`/`predict` method whenever the true labels of the training set are needed,
+            y_ext_ is used in `fit`/`predict` method whenever the true labels of the training set are needed,
             instead of y
 
         n_quantiles : int (default=8)
             The number of quantiles to represent data distribution
 
         distance : A distance function (default=l2)
             The name of the distance function used
```

### Comparing `quantificationlib-0.0.7/quantificationlib/data_utils.py` & `quantificationlib-0.1.1/quantificationlib/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/quantificationlib/decomposition/multiclass.py` & `quantificationlib-0.1.1/quantificationlib/decomposition/multiclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,20 +37,19 @@
             the examples of the training set and to obtain their distribution when the base quantifier is an
             instance of the class UsingClassifiers. Notice that some quantifiers of this kind, namely CC and PCC,
             do not require an estimator for the training distribution
 
         estimator_test : estimator object, optional, (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is used to classify
             the examples of the testing bag and to obtain their distribution when the base quantifier is an
-            instance of the class UsingClassifiers
+            instance of the class UsingClassifiers. For some experiments both estimators could be the same
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         base_quantifier : quantifier object
             The base quantifier used to build the One versus Rest decomposition
 
         estimator_train : estimator
```

### Comparing `quantificationlib-0.0.7/quantificationlib/decomposition/ordinal.py` & `quantificationlib-0.1.1/quantificationlib/decomposition/ordinal.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,20 +37,19 @@
             the examples of the training set and to obtain their distribution when the base quantifier is an
             instance of the class UsingClassifiers. Notice that some quantifiers of this kind, namely CC and PCC,
             do not require an estimator for the training distribution
 
         estimator_test : estimator object, optional, (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is used to classify
             the examples of the testing bag and to obtain their distribution when the base quantifier is an
-            instance of the class UsingClassifiers
+            instance of the class UsingClassifiers. For some experiments both estimators could be the same
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         quantifier : quantifier object
             The base quantifier used to build the FH decomposition
 
         estimator_train : estimator
@@ -177,36 +176,34 @@
 
     def predict(self, X, predictions_test=None):
         """ Aggregates the prevalences of the quantifiers_ to compute the final prediction
 
             In this kind of decomposition strategy it is important to ensure that the aggregated consecutive
             prevalencences do not decrease:
 
-            Example:
+            Example::
 
-                Quantifier 1 vs 2-3-4   Prevalence({1}) = 0.3
-                Quantifier 1-2 vs 3-4   Prevalence({1,2}) = 0.2
-                Quantifier 1-2-3 vs 4   Prevalence({1,2,3}) = 0.6
+                 Quantifier 1 vs 2-3-4   Prevalence({1}) = 0.3
+                 Quantifier 1-2 vs 3-4   Prevalence({1,2}) = 0.2
+                 Quantifier 1-2-3 vs 4   Prevalence({1,2,3}) = 0.6
 
             This is inconsistent. Following (Destercke, Yang, 2014) the method computes the upper (adjusting from
             left to right) and the lower (from right to left) cumulative prevalences. These sets of values are
             monotonically increasing (from left to right) and monotonically decreasing (from right to left),
             respectively. The average value is assigned to each group and the prevalence for each class is computed as:
 
                 Prevalence({y_k}) = Prevalence({y_1,...,y_k}) - Prevalence({y_1,...,y_k-1})
 
-            Example:
-
-                {1}   {1-2}  {1-2-3}
-
-                0.3   0.3    0.6    Upper cumulative prevalences (adjusting from left to right)
-
-                0.2   0.2    0.6    Lower cumulative prevalences (adjusting from right to left)
+            Example::
+            
+                {1}   {1-2}  {1-2-3} 
+                0.3   0.3    0.6    Upper cumulative prevalences (adjusting from left to right) 
+                0.2   0.2    0.6    Lower cumulative prevalences (adjusting from right to left) 
                 ----------------
-                0.25  0.25   0.6    Averaged prevalences
+                0.25  0.25   0.6    Averaged prevalences 
 
                 Prevalence({1}) = 0.25
                 Prevalence({2}) = Prevalence({1,2}) - Prevalence({1}) = 0.25 - 0 .25 = 0
                 Prevalence({3}) = Prevalence({1,2,3}} - Prevalence({1,2}) = 0.6 - 0.25 = 0.35
 
                 The last class is computed as 1 - the sum of prevalences for the rest of classes
 
@@ -269,34 +266,32 @@
     @staticmethod
     def check_and_correct_prevalences_asc(prevalences):
         """ This function checks and corrects the prevalences of a quantifier based on the Frank and Hall decomposition
             that are inconsistent. It is used by FrankAndHallQuantifier.
 
             To obtain consistent prevalences, we need to ensure that the consecutive probabilities do not decrease.
 
-            Example:
+            Example::
 
-                Quantifier 1 vs 2-3-4   Prevalence({1}) = 0.3
-                Quantifier 1-2 vs 3-4   Prevalence({1,2}) = 0.2
-                Quantifier 1-2-3 vs 4   Prevalence({1,2,3}) = 0.6
+                 Quantifier 1 vs 2-3-4   Prevalence({1}) = 0.3
+                 Quantifier 1-2 vs 3-4   Prevalence({1,2}) = 0.2
+                 Quantifier 1-2-3 vs 4   Prevalence({1,2,3}) = 0.6
 
             This is inconsistent. Following (Destercke, Yang, 2014) the method computes the upper (adjusting from
             left to right) and the lower (from right to left) cumulative prevalences. These sets of values are
             monotonically increasing (from left to right) and monotonically decreasing (from right to left),
             respectively. The average value is assigned to each group
 
-            Example:
-
-                {1}   {1-2}  {1-2-3}
-
-                0.3   0.3    0.6    Upper cumulative prevalences (adjusting from left to right)
-
-                0.2   0.2    0.6    Lower cumulative prevalences (adjusting from right to left)
-                ----------------
-                0.25  0.25   0.6    Averaged prevalences
+            Example::
+            
+                 {1}   {1-2}  {1-2-3}
+                 0.3   0.3    0.6      Upper cumulative prevalences (adjusting from left to right)
+                 0.2   0.2    0.6      Lower cumulative prevalences (adjusting from right to left)
+                 ----------------  
+                 0.25  0.25   0.6      Averaged prevalences
 
             Parameters
             ----------
             prevalences : array, shape(n_classes-1, )
                 The prevalences of the binary quantifiers of a FrankAndHallQuantifier for a single dataset
 
             Return
```

### Comparing `quantificationlib-0.0.7/quantificationlib/ensembles/eoq.py` & `quantificationlib-0.1.1/quantificationlib/ensembles/eoq.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,34 +54,34 @@
             features (Xs) for quantifiers derived from WithoutClassifiers class and the predictions (Ys) for
             quantifiers derived from UsingClassifiers
 
         n_bins : int, (default=100)
             Numbers of bins to estimate the distributions of training and testing bags. This is needed for
             distribution_similarity combination strategy.
 
-        bin_strategy = str, (default='equal_width')
+        bin_strategy : str, (default='equal_width')
             Method to compute the boundaries of the bins for to estimate the distributions of training and testing
             bags when the distribution_similarity combination strategy is used. Possible values:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                          (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+
+            - 'equal_width': bins of equal length (it could be affected by outliers)
+            - 'equal_count': bins of equal counts (considering the examples of all classes)
+            - 'binormal': (Only for binary quantification) It is inspired on the method devised by
+                          (Tasche, 2019, Eq (A16b)). the cut points, :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                           are computed as follows based on the assumption that the features follow a normal distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                          :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                          where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                          and $\sigma$ of the normal distribution are estimated as the average of those values for
+                          where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                          and :math:`\\sigma` of the normal distribution are estimated as the average of those values for
                           the training examples of each class.
+            - 'normal':  The idea is that each feature follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
+                         estimated as the weighted mean and std from the training distribution. The cut points
+                         :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
-                           estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
-
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                         :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         distance_bags : str, (default='euclidean')
             Distance used to compute distribution similarity
 
         percentage_of_selected_models : float, value in [0, 1], (default=0.5)
             Percentage of selected models for distribution similarity and prevalence similarity strategies
 
@@ -183,17 +183,18 @@
         self.classes_ = None
 
     def fit(self, X, y, predictions_train=None, prevalences=None, indexes=None):
         """ This method does the following tasks:
 
             1) It generates the training bags using a Bag_Generator object
             2) It fits the quantifiers of the ensemble.
+            
             In the case of quantifiers derived from the class UsingClassifiers, there are 3 possible ways to do this:
-            - train a classifier for each bag. To do this an object from the class EnsembleOfClassifiers must be
-              passed on ensemble_estimator
+            
+            - train a classifier for each bag. To do this an object from the class EnsembleOfClassifiers must be passed on ensemble_estimator
             - train a classifier for the whole training set using an estimator from other class
             - uses the predictions_train given in the predictions_train parameter (these predictions usually are
               obtained applying an estimator over the whole training set like in the previous case)
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
```

### Comparing `quantificationlib-0.0.7/quantificationlib/estimators/cross_validation.py` & `quantificationlib-0.1.1/quantificationlib/estimators/cross_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
 
 class CV_estimator(BaseEstimator, ClassifierMixin):
     """ Cross Validation Estimator
 
         The idea is to have an estimator in which the model is formed by the models of a CV. This object is needed
         to estimate the distribution of the training set and testing sets. It has a `fit` method, that trains
-        the models of the CV, and the typical methods `predict` y `predict_proba` to compute the predictions using
+        the models of the CV, and the typical methods `predict` and `predict_proba` to compute the predictions using
         such models. This implies that this object can be used by any distribution matching method that requires an
         estimator to represent the distributions
 
         Parameters
         ----------
         Mainly the same that `cross_validate` method in sklearn:
 
-        estimator : estimator object implementing 'fit'
+        estimator : estimator object implementing `fit`
             The object to use to fit the data.
 
         groups : array-like, with shape (n_samples,), optional
             Group labels for the samples used while splitting the dataset into train/test set.
 
         cv : int, cross-validation generator or an iterable, optional
             Determines the cross-validation splitting strategy. Possible inputs for cv are:
@@ -56,54 +56,51 @@
         fit_params : dict, optional
             Parameters to pass to the fit method of the estimator.
 
         pre_dispatch : int, or string, optional
             Controls the number of jobs that get dispatched during parallel execution. Reducing this number can be
             useful to avoid an explosion of memory consumption when more jobs get dispatched than CPUs can process.
             This parameter can be:
-            - None, in which case all the jobs are immediately
-              created and spawned. Use this for lightweight and
-              fast-running jobs, to avoid delays due to on-demand
-              spawning of the jobs
-            - An int, giving the exact number of total jobs that are
-              spawned
-            - A string, giving an expression as a function of n_jobs,
-              as in '2*n_jobs'
+
+            - None, in which case all the jobs are immediately created and spawned. Use this for lightweight and
+              fast-running jobs, to avoid delays due to on-demand spawning of the jobs
+            - An int, giving the exact number of total jobs that are spawned
+            - A string, giving an expression as a function of n_jobs, as in `2*n_jobs`
 
         averaged_predictions : bool, optional (default=True)
-            If True, `predict`and `predict_proba` methods average the predictions given by estimators_ for
+            If True, `predict` and `predict_proba` methods average the predictions given by estimators_ for
             each example
 
         voting : str, {'hard', 'soft'} (default='hard')
             Only used when averaged_predictions is True.
-            If 'hard', `predict`and `predict_proba` methods apply majority rule voting.
+            If 'hard', `predict` and `predict_proba` methods apply majority rule voting.
             If 'soft', predict the class label based on the argmax of the sums of the predicted probabilities,
             which is recommended for an ensemble of well-calibrated classifiers.
 
         verbose : integer, optional (default=0)
             The verbosity level.
 
+           
         Attributes
         ----------
-        In addition to the parameters needed to call `cross_validate`` the class has this important attributes:
-
         estimator : An estimator object
             The estimator to fit each model of the CV
 
         estimators_ : list of trained estimators
             The list of estimators trained by `fit`method.
             The number of estimators is equal to the number of folds times number of repetitions
 
         averaged_predictions : bool
             Determines whether the predictions for each example given by estimators_ are averaged or not
 
         voting : str, {'hard', 'soft'} (default='hard')
             How predictions are aggregated:
-                - 'hard', applying majority rule voting
-                - 'soft', based on the argmax of the sums of the predicted probabilities
+            
+            - 'hard', applying majority rule voting
+            - 'soft', based on the argmax of the sums of the predicted probabilities
 
         le_ : a LabelEncoder fitted object
             Used to compute the class labels
 
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
@@ -133,15 +130,15 @@
         self.classes_ = None
         self.X_train_ = None
         self.y_train_ = None
 
     def fit(self, X, y):
         """ Fit the models
             It calls `cross_validate` to fit the models and save them in estimators_ attribute.
-            It also stores some attributes needed by `predict` and `predict_proba`, namely, le_, classes_ X_train
+            It also stores some attributes needed by `predict` and `predict_proba`, namely, le_, classes_, X_train
             and y_train_
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Data
 
@@ -172,22 +169,22 @@
                 Test ata
 
             Returns
             -------
             preds : array-like, shape depends on two factors: the type of the examples (training or testing) and
                     the value of averaged_predictions attribute
 
+                 Crisp predictions for the examples in X
+
                  Training set:
                      - averaged_predictions == True,  shape(n_examples, )
                      - averaged_predictions == False, shape(n_examples * n_reps, )
                  Testing set:
                      - averaged_predictions == True,  shape(n_examples, )
                      - averaged_predictions == False, shape(n_examples * n_reps * n_folds, )
-
-                 Crisp predictions for the examples in X
         """
         if len(self.estimators_) == 0:
             raise NotFittedError('CV_estimator not fitted')
 
         preds = self._predict_proba(X)
 
         if self.averaged_predictions:
@@ -224,21 +221,21 @@
 
             Returns
             -------
             preds : array-like, shape depends on two factors: the type of the examples (training or testing) and
                     the value of averaged_predictions attribute
 
                 Probabilistic predictions for the examples in X.
-                Shape:
-                    Training set:
-                        - averaged_predictions == True,  shape(n_examples, n_classes)
-                        - averaged_predictions == False, shape(n_examples * n_reps, n_classes)
-                    Testing set:
-                        - averaged_predictions == True,  shape(n_examples, n_classes)
-                        - averaged_predictions == False, shape(n_examples * n_reps * n_folds, n_classes)
+                
+                Training set:
+                    - averaged_predictions == True,  shape(n_examples, n_classes)
+                    - averaged_predictions == False, shape(n_examples * n_reps, n_classes)
+                Testing set:
+                    - averaged_predictions == True,  shape(n_examples, n_classes)
+                    - averaged_predictions == False, shape(n_examples * n_reps * n_folds, n_classes)
         """
         if len(self.estimators_) == 0:
             raise NotFittedError('CV_estimator not fitted')
 
         preds = self._predict_proba(X)
 
         if self.averaged_predictions:
```

### Comparing `quantificationlib-0.0.7/quantificationlib/estimators/ensembles.py` & `quantificationlib-0.1.1/quantificationlib/estimators/ensembles.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,15 @@
         base_estimator : estimator object (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is the base estimator
             used to learn the set of classifiers
 
         n_jobs : int or None, optional (default=None)
             The number of jobs to use for the computation.
             ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-            ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-            for more details.
+            ``-1`` means using all processors 
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
         Attributes
         ----------
         base_estimator : estimator object
@@ -52,15 +51,15 @@
 
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         n_estimators_ : int,
             Number of estimators
 
-        estimators_ : ndarray, shape(n_ensembles,)
+        estimators_ : ndarray, shape(n_ensembles, )
             List of estimators
 
         References
         ----------
         Pérez-Gállego, P., Quevedo, J. R., & del Coz, J. J. (2017). Using ensembles for problems with characterizable
         changes in data distribution: A case study on quantification. Information Fusion, 34, 87-100.
```

### Comparing `quantificationlib-0.0.7/quantificationlib/estimators/frank_and_hall.py` & `quantificationlib-0.1.1/quantificationlib/estimators/frank_and_hall.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         estimator : estimator object (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is the base estimator
             used to learn the set of binary classifiers
 
         n_jobs : int or None, optional (default=None)
             The number of jobs to use for the computation.
             ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-            ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-            for more details.
+            ``-1`` means using all processors
 
         params_fit : list of dictionaries with parameters for each binary estimator, optional
             Example: 5 classes/4 binary estimators:
 
                 params_fit = [{'C':0.0001} , {'C':0.000001}, {'C':0.000001}, {'C':0.01}]
 
         verbose : int, optional, (default=0)
@@ -65,16 +64,16 @@
             The verbosity level. The default value, zero, means silent mode
 
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         estimators_ : ndarray, shape(n_classes-1,)
             List of binary estimators following the same order of the Frank and Hall decomposition:
-                estimators_[0] -> 1 vs 2-3-4-5
-                estimators_[1] -> 1-2 vs 3-4-5
+                estimators_[0] -> 1 vs 2-3-4-5, 
+                estimators_[1] -> 1-2 vs 3-4-5, 
                 ...
 
         label_binarizer_ :  FHLabelBinarizer object
             Object used to transform multiclass labels to binary labels and vice-versa
 
         References
         ----------
@@ -119,16 +118,16 @@
         clf.fit(X, y_bin)
         return clf
 
     def fit(self, X, y):
         """ Fits the set of estimators for the training set following the Frank and Hall decomposition
 
             It learns a list of binary estimators following the same order of the Frank and Hall decomposition:
-                estimators_[0] -> 1 vs 2-3-4-5
-                estimators_[1] -> 1-2 vs 3-4-5
+                estimators_[0] -> 1 vs 2-3-4-5, 
+                estimators_[1] -> 1-2 vs 3-4-5, 
                 ...
 
             The left group of each classifier ({1}, {1,2}, ...) is the positive class
 
             Parameters
             ----------
             X : (sparse) array-like, shape (n_examples, n_features)
@@ -190,27 +189,28 @@
         probs_samples = self.predict_proba(X)
         best_classes = np.argmax(probs_samples, axis=1)
         return self.classes_[best_classes]  # this returns the label of the winner class instead of its index
 
     def predict_proba(self, X):
         """ Predict the class probabilities for each example following the original rule proposed by Frank & Hall
 
-            If the classes are c_1 to c_k:
+            If the classes are c_1 to c_k::
 
                 Pr(y = c_1) = Pr (y <= c_1)
                 Pr(y = c_i) = Pr(y > c_i−1)  x (1 − Pr(y > c_i)) ; 1 < i < k
                 Pr(y = c_k) = Pr(y > c_k−1)
 
-                Notice that :  :math:`sum_{i=1}^{i=k} Pr(c_i) \neq 1`
+                Notice that :  sum_{i=1}^{i=k} Pr(c_i) \\neq 1
 
-            Example with 5 classes
+            Example with 5 classes::
 
-                We have 4 binary estimators that return two probabilities: the probability of the left group and the
-                probability of the right group, denoted as e_i.left and e_i.right respectively, in which i is the
-                number of the estimator 1<=i<k
+                We have 4 binary estimators that return two probabilities: 
+                the probability of the left group and the probability of the right group, 
+                denoted as e_i.left and e_i.right respectively, 
+                in which i is the number of the estimator 1<=i<k
 
                 Estimator 0:	c1  |   c2, c3, c4, c5          e1.left	| e1.right
                 Estimator 2:	c1, c2  |   c3, c4, c5          e2.left	| e2.right
                 Estimator 3:	c1, c2, c3  |   c4, c5          e3.left	| e3.right
                 Estimator 4:	c1, c2, c3  c4  |   c5          e4.left	| e4.right
 
                 Pr(y = c_1) = e1.left
@@ -313,16 +313,15 @@
         estimator : estimator object (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is the base estimator
             used to learn the set of binary classifiers
 
         n_jobs : int or None, optional (default=None)
             The number of jobs to use for the computation.
             ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-            ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-            for more details.
+            ``-1`` means using all processors
 
         params_fit : list of dictionaries with parameters for each binary estimator, optional
             Example: 5 classes/4 binary estimators:
 
                 params_fit = [{'C':0.0001} , {'C':0.000001}, {'C':0.000001}, {'C':0.01}]
 
         verbose : int, optional, (default=0)
@@ -343,16 +342,16 @@
              It has the parameters for each binary estimator (not used in this class)
 
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         estimators_ : ndarray, shape(n_classes-1,)
             List of binary estimators following the same order of the Frank and Hall decomposition:
-                estimators_[0] -> 1 vs 2-3-4-5
-                estimators_[1] -> 1-2 vs 3-4-5
+                estimators_[0] -> 1 vs 2-3-4-5, 
+                estimators_[1] -> 1-2 vs 3-4-5, 
                 ...
 
         label_binarizer_ :  FHLabelBinarizer object
             Object used to transform multiclass labels to binary labels and vice-versa
 
         References
         ----------
@@ -364,16 +363,16 @@
         super(FrankAndHallMonotoneClassifier, self).__init__(estimator=estimator, n_jobs=n_jobs, verbose=verbose,
                                                              params_fit=params_fit)
 
     def fit(self, X, y):
         """ Fits the set of estimators for the training set following the Frank and Hall decomposition
 
             It learns a list of binary estimators following the same order of the Frank and Hall decomposition:
-                estimators_[0] -> 1 vs 2-3-4-5
-                estimators_[1] -> 1-2 vs 3-4-5
+                estimators_[0] -> 1 vs 2-3-4-5, 
+                estimators_[1] -> 1-2 vs 3-4-5, 
                 ...
 
             The left group of each classifier ({1}, {1,2}, ...) is the positive class
 
             Parameters
             ----------
             X : (sparse) array-like, shape (n_examples, n_features)
@@ -417,43 +416,41 @@
     def predict_proba(self, X):
         """ Predict the class probabilities for each example following a new rule (different from the original
             one proposed by Frank & Hall)
 
             To obtain consistent probabilities, we need to ensure that the aggregated consecutive
             probabilities do not decrease.
 
-            Example:
+            Example::
 
                 Classifier 1 vs 2-3-4   Pr({1}) = 0.3
                 Classifier 1-2 vs 3-4   Pr({1,2}) = 0.2
                 Classifier 1-2-3 vs 4   Pr({1,2,3}) = 0.6
 
             This is inconsistent. Following (Destercke and Yang, 2014) the method computes the upper (adjusting from
             left to right) and the lower (from right to left) cumulative probabilities. These sets of values are
             monotonically increasing (from left to right) and monotonically decreasing (from right to left),
             respectively. The average value is assigned to each group and the probability for each class is computed as:
 
                 Pr({y_k}) = Pr({y_1,...,y_k}) - Pr({y_1,...,y_k-1})
 
-            Example:
+            Example::
 
                 {1}   {1-2}  {1-2-3}
-
                 0.3   0.3    0.6    Upper cumulative probabilities (adjusting from left to right)
-
                 0.2   0.2    0.6    Lower cumulative probabilities (adjusting from right to left)
                 ----------------
                 0.25  0.25   0.6    Averaged probability
 
                 Pr({1}) = 0.25
                 Pr({2}) = Pr({1,2}) - Pr({1}) = 0.25 - 0 .25 = 0
                 Pr({3}) = Pr({1,2,3}} - Pr({1,2}) = 0.6 - 0.25 = 0.35
 
                 The last class is computed as 1 - the sum of the probabilities for the rest of classes
-
+                
                 Pr({4}) = 1 - Pr({1,2,3}} = 1 - 0.6 = 0.4
 
             Parameters
             ----------
             X : (sparse) array-like, shape (n_examples, n_features)
                 Data
 
@@ -572,31 +569,34 @@
         The difference with FrankAndHallClassifier is that the original method devised by Frank & Hall computes the
         probability of each class applying the binary models from left to right: 1 vs 2-3-4-5, 1-2 vs 3-4-5, and so on.
         This classifier is based on the method proposed by (San Martino, Gao and Sebastiani, 2016). The idea is to
         build a binary tree with the binary models of the Frank and Hall decomposition, selecting at each point of the
         tree the best possible model according to their quantification performance (applying PCC algorithm with each
         binary classifier and using the KLD as performance measure).
 
-        Example:
-                                             1-2-3 vs 4-5
-                         1 vs 2-3-4-5                            1-2-3-4 vs 5
-                      1                1-2 vs 3-4-5           4                5
-                                     2              3
+        Example::
+        
+                                                1-2-3 vs 4-5
+
+                             1 vs 2-3-4-5                            1-2-3-4 vs 5
+
+                          1                1-2 vs 3-4-5           4                5
+                      
+                                       2                 3
 
         Parameters
         ----------
         estimator : estimator object (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is the base estimator
             used to learn the set of binary classifiers
 
         n_jobs : int or None, optional (default=None)
             The number of jobs to use for the computation.
             ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-            ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-            for more details.
+            ``-1`` means using all processors
 
         performance_measure : a binary quantification performance measure, (default=binary_kld)
             The binary quantification performance measure used to estimate the goodness of each binary classifier used
             as quantifier
 
         params_fit : list of dictionaries with parameters for each binary estimator, optional
             Example: 5 classes/4 binary estimators:
@@ -625,16 +625,16 @@
              It has the parameters for each binary estimator
 
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         estimators_ : ndarray, shape(n_classes-1,)
             List of binary estimators following the same order of the Frank and Hall decomposition:
-                estimators_[0] -> 1 vs 2-3-4-5
-                estimators_[1] -> 1-2 vs 3-4-5
+                estimators_[0] -> 1 vs 2-3-4-5, 
+                estimators_[1] -> 1-2 vs 3-4-5, 
                 ...
 
         label_binarizer_ :  FHLabelBinarizer object
             Object used to transform multiclass labels to binary labels and vice-versa
 
         tree_ : A tree
             A tree with the binary classifiers ordered by their quantification performance (using KLD or other measure)
@@ -705,22 +705,26 @@
         probs_samples = self.predict_proba(X)
         best_classes = np.argmax(probs_samples, axis=1)
         return self.classes_[best_classes]
 
     def predict_proba(self, X):
         """ Predict the class probabilities for each example applying the binary tree of models
 
-            Example:
+            Example::
+
                                              1-2-3 vs 4-5
+            
                          1 vs 2-3-4-5                            1-2-3-4 vs 5
+            
                       1                1-2 vs 3-4-5           4                5
+ 
                                      2              3
 
-                 Imagine that for a given example the probabily returned by each model are the following (the models
-                 return the probability of the left group of classes):
+                 Imagine that for a given example the probabily returned by each model are the following 
+                 (the models return the probability of the left group of classes):
 
                  Pr({1,2,3}) = 0.2
                  Pr({1}) = 0.9
                  Pr({1,2,3,4}) = 0.7
                  Pr({1,2}) = 0.4
 
                  with tha values, the probability for each class will be:
@@ -950,25 +954,26 @@
         ranging from 1-star to 5-star, Frank and Hall (FH) decompositon trains 4 binary classifiers:
         1 vs 2-3-4-5, 1-2 vs 3-4-5, 1-2-3 vs 4-5, 1-2-3-4 vs 5 and combines their predictions.
 
         To train all these binary classifiers, one needs to convert the original ordinal labels to binary labels
         for each of the binary problems of the Frank and Hall decomposition. FHLabelBinarizer makes this process
         easy using the transform method.
 
-         Parameters
-         ----------
-         neg_label : int (default: 0)
+        Parameters
+        ----------
+        neg_label : int (default: 0)
              Value with which negative labels must be encoded.
 
-         pos_label : int (default: 1)
+        pos_label : int (default: 1)
              Value with which positive labels must be encoded.
 
-         sparse_output : boolean (default: False)
+        sparse_output : boolean (default: False)
              True if the returned array from transform is desired to be in sparse CSR format.
-        """
+
+    """
     def __init__(self, neg_label=0, pos_label=1):
         super(FHLabelBinarizer, self).__init__(neg_label=neg_label, pos_label=pos_label, sparse_output=False)
 
     def transform(self, y):
         """ Transform ordinal labels to the Frank and Hall binary labels
 
             Parameters
```

### Comparing `quantificationlib-0.0.7/quantificationlib/estimators/ordinal_ddag.py` & `quantificationlib-0.1.1/quantificationlib/estimators/ordinal_ddag.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,146 +15,160 @@
 from sklearn.multiclass import OneVsOneClassifier
 
 
 class DDAGClassifier(OneVsOneClassifier):
     """ Decision Directed Acyclic Graph ordinal classifier
 
         This strategy consists on learning a classifier per each pair of classes, thus it requires to fit
-        n_classes * (n_classes - 1) / 2 classifiers. For this reason, this class derives from OneVsOneClassifier and
+        `n_classes * (n_classes - 1) / 2` classifiers. For this reason, this class derives from OneVsOneClassifier and
         uses most of its functionalities, mainly to train the binary models.
 
         However, there are two main differences with respect to OneVsOneClassifier:
 
         1) This class is used for ordinal classification, it does not make sense to use it for multiclass classification
         2) The rule to make predictions is different. Here, the binary classifiers are arranged into a binary tree in
            which the classifier selected at each node is the one that deals with the two more distant remaining
            classes. Thus, the root contains the classifier that decides between the first class of the order and last
            class, and this idea is recursively applied.
 
-            Example: in a ordinal classification problem with classes ranging from 1-star to 5-star,
+        Example::
+             
+            In a ordinal classification problem with classes ranging from 1-star to 5-star,
             the corresponding DDAG will be
 
                                                       1|5
+
                                  1|4                                       2|5
+
                        1|3                 2|4                   2|4                  3|5
+
                   1|2       2|3       2|3       3|4         2|3       3|4        3|4       4|5
+
                 1     2   2     3   2     3   3     4     2     3   3     4    3     4   4     5
 
             Since some subtrees are shared by different branches, for instance, the subtree labeled as node
-            2|4 is shared by the right subtree of 1|4 and the left subtree of 2|5, the tree can be depicted in a more
-            compact way:
+            2|4 is shared by the right subtree of 1|4 and the left subtree of 2|5, the tree can be depicted
+            in a more compact way:
+
                                                       1|5
+
                                               1|4             2|5
+
                                        1|3            2|4            3|5
+
                                  1|2          2|3             3|4           4|5
+
                              1          2              3              4             5
 
-            in which all internal nodes (2|4, 2|3 and 3|4) and all leaves, except the first one, and the last one
-            (2, 3 and 4) are reached from different paths.
+            in which all internal nodes (2|4, 2|3 and 3|4) and all leaves, except the first one, and 
+            the last one (2, 3 and 4) are reached from different paths.
 
 
         The class implements two different strategies to compute the probabilities for a given example:
 
         'full_probabilistic'
             The probabilities computed by each node are propagated through the tree. For those leaves that
             can be reached following different paths (all except the leaves for the first and the last class), the
             probabilities are summed. With this method, all the classes may have a probability greater that 0.
 
-            Example: For a given example, the probability of the left class returned by each model is the following:
-
-            P(1|5) = 0.2
-            P(1|4) = 0.1
-            P(2|5) = 0.1
-            P(1|3) = 0.2
-            P(2|4) = 0.3
-            P(3|5) = 0.3
-            P(1|2) = 0.3
-            P(2|3) = 0.4
-            P(3|4) = 0.4
-            P(4|5) = 0.3
-
-            P(y=1) = P(1|5) * P(1|4) * P(1|3) * P(1|2) =
-                     0.2    * 0.1    * 0.2    * 0.3    = 0.0012
-
-            P(y=2) = P(1|5)     * P(1|4)     * P(1|3)     * (1-P(1|2)) +
-                     P(1|5)     * P(1|4)     * (1-P(1|3)) * P(2|3)     +
-                     P(1|5)     * (1-P(1|4)) * P(2|4)     * P(2|3)     +
-                     (1-P(1|5)) * P(2|5)     * P(2|4)     * P(2|3)     =
-                     0.2        * 0.1        * 0.2        * 0.7        +
-                     0.2        * 0.1        * 0.8        * 0.4        +
-                     0.2        * 0.9        * 0.3        * 0.4        +
-                     0.8        * 0.1        * 0.3        * 0.4        = 0.0028 + 0.0064 + 0.0216 + 0.0096 = 0.0404
-
-            P(y=3) = P(1|5)     * P(1|4)     * (1-P(1|3)) * (1-P(2|3)) +
-                     P(1|5)     * (1-P(1|4)) * P(2|4))    * (1-P(2|3)) +
-                     P(1|5)     * (1-P(1|4)) * (1-P(2|4)) * P(3|4)     +
-                     (1-P(1|5)) * P(2|5)     * P(2|4))    * (1-P(2|3)) +
-                     (1-P(1|5)) * P(2|5)     * (1-P(2|4)) * P(3|4)     +
-                     (1-P(1|5)) * (1-P(2|5)) * P(3|5)     * P(3|4)     =
-                     0.2        * 0.1        * 0.8        * 0.6        +
-                     0.2        * 0.9        * 0.3        * 0.6        +
-                     0.2        * 0.9        * 0.7        * 0.4        +
-                     0.8        * 0.1        * 0.3        * 0.6        +
-                     0.8        * 0.1        * 0.7        * 0.4        +
-                     0.8        * 0.9        * 0.3        * 0.4        = 0.0096 + 0.0324 + 0.0504 +
-                                                                         0.0144 + 0.0224 + 0.0864 = 0.2156
-            P(y=4) = P(1|5)     * (1-P(1|4)) * (1-P(2|4)) * (1-P(3|4)) +
-                     (1-P(1|5)) * P(2|5)     * (1-P(2|4)) * (1-P(3|4)) +
-                     (1-P(1|5)) * (1-P(2|5)) * P(3|5)     * (1-P(3|4)) +
-                     (1-P(1|5)) * (1-P(2|5)) * (1-P(3|5)) * P(4|5)     =
-                     0.2        * 0.9        * 0.7        * 0.6        + 0.0756
-                     0.8        * 0.1        * 0.7        * 0.6        + 0.0336
-                     0.8        * 0.9        * 0.3        * 0.6        + 0.1296
-                     0.8        * 0.9        * 0.7        * 0.3        = 0.0756 + 0.0336 + 0.1296 + 0.1512 = 0.3900
+            Example: For a given example, the probability of the left class returned by each model is the following::
+            
+                P(1|5) = 0.2
+                P(1|4) = 0.1
+                P(2|5) = 0.1
+                P(1|3) = 0.2
+                P(2|4) = 0.3
+                P(3|5) = 0.3
+                P(1|2) = 0.3
+                P(2|3) = 0.4
+                P(3|4) = 0.4
+                P(4|5) = 0.3
+
+                P(y=1) = P(1|5) * P(1|4) * P(1|3) * P(1|2) =
+                         0.2    * 0.1    * 0.2    * 0.3    = 0.0012
+
+                P(y=2) = P(1|5)     * P(1|4)     * P(1|3)     * (1-P(1|2)) +
+                         P(1|5)     * P(1|4)     * (1-P(1|3)) * P(2|3)     +
+                         P(1|5)     * (1-P(1|4)) * P(2|4)     * P(2|3)     +
+                         (1-P(1|5)) * P(2|5)     * P(2|4)     * P(2|3)     =
+                         0.2        * 0.1        * 0.2        * 0.7        +
+                         0.2        * 0.1        * 0.8        * 0.4        +
+                         0.2        * 0.9        * 0.3        * 0.4        +
+                         0.8        * 0.1        * 0.3        * 0.4        = 
+                         0.0028 + 0.0064 + 0.0216 + 0.0096 = 0.0404
+
+                P(y=3) = P(1|5)     * P(1|4)     * (1-P(1|3)) * (1-P(2|3)) +
+                         P(1|5)     * (1-P(1|4)) * P(2|4))    * (1-P(2|3)) +
+                         P(1|5)     * (1-P(1|4)) * (1-P(2|4)) * P(3|4)     +
+                         (1-P(1|5)) * P(2|5)     * P(2|4))    * (1-P(2|3)) +
+                         (1-P(1|5)) * P(2|5)     * (1-P(2|4)) * P(3|4)     +
+                         (1-P(1|5)) * (1-P(2|5)) * P(3|5)     * P(3|4)     =
+                         0.2        * 0.1        * 0.8        * 0.6        +
+                         0.2        * 0.9        * 0.3        * 0.6        +
+                         0.2        * 0.9        * 0.7        * 0.4        +
+                         0.8        * 0.1        * 0.3        * 0.6        +
+                         0.8        * 0.1        * 0.7        * 0.4        +
+                         0.8        * 0.9        * 0.3        * 0.4        = 
+                         0.0096 + 0.0324 + 0.0504 + 0.0144 + 0.0224 + 0.0864 = 0.2156
+
+                P(y=4) = P(1|5)     * (1-P(1|4)) * (1-P(2|4)) * (1-P(3|4)) +
+                         (1-P(1|5)) * P(2|5)     * (1-P(2|4)) * (1-P(3|4)) +
+                         (1-P(1|5)) * (1-P(2|5)) * P(3|5)     * (1-P(3|4)) +
+                         (1-P(1|5)) * (1-P(2|5)) * (1-P(3|5)) * P(4|5)     =
+                         0.2        * 0.9        * 0.7        * 0.6        + 0.0756
+                         0.8        * 0.1        * 0.7        * 0.6        + 0.0336
+                         0.8        * 0.9        * 0.3        * 0.6        + 0.1296
+                         0.8        * 0.9        * 0.7        * 0.3        = 
+                         0.0756 + 0.0336 + 0.1296 + 0.1512 = 0.3900
 
-            P(y=5) = (1-P(1|5)) * (1-P(2|5)) * (1-P(3|5)) * (1-P(4|5)) =
-                     0.8        * 0.9        * 0.7        * 0.7        = 0.3528
+                P(y=5) = (1-P(1|5)) * (1-P(2|5)) * (1-P(3|5)) * (1-P(4|5)) =
+                         0.8        * 0.9        * 0.7        * 0.7        = 0.3528
 
-            Thus, the probabilities returned by `predict_proba` method would be (0.0012, 0.0404, 02156, 0.3900, 0.3528)
+                Thus, the probabilities returned by `predict_proba` method would be:
+                        (0.0012, 0.0404, 02156, 0.3900, 0.3528)
 
         'winner_node'
             Uses the probabilities of binary estimators to descent until the level previous to the leaves (it is like
             binarizing such probabilities to 0,1). Then, the method returns the probalities of such binary estimator
             for the two consecutive classes involved, and zero for the rest of classes.
 
-            Example: For a given example, the probability of the left class returned by each model is the following:
+            Example: For a given example, the probability of the left class returned by each model is the following::
 
-            P(1|5) = 0.2
-            P(1|4) = 0.1
-            P(2|5) = 0.1
-            P(1|3) = 0.2
-            P(2|4) = 0.3
-            P(3|5) = 0.3
-            P(1|2) = 0.3
-            P(2|3) = 0.4
-            P(3|4) = 0.4
-            P(4|5) = 0.3
+                P(1|5) = 0.2
+                P(1|4) = 0.1
+                P(2|5) = 0.1
+                P(1|3) = 0.2
+                P(2|4) = 0.3
+                P(3|5) = 0.3
+                P(1|2) = 0.3
+                P(2|3) = 0.4
+                P(3|4) = 0.4
+                P(4|5) = 0.3
 
-            Taking binary decisions from the root, we reach the binary classifier 4|5, thus the returned probabilities
-            are (0, 0, 0, 0.3, 0.7)
+                Taking binary decisions from the root, we reach the binary classifier 4|5, thus 
+                the returned probabilities are (0, 0, 0, 0.3, 0.7)
 
         Parameters
         ----------
         estimator : estimator object (default=None)
             An estimator object implementing `fit` and one of `predict` or `predict_proba`. It is the base estimator
             used to learn the set of binary classifiers
 
         n_jobs : int or None, optional (default=None)
             The number of jobs to use for the computation.
             ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-            ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
-            for more details.
+            ``-1`` means using all processors
 
         predict_method: str, optional (default 'full_probabilistic')
-            'full_probabilistic'
+            - 'full_probabilistic'
             The probabilities computed by each node are propagated through the tree. For those leaves that
             can be reached following different paths (all except the leaves for the first and the last class), the
             probabilities are summed. With this method, all the classes may have a probability greater that 0.
-
-            'winner_node'
+            
+            - 'winner_node'
             Uses the probabilities of binary estimators to descent until the level previous to the leaves (it is like
             binarizing such probabilities to 0,1). Then, the method returns the probalities of such binary estimator
             for the two consecutive classes involved, and zero for the rest of classes.
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
@@ -218,22 +232,22 @@
 
     def predict_proba(self, X):
         """ Predict the class probabilities for each example
 
             Two different methods are implemented depending on the value of `predict_method` attribute
 
             'full_probabilistic'
-            The probabilities computed by each node are propagated through the tree. For those leaves that
-            can be reached following different paths (all except the leaves for the first and the last class), the
-            probabilities are summed. With this method, all the classes may have a probability greater that 0.
+               The probabilities computed by each node are propagated through the tree. For those leaves that
+               can be reached following different paths (all except the leaves for the first and the last class), the
+               probabilities are summed. With this method, all the classes may have a probability greater that 0.
 
             'winner_node'
-            Uses the probabilities of binary estimators to descent until the level previous to the leaves (it is like
-            binarizing such probabilities to 0,1). Then, the method returns the probalities of such binary estimator
-            for the two consecutive classes involved, and zero for the rest of classes.
+               Uses the probabilities of binary estimators to descent until the level previous to the leaves (it is like
+               binarizing such probabilities to 0,1). Then, the method returns the probalities of such binary estimator
+               for the two consecutive classes involved, and zero for the rest of classes.
 
             The method uses a recursive auxiliar method to compute the class probabilities
 
             Parameters
             ----------
             X : (sparse) array-like, shape (n_examples, n_features)
                 Data
```

### Comparing `quantificationlib-0.0.7/quantificationlib/estimators/weighted_knn.py` & `quantificationlib-0.1.1/quantificationlib/estimators/weighted_knn.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,20 @@
         Parameters
         ----------
         n_neighbors : int, (default=10)
             Number of neighbors to use by default for :meth:`kneighbors` queries.
 
         algorithm : {'auto', 'ball_tree', 'kd_tree', 'brute'}, default='auto'
             Algorithm used to compute the nearest neighbors:
+            
             - 'ball_tree' will use :class:`BallTree`
             - 'kd_tree' will use :class:`KDTree`
-            - 'brute' will use a brute-force search.
-            - 'auto' will attempt to decide the most appropriate algorithm
-              based on the values passed to :meth:`fit` method.
-            Note: fitting on sparse input will override the setting of
-            this parameter, using brute force.
+            - 'brute' will use a brute-force search
+            - 'auto' will attempt to decide the most appropriate algorithm based on the values passed to :meth:`fit` method.
+            Note: fitting on sparse input will override the setting of this parameter, using brute force.
 
         leaf_size : int, default=30
             Leaf size passed to BallTree or KDTree.  This can affect the
             speed of the construction and query, as well as the memory
             required to store the tree.  The optimal value depends on the
             nature of the problem.
```

### Comparing `quantificationlib-0.0.7/quantificationlib/metrics/binary.py` & `quantificationlib-0.1.1/quantificationlib/metrics/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import numpy as np
 
 
 def binary_kld(p_true, p_pred, eps=1e-12):
     """ A binary version of the Kullback - Leiber divergence (KLD)
 
-            :math:`kld = p \cdot \log(p/\hat{p}) + (1-p) \cdot \log((1-p)/(1-\hat{p}))
+            :math:`kld = p \cdot \log(p/\hat{p}) + (1-p) \cdot \log((1-p)/(1-\hat{p}))`
 
         Parameters
         ----------
         p_true : array_like, shape = (n_classes)
             True prevalences
 
         p_pred : array_like, shape = (n_classes)
```

### Comparing `quantificationlib-0.0.7/quantificationlib/metrics/multiclass.py` & `quantificationlib-0.1.1/quantificationlib/metrics/multiclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 def kld(p_true, p_pred, eps=1e-12):
     """ Kullback - Leiber divergence (KLD)
 
             :math:`kld = \sum_{j=1}^{j=l} p_j \cdot \log{p_j/\hat{p}_j}`
 
-        being l the number of classes.
+        being `l` the number of classes.
 
         Also known as discrimination information, relative entropy or normalized cross-entropy
         (see [Esuli and Sebastiani 2010; Forman 2008]).
         KLD is a special case of the family of f-divergences
 
         Parameters
         ----------
@@ -84,15 +84,15 @@
 
 
 def mean_absolute_error(p_true, p_pred):
     """ Mean absolute error
 
             :math:`mae = 1/l \sum_{j=1}^{j=l} | p_j - \hat{p}_j |`
 
-        being l the number of classes
+        being `l` the number of classes
 
         Parameters
         ----------
         p_true : array_like, shape = (n_classes)
             True prevalences
 
         p_pred : array_like, shape = (n_classes)
@@ -108,15 +108,15 @@
 
 
 def l1(p_true, p_pred):
     """ L1 loss function
 
             :math:`l1 = \sum_{j=1}^{j=l} | p_j - \hat{p}_j |`
 
-        being l the number of classes
+        being `l` the number of classes
 
         Parameters
         ----------
         p_true : array_like, shape = (n_classes)
             True prevalences
 
         p_pred : array_like, shape = (n_classes)
@@ -132,15 +132,15 @@
 
 
 def mean_squared_error(p_true, p_pred):
     """ Mean squared error
 
             :math:`mse = 1/l \sum_{j=1}^{j=l} (p_j - \hat{p}_j)^2`
 
-        being l the number of classes
+        being `l` the number of classes
 
         Parameters
         ----------
         p_true : array_like, shape = (n_classes)
             True prevalences
 
         p_pred : array_like, shape = (n_classes)
@@ -156,15 +156,15 @@
 
 
 def l2(p_true, p_pred):
     """ L2 loss function
 
             :math:`l2 = \sqrt{\sum_{j=1}^{j=l} (p_j - \hat{p}_j)^2}`
 
-        being l the number of classes
+        being `l`  the number of classes
 
         Parameters
         ----------
         p_true : array_like, shape = (n_classes)
             True prevalences
 
         p_pred : array_like, shape = (n_classes)
@@ -180,15 +180,15 @@
 
 
 def hd(p_true, p_pred):
     """ Hellinger distance (HD)
 
             :math:`hd = \sqrt{\sum_{j=1}^{j=l} (\sqrt{p_j} - \sqrt{\hat{p}_j}}`
 
-        being l the number of classes
+        being `l` the number of classes
 
         Parameters
         ----------
         p_true : array_like, shape = (n_classes)
             True prevalences
 
         p_pred : array_like, shape = (n_classes)
@@ -216,15 +216,15 @@
             Predicted prevalences. In case of binary quantification, this parameter could be a single float value.
         """
     p_true, p_pred = check_prevalences(p_true, p_pred)
     return np.sum(np.abs(p_true - p_pred)) / np.sum(p_true + p_pred)
 
 
 def topsoe(p_true, p_pred, epsilon=1e-20):
-    """ Topsoe
+    """ Topsoe distance
     """
     p_true, p_pred = check_prevalences(p_true, p_pred)
     dist = np.sum(p_true*np.log((2*p_true+epsilon)/(p_true+p_pred+epsilon)) +
                   p_pred*np.log((2*p_pred+epsilon)/(p_true+p_pred+epsilon)))
     return dist
 
 
@@ -234,15 +234,15 @@
     p_true, p_pred = check_prevalences(p_true, p_pred)
     dist = np.sum(p_true*np.log(p_true+epsilon)+p_pred*np.log(p_pred+epsilon)-
                   (p_true+p_pred)*np.log((p_true+p_pred+epsilon)/2))/2
     return dist
 
 
 def probsymmetric(p_true, p_pred, epsilon=1e-20):
-    """ Probabilistic Symmetric
+    """ Probabilistic Symmetric distance
     """
     p_true, p_pred = check_prevalences(p_true, p_pred)
     dist = 2*np.sum((p_true-p_pred)**2 / (p_pred+p_true+epsilon))
     return dist
 
 
 def brier_multi(targets, probs):
```

### Comparing `quantificationlib-0.0.7/quantificationlib/metrics/ordinal.py` & `quantificationlib-0.1.1/quantificationlib/metrics/ordinal.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from sklearn.metrics.pairwise import check_pairwise_arrays
 
 from quantificationlib.metrics.multiclass import check_prevalences
 
 
 def emd(p_true, p_pred):
-    """ Return the EMD distances between two sets of prevalences
+    """ Return the EMD distance between two sets of prevalences
 
         Parameters
         ----------
         p_true: array-like, shape (n_classes, 1)
 
         p_pred: array-like, shape (n_classes, 1)
 
@@ -31,21 +31,41 @@
     """
     p_true, p_pred = check_prevalences(p_true, p_pred)
     return np.sum(np.abs(np.cumsum(p_true - p_pred)))
     # return sum([abs(sum(p_pred[:j+1]) - sum(p_true[:j+1])) for j in range(len(p_true)-1)])
 
 
 def emd_score(p_true, p_pred):
+    """ Scoring metric based on EMD distance
+    
+        References
+        ----------
+        Castaño, A., González, P., González, J. A., & Del Coz, J. J. (2022). Matching Distributions Algorithms
+        Based on the Earth Mover’s Distance for Ordinal Quantification.  IEEE Transactions on Neural Networks
+        and Learning Systems.
+        
+        Parameters
+        ----------
+        p_true: array-like, shape (n_classes, 1)
+
+        p_pred: array-like, shape (n_classes, 1)
+
+        Return
+        ------
+        emds: float, the EMD score
+    """
+        
     p_true, p_pred = check_prevalences(p_true, p_pred)
     left_mass = np.zeros_like(p_true)
     left_mass[0] = 1
     right_mass = np.zeros_like(p_true)
     right_mass[-1] = 1
     max_emd = max(emd(p_true, left_mass), emd(p_true, right_mass))
-    return (max_emd - np.sum(np.abs(np.cumsum(p_true - p_pred)))) / max_emd
+    emds = (max_emd - np.sum(np.abs(np.cumsum(p_true - p_pred)))) / max_emd
+    return emds
 
 
 def emd_distances(A, B):
     """ Return the EMD distances between the rows of A and B
 
         Parameters
         ----------
@@ -54,14 +74,15 @@
         B: array-like, shape (n_samples_2, n_features)
 
         A and B should have the same number of columns
 
         Return
         ------
         distances : array, shape (n_samples_1, n_samples_2)
+
     """
     # version #1: the most inefficient
     # return np.sum(np.abs(np.cumsum(A[:, np.newaxis] - B, axis=2)), axis=2)
 
     # version #2: this is more efficient that version#1 but a little bit worse than version#3
     # differences = A[:, 0].reshape(-1, 1) - B[:, 0].reshape(-1, 1).T
     # distances = np.abs(differences)
```

### Comparing `quantificationlib-0.0.7/quantificationlib/multiclass/df.py` & `quantificationlib-0.1.1/quantificationlib/multiclass/df.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,53 +52,54 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         distribution_function : str, (default='PDF')
             Type of distribution function used. Two types are supported 'CDF' and 'PDF'
 
         n_bins : int  (default=8)
             Number of bins to compute the CDFs/PDFs
 
         bin_strategy : str (default='norm')
             Method to compute the boundaries of the bins:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                          (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+                - 'equal_width': bins of equal length (it could be affected by outliers)
+                - 'equal_count': bins of equal counts (considering the examples of all classes)
+                - 'binormal': (Only for binary quantification) 
+                          It is inspired on the method devised by (Tasche, 2019, Eq (A16b)). The cut points, 
+                          :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                           are computed as follows based on the assumption that the features follow a normal distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                          :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                          where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                          and $\sigma$ of the normal distribution are estimated as the average of those values for
+                          where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                          and :math:`\\sigma` of the normal distribution are estimated as the average of those values for
                           the training examples of each class.
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
-                           estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
+                - 'normal': The idea is that each feacture follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
+                          estimated as the weighted mean and std from the training distribution. The cut points
+                          :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                          :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         distance : str, representing the distance function (default='HD')
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution
 
         tol : float, (default=1e-05)
             The precision of the solution when search is used to compute the prevalence
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimator_train and estimator_test could be the same
 
         Attributes
         ----------
         classes_ : ndarray, shape (n_classes, )
             Class labels
 
         estimator_train : estimator
@@ -408,31 +409,32 @@
             Type of distribution function used. Two types are supported 'CDF' and 'PDF'
 
         n_bins : int
             Number of bins to compute the PDFs
 
         bin_strategy : str (default='norm')
             Method to compute the boundaries of the bins:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                          (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+                - 'equal_width': bins of equal length (it could be affected by outliers)
+                - 'equal_count': bins of equal counts (considering the examples of all classes)
+                - 'binormal': (Only for binary quantification) 
+                          It is inspired on the method devised by (Tasche, 2019, Eq (A16b)). The cut points,
+                          :math:`-\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                           are computed as follows based on the assumption that the features follow a normal distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                          :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                          where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                          and $\sigma$ of the normal distribution are estimated as the average of those values for
+                          where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                          and :math:`\sigma` of the normal distribution are estimated as the average of those values for
                           the training examples of each class.
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
+                - 'normal': The idea is that each feacture follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
                            estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
+                           :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                           :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         distance : str, representing the distance function (default='HD')
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution
 
         tol : float, (default=1e-05)
             The precision of the solution when search is used to compute the prevalence
@@ -655,32 +657,32 @@
             Class labels
 
         n_bins : int, (default=8)
             Number of bins
 
         bin_strategy : str (default='equal_width')
             Method to compute the boundaries of the bins:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                          (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+                - 'equal_width': bins of equal length (it could be affected by outliers)
+                - 'equal_count': bins of equal counts (considering the examples of all classes)
+                - 'binormal': (Only for binary quantification) 
+                          It is inspired on the method devised by (Tasche, 2019, Eq (A16b)). The cut points, 
+                          :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                           are computed as follows based on the assumption that the features follow a normal distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                          :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                          where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                          and $\sigma$ of the normal distribution are estimated as the average of those values for
+                          where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                          and :math:`\\sigma` of the normal distribution are estimated as the average of those values for
                           the training examples of each class.
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
+                - 'normal': The idea is that each feacture follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
                            estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
-
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                           :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
+                           :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         att_range: array-like, (2,1)
             Min and Max possible values of the input feature x. These values might not coincide with the actual Min and
             Max values of vector x. For instance, in the case of x represents a set of probabilistic predictions, these
             values will be 0 and 1
 
         Returns
```

### Comparing `quantificationlib-0.0.7/quantificationlib/multiclass/em.py` & `quantificationlib-0.1.1/quantificationlib/multiclass/em.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,27 +27,27 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
         epsilon: float, (default=1e-04)
             EM algorithm (its loop) stops when the difference between the prevalences of two
             consecutive iterations is lower than epsilon
 
         max_iter: int (default=1000)
             The maximum number of iterations for the loop of the EM algorithm
 
-        For some experiments both estimator_train and estimator_test could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
```

### Comparing `quantificationlib-0.0.7/quantificationlib/multiclass/energy.py` & `quantificationlib-0.1.1/quantificationlib/multiclass/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,23 +44,23 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         distance : distance function (default=manhattan_distances)
             It is the function used to compute the distance between every pair of examples
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimator_train and estimator_test could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
@@ -250,24 +250,24 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         distance : distance function (default=manhattan_distances)
             It is the function used to compute the distance between every pair of examples
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimator_train and estimator_test could be the same
-
+            
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
             Estimator used to classify the examples of the testing bag
```

### Comparing `quantificationlib-0.0.7/quantificationlib/multiclass/friedman.py` & `quantificationlib-0.1.1/quantificationlib/multiclass/friedman.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """ Multiclass Mixture Estimation method proposed by Friedman
 
         This class works in two different ways:
 
         1) Two estimators are used to classify the examples of the training set and the testing set in order to
            compute the (probabilistic) confusion matrix of both sets. Estimators can be already trained
 
-        2) You can directly provide the predictions for the examples in the `fit`/`predict methods. This is useful
+        2) You can directly provide the predictions for the examples in the `fit`/`predict` methods. This is useful
            for synthetic/artificial experiments
 
         The idea in both cases is to guarantee that all methods based on distribution matching are using **exactly**
         the same predictions when you compare this kind of quantifiers (and others that also employ an underlying
         classifier, for instance, CC/PCC). In the first case, estimators are only trained once and can be shared
         for several quantifiers of this kind
 
@@ -36,27 +36,27 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the confusion matrix
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to obtain the confusion matrix of the testing set
+            testing set and to obtain the confusion matrix of the testing set.
+            For some experiments both estimators could be the same
 
         distance : str, representing the distance function (default='L2')
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution
 
         tol : float, (default=1e-05)
             The precision of the solution when search is used to compute the prevalence
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
@@ -145,15 +145,15 @@
         self.b_ = None
         self.problem_ = None
         self.mixtures_ = None
 
     def fit(self, X, y, predictions_train=None):
         """ This method performs the following operations: 1) fits the estimators for the training set and the
             testing set (if needed), and 2) computes predictions_train_ (probabilities) if needed. Both operations are
-            performed by the `fit method of its superclass.
+            performed by the `fit` method of its superclass.
             Then, the method computes the training distribution of the method ME suggested by Friedman. The distribution
             of a class contains the percentage of the training examples of that class whose probability to belong
             to each class is >= than the prevalence of such class in the training set
             Finally, the method computes all the parameters for solving the optimization problem needed by quadprog
             that do not need the testing distribution
 
             Parameters
@@ -203,15 +203,15 @@
 
         return self
 
     def predict(self, X, predictions_test=None):
         """ Predict the class distribution of a testing bag
 
             First, predictions_test_ are computed (if needed, when predictions_test parameter is None) by
-            `super().predict() method.
+            `super().predict()` method.
 
             After that, the method computes the distribution of the FriedmanME method for the testing bag. That is,
             the percentage of examples in the testing bag whose probability to belong each class is >= than
             the prevalence of that class in the training set
 
             Finally, the prevalences are computed solving the resulting optimization problem
```

### Comparing `quantificationlib-0.0.7/quantificationlib/multiclass/knn.py` & `quantificationlib-0.1.1/quantificationlib/multiclass/knn.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/quantificationlib/multiclass/regression.py` & `quantificationlib-0.1.1/quantificationlib/multiclass/regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,32 +28,33 @@
             Object to generate the bags with a selected shift
 
         n_bins : int (default=8)
             Number of bins to compute the PDF of each distribution
 
         bin_strategy : str (default='normal')
             Method to compute the boundaries of the bins:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                            (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+                - 'equal_width': bins of equal length (it could be affected by outliers)
+                - 'equal_count': bins of equal counts (considering the examples of all classes)
+                - 'binormal': (Only for binary quantification) 
+                            It is inspired on the method devised by (Tasche, 2019, Eq (A16b)). the cut points,
+                            :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                             are computed as follows based on the assumption that the features follow a normal
                             distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                            :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                            where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                            and $\sigma$ of the normal distribution are estimated as the average of those values for
+                            where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                            and :math:`\\sigma` of the normal distribution are estimated as the average of those values for
                             the training examples of each class.
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
+                - 'normal':  The idea is that each feature follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
                            estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
+                           :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                           :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         regression_estimator: estimator object (default=None)
             A regression estimator object. If the value is None the regression estimator used is a Generalized Linear
             Model (GLM) from statsmodels package with logit link and Binomial family as parameters (see Baum 2008).
             It is used to learn a regression model able to predict the prevalence for each class, so the method will
             fit as many regression estimators as classes in multiclass problems and just one for binary problems.
 
@@ -250,32 +251,33 @@
             Object to generate the bags with a selected shift
 
         n_bins : int (default=8)
             Number of bins to compute the PDF of each distribution
 
         bin_strategy : str (default='normal')
             Method to compute the boundaries of the bins:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                            (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+                - 'equal_width': bins of equal length (it could be affected by outliers)
+                - 'equal_count': bins of equal counts (considering the examples of all classes)
+                - 'binormal': (Only for binary quantification) 
+                            It is inspired on the method devised by (Tasche, 2019, Eq (A16b)). the cut points,
+                            :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                             are computed as follows based on the assumption that the features follow a normal
                             distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                            :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                            where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                            and $\sigma$ of the normal distribution are estimated as the average of those values for
+                            where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                            and :math:`\\sigma` of the normal distribution are estimated as the average of those values for
                             the training examples of each class.
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
+                - 'normal':  The idea is that each feacture follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
                            estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
+                           :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                           :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         regression_estimator: estimator object (default=None)
             A regression estimator object. If the value is None the regression estimator used is a Generalized Linear
             Model (GLM) from statsmodels package with logit link and Binomial family as parameters (see Baum 2008).
             It is used to learn a regression model able to predict the prevalence for each class, so the method will
             fit as many regression estimators as classes in multiclass problems and just one for binary problems.
 
@@ -418,33 +420,34 @@
         bag_generator : BagGenerator object (default=PriorShift_BagGenerator())
             Object to generate the bags with a selected shift
 
         n_bins : int (default=8)
             Number of bins to compute the PDF of each distribution
 
         bin_strategy : str (default='normal')
-            Method to compute the boundaries of the bins:
-                'equal_width': bins of equal length (it could be affected by outliers)
-                'equal_count': bins of equal counts (considering the examples of all classes)
-                'binormal': (Only for binary quantification) It is inspired on the method devised by
-                            (Tasche, 2019, Eq (A16b)). the cut points, $-\infty < c_1 < \ldots < c_{b-1} < \infty$,
+            Method to compute the boundaries of the bins
+                - 'equal_width': bins of equal length (it could be affected by outliers)
+                - 'equal_count': bins of equal counts (considering the examples of all classes)
+                - 'binormal': (Only for binary quantification) 
+                            It is inspired on the method devised by (Tasche, 2019, Eq (A16b)). the cut points,
+                            :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty`,
                             are computed as follows based on the assumption that the features follow a normal
                             distribution:
 
-                          $c_i = \frac{\sigma^+ + \sigma^{-}}{2} \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \frac{\mu^+ + \mu^{-}}{2} ,  \quad i=1,\ldots,b-1$
+                            :math:`c_i = \\frac{\\sigma^+ + \\sigma^{-}}{2} \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\frac{\\mu^+ + \\mu^{-}}{2} ,  \\quad i=1,\\ldots,b-1`
 
-                            where $\Phi^{-1}$ is the quantile function of the standard normal distribution, and $\mu$
-                            and $\sigma$ of the normal distribution are estimated as the average of those values for
+                            where :math:`\\Phi^{-1}` is the quantile function of the standard normal distribution, and :math:`\\mu`
+                            and :math:`\\sigma` of the normal distribution are estimated as the average of those values for
                             the training examples of each class.
 
-                'normal':  The idea is that each feacture follows a normal distribution. $\mu$ and $\sigma$ are
+                - 'normal':  The idea is that each feacture follows a normal distribution. :math:`\\mu` and :math:`\\sigma` are
                            estimated as the weighted mean and std from the training distribution. The cut points
-                           $-\infty < c_1 < \ldots < c_{b-1} < \infty$ are computed as follows:
+                           :math:`-\\infty < c_1 < \\ldots < c_{b-1} < \\infty` are computed as follows:
 
-                           $c_i = \sigma^ \ \Phi^{-1}\bigg(\frac{i}{b}\bigg)  + \mu ,  \quad i=1,\ldots,b-1$
+                           :math:`c_i = \\sigma^ \\ \\Phi^{-1}\\bigg(\\frac{i}{b}\\bigg)  + \\mu ,  \\quad i=1,\\ldots,b-1`
 
         regression_estimator: estimator object (default=None)
             A regression estimator object. If it is None the regression estimator used is a Generalized Linear
             Model (GLM) from statsmodels package with logit link and Binomial family as parameters.
             It is used to learn a regression model able to predict the prevalence for each class, so the method will
             fit as many regression estimators as classes in multiclass problem and just one for binary problems.
```

### Comparing `quantificationlib-0.0.7/quantificationlib/optimization.py` & `quantificationlib-0.1.1/quantificationlib/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,31 +16,32 @@
 import scipy
 
 
 ############
 #  Functions for solving optimization problems using CVXPY, loss functions: L1, HD
 ############
 def solve_l1(train_distrib, test_distrib, n_classes, problem=None, solver=None):
-    """ Solves AC, PAC, PDF and Friedman optimization problems for L1 loss function
+    """ Solves AC, PAC, DF and Friedman optimization problems for L1 loss function
 
-        min   |train_distrib * prevalences - test_distrib|
-        s.t.  prevalences_i >=0
-              sum prevalences_i = 1
+            min   |train_distrib * prevalences - test_distrib|      \n
+            s.t.  prevalences_i >=0, sum prevalences_i = 1
 
         Parameters
         ----------
         train_distrib : array, shape depends on the optimization problem
             Represents the distribution of each class in the training set
-            PDF: shape (n_bins * n_classes, n_classes)
-            AC, PAC, Friedman: shape (n_classes, n_classes)
+            
+            - DF: shape (n_bins * n_classes, n_classes)
+            - AC, PAC, Friedman: shape (n_classes, n_classes)
 
         test_distrib : array, shape depends on the optimization problem
             Represents the distribution of the testing set
-            PDF: shape shape (n_bins * n_classes, 1)
-            AC, PAC, Friedman: shape (n_classes, 1)
+            
+            - DF: shape shape (n_bins * n_classes, 1)
+            - AC, PAC, Friedman: shape (n_classes, 1)
 
         n_classes : int
             Number of classes
 
         problem : a cvxpy Problem object (default=None)
             The first time a problem is solved (this corresponds to the first testing bag) this parameter is None. For
             the rest testing bags, a Problem object is passed here to allow a warm start. This accelerates the solving
@@ -80,15 +81,15 @@
         else:
             problem.solve(warm_start=True, solver=solver)
 
         return problem, list(problem.solution.primal_vars.values())[0]
 
 
 def solve_hd(train_distrib, test_distrib, n_classes, problem=None, solver='ECOS'):
-    """ Solves the optimization problem for PDF methods using Hellinger Distance
+    """ Solves the optimization problem for DF methods using Hellinger Distance
 
         This method just uses cvxpy library
 
         Parameters
         ----------
         train_distrib : array, shape (n_bins * n_classes, n_classes)
             Represents the distribution of each class in the training set
@@ -102,15 +103,15 @@
         problem : a cvxpy Problem object (default=None)
             The first time a problem is solved (this corresponds to the first testing bag) this parameter is None. For
             the rest testing bags, a Problem object is passed here to allow a warm start. This accelerates the solving
             process.
 
         solver : str, (default='ECOS')
             The solver used to solve the optimization problem. Here 'ECOS' is used. If another solver is prefered,
-            you may need to install additional libraries
+            you may need to install additional libraries.
 
         Returns
         -------
         prevalences : array, shape=(n_classes, )
             Vector containing the predicted prevalence for each class
     """
     if problem is None:
@@ -131,107 +132,117 @@
         return problem, list(problem.solution.primal_vars.values())[0]
 
 
 ############
 #  Functions for solving optimization problems using QUADPROG (L2 loss function)
 ############
 def solve_l2(train_distrib, test_distrib, G, C, b):
-    """ Solves AC, PAC, PDF and Friedman optimization problems for L2 loss function
+    """ Solves AC, PAC, DF and Friedman optimization problems for L2 loss function
 
-        min    (test_distrib - train_distrib * prevalences).T (test_distrib - train_distrib * prevalences)
-        s.t.   prevalences_i >=0
-               sum prevalences_i = 1
+            min    (test_distrib - train_distrib * prevalences).T * (test_distrib - train_distrib * prevalences) \n
+            s.t.   prevalences_i >=0,  sum prevalences_i = 1
 
         Expanding the objective function, we obtain:
 
-        prevalences.T train_distrib.T train_distrib prevalences
-        - 2 prevalences train_distrib.T test_distrib + test_distrib.T test_distrib
+            `prevalences.T * train_distrib.T * train_distrib * prevalences`                       \n
+            `- 2 * prevalences * train_distrib.T * test_distrib + test_distrib.T * test_distrib`
 
         Notice that the last term is constant w.r.t prevalences.
 
-        Let G = 2 train_distrib.T train_distrib  and a = 2 * train_distrib.T test_distrib, we can use directly
+        Let `G = 2 * train_distrib.T * train_distrib`  and `a = 2 * train_distrib.T * test_distrib`, we can use directly
         quadprog.solve_qp because it solves the following kind of problems:
 
-        Minimize     1/2 x^T G x - a^T x
-        Subject to   C.T x >= b
+            Minimize     1/2 x^T G x - a^T x    \n
+            Subject to   C.T x >= b
 
-        `solve_l2` just computes the term a, shape (n_classes,1), and then calls quadprog.solve_qp.
-        G, C and b were computed by `compute_l2_param_train` before, in the 'fit' method` of the PDF/Friedman object.
+        `solve_l2` just computes the term a, shape (n_classes,1), and then calls `quadprog.solve_qp`.
+        G, C and b were computed by `compute_l2_param_train` before, in the `fit` method of the DF/Friedman object.
         quadprog is used here because it is faster than cvxpy.
 
         Parameters
         ----------
         train_distrib : array, shape depends on the optimization problem
             Represents the distribution of each class in the training set
-            PDF: shape (n_bins * n_classes, n_classes)
-            AC, PAC Friedman: shape (n_classes, n_classes)
+
+            - DF: shape (n_bins * n_classes, n_classes)
+            - AC, PAC Friedman: shape (n_classes, n_classes)
 
         test_distrib : array, shape depends on the optimization problem
             Represents the distribution of the testing set
-            PDF: shape shape (n_bins * n_classes, 1)
-            AC, PAC, Friedman: shape (n_classes, 1)
+
+            - DF: shape shape (n_bins * n_classes, 1)
+            - AC, PAC, Friedman: shape (n_classes, 1)
 
         G : array, shape (n_classes, n_classes)
 
         C : array, shape (n_classes, n_constraints)
             n_constraints will be n_classes + 1
 
         b : array, shape (n_constraints,)
 
-        G, C and b are computed by `compute_l2_param_train` in the 'fit' method
-
         Returns
         -------
         prevalences : array, shape=(n_classes, )
            Vector containing the predicted prevalence for each class
+
+        Notes
+        -----
+        G, C and b are computed by `compute_l2_param_train` in the 'fit' method
+
     """
     a = 2 * train_distrib.T.dot(test_distrib)
     a = np.squeeze(a)
     prevalences = quadprog.solve_qp(G=G, a=a, C=C, b=b, meq=1)
     return prevalences[0]
 
 
 def compute_l2_param_train(train_distrib, classes):
-    """ Computes params related to the train distribution for solving PDF optimization problems using
-        L2 loss function
+    """ Computes params related to the train distribution for solving QP using L2 loss function. 
+        For instance, this library  uses quadprog.solve_qp that solves the following kind of problems::
+
+            Minimize     1/2 x^T G x - a^T x
+            Subject to   C.T x >= b
+
+            Thus, the values of G, C and b must be the following
+
+            G = train_distrib.T * train_distrib
+            G shape (n_classes, n_classes)
+
+            C = [[ 1, 1, ...,  1],
+                 [ 1, 0, ...,  0],
+                 [ 0, 1, 0,.., 0],
+                 ...
+                 [ 0, 0, ..,0, 1]].T
+            C shape (n_classes+1, n_classes)
+            
+            b = [1, 0, ..., 0]
+            b shape (n_classes, )        
+
+            This function computes and returns G, C and b.
 
         Parameters
         ----------
         train_distrib : array, shape (n_bins * n_classes, n_classes)
             Represents the distribution of each class in the training set
 
         classes : ndarray, shape (n_classes, )
             Class labels
 
         Returns
         -------
         G : array, shape (n_classes, n_classes)
 
-        C : array, shape (n_classes, n_constraints)
-            n_constraints will be n_classes + 1  (n_classes constraints to guarantee that prevalences_i>=0, and
-            an additional constraints for ensuring that sum(prevalences)==1
-
-        b : array, shape (n_constraints,)
+        C : array, shape (n_classes, n_classes+1)
+            The number of columns is equal to the number of the constraints of the optimization 
+            problem. It must be n_classes + 1: n_classes constraints to guarantee that 
+            prevalences_i>=0, and an additional constraint for ensuring that sum(prevalences)==1
 
-        quadprog.solve_qp solves the following kind of problems:
+        b : array, shape (n_classes + 1,)
+            The size of b corresponds to the number of constraints of the optimization problem.
 
-        Minimize     1/2 x^T G x  a^T x
-        Subject to   C.T x >= b
-
-        Thus, the values of G, C and b must be the following
-
-        G = train_distrib.T train_distrib
-        C = [[ 1, 1, ...,  1],
-             [ 1, 0, ...,  0],
-             [ 0, 1, 0,.., 0],
-             ...
-             [ 0, 0, ..,0, 1]].T
-        C shape (n_classes+1, n_classes)
-        b = [1, 0, ..., 0]
-        b shape (n_classes, )
     """
     G = 2 * train_distrib.T.dot(train_distrib)
     if not is_pd(G):
         G = nearest_pd(G)
     #  constraints, sum prevalences = 1, every prevalence >=0
     n_classes = len(classes)
     C = np.vstack([np.ones((1, n_classes)), np.eye(n_classes)]).T
@@ -248,16 +259,16 @@
 
         A Python/Numpy port of John D'Errico's `nearestSPD` MATLAB code [1], which credits [2].
 
         References
         ----------
         [1] https://www.mathworks.com/matlabcentral/fileexchange/42885-nearestspd
 
-        [2] N.J. Higham, "Computing a nearest symmetric positive semidefinite
-        matrix" (1988): https://doi.org/10.1016/0024-3795(88)90223-6
+        [2] N.J. Higham, "Computing a nearest symmetric positive semidefinite matrix" (1988):
+            https://doi.org/10.1016/0024-3795(88)90223-6
     """
     B = (A + A.T) / 2
     _, s, V = np.linalg.svd(B)
 
     H = np.dot(V.T, np.dot(np.diag(s), V))
 
     A2 = (B + H) / 2
@@ -296,20 +307,22 @@
         Parameters
         ----------
         m : symmetric matrix, typically the shape is (n_classes, n_classes)
             The matrix to be factored. Only the diagonal and upper triangle are used
 
         Returns
         -------
-        k : int,
-            == 0  m is positive definite and the factorization has been completed
-            >  0  the leading minor of order k is not positive definite
+        k : int, 
+            This value is:
+
+            == 0  if m is positive definite and the factorization has been completed  \n
+            >  0  when the leading minor of order k is not positive definite
 
         r : array, an upper triangular matrix
-            When k==0, the factorization is complete and r.T.dot(r) == m
+            When k==0, the factorization is complete and `r.T.dot(r) == m`.
             The strict lower triangle is unaltered (it is equal to the strict lower triangle of matrix m), so it
             could be different from 0.
    """
     r = np.array(m, copy=True)
     n = len(r)
     for k in range(n):
         s = 0.0
@@ -365,21 +378,23 @@
         C : array, shape (n_classes, n_constraints)
             n_constraints will be n_classes + 1
 
         b : array, shape (n_constraints,)
 
         a : array, shape (n_classes, )
 
-        G, C and b are computed by `compute_ed_param_train` and a by `compute_ed_param_test`
-
         Returns
         -------
         prevalences : array, shape=(n_classes, )
            Vector containing the predicted prevalence for each class
 
+        Notes
+        -----   
+        G, C and b are computed by `compute_ed_param_train` and a by `compute_ed_param_test`
+        
         References
         ----------
         Alberto Castaño, Laura Morán-Fernández, Jaime Alonso, Verónica Bolón-Canedo, Amparo Alonso-Betanzos,
         Juan José del Coz: An analysis of quantification methods based on matching distributions
 
         Hideko Kawakubo, Marthinus Christoffel Du Plessis, and Masashi Sugiyama. 2016. Computationally efficient
         class-prior estimation under class balance change using energy distance. Transactions on Information
@@ -416,16 +431,14 @@
         G : array, shape (n_classes - 1, n_classes - 1)
 
         C : array, shape (n_classes - 1, n_constraints)
             n_constraints will be equal to the number of classes (n_classes)
 
         b : array, shape (n_constraints,)
 
-        See references below for further details
-
         References
         ----------
         Alberto Castaño, Laura Morán-Fernández, Jaime Alonso, Verónica Bolón-Canedo, Amparo Alonso-Betanzos,
         Juan José del Coz: An analysis of quantification methods based on matching distributions
 
         Hideko Kawakubo, Marthinus Christoffel Du Plessis, and Masashi Sugiyama. 2016. Computationally efficient
         class-prior estimation under class balance change using energy distance. Transactions on Information
@@ -486,16 +499,15 @@
             The number of examples of each class
 
         Returns
         -------
         a : array, shape (n_classes, )
             Term a for solving optimization problems using `quadprog.solve_qp`
 
-        See references below for further details
-
+   
         References
         ----------
         Alberto Castaño, Laura Morán-Fernández, Jaime Alonso, Verónica Bolón-Canedo, Amparo Alonso-Betanzos,
         Juan José del Coz: An analysis of quantification methods based on matching distributions
 
         Hideko Kawakubo, Marthinus Christoffel Du Plessis, and Masashi Sugiyama. 2016. Computationally efficient
         class-prior estimation under class balance change using energy distance. Transactions on Information
```

### Comparing `quantificationlib-0.0.7/quantificationlib/ordinal/ac_ordinal.py` & `quantificationlib-0.1.1/quantificationlib/ordinal/ac_ordinal.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         confusion matrix) and the prevalences observed in the testing distribution using the CC method.
 
         This class works in two different ways:
 
         1) Two estimators are used to classify the examples of the training set and the testing set in order to
            compute the confusion matrix of both sets. Estimators can be already trained
 
-        2) You can directly provide the predictions for the examples in the `fit`/`predict methods. This is useful
+        2) You can directly provide the predictions for the examples in the `fit`/`predict` methods. This is useful
            for synthetic/artificial experiments
 
         The idea in both cases is to guarantee that all methods based on distribution matching are using **exactly**
         the same predictions when you compare this kind of quantifiers (and others that also employ an underlying
         classifier, for instance, PDFyOrdinal). In the first case, estimators are only trained once and can be shared
         for several quantifiers of this kind
 
@@ -40,20 +40,19 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict`. It is used to classify the examples of the training
             set and to compute the confusion matrix
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict`. It is used to classify the examples of the testing
-            set and to obtain their predictions
+            set and to obtain their predictions. For some experiments both estimators could be the same
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimators could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
@@ -132,15 +131,15 @@
                 Data
 
             y : array-like, shape (n_examples, )
                 True classes
 
             predictions_train : ndarray, shape (n_examples, ) or (n_examples, n_classes)
                 Predictions of the examples in the training set. If shape is (n_examples, n_classes) predictions are
-                converted to crisp values by `super().fit()
+                converted to crisp values by `super().fit()`
 
             Raises
             ------
             ValueError
                 When estimator_train and predictions_train are both None
         """
         super().fit(X, y, predictions_train=predictions_train)
@@ -171,25 +170,24 @@
 
             First, predictions_test_ are computed (if needed, when predictions_test parameter is None) by
             `super().predict()` method.
 
             After that, the distribution of such predictions are computed and stored in test_distrib_ attribute
             Finally, the prevalences are computed solving the following optimization problem:
 
-                      Min   | train_distrib_ * prevalences -  test_distrib_ |
-                      s.t.  sum(prevalences) = 1
-                            prevalecences_i >= 0
+                      Min   | train_distrib_ * prevalences -  test_distrib_ | 
+                      s.t.  sum(prevalences) = 1, prevalecences_i >= 0
 
             Parameters
             ----------
             X : array-like, shape (n_examples, n_features)
                 Testing bag
 
             predictions_test : ndarray, shape (n_examples, n_classes) (default=None)
-                They must be probabilities (the estimator used must have a `predict_proba method)
+                They must be probabilities (the estimator used must have a `predict_proba` method)
 
                 If predictions_test is not None they are copied on predictions_test_ and used.
                 If predictions_test is None, predictions for the testing examples are computed using the `predict`
                 method of estimator_test (it must be an actual estimator)
 
             Raises
             ------
```

### Comparing `quantificationlib-0.0.7/quantificationlib/ordinal/pdf.py` & `quantificationlib-0.1.1/quantificationlib/ordinal/pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,35 +39,35 @@
         ----------
         estimator_train : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
             training set and to compute the distribution of each class individually
 
         estimator_test : estimator object (default=None)
             An estimator object implementing `fit` and `predict_proba`. It is used to classify the examples of the
-            testing set and to compute the distribution of the whole testing set
+            testing set and to compute the distribution of the whole testing set.
+            For some experiments both estimator_train and estimator_test could be the same
 
         n_bins : int
             Number of bins to compute the PDFs
 
         distance : str, representing the distance function (default='HD')
             It is the name of the distance used to compute the difference between the mixture of the training
             distribution and the testing distribution
 
         method : str
-            'full_probabilistic' predictions for training and testing set contain a probability for each class
-            'winner_node' this method is only applicable for DDAGClassifier, and predictions contain just the
-                          probabilities for the two consecutive classes of the winner node previous to the leaves
+            - 'full_probabilistic': predictions for training and testing set contain a probability for each class
+            - 'winner_node': (this method is only applicable for DDAGClassifier) predictions contain just
+              the probabilities for the two consecutive classes of the winner node previous to the leaves
 
         tol : float, (default=1e-05)
             The precision of the solution when search is used to compute the prevalence
 
         verbose : int, optional, (default=0)
             The verbosity level. The default value, zero, means silent mode
 
-        For some experiments both estimator_train and estimator_test could be the same
 
         Attributes
         ----------
         estimator_train : estimator
             Estimator used to classify the examples of the training set
 
         estimator_test : estimator
```

### Comparing `quantificationlib-0.0.7/quantificationlib/ordinal/trees.py` & `quantificationlib-0.1.1/quantificationlib/ordinal/trees.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/quantificationlib/search.py` & `quantificationlib-0.1.1/quantificationlib/search.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/quantificationlib.egg-info/PKG-INFO` & `quantificationlib-0.1.1/quantificationlib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quantificationlib
-Version: 0.0.7
+Version: 0.1.1
 Summary: quantificationlib: A library for Quantification Learning
 Home-page: https://github.com/AICGijon/quantificationlib
-Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.7.tar.gz
+Download-URL: https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.8.tar.gz
 Author: Alberto Castaño, Pablo González, Jaime Alonso, Pablo Pérez, Juan José del Coz
 Author-email: bertocast@gmail.com, gonzalezgpablo@uniovi.es, jalonso@uniovi.es, pabloperez@uniovi.es, juanjo@uniovi.es
 Keywords: quantification,label shift,prevalence estimation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
@@ -27,14 +27,10 @@
 [![Downloads PyPI](https://static.pepy.tech/personalized-badge/quantificationlib?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=pypi)](https://pypi.org/project/quantificationlib/)
 
 
 # QuantificationLib
 
 QuantificationLib is an open-source library for quantification learning. 
 
-### Last updates:
-- Adding plots [0.0.7]
-- Initial version of the library released [0.0.6].
-
 ### Installation and documentation
 
 The installation, quick-start guide and documentation are available [here](https://aicgijon.github.io/quantificationlib/).
```

### Comparing `quantificationlib-0.0.7/quantificationlib.egg-info/SOURCES.txt` & `quantificationlib-0.1.1/quantificationlib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,8 +51,10 @@
 quantificationlib/plot/qlplot.py
 tests/test_bag_generators.py
 tests/test_binary_quantifiers.py
 tests/test_cv_estimator.py
 tests/test_decomposition.py
 tests/test_ensembles.py
 tests/test_metrics.py
-tests/test_ordinal_quantifiers.py
+tests/test_multiclass_quantifiers.py
+tests/test_ordinal_quantifiers.py
+tests/test_plot.py
```

### Comparing `quantificationlib-0.0.7/setup.py` & `quantificationlib-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     long_description_content_type='text/markdown',  # Optional (see note above)
 
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     url='https://github.com/AICGijon/quantificationlib',  # Optional
-    download_url='https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.7.tar.gz',
+    download_url='https://github.com/AICGijon/quantificationlib/archive/refs/tags/0.0.8.tar.gz',
 
     author='Alberto Castaño, Pablo González, Jaime Alonso, Pablo Pérez, Juan José del Coz',
 
     author_email='bertocast@gmail.com, gonzalezgpablo@uniovi.es, jalonso@uniovi.es, pabloperez@uniovi.es, juanjo@uniovi.es',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `quantificationlib-0.0.7/tests/test_bag_generators.py` & `quantificationlib-0.1.1/tests/test_bag_generators.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/tests/test_binary_quantifiers.py` & `quantificationlib-0.1.1/tests/test_binary_quantifiers.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
     dataset='examples/datasets/binary/iris.3.csv'
     n_bags=5
     master_seed=2032
 
     method_name = ['CC', 'AC', 'PCC', 'PAC', 'EM',
                    'HDX-8b', 'CDFX-100b-L1', 'CDFX-100b-L2',
-                   'HDy-8b', 'PDFy-8b-tipsoe',
+                   'HDy-8b','HDy-8b-equal_with','HDy-8b-binormal','HDy-8b-normal', 
+                   'PDFy-8b-tipsoe',
                    'CDFy-100b-L1', 'CDFy-100b-L2', 'MMy-100', 'SORDy',
                    'DeBias', 'FriedmanME-L1',
                    'EDX', 'EDy', 'CvMy',
                    'QUANTy-L1', 'QUANTy-L2',
                    'REGX', 'REGy',
                    'PWKQuantifier']
 
@@ -63,94 +64,106 @@
     #  CC
     cc = CC(estimator_test=estimator)
     cc.fit(X_train, y_train)
     #  PCC
     pcc = PCC(estimator_test=estimator)
     pcc.fit(X_train, y_train)
     #  PAC
-    pac = PAC(estimator_train=estimator, estimator_test=estimator)
+    pac = PAC(estimator_train=estimator, estimator_test=estimator, verbose=1)
     pac.fit(X_train, y_train)
 
     # EM
-    em = EM(estimator_train=estimator, estimator_test=estimator)
+    em = EM(estimator_train=estimator, estimator_test=estimator, verbose=1)
     em.fit(X_train, y_train)
 
     #  HDX
     hdx = HDX(n_bins=8)
     hdx.fit(X_train, y_train)
 
     #  CDFX-L1
-    cdfx_l1 = DFX(distribution_function='CDF', n_bins=100, distance='L1')
+    cdfx_l1 = DFX(distribution_function='CDF', n_bins=100, distance='L1', verbose=1)
     cdfx_l1.fit(X_train, y_train)
     #  CDFX-L2
-    cdfx_l2 = DFX(distribution_function='CDF', n_bins=100, distance='L2')
+    cdfx_l2 = DFX(distribution_function='CDF', n_bins=100, distance='L2', verbose=1)
     cdfx_l2.fit(X_train, y_train)
 
     #  HDY
-    hdy = HDy(estimator_train=estimator, estimator_test=estimator, n_bins=8)
+    hdy = HDy(estimator_train=estimator, estimator_test=estimator, n_bins=8, verbose=1)
     hdy.fit(X_train, y_train)
 
+    #  HDY equal count
+    hdy_equal_count = HDy(estimator_train=estimator, estimator_test=estimator, n_bins=8, bin_strategy='equal_count', verbose=1)
+    hdy_equal_count.fit(X_train, y_train)
+
+    #  HDY binormal
+    hdy_binormal = HDy(estimator_train=estimator, estimator_test=estimator, n_bins=8, bin_strategy='binormal', verbose=1)
+    hdy_binormal.fit(X_train, y_train)
+
+    #  HDY normal
+    hdy_normal = HDy(estimator_train=estimator, estimator_test=estimator, n_bins=8, bin_strategy='normal', verbose=1)
+    hdy_normal.fit(X_train, y_train)
+
     #  PDFY - topsoe
     pdfy_topsoe = DFy(estimator_train=estimator, estimator_test=estimator, distribution_function='PDF',
-                        distance=topsoe, n_bins=8)
+                        distance=topsoe, n_bins=8, verbose=1)
     pdfy_topsoe.fit(X_train, y_train)
 
     #  MMy
-    mmy = MMy(estimator_train=estimator, estimator_test=estimator, n_bins=100)
+    mmy = MMy(estimator_train=estimator, estimator_test=estimator, n_bins=100, verbose=1)
     mmy.fit(X_train, y_train)
 
     #  SORDy
-    sordy = SORDy(estimator_train=estimator, estimator_test=estimator)
+    sordy = SORDy(estimator_train=estimator, estimator_test=estimator, verbose=1)
     sordy.fit(X_train, y_train)
 
     #  CDFy-L1
     cdfy_l1 = DFy(estimator_train=estimator, estimator_test=estimator, distribution_function='CDF',
-                    n_bins=100, distance='L1')
+                    n_bins=100, distance='L1', verbose=1)
     cdfy_l1.fit(X_train, y_train)
     #  CDFy-L2
     cdfy_l2 = DFy(estimator_train=estimator, estimator_test=estimator, distribution_function='CDF',
-                    n_bins=100, distance='L2')
+                    n_bins=100, distance='L2', verbose=1)
     cdfy_l2.fit(X_train, y_train)
 
     #  Friedman DeBias
-    db = DeBias(estimator_train=estimator, estimator_test=estimator)
+    db = DeBias(estimator_train=estimator, estimator_test=estimator, verbose=1)
     db.fit(X_train, y_train)
     #  FriedmanME - L1
-    me_l1 = FriedmanME(estimator_train=estimator, estimator_test=estimator, distance='L1')
+    me_l1 = FriedmanME(estimator_train=estimator, estimator_test=estimator, distance='L1', verbose=1)
     me_l1.fit(X_train, y_train)
 
     #  EDX
-    edx = EDX()
+    edx = EDX(verbose=1)
     edx.fit(X_train, y_train)
     #  EDy
-    edy = EDy(estimator_train=estimator, estimator_test=estimator)
+    edy = EDy(estimator_train=estimator, estimator_test=estimator, verbose=1)
     edy.fit(X_train, y_train)
     #  CvMy
-    cvmy = CvMy(estimator_train=estimator, estimator_test=estimator)
+    cvmy = CvMy(estimator_train=estimator, estimator_test=estimator, verbose=1)
     cvmy.fit(X_train, y_train)
 
     #  QUANTy-L1
-    quanty_l1 = QUANTy(estimator_train=estimator, estimator_test=estimator, n_quantiles=8, distance=l1)
+    quanty_l1 = QUANTy(estimator_train=estimator, estimator_test=estimator, n_quantiles=8, distance=l1, verbose=1)
     quanty_l1.fit(X_train, y_train)
     #  QUANTy-L2
-    quanty_l2 = QUANTy(estimator_train=estimator, estimator_test=estimator, n_quantiles=8, distance=l2)
+    quanty_l2 = QUANTy(estimator_train=estimator, estimator_test=estimator, n_quantiles=8, distance=l2, verbose=1)
     quanty_l2.fit(X_train, y_train)
 
     #  REGX
     bag_generator = PriorShift_BagGenerator(n_bags=1000, bag_size=len(X_train),
                                             min_prevalence=None, random_state=master_seed)
-    regx = REGX(bag_generator=bag_generator, n_bins=8, bin_strategy='equal_width', regression_estimator=None)
+    regx = REGX(bag_generator=bag_generator, n_bins=8, bin_strategy='equal_width', regression_estimator=None, verbose=1)
     regx.fit(X_train, y_train)
     # REGy
     regy = REGy(estimator_train=estimator, estimator_test=estimator, bag_generator=bag_generator,
-                n_bins=8, bin_strategy='equal_width', regression_estimator=None)
+                n_bins=8, bin_strategy='equal_width', regression_estimator=None, verbose=1)
     regy.fit(X_train, y_train)
 
     # PWK
-    knn_q = PWKQuantifier()
+    knn_q = PWKQuantifier(verbose=1)
     knn_q.fit(X_train, y_train)
 
     #  Testing bags
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
@@ -162,14 +175,17 @@
             pcc.predict(X_test[indexes[:, n_bag], :]),
             pac.predict(X_test[indexes[:, n_bag], :]),
             em.predict(X_test[indexes[:, n_bag], :]),
             hdx.predict(X_test[indexes[:, n_bag], :]),
             cdfx_l1.predict(X_test[indexes[:, n_bag], :]),
             cdfx_l2.predict(X_test[indexes[:, n_bag], :]),
             hdy.predict(X_test[indexes[:, n_bag], :]),
+            hdy_equal_count.predict(X_test[indexes[:, n_bag], :]),
+            hdy_binormal.predict(X_test[indexes[:, n_bag], :]),
+            hdy_normal.predict(X_test[indexes[:, n_bag], :]),
             pdfy_topsoe.predict(X_test[indexes[:, n_bag], :]),
             mmy.predict(X_test[indexes[:, n_bag], :]),
             sordy.predict(X_test[indexes[:, n_bag], :]),
             cdfy_l1.predict(X_test[indexes[:, n_bag], :]),
             cdfy_l2.predict(X_test[indexes[:, n_bag], :]),
             db.predict(X_test[indexes[:, n_bag], :]),
             me_l1.predict(X_test[indexes[:, n_bag], :]),
```

### Comparing `quantificationlib-0.0.7/tests/test_cv_estimator.py` & `quantificationlib-0.1.1/tests/test_cv_estimator.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/tests/test_decomposition.py` & `quantificationlib-0.1.1/tests/test_decomposition.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from quantificationlib.multiclass.df import HDX
 
 from quantificationlib.decomposition.multiclass import OneVsRestQuantifier
 
 from quantificationlib.metrics.ordinal import emd, emd_score
 
 from quantificationlib.estimators.frank_and_hall import FrankAndHallClassifier
+from quantificationlib.estimators.frank_and_hall import FrankAndHallMonotoneClassifier
 from quantificationlib.decomposition.ordinal import FrankAndHallQuantifier
 
 from quantificationlib.estimators.cross_validation import CV_estimator
 from quantificationlib.bag_generator import PriorShift_BagGenerator
 from quantificationlib.metrics.multiclass import mean_absolute_error
 
 from quantificationlib.data_utils import load_data, normalize
@@ -77,15 +78,15 @@
 
 def test_decomposition_ordinal():
 
     dataset='examples/datasets/ordinal/ESL.csv'
     n_bags=5
     master_seed=2032
 
-    method_name = ['FH-CC', 'FH-AC']
+    method_name = ['FH-CC', 'FH-AC', 'FHM-AC']
 
     results_emd = np.zeros((n_bags, len(method_name)))
     results_emd_score = np.zeros((n_bags, len(method_name)))
 
     X, y = load_data(dataset)
 
     current_seed = master_seed
@@ -94,32 +95,40 @@
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, stratify=y, random_state=current_seed)
     X_train, X_test = normalize(X_train, X_test)
 
     # classifiers are fitted by each object (all methods will use exactly the same predictions)
     # but they checked whether the estimator is already fitted (by a previous object) or not
     fh = FrankAndHallClassifier(estimator=RandomForestClassifier(n_estimators=100,
                                                                     random_state=master_seed,
-                                                                    class_weight='balanced'), n_jobs=-1)
+                                                                    class_weight='balanced'), n_jobs=-1, verbose=1)
+    fhm = FrankAndHallMonotoneClassifier(estimator=RandomForestClassifier(n_estimators=100,
+                                                                    random_state=master_seed,
+                                                                    class_weight='balanced'), n_jobs=-1, verbose=1)
+
 
-    #  AC_HD
-    fh_ac = FrankAndHallQuantifier(quantifier=AC(), estimator_train=fh, estimator_test=fh)
+    #  AC
+    fh_ac = FrankAndHallQuantifier(quantifier=AC(), estimator_train=fh, estimator_test=fh, verbose=1)
     fh_ac.fit(X_train, y_train)
+    #  AC
+    fhm_ac = FrankAndHallQuantifier(quantifier=AC(), estimator_train=fh, estimator_test=fhm, verbose=1)
+    fhm_ac.fit(X_train, y_train)
     #  CC
-    fh_hdx = FrankAndHallQuantifier(quantifier=HDX(), estimator_train=None, estimator_test=None)
+    fh_hdx = FrankAndHallQuantifier(quantifier=HDX(), estimator_train=None, estimator_test=None, verbose=1)
     fh_hdx.fit(X_train, y_train)
     
 
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
     for n_bag in range(n_bags):
         prev_preds = [
             fh_hdx.predict(X_test[indexes[:, n_bag], :]),
             fh_ac.predict(X_test[indexes[:, n_bag], :]),
+            fhm_ac.predict(X_test[indexes[:, n_bag], :]),
         ]
 
     for n_method, prev_pred in enumerate(prev_preds):
         results_emd[n_bag, n_method] = emd(prev_true[:, n_bag], prev_pred)
         results_emd_score[n_bag, n_method] = emd_score(prev_true[:, n_bag], prev_pred)
 
     avg_emd = np.mean(results_emd, axis=0)
```

### Comparing `quantificationlib-0.0.7/tests/test_ensembles.py` & `quantificationlib-0.1.1/tests/test_ensembles.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,41 +48,41 @@
 
     bag_generator_eoq = PriorShift_BagGenerator(n_bags=100, bag_size=len(X_train),
                                                 min_prevalence=0.05, random_state=current_seed)
 
     #  HDX
     eoq_hdx = EoQ(base_quantifier=HDX(),
                     n_quantifiers=10, bag_generator=bag_generator_eoq,
-                    combination_strategy='prevalence_similarity')
+                    combination_strategy='prevalence_similarity', verbose=1)
     eoq_hdx.fit(X_train, y_train)
     #  PAC
     eoq_pac = EoQ(base_quantifier=PAC(),
                     n_quantifiers=10, bag_generator=bag_generator_eoq,
                     combination_strategy='median',
-                    ensemble_estimator_train=ensemble_estimator, ensemble_estimator_test=ensemble_estimator)
+                    ensemble_estimator_train=ensemble_estimator, ensemble_estimator_test=ensemble_estimator, verbose=1)
     eoq_pac.fit(X_train, y_train)
 
     # EM
     eoq_em = EoQ(base_quantifier=EM(),
                     n_quantifiers=10, bag_generator=bag_generator_eoq,
-                    combination_strategy='mean',
-                    ensemble_estimator_train=ensemble_estimator, ensemble_estimator_test=ensemble_estimator)
+                    combination_strategy='all',
+                    ensemble_estimator_train=ensemble_estimator, ensemble_estimator_test=ensemble_estimator, verbose=1)
     eoq_em.fit(X_train, y_train)
 
     #  Testing bags
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
     for n_bag in range(n_bags):
 
         prev_preds = [
             eoq_hdx.predict(X_test[indexes[:, n_bag], :]),
             eoq_pac.predict(X_test[indexes[:, n_bag], :]),
-            eoq_em.predict(X_test[indexes[:, n_bag], :]),
+            eoq_em.predict(X_test[indexes[:, n_bag], :])['all'],
         ]
 
         for n_method, prev_pred in enumerate(prev_preds):
             results[n_bag, n_method] = mean_absolute_error(prev_true[:, n_bag], prev_pred)
 
     avg = np.mean(results, axis=0)
     for name, result in zip(method_name,avg):
```

### Comparing `quantificationlib-0.0.7/tests/test_metrics.py` & `quantificationlib-0.1.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `quantificationlib-0.0.7/tests/test_ordinal_quantifiers.py` & `quantificationlib-0.1.1/tests/test_ordinal_quantifiers.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,48 +39,48 @@
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, stratify=y, random_state=current_seed)
     X_train, X_test = normalize(X_train, X_test)
 
     # classifiers are fitted by each object (all methods will use exactly the same predictions)
     # but they checked whether the estimator is already fitted (by a previous object) or not
     fh = FrankAndHallTreeClassifier(estimator=RandomForestClassifier(n_estimators=100,
                                                                         random_state=master_seed,
-                                                                        class_weight='balanced'), n_jobs=-1)
+                                                                        class_weight='balanced'), n_jobs=-1, verbose=1)
 
     #  PCC
     pcc = PCC(estimator_test=fh)
     pcc.fit(X_train, y_train)
 
     #  OQT
     oqt = OrdinalQuantificationTree(estimator_test=RandomForestClassifier(n_estimators=100,
                                                                             random_state=master_seed,
-                                                                            class_weight='balanced'))
+                                                                            class_weight='balanced', verbose=1))
     oqt.fit(X_train, y_train)
 
     #  AC L2
-    ac_l2 = AC(estimator_train=fh, estimator_test=fh, distance='L2')
+    ac_l2 = AC(estimator_train=fh, estimator_test=fh, distance='L2', verbose=1)
     ac_l2.fit(X_train, y_train)
 
     #  AC ORD
-    ac_ord = ACOrdinal(estimator_train=fh, estimator_test=fh)
+    ac_ord = ACOrdinal(estimator_train=fh, estimator_test=fh, verbose=1)
     ac_ord.fit(X_train, y_train)
 
     #  PAC L2
-    pac_l2 = PAC(estimator_train=fh, estimator_test=fh, distance='L2')
+    pac_l2 = PAC(estimator_train=fh, estimator_test=fh, distance='L2', verbose=1)
     pac_l2.fit(X_train, y_train)
 
     #  EDy
-    edy = EDy(estimator_train=fh, estimator_test=fh, distance=emd_distances)
+    edy = EDy(estimator_train=fh, estimator_test=fh, distance=emd_distances, verbose=1)
     edy.fit(X_train, y_train)
 
     #  PDF L2
-    pdf_l2 = PDFOrdinaly(estimator_train=fh, estimator_test=fh, distance='L2')
+    pdf_l2 = PDFOrdinaly(estimator_train=fh, estimator_test=fh, distance='L2', verbose=1)
     pdf_l2.fit(X_train, y_train)
 
     #  PDF EMD
-    pdf_emd = PDFOrdinaly(estimator_train=fh, estimator_test=fh, distance='EMD')
+    pdf_emd = PDFOrdinaly(estimator_train=fh, estimator_test=fh, method='winner_node', distance='EMD', verbose=1)
     pdf_emd.fit(X_train, y_train)
 
     bag_generator = PriorShift_BagGenerator(n_bags=n_bags, bag_size=len(X_test),
                                             min_prevalence=None, random_state=current_seed)
 
     prev_true, indexes = bag_generator.generate_bags(X_test, y_test)
     for n_bag in range(n_bags):
```

