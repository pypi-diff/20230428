# Comparing `tmp/scikit-rt-0.4.4.tar.gz` & `tmp/scikit-rt-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.4.4.tar", last modified: Tue Apr 25 08:43:09 2023, max compression
+gzip compressed data, was "scikit-rt-0.4.5.tar", last modified: Fri Apr 28 15:46:01 2023, max compression
```

## Comparing `scikit-rt-0.4.4.tar` & `scikit-rt-0.4.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.202419 scikit-rt-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-25 08:43:09.202419 scikit-rt-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/pypi.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-25 08:43:09.202419 scikit-rt-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.194419 scikit-rt-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.194419 scikit-rt-0.4.4/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-25 08:43:08.000000 scikit-rt-0.4.4/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-25 08:43:09.000000 scikit-rt-0.4.4/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:43:08.000000 scikit-rt-0.4.4/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-25 08:43:08.000000 scikit-rt-0.4.4/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 08:43:08.000000 scikit-rt-0.4.4/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.198419 scikit-rt-0.4.4/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.198419 scikit-rt-0.4.4/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   132020 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    73050 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.194419 scikit-rt-0.4.4/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.198419 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.198419 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39459 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   240666 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   105267 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   132720 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    52538 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   351006 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.198419 scikit-rt-0.4.4/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:43:09.202419 scikit-rt-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    58059 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-25 08:38:57.000000 scikit-rt-0.4.4/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.860000 scikit-rt-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-28 15:46:01.860000 scikit-rt-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-28 15:46:01.863999 scikit-rt-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.812000 scikit-rt-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.816000 scikit-rt-0.4.5/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-28 15:46:01.000000 scikit-rt-0.4.5/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-28 15:46:01.000000 scikit-rt-0.4.5/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:46:01.000000 scikit-rt-0.4.5/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 15:46:01.000000 scikit-rt-0.4.5/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 15:46:01.000000 scikit-rt-0.4.5/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.827999 scikit-rt-0.4.5/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.832000 scikit-rt-0.4.5/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   132020 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73050 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.812000 scikit-rt-0.4.5/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.836000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.840000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39459 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   250886 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105267 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132720 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52538 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   351006 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.843999 scikit-rt-0.4.5/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:46:01.860000 scikit-rt-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61362 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-28 15:40:28.000000 scikit-rt-0.4.5/tests/test_viewer.py
```

### Comparing `scikit-rt-0.4.4/LICENSE` & `scikit-rt-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/PKG-INFO` & `scikit-rt-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.4
+Version: 0.4.5
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.4/README.md` & `scikit-rt-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/pypi.md` & `scikit-rt-0.4.5/pypi.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/setup.cfg` & `scikit-rt-0.4.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.4.4
+version = 0.4.5
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for analysis of radiotherapy data
 long_description = file: pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.4.4/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.4.5/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.4
+Version: 0.4.5
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.4/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.4.5/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.4.5/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/__init__.py` & `scikit-rt-0.4.5/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/application.py` & `scikit-rt-0.4.5/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.4.5/src/skrt/better_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/better_viewer/options.py` & `scikit-rt-0.4.5/src/skrt/better_viewer/options.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/core.py` & `scikit-rt-0.4.5/src/skrt/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.4.5/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/dicom_writer.py` & `scikit-rt-0.4.5/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/dose.py` & `scikit-rt-0.4.5/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/image.py` & `scikit-rt-0.4.5/src/skrt/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Classes for loading and comparing medical images."""
 
 import numbers
 import pathlib
+from inspect import signature
 
 from matplotlib.ticker import MultipleLocator, AutoMinorLocator
 from pydicom.dataset import FileDataset, FileMetaDataset
 import scipy.ndimage
 import scipy.interpolate
 import copy
 import datetime
@@ -16,14 +17,15 @@
 import matplotlib as mpl
 import matplotlib.cm
 import matplotlib.colors
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import nibabel
 import numpy as np
+import pandas as pd
 import os
 import shutil
 import pydicom
 import tempfile
 import time
 import uuid
 import skimage.transform
@@ -50,14 +52,16 @@
 
 # Matplotlib settings
 mpl.rcParams["figure.figsize"] = (7.4, 4.8)
 mpl.rcParams["font.serif"] = "Times New Roman"
 mpl.rcParams["font.family"] = "serif"
 mpl.rcParams["font.size"] = 14.0
 
+skrt.core.Defaults().foreground_name = "foreground"
+
 class Image(skrt.core.Archive):
     """
     Class representing a medical image.
 
     Attributes of an Image object should usually be accessed via
     their getter methods, rather than directly, to ensure that
     attribute values have been loaded.
@@ -1192,17 +1196,17 @@
         try:
             z_array = np.linspace(z, z + (nz - 1) * dz, nz)
         except TypeError:
             z_array = None
 
         return (x_array, y_array, z_array)
 
-    def get_foreground_box_mask(self, dx=0, dy=0, threshold=-200):
+    def get_foreground_box_mask(self, dx=0, dy=0, threshold=-150):
         '''
-        Slice by slice, create rectangular mask encolosing foreground mask.
+        Slice by slice, create rectangular mask enclosing foreground mask.
 
         dx : int, default=0
             Margin along columns to be added on each side of mask bounding box.
 
         dy : int, default=0
             Margin along rows to be added on each side of mask bounding box.
 
@@ -1212,15 +1216,15 @@
         '''
 
         foreground_mask = self.get_foreground_mask(threshold)
         foreground_box_mask = get_box_mask_from_mask(foreground_mask, dx, dy)
 
         return foreground_box_mask
 
-    def get_foreground_bbox(self, threshold=None, convex_hull=False,
+    def get_foreground_bbox(self, threshold=-150, convex_hull=False,
             fill_holes=True, dxy=0):
         """
         Obtain bounding box of image foreground.
 
         The bounding box is returned as
         [(xmin, xmax), (ymin, ymax), (zmin, zmax)], with values in mm.
 
@@ -1228,30 +1232,122 @@
         to obtain a mask defining the image foreground.  For parameter
         explanations, see skrt.image.Image.get_foreground_mask() documentation.
         """
         return (get_mask_bbox(
             self.get_foreground_mask(threshold, convex_hull, fill_holes, dxy)))
 
     def get_foreground_bbox_centre_and_widths(self,
-            threshold=None, convex_hull=False, fill_holes=True, dxy=0):
+            threshold=-150, convex_hull=False, fill_holes=True, dxy=0):
         """
         Get centre and widths in mm along all three axes of a
         bounding box enclosing the image foreground.  Centre
         and widths are returned as a tuple ([x, y, z], [dx, dy, dz]).
 
         Method parameters are passed to skrt.image.Image.get_foreground_mask()
         to obtain a mask defining the image foreground.  For parameter
         explanations, see skrt.image.Image.get_foreground_mask() documentation.
         """
         extents = self.get_foreground_bbox()
         centre = [0.5 * (extent[0] + extent[1]) for extent in extents]
         widths = [(extent[1] - extent[0]) for extent in extents]
         return (centre, widths)
 
-    def get_foreground_mask(self, threshold=None, convex_hull=False,
+    def get_foreground_comparison(
+            self, other, name=None, threshold=-150, convex_hull=False,
+            fill_holes=True, dxy=0, voxel_size=None, **kwargs):
+        """
+        Return a pandas DataFrame comparing the foregrounds of
+        this image and another.
+
+        ROIs obtaining the image foregrounds are obtained, then
+        these are compared using skrt.structures.ROI.get_comparison().
+
+        **Parameters:**
+
+        other: skrt.image.Image
+            Image with which this image is to be compared.
+
+        name: str, default=None
+            Name to be assigned to the ROI representing the foreground
+            of this image, and by default used as row index in DataFrame.
+            If null, the name used is the image title, or if this is null
+            then f"{skrt.core.Defaults().foreground_name}_1" is used.
+
+        threshold : int/float, default=None
+            Intensity value above which pixels in a slice are assigned to
+            regions for determination of foreground.
+    
+        convex_hull : bool, default=False
+            If True, create mask from the convex hulls of the
+            slice foreground masks initially obtained.
+
+        fill_holes : bool, default=False
+            If True, fill holes in the slice foreground masks initially
+            obtained.
+
+        dxy : int, default=0
+            Margin, in pixel units, to be added to each slice foreground mask.
+
+        voxel_size : tuple, default=None
+            Voxel size (dx, dy, dz) in mm passed to
+            skrt.structures.ROI.get_comparison().  The default there
+            (1, 1, 1) is different from the default set here (None).
+
+        kwargs: dict
+            Keyword arguments, in addition to voxel_size, passed to
+            skrt.structures.ROI.get_comparison().
+        """
+        name = (name or self.title
+                or f"{skrt.core.Defaults().foreground_name}_1")
+        roi1 = self.get_foreground_roi(
+                threshold=threshold, convex_hull=convex_hull,
+                fill_holes=fill_holes, dxy=dxy, name=name)
+        roi2 = other.get_foreground_roi(
+                threshold=threshold, convex_hull=convex_hull,
+                fill_holes=fill_holes, dxy=dxy)
+
+        return roi1.get_comparison(roi2, voxel_size=voxel_size, **kwargs)
+
+    def get_foreground_roi(self, threshold=-150, convex_hull=False,
+            fill_holes=True, dxy=0, **kwargs):
+        '''
+        Create ROI represening image foreground.
+
+        Slice by slice, the foreground is taken to correspond to the
+        largest region of contiguous pixels above a threshold value.
+        A binary mask representing the foreground is created, and
+        is used as source for creating an ROI.
+
+        **Parameters:**
+
+        threshold : int/float, default=None
+            Intensity value above which pixels in a slice are assigned to
+            regions for determination of foreground.
+    
+        convex_hull : bool, default=False
+            If True, create mask from the convex hulls of the
+            slice foreground masks initially obtained.
+
+        fill_holes : bool, default=False
+            If True, fill holes in the slice foreground masks initially
+            obtained.
+
+        dxy : int, default=0
+            Margin, in pixel units, to be added to each slice foreground mask.
+
+        **kwargs
+            Keyword arguments passed to ROI constructor.
+        '''
+        from skrt.structures import ROI
+        if not "name" in kwargs:
+            kwargs["name"] = skrt.core.Defaults().foreground_name
+        return ROI(self.get_foreground_mask(
+            threshold, convex_hull, fill_holes, dxy), **kwargs)
+
+    def get_foreground_mask(self, threshold=-150, convex_hull=False,
             fill_holes=True, dxy=0):
         '''
         Create foreground mask.
 
         Slice by slice, the foreground is taken to correspond to the
         largest region of contiguous pixels above a threshold value.
 
@@ -1286,15 +1382,15 @@
         # Clone the current image, and replace its data with
         # the foreground mask.
         out_image = Image(self)
         out_image.data = out_array
 
         return out_image
 
-    def get_slice_foreground(self, idx=0, threshold=None,
+    def get_slice_foreground(self, idx=0, threshold=-150,
             convex_hull=False, fill_holes=False, dxy=0):
         '''
         Create foreground mask for image slice.
 
         The foreground is taken to correspond to the largest region
         of contiguous pixels above a threshold value.
 
@@ -1365,21 +1461,21 @@
                 # Take the convex hull of the mask.
                 label_array2 = skimage.morphology.convex_hull_image(
                         label_array2)
 
         # Handle the cases where all intensities are the same.
         else:
             if test_slice.max() > rescaled_threshold:
-                label_array2 = np.ones(image_slice.shape)
+                label_array2 = np.ones(image_slice.shape, dtype=bool)
             else:
-                label_array2 = np.zeros(image_slice.shape)
+                label_array2 = np.zeros(image_slice.shape, dtype=bool)
 
         return label_array2
 
-    def select_foreground(self, threshold=None, convex_hull=False,
+    def select_foreground(self, threshold=-150, convex_hull=False,
             fill_holes=True, dxy=0, background=None):
         '''
         Modify image to show intensity information only for foreground.
 
         Slice by slice, the foreground is taken to correspond to the
         largest region of contiguous pixels above a threshold value.
         Voxels outside the foreground region are all assigned the
@@ -3863,16 +3959,16 @@
 
             # Find array indices at which to crop
             i1 = im.pos_to_idx(lims[i_ax][0], ax=i_ax, return_int=False)
             i2 = im.pos_to_idx(lims[i_ax][1], ax=i_ax, return_int=False)
             i_big, i_small = i2, i1
             if i1 > i2:
                 i_big, i_small = i_small, i_big
-            i_small = int(np.floor(i_small + 0.5))
-            i_big = int(np.floor(i_big + 0.5))
+            i_small = int(np.floor(round(i_small, 6) + 0.5))
+            i_big = int(np.floor(round(i_big, 6) + 0.5))
 
             # Ensure indices are within image range
             if i_small < 0:
                 i_small = 0
             if i_big > im.n_voxels[i_ax]:
                 i_big = im.n_voxels[i_ax]
 
@@ -4307,16 +4403,143 @@
         if invert_mask:
             masked_image.data = np.ma.masked_where(mask.data, self.data)
         else:
             masked_image.data = np.ma.masked_where(~mask.data, self.data)
 
         return masked_image
 
+    def get_comparison(
+            self, other, metrics=None, name=None, name_as_index=True,
+            nice_columns=False, decimal_places=None,
+            base=2, bins=100, xyrange=None):
+        """
+        Return a pandas DataFrame comparing this image with another.
+
+        If this image doesn't have the same shape and geometry as
+        the other image, comparison metrics are evaluated for a clone
+        of this image, resized to match the other.
+
+        **Parameters:**
+        
+        other : skrt.image.Image
+            Other image, with which to compare this image.
+
+        metrics : list, default=None
+            List of metrics to evaluate.  Available metrics:
+                
+            Calculated in Image.get_mutual_information():
+
+                * "mutual_information";
+                * "normalised_mutual_information";
+                * "information_quality_ratio";
+                * "rajski_distance".
+
+            Calculated in Image.get_quality():
+
+                * "relative_structural_content";
+                * "fidelity";
+                * "correlation_quality".
+
+            If None, defaults to ["mutual_information"]
+
+        name : str, default=None
+            Name identifying comparison.  If null, the name is
+            constructed from the titles of the two images compared,
+            as "title1_vs_title2".
+
+        name_as_index : bool, default=True
+            If True, the index column of the pandas DataFrame will 
+            contain the name of this comparison; otherwise, the name will
+            appear in a column labelled "images".
+
+        nice_columns : bool, default=False
+            If False, column labels will be the same as the input metric names;
+            if True, the names will be capitalized and underscores will be 
+            replaced with spaces.
+
+        decimal_places : int, default=None
+            Number of decimal places to keep for each metric. If None, full
+            precision will be used.
+
+        base : int/None, default=2
+            Base to use when taking logarithms, in calculations of
+            mutual information and variants.  If None, use base e.
+
+        bins : int/list, default=50
+            Numbers of bins to use when histogramming grey-level joint
+            probabilities for self and other, in calculations of
+            mutual information and variants.  This is passed as
+            the bins parameter of numpy.histogram2d:
+            https://numpy.org/doc/stable/reference/generated/numpy.histogram2d.html
+
+        xyrange : list, default=None
+            Upper and lower of each axis when histogramming grey-level
+            joint probabilities for self and image, in calculations of
+            mutual informatio and variants.  This is passed as
+            the range parameter of numpy.histogram2d:
+            https://numpy.org/doc/stable/reference/generated/numpy.histogram2d.html
+        """
+        # Ensure that images for comparison have the same geometry.
+        if self.has_same_geometry(other):
+            im1 = self
+        else:
+            im1 = self.clone()
+            im1.match_size(other)
+        im2 = other
+
+        # Ensure that comparison name is defined.
+        if not name:
+            title1 = im1.title or "image"
+            title2 = im2.title or "other"
+            name = f"{title1}_vs_{title2}"
+
+        # Set default metric.
+        metrics = metrics or ["mutual_information"]
+
+        # Check that specified metrics are recognised,
+        # and identify quality metrics.
+        quality_metrics = []
+        for metric in metrics:
+            if metric not in get_image_comparison_metrics():
+                raise RuntimeError(f"Metric {metric} not recognised by "
+                                   "Image.get_comparison()")
+            if metric in get_quality_metrics():
+                quality_metrics.append(metric)
+
+        # Compute metric scores.
+        quality_scores = im1.get_quality(im2, quality_metrics)
+        scores = {}
+        for metric in metrics:
+            # Store scores for quality metrics.
+            if metric in get_quality_metrics():
+                scores[metric] = quality_scores[metric]
+            # Store scores for mutual information and variants.
+            else:
+                scores[metric] = im1.get_mutual_information(
+                        im2, base=base, bins=bins, xyrange=xyrange,
+                        variant=metric)
+            if decimal_places is not None:
+                scores[metric] = round(scores[metric], decimal_places)
+
+        # Convert to pandas DataFrame.
+        df = pd.DataFrame(scores, index=[name])
+
+        # Turn name into a regular column if requested
+        if not name_as_index:
+            df = df.reset_index().rename({"index": "images"}, axis=1)
+
+        # Capitalize column names and remove underscores if requested.
+        if nice_columns:
+            df.columns = [col.capitalize().replace("_", " ")
+                          if len(col) > 3 else col.upper()
+                          for col in df.columns]
+        return df
+
     def get_mutual_information(self, image, base=2, bins=100, xyrange=None,
-                               variant=None):
+                               variant="mutual_information"):
         """
         For this and another image, calculate mutual information or a variant.
 
         The two images considered must have the same shape.
 
         **Parameters:**
 
@@ -4337,30 +4560,38 @@
             joint probabilities for self and image.  This is passed as
             the range parameter of numpy.histogram2d:
             https://numpy.org/doc/stable/reference/generated/numpy.histogram2d.html
 
         variant : str, default=None
             Variant of mutual information to be returned.
 
+            - "mi", "mutual_information":
+              return mutual information, as introduced in:
+              https://doi.org/10.1002/j.1538-7305.1948.tb01338.x
+
             - "nmi", "normalised_mutual_information":
               return normalised mutual information (range 1 to 2) as defined in:
               https://doi.org/10.1117/12.310835
 
             - "iqr", "information_quality_ratio":
               return information quality ratio (range 0 to 1) as defined in:
               https://doi.org/10.1016/j.chemolab.2016.11.012
               => information_quality_ratio = normalised_mutual_information - 1
 
             - "rajski", "rajski_distance":
               return Rajski distance (range 1 to 0) as defined in:
               https://doi.org/10.1016/S0019-9958(61)80055-7
               => rajski_distance = 2 - normalised_mutual_information
 
-            - Any other value, return mutual information.
+            - Any other value, return None
         """
+        # Check that requested variant is recognised.
+        if not variant in get_mi_metrics():
+            return
+
         # Check base for taking logarithms.
         if base is None:
             base = math.e
 
         # Create 2d histogram of voxel-by-voxel grey-level values,
         # comparing images.
         hist2d, xedges, yedges = np.histogram2d(
@@ -4378,139 +4609,141 @@
         small_number = 1.e-6
         hx = entropy(px, base)
         hy = entropy(py, base)
         hxy = entropy(np.reshape(pxy, -1), base)
 
         mi = hx + hy - hxy
         # Return mutual information or a variant.
+        if variant in ["mi", "mutual_information"]:
+            return mi
         if variant in ["nmi", "normalised_mutual_information"]:
             return 1 + mi / (hxy or small_number)
         elif variant in ["iqr", "information_quality_ratio"]:
             return mi / (hxy or small_number)
         if variant in ["rajski", "rajski_distance"]:
             return 1 - mi / (hxy or small_number)
 
-        return mi
-
-    def get_relative_structural_content(
-            self, image, v_min=None, v_max=None, constant=None):
+    def get_quality(self, image, metrics=None):
         """
-        Quantify structural content of this image relative to another.
+        Evaluate quality of this image relative to another.
+
+        The metrics considered are:
 
-        The calculation of relative structural content is based on
-        the definition of:
+        - relative structural content;
+        - fidelity;
+        - correlation quality.
+
+        These are defined in:
 
         - https://doi.org/10.1364/JOSA.46.000740
         - https://doi.org/10.1080/713826248
 
-        The result should be from 0 (no agreement) to 1 (perfect agreement).
+        The three metrics should each have a value between 0 and 1,
+        and are related by:
+
+        correlation quality = 0.5 * (relative structural content + fidelity).
 
-        The parameters v_min, v_max, constant allow for linear rescaling
-        of image greyscale values prior to calculation of relative
-        structural content.  Any rescaling is performed on clones of
-        the images to be compared, with the originals left unaltered.
+        Quality scores are returned in a dictionary, with a key corresponding
+        to each metric: "relative_structural_content", "fidelity",
+        "correlation_quality".  If a metric isn't evaluated, the value
+        returned for it is None.
 
         **Parameters:**
 
         image : skrt.image.Image
-            Image with respect to which relative structural content
-            is to be calculated.
+            Image with respect to which quality metrics are to be calculated.
 
-        v_min: float, default=None
-            Minimum greyscale value after rescaling.  If None,
-            no rescaling is performed.
+        metrics: list, default=None
+            List of strings specifying quality metrics to be evaluated.
+            If None, all defined quality metrics are evaluated.
+        """
+        # Define metrics to be evaluated.
+        all_metrics = ["relative_structural_content",
+                       "fidelity", "correlation_quality"]
+        if metrics is None:
+            metrics = all_metrics
+        else:
+            if not skrt.core.is_list(metrics):
+                metrics = [metrics]
+            metrics = [metric for metric in metrics if metric in all_metrics]
+
+        # Initialise dictionary of metric values.
+        quality = {metric: None for metric in all_metrics}
+
+        if metrics:
+            # Recale intensity values, so that the minimum is 0.
+            v_min = min(self.get_min(), image.get_min())
+            data1 = self.get_data() - v_min
+            data2 = image.get_data() - v_min
+
+            # If intensity values have non-zero sum, normalise to 1.
+            if data1.sum():
+                data1 = data1 / data1.sum()
+            if data2.sum():
+                data2 = data2 / data2.sum()
+
+            # Evaluate quality metrics.
+            denominator = (data2**2).sum()
+            metric = "relative_structural_content"
+            if metric in metrics:
+                quality[metric] = (data1**2).sum() / denominator
+            metric = "fidelity"
+            if metric in metrics:
+                quality[metric] = (
+                        1 - (((data2 - data1)**2).sum() / denominator))
+            metric = "correlation_quality"
+            if metric in metrics:
+                quality[metric] = (data2 * data1).sum() / denominator
 
-        v_max: float, default=None
-            Maximum greyscale value after rescaling.  If None,
-            no rescaling is performed.
+        return quality
 
-        constant: float, default=None
-            Greyscale value to assign after rescaling if all values
-            in the original image are the same.  If None,
-            original value is kept.
+    def get_relative_structural_content(self, image):
         """
-        im1, im2 = rescale_images([self, image], v_min, v_max, constant)
-        return ((im1.get_data()**2).sum() / (im2.get_data()**2).sum())
+        Calculate structural content of this image relative to another.
 
-    def get_fidelity(self, image, v_min=None, v_max=None, constant=None):
-        """
-        Calculate fidelity with which this image matches another.
+        Uses method get_quality().
 
-        The calculation of fidelity is based on the definition of:
+        **Parameter:**
 
-        - https://doi.org/10.1364/JOSA.46.000740
-        - https://doi.org/10.1080/713826248
+        image : skrt.image.Image
+            Image with respect to which relative structural content is
+            to be evaluated
+        """
+        metric = "relative_structural_content"
+        return self.get_quality(image, metrics=[metric])[metric]
 
-        The result should be from 0 (no agreement) to 1 (perfect agreement).
+    def get_fidelity(self, image):
+        """
+        Calculate fidelity with which this image matches another.
 
-        The parameters v_min, v_max, constant allow for linear rescaling
-        of image greyscale values prior to calculation of fidelity.  Any
-        rescaling is performed on clones of the images to be compared,
-        with the originals left unaltered.
+        Uses method get_quality().
 
-        **Parameters:**
+        **Parameter:**
 
         image : skrt.image.Image
             Image with respect to which fidelity is to be calculated.
-
-        v_min: float, default=None
-            Minimum greyscale value after rescaling.  If None,
-            no rescaling is performed.
-
-        v_max: float, default=None
-            Maximum greyscale value after rescaling.  If None,
-            no rescaling is performed.
-
-        constant: float, default=None
-            Greyscale value to assign after rescaling if all values
-            in the original image are the same.  If None,
-            original value is kept.
+            to be evaluated
         """
-        im1, im2 = rescale_images([self, image], v_min, v_max, constant)
-        return (1 - (((im2.get_data() - im1.get_data())**2).sum()
-                / (im2.get_data()**2).sum()))
+        metric = "fidelity"
+        return self.get_quality(image, metrics=[metric])[metric]
 
-    def get_correlation_quality(
-            self, image, v_min=None, v_max=None, constant=None):
+    def get_correlation_quality(self, image):
         """
         Calculate quality of correlation between this image and another.
 
-        The calculation of correlation quality is based on the definition of:
+        Uses method get_quality().
 
-        - https://doi.org/10.1364/JOSA.46.000740
-        - https://doi.org/10.1080/713826248
-
-        The result should be from 0 (no agreement) to 1 (perfect agreement).
-
-        The parameters v_min, v_max, constant allow for linear rescaling
-        of image greyscale values prior to calculation of correlation
-        quality.  Any rescaling is performed on clones of the images
-        to be compared, with the originals left unaltered.
-
-        **Parameters:**
+        **Parameter:**
 
         image : skrt.image.Image
             Image with respect to which correlation quality is to be calculated.
-
-        v_min: float, default=None
-            Minimum greyscale value after rescaling.  If None,
-            no rescaling is performed.
-
-        v_max: float, default=None
-            Maximum greyscale value after rescaling.  If None,
-            no rescaling is performed.
-
-        constant: float, default=None
-            Greyscale value to assign after rescaling if all values
-            in the original image are the same.  If None,
-            original value is kept.
+            to be evaluated
         """
-        im1, im2 = rescale_images([self, image], v_min, v_max, constant)
-        return ((im2.get_data() * im1.get_data()).sum()
-                / (im2.get_data()**2).sum())
+        metric = "correlation_quality"
+        return self.get_quality(image, metrics=[metric])[metric]
 
 
 class ImageComparison(Image):
     """Plot comparisons of two images and calculate comparison metrics."""
 
     def __init__(self, im1, im2, plot_type="overlay", title=None, **kwargs):
 
@@ -6311,14 +6544,18 @@
         method skrt.image.Image.apply_banding().
     """
     im1 = im1.clone_with_structure_set(ss1, roi_names, ss1_index, ss1_name)
     ss1 = im1.structure_sets[0] if im1.structure_sets else None
     im2 = im2.clone_with_structure_set(ss2, roi_names, ss2_index, ss1_name)
     ss2 = im2.structure_sets[0] if im2.structure_sets else None
 
+    if alignment is not False:
+        im1.crop_to_image(im2, alignment)
+        im2.crop_to_image(im1, alignment)
+
     # Resample images to same voxel size.
     match_image_voxel_sizes(im1, im2, voxel_size)
 
     # Crop im2 to region around focus.
     if ss2 is not None and im2_crop_focus in ss2.get_roi_names():
         im2.crop_to_roi(ss2[im2_crop_focus], crop_margins=im2_crop_margins,
                         crop_about_centre=im2_crop_about_centre)
@@ -6326,14 +6563,17 @@
           and skrt.core.is_list(im2_crop_margins)):
         im2.crop_about_point(im2_crop_focus, *im2_crop_margins)
 
     # Crop images to same size.
     if alignment is not False:
         im1.crop_to_image(im2, alignment)
         im2.crop_to_image(im1, alignment)
+        if (im1.get_voxel_size() == im2.get_voxel_size()
+            and not im1.has_same_geometry(im2)):
+            im1.match_size(im1)
 
     # Perform banding of image grey levels.
     im1.apply_selective_banding(bands)
     im2.apply_selective_banding(bands)
 
     # Reset structure-set images.
     for im, ss in [(im1, ss1), (im2, ss2)]:
@@ -6367,17 +6607,17 @@
            specified dimensions in mm.
          - dxyz: both images are resampled, to have voxels with the
            specified dimension in mm along all axes.
 
     order: int, default = 1
         Order of the b-spline used in interpolating voxel intensity values.
     """
-    # No resampling needed:V
+    # No resampling needed.
     if not voxel_size:
-        return
+        return (im1, im2)
 
     # Initialise voxel sizes for resampled images.
     vs1 = None
     vs2 = None
 
     # If voxel size specified by a single number,
     # convert to a list with this number repeated.
@@ -6575,7 +6815,49 @@
         images = [image.clone() for image in images]
 
     # Perform rescaling.
     for image in images:
         image.rescale(v_min=v_min, v_max=v_max, constant=constant)
 
     return images
+
+def get_image_comparison_metrics():
+    """
+    Get list of image-comparison metrics.
+
+    This returns the combined list of metrics based on mutual information
+    (returned by get_mi_metrics()) and quality metrics
+    (returned by get_quality_metrics()).
+    """
+    return (get_mi_metrics() + get_quality_metrics())
+
+def get_mi_metrics():
+    """
+    Get list of metrics based on mutual information.
+
+    All metrics listed here should be recognised by
+    Image.get_mutual_information(), and all metrics recognised by
+    Image.get_mutual_information() should be listed here.
+    """
+    return [
+            "iqr",
+            "information_quality_ratio",
+            "mi",
+            "mutual_information",
+            "nmi",
+            "normalised_mutual_information",
+            "rajski",
+            "rajski_distance",
+            ]
+
+def get_quality_metrics():
+    """
+    Get list of metrics measuring quality of one metric relative to another.
+
+    All metrics listed here should be recognised by Image.get_quality(),
+    and all metrics recognised by Image.get_quality() should be listed here.
+    """
+    return [
+            "correlation_quality",
+            "fidelity",
+            "relative_structural_content",
+            ]
```

### Comparing `scikit-rt-0.4.4/src/skrt/multi.py` & `scikit-rt-0.4.5/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/patient.py` & `scikit-rt-0.4.5/src/skrt/patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/registration.py` & `scikit-rt-0.4.5/src/skrt/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
                     f"found for registration step {step} listed in "
                     f"{self.steps_file}. This step will be ignored."
                 )
                 continue
 
             pfile = os.path.join(outdir, "InputParameters.txt")
             tfile = self.get_tfile(outdir)
-            if not os.path.exists(pfile) and not tifle:
+            if not os.path.exists(pfile) and not tfile:
                 self.logger.warning(
                     f"No parameter file ({pfile}) "
                     f"and no transform file ({outdir}/TransformParameters*) "
                     f"found for registration step {step} listed in "
                     f"{self.steps_file}. This step will be ignored."
                 )
                 continue
```

### Comparing `scikit-rt-0.4.4/src/skrt/segmentation.py` & `scikit-rt-0.4.5/src/skrt/segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/simulation.py` & `scikit-rt-0.4.5/src/skrt/simulation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/structures.py` & `scikit-rt-0.4.5/src/skrt/structures.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/viewer/core.py` & `scikit-rt-0.4.5/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/src/skrt/viewer/viewer.py` & `scikit-rt-0.4.5/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_01_setup.py` & `scikit-rt-0.4.5/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_application.py` & `scikit-rt-0.4.5/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_core.py` & `scikit-rt-0.4.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_dose.py` & `scikit-rt-0.4.5/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_image.py` & `scikit-rt-0.4.5/tests/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 from pathlib import Path
 
 import math
 import os
 import random
 import pytest
 import numpy as np
+import pandas as pd
 import shutil
 import pydicom
 
 from pydicom._storage_sopclass_uids import\
         PositronEmissionTomographyImageStorage
 
-from skrt.core import File, fullpath
+from skrt.core import Defaults, File, fullpath
 from skrt.image import (Image, checked_crop_limits, get_alignment_translation,
-                        get_geometry, get_mask_bbox, get_translation_to_align,
+                        get_geometry, get_image_comparison_metrics,
+                        get_mask_bbox, get_translation_to_align,
                         match_images, match_image_voxel_sizes, rescale_images)
 from skrt.simulation import SyntheticImage
+from skrt.structures import ROI
 
 try:
     import mahotas
     has_mahotas = True
 except ModuleNotFoundError:
     has_mahotas = False
 
@@ -881,30 +884,64 @@
     sim.add_cube(side_length=5, name="cube", centre=(25, 60, 12), intensity=60)
     sim.add_sphere(radius=10, name="sphere", centre=(80, 20, 12), intensity=50)
 
     # Should detect sphere in first loop and cube in second
     for intensity in [50, 60]:
         threshold = intensity - 5
         mask1 = sim.get_foreground_mask(threshold=threshold).get_data()
-        mask1 = mask1.astype(np.uint32)
-        mask1[mask1 > 0] =1
+        assert mask1.dtype == bool
 
         nx, ny, nz = sim.get_n_voxels()
         mask2 = np.zeros((ny, nx, nz), dtype=np.uint32)
-        mask2[sim.get_data() == intensity] = 1
+        mask2[sim.get_data() == intensity] = True
 
         assert mask1.shape == mask2.shape
         assert mask1.min() == 0
         assert mask1.max() == 1
         assert mask1.min() == mask2.min()
         assert mask1.max() == mask2.max()
         assert mask1.sum() == mask2.sum()
     assert np.all(mask1 == mask2)
 
 @needs_mahotas
+def test_get_foreground_roi():
+    """Test creation of ROI representing image foreground."""
+    # Create synthetic image, featuring cube and sphere.
+    sim = SyntheticImage((100, 100, 40))
+    cube_length = 5
+    sphere_radius = 10
+
+    shapes = {
+            "cube": [cube_length, (25, 60, 12), 60, cube_length**3],
+            "sphere": [sphere_radius, (80, 20, 12), 50,
+                       (4. / 3.) * math.pi * sphere_radius**3],
+            }
+
+    for name, values in shapes.items():
+        length, centre, intensity, volume = values
+        if "cube" == name:
+            sim.add_cube(length, centre, intensity, name=name)
+        elif "sphere" == name:
+            sim.add_sphere(length, centre, intensity, name=name)
+
+    # Should detect sphere as foreground in first loop and cube in second.
+    for name, values in shapes.items():
+        length, centre, intensity, volume = values
+        threshold = intensity - 5
+        roi = sim.get_foreground_roi(threshold=threshold, name=name)
+        assert isinstance(roi, ROI)
+        assert roi.name == name
+        assert roi.get_volume() == pytest.approx(volume, rel=0.005)
+        assert tuple(roi.get_centre()) == centre
+
+    # For case where no name is specified, check that default is assigned.
+    roi = sim.get_foreground_roi(threshold=threshold)
+    assert roi.name == Defaults().foreground_name
+
+@needs_mahotas
 def test_mask_bbox():
     """Test calculation of mask bounding box."""
 
     # Create synthetic image featuring a sphere.
     sim = SyntheticImage((100, 100, 40))
     centre = (80, 20, 12)
     radius = 10
@@ -1544,42 +1581,87 @@
         assert np.all(im2.data == v_fill)
 
 def test_get_relative_structural_content():
     """Test calculation of relative structural content."""
     # For image compared with itself,
     # check that relative structural content is 1.
     im1 = create_test_image(shape, voxel_size, origin)
-    for v_min, v_max in [(None, None), (0, 1)]:
-        assert im1.get_relative_structural_content(im1, v_min, v_max) == 1
+    assert im1.get_relative_structural_content(im1) == 1
 
-    # For image of zeros (after rescaling), compared with another image,
+    # For image of zeros, compared with another image,
     # check that relative structural content is 0.
-    im2 = im1.clone()
-    im2.data.fill(5)
-    assert im2.get_relative_structural_content(
-            im1, v_min=0, v_max=1, constant=0) == 0
+    im2 = create_test_image(shape, voxel_size, origin, "zeros")
+    assert im2.get_relative_structural_content(im1) == 0
 
 def test_get_fidelity():
     """Test calculation of fidelity."""
     # For image compared with itself, check that fidelity is 1.
     im1 = create_test_image(shape, voxel_size, origin)
-    for v_min, v_max in [(None, None), (0, 1)]:
-        assert im1.get_fidelity(im1, v_min, v_max) == 1
+    assert im1.get_fidelity(im1) == 1
 
-    # For image of zeros (after rescaling), compared with another image,
+    # For image of zeros, compared with another image,
     # check that fidelity is 0.
-    im2 = im1.clone()
-    im2.data.fill(5)
-    assert im2.get_fidelity(im1, v_min=0, v_max=1, constant=0) == 0
+    im2 = create_test_image(shape, voxel_size, origin, "zeros")
+    assert im2.get_fidelity(im1) == 0
 
 def test_get_correlation_quality():
     """Test calculation of correlation quality."""
     # For image compared with itself, check that correlation_quality is 1.
     im1 = create_test_image(shape, voxel_size, origin)
-    for v_min, v_max in [(None, None), (0, 1)]:
-        assert im1.get_correlation_quality(im1, v_min, v_max) == 1
+    assert im1.get_correlation_quality(im1) == 1
 
-    # For image of zeros (after rescaling), compared with another image,
+    # For image of zeros, compared with another image,
     # check that correlation quality is 0.
-    im2 = im1.clone()
-    im2.data.fill(5)
-    assert im2.get_correlation_quality(im1, v_min=0, v_max=1, constant=0) == 0
+    im2 = create_test_image(shape, voxel_size, origin, "zeros")
+    assert im2.get_correlation_quality(im1) == 0
+
+def test_get_quality():
+    """Test quality of image with respect to another image."""
+    # Create test images, and perform comparison.
+    im1 = create_test_image(shape, voxel_size, origin)
+    im2 = create_test_image(shape, voxel_size, origin)
+
+    metrics = {
+            "relative_structural_content" : 1,
+            "fidelity" : 0.5,
+            "correlation_quality" : 0.75
+            }
+
+    # Check that only None values returned for null or invalid metrics.
+    for metric in [[], "", "unknown_metric"]:
+        scores = im1.get_quality(im2, metric)
+        assert isinstance(scores, dict)
+        assert len(scores) == len(metrics)
+        assert all([score is None for score in scores.values()])
+
+    # Check that scores are as expected for images with random intensity values.
+    scores = im1.get_quality(im2, list(metrics))
+    assert isinstance(scores, dict)
+    assert len(scores) == len(metrics)
+    for metric, score in metrics.items():
+        assert scores[metric] == pytest.approx(score, abs=0.02)
+
+def test_get_image_comparison_metrics():
+    """Check that get_image_comparison_metrics() returns a list of strings."""
+    metrics = get_image_comparison_metrics()
+    assert isinstance(metrics, list)
+    for metric in metrics:
+        assert isinstance(metric, str)
+
+def test_get_comparison():
+    """Test evaluation of image-comparison metrics."""
+    # Create test images, and perform comparison.
+    im1 = create_test_image(shape, voxel_size, origin)
+    im2 = create_test_image(shape, voxel_size, origin)
+    metrics = get_image_comparison_metrics()
+    comparison = im1.get_comparison(im2, metrics=metrics)
+
+    # Check that resulting DataFrame is as expected.
+    assert isinstance(comparison, pd.DataFrame)
+    assert comparison.shape[0] == 1
+    assert comparison.shape[1] == len(metrics)
+    assert list(comparison.columns) == metrics
+
+    # Check that exception is raised for unknown metric.
+    with pytest.raises(RuntimeError) as error_info:
+        comparison = im1.get_comparison(im2, metrics=["unknown_metric"])
+    assert "Metric unknown_metric not recognised" in str(error_info.value)
```

### Comparing `scikit-rt-0.4.4/tests/test_multi.py` & `scikit-rt-0.4.5/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_patient.py` & `scikit-rt-0.4.5/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_qv_image.py` & `scikit-rt-0.4.5/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_qv_quickviewer.py` & `scikit-rt-0.4.5/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_qv_struct_loader.py` & `scikit-rt-0.4.5/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_qv_struct_metrics.py` & `scikit-rt-0.4.5/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_qv_structs.py` & `scikit-rt-0.4.5/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_registration.py` & `scikit-rt-0.4.5/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_roi_metrics.py` & `scikit-rt-0.4.5/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_segmentation.py` & `scikit-rt-0.4.5/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_structs.py` & `scikit-rt-0.4.5/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_synthetic_image.py` & `scikit-rt-0.4.5/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.4/tests/test_viewer.py` & `scikit-rt-0.4.5/tests/test_viewer.py`

 * *Files identical despite different names*

