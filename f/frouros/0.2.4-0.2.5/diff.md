# Comparing `tmp/frouros-0.2.4.tar.gz` & `tmp/frouros-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.2.4.tar", last modified: Fri Apr 28 13:44:57 2023, max compression
+gzip compressed data, was "frouros-0.2.5.tar", last modified: Fri Apr 28 19:16:45 2023, max compression
```

## Comparing `frouros-0.2.4.tar` & `frouros-0.2.5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.513455 frouros-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-04-28 13:44:42.000000 frouros-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-28 13:44:42.000000 frouros-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-28 13:44:57.513455 frouros-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-04-28 13:44:42.000000 frouros-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.497455 frouros-0.2.4/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.497455 frouros-0.2.4/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.501455 frouros-0.2.4/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.505455 frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.505455 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.505455 frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/concept_drift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.505455 frouros-0.2.4/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6426 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.505455 frouros-0.2.4/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8231 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.509455 frouros-0.2.4/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.513455 frouros-0.2.4/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8942 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14872 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.513455 frouros-0.2.4/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.513455 frouros-0.2.4/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.513455 frouros-0.2.4/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-04-28 13:44:42.000000 frouros-0.2.4/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:44:57.497455 frouros-0.2.4/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-28 13:44:56.000000 frouros-0.2.4/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-04-28 13:44:57.000000 frouros-0.2.4/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 13:44:56.000000 frouros-0.2.4/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 13:44:56.000000 frouros-0.2.4/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-28 13:44:57.000000 frouros-0.2.4/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-28 13:44:57.000000 frouros-0.2.4/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-28 13:44:42.000000 frouros-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 13:44:57.513455 frouros-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-04-28 13:44:42.000000 frouros-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.358342 frouros-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-04-28 19:16:28.000000 frouros-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-28 19:16:28.000000 frouros-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-28 19:16:45.358342 frouros-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-04-28 19:16:28.000000 frouros-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.342342 frouros-0.2.5/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.342342 frouros-0.2.5/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.342342 frouros-0.2.5/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/batch/reset_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.346342 frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/concept_drift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8231 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.350342 frouros-0.2.5/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.354342 frouros-0.2.5/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.354342 frouros-0.2.5/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.354342 frouros-0.2.5/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.354342 frouros-0.2.5/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.358342 frouros-0.2.5/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8945 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14872 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.358342 frouros-0.2.5/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.358342 frouros-0.2.5/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.358342 frouros-0.2.5/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-04-28 19:16:28.000000 frouros-0.2.5/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 19:16:45.342342 frouros-0.2.5/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-28 19:16:44.000000 frouros-0.2.5/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-04-28 19:16:45.000000 frouros-0.2.5/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 19:16:44.000000 frouros-0.2.5/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 19:16:44.000000 frouros-0.2.5/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-28 19:16:45.000000 frouros-0.2.5/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-28 19:16:45.000000 frouros-0.2.5/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-28 19:16:28.000000 frouros-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 19:16:45.358342 frouros-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-04-28 19:16:28.000000 frouros-0.2.5/setup.py
```

### Comparing `frouros-0.2.4/LICENSE` & `frouros-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/PKG-INFO` & `frouros-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.4
+Version: 0.2.5
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
-Metadata-Version: 2.1 Name: frouros Version: 0.2.4 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.5 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.4/README.md` & `frouros-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/callbacks/base.py` & `frouros-0.2.5/frouros/callbacks/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,21 +51,21 @@
     #     if not isinstance(
     #             value, (ConceptDriftBase, DataDriftBatchBase)):
     #         raise TypeError(
     #             "value must be of type ConceptDriftBase or DataDriftBatchBase."
     #         )
     #     self._detector = value
 
-    def on_fit_start(self) -> None:
+    def on_fit_start(self, **kwargs) -> None:
         """On fit start method."""
 
-    def on_fit_end(self) -> None:
+    def on_fit_end(self, **kwargs) -> None:
         """On fit end method."""
 
-    def on_drift_detected(self) -> None:
+    def on_drift_detected(self, **kwargs) -> None:
         """On drift detected method."""
 
     @abc.abstractmethod
     def reset(self) -> None:
         """Reset method."""
 
     def __repr__(self) -> str:
```

### Comparing `frouros-0.2.4/frouros/callbacks/batch/base.py` & `frouros-0.2.5/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/callbacks/batch/permutation_test.py` & `frouros-0.2.5/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/callbacks/batch/reset_drift.py` & `frouros-0.2.5/frouros/callbacks/batch/reset_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/callbacks/streaming/base.py` & `frouros-0.2.5/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/callbacks/streaming/history.py` & `frouros-0.2.5/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/callbacks/streaming/msprt.py` & `frouros-0.2.5/frouros/callbacks/streaming/msprt.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     .. [johari2022always] Ramesh, Johari, et al.
         "Always valid inference: Continuous monitoring of a/b tests"
         Operations Research 70.3 (2022): 1806-1821.
     """
 
     def __init__(
         self,
-        alpha: float = 0.05,
+        alpha: float,
         sigma: float = 1.0,
         tau: Optional[float] = None,
         truncation: int = 1,
         name: Optional[str] = None,
     ) -> None:
         """Init method.
 
@@ -93,14 +93,18 @@
         :param value: value to be set
         :type value: Optional[float]
         """
         if value is not None and not isinstance(value, float):
             raise TypeError("tau must be a float or None")
         self._tau = value
 
+    def on_fit_end(self, **kwargs) -> None:
+        """On fit end method."""
+        self.incremental_mean.num_values = len(kwargs["X"])
+
     def on_update_end(self, value: Union[int, float], **kwargs) -> None:
         """On update end method.
 
         :param value: value to update detector
         :type value: int
         """
         self.incremental_mean.update(value=value)
```

### Comparing `frouros-0.2.4/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.2.5/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/datasets/base.py` & `frouros-0.2.5/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/datasets/real.py` & `frouros-0.2.5/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/datasets/synthetic.py` & `frouros-0.2.5/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/base.py` & `frouros-0.2.5/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/__init__.py` & `frouros-0.2.5/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/base.py` & `frouros-0.2.5/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/base.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.2.5/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/__init__.py` & `frouros-0.2.5/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         :rtype: Dict[str, Any]
         """
         self._check_fit_dimensions(X=X)
         for callback in self.callbacks:  # type: ignore
             callback.on_fit_start()
         self._fit(X=X, **kwargs)
         for callback in self.callbacks:  # type: ignore
-            callback.on_fit_end()
+            callback.on_fit_end(X=X, **kwargs)
 
         logs = self._get_callbacks_logs()
         return logs
 
     def reset(self) -> None:
         """Reset method."""
         self.X_ref = None
```

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.2.5/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.2.5/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.2.5/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.2.5/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/metrics/base.py` & `frouros-0.2.5/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/metrics/prequential_error.py` & `frouros-0.2.5/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/tests/conftest.py` & `frouros-0.2.5/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/tests/integration/test_callback.py` & `frouros-0.2.5/frouros/tests/integration/test_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 @pytest.mark.parametrize(
     "detector_class,"
     " expected_drift_idx,"
     " expected_distance_mean,"
     " expected_p_value,"
     " expected_likelihood",
     [
-        (MMDStreaming, 70, 0.3622854, 0.0324733, 30.79452443),
+        (MMDStreaming, 40, 0.08821576, 0.00494882, 202.06836342),
     ],
 )
 def test_streaming_msprt_multivariate_different_distribution(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,
     detector_class: DataDriftBatchBase,
     expected_drift_idx: int,
```

### Comparing `frouros-0.2.4/frouros/tests/integration/test_concept_drift.py` & `frouros-0.2.5/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/tests/integration/test_data_drift.py` & `frouros-0.2.5/frouros/tests/integration/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/tests/integration/test_real.py` & `frouros-0.2.5/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/tests/integration/test_synthetic.py` & `frouros-0.2.5/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.2.5/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/utils/data_structures.py` & `frouros-0.2.5/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/utils/decorators.py` & `frouros-0.2.5/frouros/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros/utils/stats.py` & `frouros-0.2.5/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/frouros.egg-info/PKG-INFO` & `frouros-0.2.5/frouros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.4
+Version: 0.2.5
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
-Metadata-Version: 2.1 Name: frouros Version: 0.2.4 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.5 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.4/frouros.egg-info/SOURCES.txt` & `frouros-0.2.5/frouros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frouros-0.2.4/pyproject.toml` & `frouros-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.2.4"
+version = "0.2.5"
 description = "A Python library for drift detection in Machine Learning problems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
```

### Comparing `frouros-0.2.4/setup.py` & `frouros-0.2.5/setup.py`

 * *Files identical despite different names*

