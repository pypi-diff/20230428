# Comparing `tmp/frouros-0.2.2.tar.gz` & `tmp/frouros-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.2.2.tar", last modified: Mon Apr 10 10:18:37 2023, max compression
+gzip compressed data, was "frouros-0.2.3.tar", last modified: Fri Apr 28 11:01:54 2023, max compression
```

## Comparing `frouros-0.2.2.tar` & `frouros-0.2.3.tar`

### file list

```diff
@@ -1,127 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-04-10 10:18:18.000000 frouros-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-10 10:18:18.000000 frouros-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-10 10:18:37.900965 frouros-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-04-10 10:18:18.000000 frouros-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.884965 frouros-0.2.2/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.888965 frouros-0.2.2/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/concept_drift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6426 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.892964 frouros-0.2.2/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8221 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7249 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.896965 frouros-0.2.2/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6499 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    12399 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.900965 frouros-0.2.2/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-04-10 10:18:18.000000 frouros-0.2.2/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 10:18:37.884965 frouros-0.2.2/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4399 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-10 10:18:37.000000 frouros-0.2.2/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-10 10:18:18.000000 frouros-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 10:18:37.900965 frouros-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-04-10 10:18:18.000000 frouros-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.218322 frouros-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-04-28 11:01:41.000000 frouros-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-28 11:01:41.000000 frouros-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-28 11:01:54.218322 frouros-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-04-28 11:01:41.000000 frouros-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.206322 frouros-0.2.3/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.206322 frouros-0.2.3/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.206322 frouros-0.2.3/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/batch/reset_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/concept_drift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.210322 frouros-0.2.3/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6426 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8221 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8942 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14872 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.214322 frouros-0.2.3/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.218322 frouros-0.2.3/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-04-28 11:01:41.000000 frouros-0.2.3/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 11:01:54.206322 frouros-0.2.3/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-28 11:01:53.000000 frouros-0.2.3/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-04-28 11:01:54.000000 frouros-0.2.3/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 11:01:53.000000 frouros-0.2.3/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 11:01:53.000000 frouros-0.2.3/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-28 11:01:54.000000 frouros-0.2.3/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-28 11:01:54.000000 frouros-0.2.3/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-28 11:01:41.000000 frouros-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 11:01:54.218322 frouros-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-04-28 11:01:41.000000 frouros-0.2.3/setup.py
```

### Comparing `frouros-0.2.2/LICENSE` & `frouros-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/PKG-INFO` & `frouros-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library for drift detection in Machine Learning problems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.2.2 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.3 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.2/README.md` & `frouros-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/base.py` & `frouros-0.2.3/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/batch/base.py` & `frouros-0.2.3/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/batch/permutation_test.py` & `frouros-0.2.3/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/batch/reset_drift.py` & `frouros-0.2.3/frouros/callbacks/batch/reset_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/streaming/base.py` & `frouros-0.2.3/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/streaming/history.py` & `frouros-0.2.3/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.2.3/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/datasets/base.py` & `frouros-0.2.3/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/datasets/real.py` & `frouros-0.2.3/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/datasets/synthetic.py` & `frouros-0.2.3/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/base.py` & `frouros-0.2.3/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/__init__.py` & `frouros-0.2.3/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/base.py` & `frouros-0.2.3/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/base.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.2.3/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/__init__.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-"""Data drift detection methods init."""
+"""Data drift batch detection methods init."""
 
-from .batch import (
+from .distance_based import (
     BhattacharyyaDistance,
-    ChiSquareTest,
-    CVMTest,
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     JS,
     KL,
-    KSTest,
     PSI,
     MMD,
+)
+from .statistical_test import (
+    ChiSquareTest,
+    CVMTest,
+    KSTest,
     WelchTTest,
 )
 
-from .streaming import IncrementalKSTest
-
 __all__ = [
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
     "HellingerDistance",
     "HINormalizedComplement",
-    "IncrementalKSTest",
     "JS",
     "KL",
     "KSTest",
     "PSI",
     "MMD",
     "WelchTTest",
 ]
```

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/base.py` & `frouros-0.2.3/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.2.3/frouros/detectors/data_drift/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-"""Data drift batch detection methods init."""
+"""Data drift detection methods init."""
 
-from .distance_based import (
+from .batch import (  # noqa: F401
     BhattacharyyaDistance,
+    ChiSquareTest,
+    CVMTest,
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     JS,
     KL,
+    KSTest,
     PSI,
     MMD,
-)
-from .statistical_test import (
-    ChiSquareTest,
-    CVMTest,
-    KSTest,
     WelchTTest,
 )
 
+from .streaming import IncrementalKSTest, MMD as MMDStreaming  # noqa: N811
+
 __all__ = [
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
     "HellingerDistance",
     "HINormalizedComplement",
+    "IncrementalKSTest",
     "JS",
     "KL",
     "KSTest",
     "PSI",
-    "MMD",
+    "MMDStreaming",
     "WelchTTest",
 ]
```

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/base.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.2.3/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.2.3/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         callbacks: Optional[Union[Callback, List[Callback]]] = None,
         window_size: int = 10,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
         :type callbacks: Optional[Union[Callback, List[Callback]]]
+        :param window_size: window size
+        :type window_size: int
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
         self.window_size = window_size
```

### Comparing `frouros-0.2.2/frouros/metrics/base.py` & `frouros-0.2.3/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/metrics/prequential_error.py` & `frouros-0.2.3/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/tests/conftest.py` & `frouros-0.2.3/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/tests/integration/test_callback.py` & `frouros-0.2.3/frouros/tests/integration/test_callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from frouros.callbacks.batch import (
     PermutationTestOnBatchData,
     ResetOnBatchDataDrift,
 )
 from frouros.callbacks.streaming import (
     History,
+    mSPRT,
     WarningSamplesBuffer,
 )
 from frouros.detectors.concept_drift import (
     ADWIN,
     CUSUM,
     DDM,
     ECDDWT,
@@ -40,53 +41,54 @@
     KL,
     KSTest,
     MMD,
     PSI,
     WelchTTest,
 )
 from frouros.detectors.data_drift.batch.base import DataDriftBatchBase
+from frouros.detectors.data_drift.streaming import MMD as MMDStreaming  # noqa: N811
 
 
 @pytest.mark.parametrize(
-    "detector, expected_distance, expected_p_value",
+    "detector_class, expected_distance, expected_p_value",
     [
         (BhattacharyyaDistance, 0.55516059, 0.0),
         (EMD, 3.85346006, 0.0),
         (HellingerDistance, 0.74509099, 0.0),
         (HINormalizedComplement, 0.78, 0.0),
         (JS, 0.67010107, 0.0),
         (KL, np.inf, 0.0),
         (MMD, 0.71529206, 0.0),
         (PSI, 461.20379435, 0.0),
     ],
 )
 def test_batch_permutation_test_data_univariate_different_distribution(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,
-    detector: DataDriftBatchBase,
+    detector_class: DataDriftBatchBase,
     expected_distance: float,
     expected_p_value: float,
 ) -> None:
     """Test batch permutation test on data callback.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
-    :param detector: detector distance
-    :type detector: DataDriftBatchBase
+    :param detector_class: detector distance
+    :type detector_class: DataDriftBatchBase
     :param expected_distance: expected distance value
     :type expected_distance: float
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     """
     np.random.seed(seed=31)
 
     permutation_test_name = "permutation_test"
-    detector = detector(  # type: ignore
+    detector = detector_class(  # type: ignore
         callbacks=[
             PermutationTestOnBatchData(
                 num_permutations=100,
                 random_state=31,
                 num_jobs=-1,
                 name=permutation_test_name,
             )
@@ -96,42 +98,48 @@
     distance, callback_logs = detector.compare(X=X_test_univariate)
 
     assert np.isclose(distance, expected_distance)
     assert np.isclose(callback_logs[permutation_test_name]["p_value"], expected_p_value)
 
 
 @pytest.mark.parametrize(
-    "detector",
+    "detector_class",
     [CVMTest, KSTest, WelchTTest],
 )
 def test_batch_reset_on_data_drift(
     X_ref_univariate,  # noqa: N803
     X_test_univariate,
-    detector: DataDriftBatchBase,
+    detector_class: DataDriftBatchBase,
     mocker,
 ) -> None:
     """Test batch reset on data drift callback.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
-    :param detector: detector distance
-    :type detector: DataDriftBatchBase
+    :param detector_class: detector distance
+    :type detector_class: DataDriftBatchBase
     """
     mocker.patch("frouros.detectors.data_drift.batch.base.DataDriftBatchBase.reset")
 
-    detector = detector(callbacks=[ResetOnBatchDataDrift(alpha=0.01)])  # type: ignore
+    detector = detector_class(  # type: ignore
+        callbacks=[
+            ResetOnBatchDataDrift(
+                alpha=0.01,
+            ),
+        ],
+    )
     _ = detector.fit(X=X_ref_univariate)
     _ = detector.compare(X=X_test_univariate)
     detector.reset.assert_called_once()  # type: ignore # pylint: disable=no-member
 
 
 @pytest.mark.parametrize(
-    "detector",
+    "detector_class",
     [
         ADWIN,
         CUSUM,
         DDM,
         ECDDWT,
         EDDM,
         GeometricMovingAverage,
@@ -141,25 +149,25 @@
         PageHinkley,
         RDDM,
         STEPD,
     ],
 )
 def test_streaming_history_on_concept_drift(
     model_errors: List[int],
-    detector: ConceptDriftBase,
+    detector_class: ConceptDriftBase,
 ):
     """Test streaming history on concept drift callback.
 
     :param model_errors: model errors
     :type model_errors: List[int]
-    :param detector: concept drift detector
-    :type detector: ConceptDriftBase
+    :param detector_class: concept drift detector
+    :type detector_class: ConceptDriftBase
     """
     name = "history"
-    detector = detector(callbacks=History(name=name))  # type: ignore
+    detector = detector_class(callbacks=History(name=name))  # type: ignore
 
     for error in model_errors:
         history = detector.update(value=error)
         status = detector.status
         if status["drift"]:
             assert history[name]["drift"][-1]
             assert not any(history[name]["drift"][:-1])
@@ -168,42 +176,42 @@
 
 def _fit_model(model, X, y):  # noqa: N803
     model.fit(X=X, y=y)
     return model
 
 
 @pytest.mark.parametrize(
-    "detector",
+    "detector_class",
     [
         DDM,
         ECDDWT,
         EDDM,
         HDDMA,
         HDDMW,
         RDDM,
         STEPD,
-    ],
+    ],  # pylint: disable=too-many-locals
 )
 def test_streaming_warning_samples_buffer_on_concept_drift(
     dataset_simple: Tuple[Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]],
     model: sklearn.pipeline.Pipeline,
-    detector: DDMBased,
+    detector_class: DDMBased,
 ):
     """Test streaming warning samples buffer on concept drift callback.
 
     :param dataset_simple: dataset with concept drift
     :type dataset_simple: Tuple[Tuple[numpy.ndarray, numpy.ndarray],
     :param model: trained model
     :type model: sklearn.pipeline.Pipeline
-    :param detector: concept drift detector
-    :type detector: DDMBased
+    :param detector_class: concept drift detector
+    :type detector_class: DDMBased
     """
     _, test = dataset_simple  # noqa: N806
 
-    detector = detector(
+    detector = detector_class(
         callbacks=WarningSamplesBuffer(name="samples"),  # type: ignore
     )
 
     collect_example_warning_samples = False
     X_extra, y_extra = [], []  # noqa: N806
 
     for X, y in zip(*test):  # noqa: N806
@@ -221,7 +229,70 @@
             else:
                 X_new_ref = callbacks_logs["samples"]["X"] + X_extra  # noqa: N806
                 collect_example_warning_samples = False
                 X_extra.clear()
                 y_extra.clear()
                 detector.reset()
                 model = _fit_model(model=model, X=X_new_ref, y=y_new_ref)
+
+
+@pytest.mark.parametrize(
+    "detector_class,"
+    " expected_drift_idx,"
+    " expected_distance_mean,"
+    " expected_p_value,"
+    " expected_likelihood",
+    [
+        (MMDStreaming, 70, 0.3622854, 0.0324733, 30.79452443),
+    ],
+)
+def test_streaming_msprt_multivariate_different_distribution(
+    X_ref_multivariate: np.ndarray,  # noqa: N803
+    X_test_multivariate: np.ndarray,
+    detector_class: DataDriftBatchBase,
+    expected_drift_idx: int,
+    expected_distance_mean: float,
+    expected_p_value: float,
+    expected_likelihood: float,
+) -> None:
+    """Test streaming mSPRT test on data callback.
+
+    :param X_ref_multivariate: reference multivariate data
+    :type X_ref_multivariate: numpy.ndarray
+    :param X_test_multivariate: test multivariate data
+    :type X_test_multivariate: numpy.ndarray
+    :param detector_class: detector distance
+    :type detector_class: DataDriftBatchBase
+    :param expected_drift_idx: expected drift index
+    :type expected_drift_idx: int
+    :param expected_distance_mean: expected distance mean value
+    :type expected_distance_mean: float
+    :param expected_p_value: expected p-value value
+    :type expected_p_value: float
+    :param expected_likelihood: expected likelihood value
+    :type expected_likelihood: float
+    """
+    np.random.seed(seed=31)
+
+    alpha = 0.05
+
+    detector = detector_class(  # type: ignore
+        callbacks=mSPRT(
+            alpha=alpha,
+            sigma=0.5,
+        ),
+        window_size=5,
+    )
+    _ = detector.fit(X=X_ref_multivariate)
+
+    drift_idx = -1
+    for i, sample in enumerate(X_test_multivariate, start=1):
+        value, callbacks_logs = detector.update(value=sample)
+        if value is not None:
+            if callbacks_logs["mSPRT"]["p_value"] < alpha:
+                drift_idx = i
+                break
+
+    assert np.isclose(drift_idx, expected_drift_idx)
+    assert np.isclose(callbacks_logs["mSPRT"]["distance_mean"], expected_distance_mean)
+    assert np.isclose(callbacks_logs["mSPRT"]["p_value"], expected_p_value)
+    assert np.isclose(callbacks_logs["mSPRT"]["likelihood"], expected_likelihood)
```

### Comparing `frouros-0.2.2/frouros/tests/integration/test_concept_drift.py` & `frouros-0.2.3/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/tests/integration/test_data_drift.py` & `frouros-0.2.3/frouros/tests/integration/test_data_drift.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 )
 from frouros.detectors.data_drift.batch import (
     ChiSquareTest,
     CVMTest,
     KSTest,
     WelchTTest,
 )
-from frouros.detectors.data_drift.streaming import IncrementalKSTest
+from frouros.detectors.data_drift.streaming import (  # noqa: N811
+    IncrementalKSTest,
+    MMD as MMDStreaming,
+)
 
 
 @pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [(ChiSquareTest(), 6.13333333, 0.04657615)],
 )
 def test_batch_distance_based_categorical(
@@ -319,15 +322,15 @@
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
     X_test = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
 
     _ = detector.fit(X=X_ref)
 
     for value in X_test:
-        test = detector.update(value=value)  # type: ignore
+        test, _ = detector.update(value=value)  # type: ignore
 
     # Check last statistic and p-value
     assert np.isclose(test.statistic, expected_statistic)
     assert np.isclose(test.p_value, expected_p_value)
 
 
 @pytest.mark.parametrize(
@@ -359,12 +362,81 @@
     np.random.seed(seed=31)
     X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
     X_test = np.random.normal(*univariate_distribution_q, size=100)  # noqa: N806
 
     _ = detector.fit(X=X_ref)
 
     for value in X_test:
-        test = detector.update(value=value)  # type: ignore
+        test, _ = detector.update(value=value)  # type: ignore
 
     # Check last statistic and p-value
     assert np.isclose(test.statistic, expected_statistic)
     assert np.isclose(test.p_value, expected_p_value)
+
+
+@pytest.mark.parametrize(
+    "detector, expected_distance",
+    [
+        (MMDStreaming(), 0.09793799),
+    ],
+)
+def test_streaming_distance_based_univariate_same_distribution(
+    univariate_distribution_p: Tuple[float, float],
+    detector: DataDriftBatchBase,
+    expected_distance: float,
+) -> None:
+    """Test streaming distance based univariate same distribution method.
+
+    :param univariate_distribution_p: mean and standard deviation of distribution p
+    :type univariate_distribution_p: Tuple[float, float]
+    :param detector: detector statistical test
+    :type detector: DataDriftStreamingBase
+    :param expected_distance: expected distance value
+    :type expected_distance: float
+    """
+    np.random.seed(seed=31)
+    X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
+    X_test = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
+
+    _ = detector.fit(X=X_ref)
+
+    for value in X_test:
+        result, _ = detector.update(value=value)  # type: ignore
+
+    # Check last distance
+    assert np.isclose(result.distance, expected_distance)
+
+
+@pytest.mark.parametrize(
+    "detector, expected_distance",
+    [
+        (MMDStreaming(), 0.98688562),
+    ],
+)
+def test_streaming_distance_based_univariate_different_distribution(
+    univariate_distribution_p: Tuple[float, float],
+    univariate_distribution_q: Tuple[float, float],
+    detector: DataDriftBatchBase,
+    expected_distance: float,
+) -> None:
+    """Test streaming distance based univariate different distribution method.
+
+    :param univariate_distribution_p: mean and standard deviation of distribution p
+    :type univariate_distribution_p: Tuple[float, float]
+    :param univariate_distribution_q: mean and standard deviation of distribution q
+    :type univariate_distribution_q: Tuple[float, float]
+    :param detector: detector statistical test
+    :type detector: DataDriftStreamingBase
+    :param expected_distance: expected distance value
+    :type expected_distance: float
+    """
+    np.random.seed(seed=31)
+    X_ref = np.random.normal(*univariate_distribution_p, size=100)  # noqa: N806
+    X_test = np.random.normal(*univariate_distribution_q, size=100)  # noqa: N806
+
+    _ = detector.fit(X=X_ref)
+
+    for value in X_test:
+        result, _ = detector.update(value=value)  # type: ignore
+
+    # Check last distance
+    assert np.isclose(result.distance, expected_distance)
```

### Comparing `frouros-0.2.2/frouros/tests/integration/test_real.py` & `frouros-0.2.3/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/tests/integration/test_synthetic.py` & `frouros-0.2.3/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.2.3/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/utils/data_structures.py` & `frouros-0.2.3/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/utils/decorators.py` & `frouros-0.2.3/frouros/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros/utils/stats.py` & `frouros-0.2.3/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.2/frouros.egg-info/PKG-INFO` & `frouros-0.2.3/frouros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library for drift detection in Machine Learning problems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.2.2 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.3 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.2/frouros.egg-info/SOURCES.txt` & `frouros-0.2.3/frouros.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 frouros/callbacks/batch/__init__.py
 frouros/callbacks/batch/base.py
 frouros/callbacks/batch/permutation_test.py
 frouros/callbacks/batch/reset_drift.py
 frouros/callbacks/streaming/__init__.py
 frouros/callbacks/streaming/base.py
 frouros/callbacks/streaming/history.py
+frouros/callbacks/streaming/msprt.py
 frouros/callbacks/streaming/warning_samples.py
 frouros/common/__init__.py
 frouros/common/exceptions.py
 frouros/datasets/__init__.py
 frouros/datasets/base.py
 frouros/datasets/exceptions.py
 frouros/datasets/real.py
@@ -71,14 +72,17 @@
 frouros/detectors/data_drift/batch/statistical_test/base.py
 frouros/detectors/data_drift/batch/statistical_test/chisquare.py
 frouros/detectors/data_drift/batch/statistical_test/cvm.py
 frouros/detectors/data_drift/batch/statistical_test/ks.py
 frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
 frouros/detectors/data_drift/streaming/__init__.py
 frouros/detectors/data_drift/streaming/base.py
+frouros/detectors/data_drift/streaming/distance_based/__init__.py
+frouros/detectors/data_drift/streaming/distance_based/base.py
+frouros/detectors/data_drift/streaming/distance_based/mmd.py
 frouros/detectors/data_drift/streaming/statistical_test/__init__.py
 frouros/detectors/data_drift/streaming/statistical_test/base.py
 frouros/detectors/data_drift/streaming/statistical_test/ks.py
 frouros/metrics/__init__.py
 frouros/metrics/base.py
 frouros/metrics/prequential_error.py
 frouros/tests/__init__.py
```

### Comparing `frouros-0.2.2/pyproject.toml` & `frouros-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Python library for drift detection in Machine Learning problems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
```

### Comparing `frouros-0.2.2/setup.py` & `frouros-0.2.3/setup.py`

 * *Files identical despite different names*

