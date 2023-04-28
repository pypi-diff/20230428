# Comparing `tmp/mthree-2.4.0.tar.gz` & `tmp/mthree-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mthree-2.4.0.tar", last modified: Thu Apr 13 15:43:06 2023, max compression
+gzip compressed data, was "mthree-2.5.0.tar", last modified: Fri Apr 28 15:24:33 2023, max compression
```

## Comparing `mthree-2.4.0.tar` & `mthree-2.5.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.861947 mthree-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-13 15:42:48.000000 mthree-2.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 15:42:48.000000 mthree-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-13 15:43:06.861947 mthree-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-13 15:42:48.000000 mthree-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.857947 mthree-2.4.0/mthree/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)   157773 2023-04-13 15:43:01.000000 mthree-2.4.0/mthree/compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/compute.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/compute.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   131033 2023-04-13 15:43:01.000000 mthree-2.4.0/mthree/converters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/converters.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/converters.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   924041 2023-04-13 15:43:02.000000 mthree-2.4.0/mthree/expval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/expval.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   819929 2023-04-13 15:43:02.000000 mthree-2.4.0/mthree/hamming.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/hamming.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   981155 2023-04-13 15:43:04.000000 mthree-2.4.0/mthree/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/matrix.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1003068 2023-04-13 15:43:05.000000 mthree-2.4.0/mthree/matvec.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/matvec.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    34995 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/mitigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)   182404 2023-04-13 15:43:05.000000 mthree-2.4.0/mthree/probability.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/probability.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.861947 mthree-2.4.0/mthree/test/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   890344 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree/test/column_testing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/column_testing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   209983 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree/test/converters_testing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/converters_testing.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.861947 mthree-2.4.0/mthree/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/data/8Qcal_Hanoi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_balanced_cals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_default_shots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_expvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_extra_cals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_faulty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_hamming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_inoperable_qubits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_list_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_marginals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_matvec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_meas_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_multi_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_odd_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_quasi_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_qubits_from_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_reduced_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_sdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_v2_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 15:43:00.000000 mthree-2.4.0/mthree/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.857947 mthree-2.4.0/mthree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 15:42:48.000000 mthree-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 15:42:48.000000 mthree-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:43:06.861947 mthree-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-13 15:42:48.000000 mthree-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:33.394060 mthree-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-28 15:24:11.000000 mthree-2.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 15:24:11.000000 mthree-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-28 15:24:33.394060 mthree-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-28 15:24:11.000000 mthree-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:33.386060 mthree-2.5.0/mthree/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157773 2023-04-28 15:24:26.000000 mthree-2.5.0/mthree/compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/compute.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/compute.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   131033 2023-04-28 15:24:26.000000 mthree-2.5.0/mthree/converters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/converters.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/converters.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   924041 2023-04-28 15:24:27.000000 mthree-2.5.0/mthree/expval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/expval.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   819929 2023-04-28 15:24:28.000000 mthree-2.5.0/mthree/hamming.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/hamming.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   981155 2023-04-28 15:24:30.000000 mthree-2.5.0/mthree/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/matrix.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1003068 2023-04-28 15:24:31.000000 mthree-2.5.0/mthree/matvec.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/matvec.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182404 2023-04-28 15:24:31.000000 mthree-2.5.0/mthree/probability.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/probability.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:33.394060 mthree-2.5.0/mthree/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   890344 2023-04-28 15:24:32.000000 mthree-2.5.0/mthree/test/column_testing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/column_testing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   209983 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree/test/converters_testing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/converters_testing.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:33.394060 mthree-2.5.0/mthree/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/data/8Qcal_Hanoi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_balanced_cals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_default_shots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_expvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_extra_cals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_faulty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_hamming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_inoperable_qubits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_list_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_marginals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_meas_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_multi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_odd_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_quasi_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_qubits_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_reduced_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_sdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/test/test_v2_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-28 15:24:11.000000 mthree-2.5.0/mthree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-28 15:24:26.000000 mthree-2.5.0/mthree/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:33.390060 mthree-2.5.0/mthree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 15:24:33.000000 mthree-2.5.0/mthree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 15:24:11.000000 mthree-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 15:24:11.000000 mthree-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:24:33.394060 mthree-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-28 15:24:11.000000 mthree-2.5.0/setup.py
```

### Comparing `mthree-2.4.0/LICENSE.txt` & `mthree-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/PKG-INFO` & `mthree-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mthree
-Version: 2.4.0
+Version: 2.5.0
 Summary: M3: Matrix-free measurement mitigation
 Home-page: UNKNOWN
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mthree-2.4.0/README.md` & `mthree-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/__init__.py` & `mthree-2.5.0/mthree/__init__.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/_helpers.py` & `mthree-2.5.0/mthree/_helpers.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/circuits.py` & `mthree-2.5.0/mthree/circuits.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/classes.py` & `mthree-2.5.0/mthree/classes.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/compute.cpp` & `mthree-2.5.0/mthree/compute.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/compute.pxd` & `mthree-2.5.0/mthree/compute.pxd`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/compute.pyx` & `mthree-2.5.0/mthree/compute.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/converters.cpp` & `mthree-2.5.0/mthree/converters.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/converters.pxd` & `mthree-2.5.0/mthree/converters.pxd`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/converters.pyx` & `mthree-2.5.0/mthree/converters.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/exceptions.py` & `mthree-2.5.0/mthree/exceptions.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/expval.cpp` & `mthree-2.5.0/mthree/expval.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/expval.pyx` & `mthree-2.5.0/mthree/expval.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/hamming.cpp` & `mthree-2.5.0/mthree/hamming.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/hamming.pyx` & `mthree-2.5.0/mthree/hamming.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/matrix.cpp` & `mthree-2.5.0/mthree/matrix.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/matrix.pyx` & `mthree-2.5.0/mthree/matrix.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/matvec.cpp` & `mthree-2.5.0/mthree/matvec.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/matvec.pyx` & `mthree-2.5.0/mthree/matvec.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/mitigation.py` & `mthree-2.5.0/mthree/mitigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,34 +498,45 @@
         # Check if using faulty qubits
         bad_qubits = set()
         for item in qubits:
             for qu in item:
                 if qu in self.faulty_qubits:
                     bad_qubits.add(qu)
         if any(bad_qubits):
-            raise M3Error("Using faulty qubits: {}".format(bad_qubits))
+            warnings.warn("Using faulty qubits: {}".format(bad_qubits))
 
         quasi_out = []
+        details_out = []
         for idx, cnts in enumerate(counts):
-            quasi_out.append(
-                self._apply_correction(
+            corrected = self._apply_correction(
                     cnts,
                     qubits=qubits[idx],
                     distance=distance,
                     method=method,
                     max_iter=max_iter,
                     tol=tol,
                     return_mitigation_overhead=return_mitigation_overhead,
                     details=details,
-                )
             )
+            if details:
+                quasi_out.append(corrected[0])
+                details_out.append(corrected[1])
+            else:
+                quasi_out.append(corrected)
 
         if not given_list:
+            if details:
+                return quasi_out[0], details_out[0]
             return quasi_out[0]
-        return QuasiCollection(quasi_out)
+
+        quasi_out = QuasiCollection(quasi_out)
+        if details:
+            return quasi_out, details_out
+
+        return quasi_out
 
     def _apply_correction(
         self,
         counts,
         qubits,
         distance=None,
         method="auto",
```

### Comparing `mthree-2.4.0/mthree/norms.py` & `mthree-2.5.0/mthree/norms.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/probability.cpp` & `mthree-2.5.0/mthree/probability.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/probability.pyx` & `mthree-2.5.0/mthree/probability.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/column_testing.cpp` & `mthree-2.5.0/mthree/test/column_testing.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/column_testing.pyx` & `mthree-2.5.0/mthree/test/column_testing.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/converters_testing.cpp` & `mthree-2.5.0/mthree/test/converters_testing.cpp`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/converters_testing.pyx` & `mthree-2.5.0/mthree/test/converters_testing.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/data/8Qcal_Hanoi.json` & `mthree-2.5.0/mthree/test/data/8Qcal_Hanoi.json`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_balanced_cals.py` & `mthree-2.5.0/mthree/test/test_balanced_cals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_collections.py` & `mthree-2.5.0/mthree/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_columns.py` & `mthree-2.5.0/mthree/test/test_columns.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_converters.py` & `mthree-2.5.0/mthree/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_default_shots.py` & `mthree-2.5.0/mthree/test/test_default_shots.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_dynamic.py` & `mthree-2.5.0/mthree/test/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_expvals.py` & `mthree-2.5.0/mthree/test/test_expvals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_extra_cals.py` & `mthree-2.5.0/mthree/test/test_extra_cals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_faulty.py` & `mthree-2.5.0/mthree/test/test_faulty.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,33 @@
 import numpy as np
 import pytest
 
 import mthree
 
 
 def test_faulty_logic():
-    """Test faulty qubits block correction"""
+    """Test faulty qubits raise warning"""
 
     mit = mthree.M3Mitigation(None)
     mit.single_qubit_cals = [np.array([[0.9819, 0.043],
                                        [0.0181, 0.957]]),
                              np.array([[0.4849, 0.5233],
                                        [0.5151, 0.4767]]),
                              np.array([[0.9092, 0.4021],
                                        [0.0908, 0.5979]]),
                              np.array([[0.4117, 0.8101],
                                        [0.5883, 0.1899]])]
     mit.faulty_qubits = [1, 3]
     counts = {"00": 0.4, "01": 0.1, "11": 0.5}
-    with pytest.raises(mthree.exceptions.M3Error) as _:
+    with pytest.warns(UserWarning) as record:
         _ = mit.apply_correction(counts, qubits=[3, 2])
 
+    assert len(record) == 1
+    assert record[0].message.args[0] == "Using faulty qubits: {3}"
+
 
 def test_faulty_io():
     """Check round-tripping IO still has faulty qubits"""
     mit = mthree.M3Mitigation(None)
     mit.single_qubit_cals = [np.array([[0.9819, 0.043],
                                        [0.0181, 0.957]]),
                              np.array([[0.4849, 0.5233],
```

### Comparing `mthree-2.4.0/mthree/test/test_file_io.py` & `mthree-2.5.0/mthree/test/test_file_io.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_full.py` & `mthree-2.5.0/mthree/test/test_full.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_grouping.py` & `mthree-2.5.0/mthree/test/test_grouping.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_hamming.py` & `mthree-2.5.0/mthree/test/test_hamming.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_inoperable_qubits.py` & `mthree-2.5.0/mthree/test/test_inoperable_qubits.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_list_inputs.py` & `mthree-2.5.0/mthree/test/test_list_inputs.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_marginals.py` & `mthree-2.5.0/mthree/test/test_marginals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_matvec.py` & `mthree-2.5.0/mthree/test/test_matvec.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_meas_mapping.py` & `mthree-2.5.0/mthree/test/test_meas_mapping.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_methods.py` & `mthree-2.5.0/mthree/test/test_methods.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_multi_job.py` & `mthree-2.5.0/mthree/test/test_multi_job.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_odd_cases.py` & `mthree-2.5.0/mthree/test/test_odd_cases.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_probability.py` & `mthree-2.5.0/mthree/test/test_probability.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_quasi_attr.py` & `mthree-2.5.0/mthree/test/test_quasi_attr.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_qubits_from_mapping.py` & `mthree-2.5.0/mthree/test/test_qubits_from_mapping.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_reduced_matrix.py` & `mthree-2.5.0/mthree/test/test_reduced_matrix.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_sdd.py` & `mthree-2.5.0/mthree/test/test_sdd.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_sim.py` & `mthree-2.5.0/mthree/test/test_sim.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_threading.py` & `mthree-2.5.0/mthree/test/test_threading.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_utils.py` & `mthree-2.5.0/mthree/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/test/test_v2_backends.py` & `mthree-2.5.0/mthree/test/test_v2_backends.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree/utils.py` & `mthree-2.5.0/mthree/utils.py`

 * *Files identical despite different names*

### Comparing `mthree-2.4.0/mthree.egg-info/PKG-INFO` & `mthree-2.5.0/mthree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mthree
-Version: 2.4.0
+Version: 2.5.0
 Summary: M3: Matrix-free measurement mitigation
 Home-page: UNKNOWN
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mthree-2.4.0/mthree.egg-info/SOURCES.txt` & `mthree-2.5.0/mthree.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 mthree/test/converters_testing.cpp
 mthree/test/converters_testing.pyx
 mthree/test/test_balanced_cals.py
 mthree/test/test_collections.py
 mthree/test/test_columns.py
 mthree/test/test_converters.py
 mthree/test/test_default_shots.py
+mthree/test/test_details.py
 mthree/test/test_dynamic.py
 mthree/test/test_expvals.py
 mthree/test/test_extra_cals.py
 mthree/test/test_faulty.py
 mthree/test/test_file_io.py
 mthree/test/test_full.py
 mthree/test/test_grouping.py
```

### Comparing `mthree-2.4.0/setup.py` & `mthree-2.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import subprocess
 import setuptools
 
 import numpy as np
 from Cython.Build import cythonize
 
 MAJOR = 2
-MINOR = 4
+MINOR = 5
 MICRO = 0
 
 ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 with open("requirements.txt") as f:
     REQUIREMENTS = f.read().splitlines()
```

