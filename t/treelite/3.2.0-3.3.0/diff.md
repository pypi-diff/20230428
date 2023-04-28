# Comparing `tmp/treelite-3.2.0.tar.gz` & `tmp/treelite-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treelite-3.2.0.tar", last modified: Mon Mar 27 20:14:16 2023, max compression
+gzip compressed data, was "treelite-3.3.0.tar", last modified: Fri Apr 28 00:37:19 2023, max compression
```

## Comparing `treelite-3.2.0.tar` & `treelite-3.3.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.474122 treelite-3.2.0/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      250 2022-02-03 01:31:21.000000 treelite-3.2.0/MANIFEST.in
--rw-r--r--   0 phcho     (1000) phcho     (1000)      659 2023-03-27 20:14:16.474122 treelite-3.2.0/PKG-INFO
--rw-r--r--   0 phcho     (1000) phcho     (1000)       38 2023-03-27 20:14:16.474122 treelite-3.2.0/setup.cfg
--rw-r--r--   0 phcho     (1000) phcho     (1000)    10961 2022-11-29 02:15:48.000000 treelite-3.2.0/setup.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.426123 treelite-3.2.0/treelite/
--rw-r--r--   0 phcho     (1000) phcho     (1000)     4363 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite/CMakeLists.txt
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    11357 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite/LICENSE
--rw-r--r--   0 phcho     (1000) phcho     (1000)        6 2023-03-27 20:13:47.000000 treelite-3.2.0/treelite/VERSION
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      628 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/__init__.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2852 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/annotator.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.430123 treelite-3.2.0/treelite/cmake/
--rw-r--r--   0 phcho     (1000) phcho     (1000)      425 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/cmake/Doxygen.cmake
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1786 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/cmake/ExternalLibs.cmake
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      345 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/cmake/FetchContentMakeAvailable.cmake
--rw-r--r--   0 phcho     (1000) phcho     (1000)       72 2023-03-27 20:13:47.000000 treelite-3.2.0/treelite/cmake/Python_version.in
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1818 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/cmake/Sanitizer.cmake
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      305 2022-02-03 09:03:26.000000 treelite-3.2.0/treelite/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2228 2022-09-01 09:31:43.000000 treelite-3.2.0/treelite/cmake/Utils.cmake
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      527 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/cmake/Version.cmake
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      312 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/cmake/version.h.in
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      356 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/compat.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.430123 treelite-3.2.0/treelite/contrib/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    11489 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/contrib/__init__.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1263 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/contrib/gcc.py
--rw-r--r--   0 phcho     (1000) phcho     (1000)     4294 2022-02-17 23:56:59.000000 treelite-3.2.0/treelite/contrib/msvc.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     5829 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/contrib/util.py
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2011 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/core.py
--rw-r--r--   0 phcho     (1000) phcho     (1000)    43172 2023-03-25 05:33:02.000000 treelite-3.2.0/treelite/frontend.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.430123 treelite-3.2.0/treelite/gallery/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      279 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/gallery/__init__.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.430123 treelite-3.2.0/treelite/gallery/sklearn/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      433 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/gallery/sklearn/__init__.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.430123 treelite-3.2.0/treelite/gtil/
--rw-r--r--   0 phcho     (1000) phcho     (1000)      163 2023-03-02 19:43:55.000000 treelite-3.2.0/treelite/gtil/__init__.py
--rw-r--r--   0 phcho     (1000) phcho     (1000)     6858 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/gtil/gtil.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.426123 treelite-3.2.0/treelite/include/
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.434123 treelite-3.2.0/treelite/include/treelite/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1775 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/include/treelite/annotator.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     3554 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/include/treelite/base.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    43517 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/c_api.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     3870 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/c_api_common.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1599 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/include/treelite/c_api_error.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     7754 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/c_api_runtime.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2298 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/compiler.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2076 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/compiler_param.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     4836 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/include/treelite/data.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)      498 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/include/treelite/error.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     1164 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/filesystem.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    28276 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/include/treelite/frontend.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     1321 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/include/treelite/frontend_impl.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     4998 2023-03-02 19:43:55.000000 treelite-3.2.0/treelite/include/treelite/gtil.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     6095 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/include/treelite/logging.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1237 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/include/treelite/math.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)      818 2022-02-12 10:43:13.000000 treelite-3.2.0/treelite/include/treelite/omp.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     1470 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/include/treelite/omp_exception.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1129 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/include/treelite/optional.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     7569 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/include/treelite/predictor.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      551 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/include/treelite/thread_local.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    34061 2023-03-25 05:33:02.000000 treelite-3.2.0/treelite/include/treelite/tree.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    34465 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/include/treelite/tree_impl.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     5913 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/include/treelite/typeinfo.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2780 2023-03-21 07:57:45.000000 treelite-3.2.0/treelite/libpath.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.434123 treelite-3.2.0/treelite/serialize/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)       16 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/serialize/__init__.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1597 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/serialize/__main__.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.434123 treelite-3.2.0/treelite/sklearn/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     4562 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/sklearn/__init__.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2238 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/sklearn/common.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1803 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/sklearn/gbm_classifier.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2009 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/sklearn/gbm_multi_classifier.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1629 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/sklearn/gbm_regressor.py
--rw-r--r--   0 phcho     (1000) phcho     (1000)    17226 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/sklearn/importer.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1473 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/sklearn/rf_classifier.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1620 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/sklearn/rf_multi_classifier.py
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1459 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/sklearn/rf_regressor.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.466122 treelite-3.2.0/treelite/src/
--rw-r--r--   0 phcho     (1000) phcho     (1000)     5907 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/CMakeLists.txt
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    10797 2023-01-07 03:05:24.000000 treelite-3.2.0/treelite/src/annotator.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.466122 treelite-3.2.0/treelite/src/c_api/
--rw-r--r--   0 phcho     (1000) phcho     (1000)    25123 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/c_api/c_api.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2192 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/c_api/c_api_common.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1190 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/c_api/c_api_error.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     5005 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/c_api/c_api_runtime.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.466122 treelite-3.2.0/treelite/src/compiler/
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/compiler/ast/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     6316 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/ast.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3691 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/build.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3695 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/builder.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1163 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/dump.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3645 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/fold_code.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1306 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/is_categorical_array.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1231 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/load_data_counts.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3662 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/quantize.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2934 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast/split.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    30563 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/ast_native.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      758 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/ast_native.h
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/compiler/common/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1111 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/common/categorical_bitmap.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     6519 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/common/code_folding_util.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3942 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/common/format_util.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3131 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/compiler.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/compiler/elf/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    10806 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/elf/elf_formatter.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1380 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/elf/elf_formatter.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    15086 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/compiler/failsafe.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      832 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/failsafe.h
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/compiler/native/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1630 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/native/code_folder_template.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1598 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/native/header_template.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1868 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/native/main_template.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     7131 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/native/pred_transform.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1871 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/native/qnode_template.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     3481 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/src/compiler/native/typeinfo_ctypes.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     6152 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/pred_transform.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      533 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/compiler/pred_transform.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     7752 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/data.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2696 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/filesystem.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/frontend/
--rw-r--r--   0 phcho     (1000) phcho     (1000)    22602 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/frontend/builder.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)    10562 2023-03-25 05:33:02.000000 treelite-3.2.0/treelite/src/frontend/json_importer.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    21059 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/frontend/lightgbm.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)    22631 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/frontend/sklearn.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/frontend/xgboost/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1125 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/frontend/xgboost/xgboost.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    18057 2023-02-08 04:25:28.000000 treelite-3.2.0/treelite/src/frontend/xgboost/xgboost_json.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    16921 2022-06-01 08:18:33.000000 treelite-3.2.0/treelite/src/frontend/xgboost.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)    27874 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/frontend/xgboost_json.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2501 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/frontend/xgboost_util.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/gtil/
--rw-r--r--   0 phcho     (1000) phcho     (1000)     1572 2023-03-02 19:43:55.000000 treelite-3.2.0/treelite/src/gtil/config.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     4357 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/gtil/pred_transform.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)      577 2022-02-03 01:31:21.000000 treelite-3.2.0/treelite/src/gtil/pred_transform.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)    34278 2023-03-10 04:29:56.000000 treelite-3.2.0/treelite/src/gtil/predict.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)     6687 2023-03-25 05:33:02.000000 treelite-3.2.0/treelite/src/json_serializer.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)      618 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/src/logging.cc
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     1652 2023-01-07 03:27:59.000000 treelite-3.2.0/treelite/src/model_concat.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/predictor/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)    19155 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/predictor/predictor.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/predictor/thread_pool/
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     3435 2022-02-03 09:02:56.000000 treelite-3.2.0/treelite/src/predictor/thread_pool/spsc_queue.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)     4108 2022-02-17 23:56:59.000000 treelite-3.2.0/treelite/src/predictor/thread_pool/thread_pool.h
--rw-rw-r--   0 phcho     (1000) phcho     (1000)     2240 2022-09-29 22:11:36.000000 treelite-3.2.0/treelite/src/serializer.cc
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.470122 treelite-3.2.0/treelite/src/threading_utils/
--rw-r--r--   0 phcho     (1000) phcho     (1000)     4181 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/src/threading_utils/parallel_for.h
--rw-r--r--   0 phcho     (1000) phcho     (1000)      627 2022-08-30 21:28:39.000000 treelite-3.2.0/treelite/src/typeinfo.cc
--rw-r--r--   0 phcho     (1000) phcho     (1000)     2066 2023-03-21 01:57:17.000000 treelite-3.2.0/treelite/util.py
-drwxr-xr-x   0 phcho     (1000) phcho     (1000)        0 2023-03-27 20:14:16.430123 treelite-3.2.0/treelite.egg-info/
--rw-r--r--   0 phcho     (1000) phcho     (1000)      659 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite.egg-info/PKG-INFO
--rw-r--r--   0 phcho     (1000) phcho     (1000)     4292 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite.egg-info/SOURCES.txt
--rw-r--r--   0 phcho     (1000) phcho     (1000)        1 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite.egg-info/dependency_links.txt
--rw-r--r--   0 phcho     (1000) phcho     (1000)        1 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite.egg-info/not-zip-safe
--rw-r--r--   0 phcho     (1000) phcho     (1000)       41 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite.egg-info/requires.txt
--rw-r--r--   0 phcho     (1000) phcho     (1000)       21 2023-03-27 20:14:16.000000 treelite-3.2.0/treelite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.619170 treelite-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 00:36:18.000000 treelite-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 00:37:19.619170 treelite-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:37:19.619170 treelite-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-28 00:36:18.000000 treelite-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/annotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Doxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/ExternalLibs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/FetchContentMakeAvailable.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Python_version.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/Version.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/cmake/version.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/gcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/msvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45355 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gallery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/gallery/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gallery/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gtil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/gtil/gtil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.603170 treelite-3.3.0/treelite/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/include/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/annotator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/c_api_runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/compiler_param.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/frontend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/frontend_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/gtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/omp_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/optional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/predictor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/thread_local.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/tree_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/include/treelite/typeinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/libpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/serialize/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/gbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/gbm_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/gbm_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/rf_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/rf_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/sklearn/rf_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/annotator.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.611170 treelite-3.3.0/treelite/src/c_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api_common.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api_error.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/c_api/c_api_runtime.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/build.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/dump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/fold_code.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/is_categorical_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/load_data_counts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/quantize.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast/split.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast_native.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/ast_native.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/common/categorical_bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/common/code_folding_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/common/format_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/compiler.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/failsafe.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/failsafe.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/compiler/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/code_folder_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/header_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/main_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/qnode_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/native/typeinfo_ctypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/compiler/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/filesystem.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/json_importer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/lightgbm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/sklearn.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/frontend/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost/xgboost.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost/xgboost_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/frontend/xgboost_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/config.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/gtil/predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/json_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/model_concat.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.615170 treelite-3.3.0/treelite/src/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/predictor/predictor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.619170 treelite-3.3.0/treelite/src/predictor/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/predictor/thread_pool/spsc_queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/predictor/thread_pool/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/serializer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.619170 treelite-3.3.0/treelite/src/threading_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/threading_utils/parallel_for.h
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/src/typeinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-28 00:36:18.000000 treelite-3.3.0/treelite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:19.607170 treelite-3.3.0/treelite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 00:37:19.000000 treelite-3.3.0/treelite.egg-info/top_level.txt
```

### Comparing `treelite-3.2.0/PKG-INFO` & `treelite-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite
-Version: 3.2.0
+Version: 3.3.0
 Summary: Treelite: model compiler for decision trees
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite-3.2.0/setup.py` & `treelite-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/CMakeLists.txt` & `treelite-3.3.0/treelite/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 set (CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
 cmake_minimum_required (VERSION 3.13)
-project(treelite LANGUAGES CXX C VERSION 3.2.0)
+project(treelite LANGUAGES CXX C VERSION 3.3.0)
 
 # check MSVC version
 if(MSVC)
   if(MSVC_VERSION LESS 1910)
     message(FATAL_ERROR "Need Visual Studio 2017 or newer to compile Treelite")
   endif()
 endif()
```

### Comparing `treelite-3.2.0/treelite/LICENSE` & `treelite-3.3.0/treelite/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/__init__.py` & `treelite-3.3.0/treelite/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/annotator.py` & `treelite-3.3.0/treelite/annotator.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/cmake/ExternalLibs.cmake` & `treelite-3.3.0/treelite/cmake/ExternalLibs.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/cmake/Sanitizer.cmake` & `treelite-3.3.0/treelite/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/cmake/Utils.cmake` & `treelite-3.3.0/treelite/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/cmake/Version.cmake` & `treelite-3.3.0/treelite/cmake/Version.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/contrib/__init__.py` & `treelite-3.3.0/treelite/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/contrib/gcc.py` & `treelite-3.3.0/treelite/contrib/gcc.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/contrib/msvc.py` & `treelite-3.3.0/treelite/contrib/msvc.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/contrib/util.py` & `treelite-3.3.0/treelite/contrib/util.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/core.py` & `treelite-3.3.0/treelite/core.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/frontend.py` & `treelite-3.3.0/treelite/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,31 @@
             Please see :doc:`/notes-on-serialization`.
 
         Parameters
         ----------
         filename : :py:class:`str <python:str>`
             Path to checkpoint
         """
-        _check_call(_LIB.TreeliteSerializeModel(c_str(filename), self.handle))
+        _check_call(_LIB.TreeliteSerializeModelToFile(self.handle, c_str(filename)))
+
+    def serialize_bytes(self) -> bytes:
+        """
+        Serialize (persist) the model to a byte sequence, using a fast binary representation.
+        To recover the model from the byte sequence, use :py:func:`deserialize_bytes` method.
+
+        .. note:: Notes on forward and backward compatibility
+
+            Please see :doc:`/notes-on-serialization`.
+        """
+        char_ptr_t = ctypes.POINTER(ctypes.c_char)
+        out_bytes = char_ptr_t()
+        out_bytes_len = ctypes.c_size_t()
+        _check_call(_LIB.TreeliteSerializeModelToBytes(
+            self.handle, ctypes.byref(out_bytes), ctypes.byref(out_bytes_len)))
+        return ctypes.string_at(out_bytes, out_bytes_len.value)
 
     def dump_as_json(self, *, pretty_print=True):
         """
         Dump the model as a JSON string. This is useful for inspecting details of the tree ensemble
         model.
 
         .. note::
@@ -122,15 +138,44 @@
 
         Returns
         -------
         model : :py:class:`Model` object
             Recovered model
         """
         handle = ctypes.c_void_p()
-        _check_call(_LIB.TreeliteDeserializeModel(c_str(filename), ctypes.byref(handle)))
+        _check_call(_LIB.TreeliteDeserializeModelFromFile(c_str(filename), ctypes.byref(handle)))
+        return Model(handle)
+
+    @classmethod
+    def deserialize_bytes(cls, model_bytes: bytes) -> Model:
+        """
+        Deserialize (recover) the model from a byte sequence. It is expected that
+        the byte sequence was generated by a call to the :py:func:`serialize_bytes` method.
+
+        .. note:: Notes on forward and backward compatibility
+
+            Please see :doc:`/notes-on-serialization`.
+
+        Parameters
+        ----------
+        model_bytes : :py:class:`bytes <python:bytes>`
+            Byte sequence representing the serialized model
+
+        Returns
+        -------
+        model : :py:class:`Model` object
+            Recovered model
+        """
+        handle = ctypes.c_void_p()
+        model_bytes_len = len(model_bytes)
+        buffer = ctypes.create_string_buffer(model_bytes, model_bytes_len)
+        _check_call(_LIB.TreeliteDeserializeModelFromBytes(
+            ctypes.POINTER(ctypes.c_char)(buffer),
+            ctypes.c_size_t(model_bytes_len),
+            ctypes.byref(handle)))
         return Model(handle)
 
     @property
     def num_tree(self):
         """Number of decision trees in the model"""
         if self.handle is None:
             raise AttributeError('Model not loaded yet')
@@ -505,14 +550,18 @@
         filename: str,
         model_format: str,
         allow_unknown_field: Optional[bool] = False
     ):
         """
         Load a tree ensemble model from a file
 
+        .. note::
+
+            To load scikit-learn models, use :py:meth:`~treelite.sklearn.import_model` instead.
+
         Parameters
         ----------
         filename : str
             Path to model file
         model_format : str
             Model file format. Must be "xgboost", "xgboost_json", or "lightgbm"
         allow_unknown_field: bool, optional
@@ -563,14 +612,20 @@
         json_str: str
     ) -> Model:
         """
         Import a tree ensemble model from a JSON string.
 
         See :doc:`tutorials/json_import` for details.
 
+        .. note:: ``import_from_json()`` is strict about which JSON strings to accept
+
+            Some tree libraries let users to export models as JSON strings, but in
+            general :py:meth:`~treelite.Model.import_from_json` will not accept them.
+            See the warning at the top of :doc:`tutorials/json_import`.
+
         .. note::
 
             The operation performed in :py:meth:`~treelite.Model.import_from_json`
             is strictly one-way. So the output of
             :py:meth:`~treelite.Model.dump_as_json` will differ from the JSON
             string you used in calling :py:meth:`~treelite.Model.import_from_json`.
```

### Comparing `treelite-3.2.0/treelite/gtil/gtil.py` & `treelite-3.3.0/treelite/gtil/gtil.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/annotator.h` & `treelite-3.3.0/treelite/include/treelite/annotator.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/base.h` & `treelite-3.3.0/treelite/include/treelite/base.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/c_api.h` & `treelite-3.3.0/treelite/include/treelite/c_api.h`

 * *Files 2% similar despite different names*

```diff
@@ -501,30 +501,61 @@
  * \param handle model
  * \param limit number of trees to keep
  * \return 0 for success, -1 for failure
  */
 TREELITE_DLL int TreeliteSetTreeLimit(ModelHandle handle, size_t limit);
 
 /*!
+ * \brief Deprecated. Please use \ref TreeliteSerializeModelToFile instead.
+ */
+TREELITE_DLL int TreeliteSerializeModel(const char* filename, ModelHandle handle);
+
+/*!
+ * \brief Deprecated. Please use \ref TreeliteDeserializeModelFromFile instead.
+ */
+TREELITE_DLL int TreeliteDeserializeModel(const char* filename, ModelHandle* out);
+
+/*!
  * \brief Serialize (persist) a model object to disk
- * \param filename name of the file to which to serialize the model. The file will be using a
+ * \param handle Handle to the model object
+ * \param filename Name of the file to which to serialize the model. The file will be using a
  *                 binary format that's optimized to store the Treelite model object efficiently.
- * \param handle handle to the model object
  * \return 0 for success, -1 for failure
  */
-TREELITE_DLL int TreeliteSerializeModel(const char* filename, ModelHandle handle);
+TREELITE_DLL int TreeliteSerializeModelToFile(ModelHandle handle, const char* filename);
 
 /*!
  * \brief Deserialize (load) a model object from disk
- * \param filename name of the file from which to deserialize the model. The file should be created
- *                 by a call to TreeliteSerializeModel().
+ * \param filename Name of the file from which to deserialize the model. The file should be created
+ *                 by a call to \ref TreeliteSerializeModelToFile.
  * \param out Handle to the model object
  * \return 0 for success, -1 for failure
  */
-TREELITE_DLL int TreeliteDeserializeModel(const char* filename, ModelHandle* out);
+TREELITE_DLL int TreeliteDeserializeModelFromFile(const char* filename, ModelHandle* out);
+
+/*!
+ * \brief Serialize (persist) a model object to a byte sequence
+ * \param handle Handle to the model object
+ * \param out_bytes Byte sequence containing serialized model
+ * \param out_bytes_len Length of out_bytes
+ * \return 0 for success, -1 for failure
+ */
+TREELITE_DLL int TreeliteSerializeModelToBytes(
+    ModelHandle handle, const char** out_bytes, size_t* out_bytes_len);
+
+/*!
+ * \brief Deserialize (load) a model object from a byte sequence
+ * \param bytes Byte sequence containing serialized model. The string should be created by a call to
+ *              \ref TreeliteSerializeModelToBytes.
+ * \param bytes_len Length of bytes
+ * \param out Handle to the model object
+ * \return 0 for success, -1 for failure
+ */
+TREELITE_DLL int TreeliteDeserializeModelFromBytes(
+    const char* bytes, size_t bytes_len, ModelHandle* out);
 
 /*!
  * \brief Concatenate multiple model objects into a single model object by copying
  *        all member trees into the destination model object
  * \param objs Pointer to the beginning of the list of model objects
  * \param len Number of model objects
  * \param out Used to save the concatenated model
```

### Comparing `treelite-3.2.0/treelite/include/treelite/c_api_common.h` & `treelite-3.3.0/treelite/include/treelite/c_api_common.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/c_api_error.h` & `treelite-3.3.0/treelite/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/c_api_runtime.h` & `treelite-3.3.0/treelite/include/treelite/c_api_runtime.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/compiler.h` & `treelite-3.3.0/treelite/include/treelite/compiler.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/compiler_param.h` & `treelite-3.3.0/treelite/include/treelite/compiler_param.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/data.h` & `treelite-3.3.0/treelite/include/treelite/data.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/filesystem.h` & `treelite-3.3.0/treelite/include/treelite/filesystem.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/frontend.h` & `treelite-3.3.0/treelite/include/treelite/frontend.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/frontend_impl.h` & `treelite-3.3.0/treelite/include/treelite/frontend_impl.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/gtil.h` & `treelite-3.3.0/treelite/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/logging.h` & `treelite-3.3.0/treelite/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/math.h` & `treelite-3.3.0/treelite/include/treelite/math.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/omp.h` & `treelite-3.3.0/treelite/include/treelite/omp.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/omp_exception.h` & `treelite-3.3.0/treelite/include/treelite/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/optional.h` & `treelite-3.3.0/treelite/include/treelite/optional.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/predictor.h` & `treelite-3.3.0/treelite/include/treelite/predictor.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/thread_local.h` & `treelite-3.3.0/treelite/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/include/treelite/tree.h` & `treelite-3.3.0/treelite/include/treelite/tree.h`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #include <treelite/base.h>
 #include <treelite/version.h>
 #include <treelite/logging.h>
 #include <algorithm>
 #include <map>
 #include <memory>
-#include <ostream>
+#include <iostream>
 #include <sstream>
 #include <string>
 #include <vector>
 #include <utility>
 #include <type_traits>
 #include <limits>
 #include <cstddef>
@@ -378,20 +378,20 @@
   Tree(Tree&&) noexcept = default;
   Tree& operator=(Tree&&) noexcept = default;
 
   inline Tree<ThresholdType, LeafOutputType> Clone() const;
 
   inline const char* GetFormatStringForNode();
   inline void GetPyBuffer(std::vector<PyBufferFrame>* dest);
-  inline void SerializeToFile(FILE* dest_fp);
+  inline void SerializeToStream(std::ostream& os);
   // Load a Tree object from a sequence of PyBuffer frames
   // Returns the updated position of the cursor in the sequence
   inline std::vector<PyBufferFrame>::iterator
     InitFromPyBuffer(std::vector<PyBufferFrame>::iterator it);
-  inline void DeserializeFromFile(FILE* src_fp);
+  inline void DeserializeFromStream(std::istream& is);
 
  private:
   // vector of nodes
   ContiguousArray<Node> nodes_;
   ContiguousArray<LeafOutputType> leaf_vector_;
   // Map nid to the start and end index in leaf_vector_
   // We could use std::pair, but it is not POD, so easier to use two vectors
@@ -803,16 +803,16 @@
 
   /* In-memory serialization, zero-copy */
   TREELITE_DLL_EXPORT std::vector<PyBufferFrame> GetPyBuffer();
   TREELITE_DLL_EXPORT static std::unique_ptr<Model>
     CreateFromPyBuffer(std::vector<PyBufferFrame> frames);
 
   /* Serialization to a file stream */
-  void SerializeToFile(FILE* dest_fp);
-  static std::unique_ptr<Model> DeserializeFromFile(FILE* src_fp);
+  void SerializeToStream(std::ostream& os);
+  static std::unique_ptr<Model> DeserializeFromStream(std::istream& is);
 
   /*!
    * \brief number of features used for the model.
    * It is assumed that all feature indices are between 0 and [num_feature]-1.
    */
   int32_t num_feature{0};
   /*! \brief Task type */
@@ -836,20 +836,20 @@
   int32_t patch_ver_;
 
  private:
   TypeInfo threshold_type_{TypeInfo::kInvalid};
   TypeInfo leaf_output_type_{TypeInfo::kInvalid};
   // Internal functions for serialization
   virtual void GetPyBuffer(std::vector<PyBufferFrame>* dest) = 0;
-  virtual void SerializeToFileImpl(FILE* dest_fp) = 0;
+  virtual void SerializeToStreamImpl(std::ostream& os) = 0;
   // Load a Model object from a sequence of PyBuffer frames
   // Returns the updated position of the cursor in the sequence
   virtual std::vector<PyBufferFrame>::iterator InitFromPyBuffer(
     std::vector<PyBufferFrame>::iterator it, std::size_t num_frame) = 0;
-  virtual void DeserializeFromFileImpl(FILE* src_fp) = 0;
+  virtual void DeserializeFromStreamImpl(std::istream& is) = 0;
   template <typename HeaderPrimitiveFieldHandlerFunc>
   inline void SerializeTemplate(HeaderPrimitiveFieldHandlerFunc header_primitive_field_handler);
   template <typename HeaderPrimitiveFieldHandlerFunc>
   inline static void DeserializeTemplate(
       HeaderPrimitiveFieldHandlerFunc header_primitive_field_handler,
       int32_t& major_ver, int32_t& minor_ver, int32_t& patch_ver,
       TypeInfo& threshold_type, TypeInfo& leaf_output_type);
@@ -874,20 +874,20 @@
     return trees.size();
   }
   void SetTreeLimit(std::size_t limit) override {
     return trees.resize(limit);
   }
 
   inline void GetPyBuffer(std::vector<PyBufferFrame>* dest) override;
-  inline void SerializeToFileImpl(FILE* dest_fp) override;
+  inline void SerializeToStreamImpl(std::ostream& os) override;
   // Load a ModelImpl object from a sequence of PyBuffer frames
   // Returns the updated position of the cursor in the sequence
   inline std::vector<PyBufferFrame>::iterator InitFromPyBuffer(
     std::vector<PyBufferFrame>::iterator it, std::size_t num_frame) override;
-  inline void DeserializeFromFileImpl(FILE* src_fp) override;
+  inline void DeserializeFromStreamImpl(std::istream& is) override;
 
  private:
   template <typename HeaderPrimitiveFieldHandlerFunc, typename HeaderCompositeFieldHandlerFunc,
       typename TreeHandlerFunc>
   inline void SerializeTemplate(
       HeaderPrimitiveFieldHandlerFunc header_primitive_field_handler,
       HeaderCompositeFieldHandlerFunc header_composite_field_handler,
```

### Comparing `treelite-3.2.0/treelite/include/treelite/tree_impl.h` & `treelite-3.3.0/treelite/include/treelite/tree_impl.h`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #include <unordered_map>
 #include <sstream>
 #include <iomanip>
 #include <typeinfo>
 #include <stdexcept>
 #include <iostream>
 #include <cstddef>
+#include <cstdint>
 
 namespace {
 
 template <typename T>
 inline std::string GetString(T x) {
   return std::to_string(x);
 }
@@ -453,73 +454,57 @@
     throw Error("nitem must be 1 for a scalar");
   }
   T* t = static_cast<T*>(buffer.buf);
   *scalar = *t;
 }
 
 template <typename T>
-inline void ReadScalarFromFile(T* scalar, FILE* fp) {
+inline void ReadScalarFromStream(T* scalar, std::istream& is) {
   static_assert(std::is_standard_layout<T>::value, "T must be in the standard layout");
-  if (std::fread(scalar, sizeof(T), 1, fp) < 1) {
-    throw Error("Could not read a scalar");
-  }
+  is.read(reinterpret_cast<char*>(scalar), sizeof(T));
 }
 
 template <typename T>
-inline void WriteScalarToFile(T* scalar, FILE* fp) {
+inline void WriteScalarToStream(T* scalar, std::ostream& os) {
   static_assert(std::is_standard_layout<T>::value, "T must be in the standard layout");
-  if (std::fwrite(scalar, sizeof(T), 1, fp) < 1) {
-    throw Error("Could not write a scalar");
-  }
+  os.write(reinterpret_cast<const char*>(scalar), sizeof(T));
 }
 
 template <typename T>
-inline void ReadArrayFromFile(ContiguousArray<T>* vec, FILE* fp) {
-  uint64_t nelem;
-  if (std::fread(&nelem, sizeof(nelem), 1, fp) < 1) {
-    throw Error("Could not read the number of elements");
-  }
+inline void ReadArrayFromStream(ContiguousArray<T>* vec, std::istream& is) {
+  std::uint64_t nelem;
+  is.read(reinterpret_cast<char*>(&nelem), sizeof(nelem));
   vec->Clear();
   vec->Resize(nelem);
   if (nelem == 0) {
     return;  // handle empty arrays
   }
-  const auto nelem_size_t = static_cast<std::size_t>(nelem);
-  if (std::fread(vec->Data(), sizeof(T), nelem_size_t, fp) < nelem_size_t) {
-    throw Error("Could not read an array");
-  }
+  is.read(reinterpret_cast<char*>(vec->Data()), sizeof(T) * nelem);
 }
 
 template <typename T>
-inline void WriteArrayToFile(ContiguousArray<T>* vec, FILE* fp) {
-  static_assert(sizeof(uint64_t) >= sizeof(size_t), "size_t too large");
-  const auto nelem = static_cast<uint64_t>(vec->Size());
-  if (std::fwrite(&nelem, sizeof(nelem), 1, fp) < 1) {
-    throw Error("Could not write the number of elements");
-  }
+inline void WriteArrayToStream(ContiguousArray<T>* vec, std::ostream& os) {
+  static_assert(sizeof(std::uint64_t) >= sizeof(std::size_t), "size_t too large");
+  const auto nelem = static_cast<std::uint64_t>(vec->Size());
+  os.write(reinterpret_cast<const char*>(&nelem), sizeof(nelem));
   if (nelem == 0) {
     return;  // handle empty arrays
   }
-  const auto nelem_size_t = vec->Size();
-  if (std::fwrite(vec->Data(), sizeof(T), nelem_size_t, fp) < nelem_size_t) {
-    throw Error("Could not write an array");
-  }
+  os.write(reinterpret_cast<const char*>(vec->Data()), sizeof(T) * vec->Size());
 }
 
-inline void SkipOptFieldInFile(FILE* fp) {
-  uint16_t elem_size;
-  uint64_t nelem;
-  ReadScalarFromFile(&elem_size, fp);
-  ReadScalarFromFile(&nelem, fp);
-
-  const uint64_t nbytes = elem_size * nelem;
-  TREELITE_CHECK_LE(nbytes, std::numeric_limits<long>::max());  // NOLINT
-  if (std::fseek(fp, static_cast<long>(nbytes), SEEK_CUR) != 0) {  // NOLINT
-    throw Error("Reached end of file");
-  }
+inline void SkipOptFieldInStream(std::istream& is) {
+  std::uint16_t elem_size;
+  std::uint64_t nelem;
+  ReadScalarFromStream(&elem_size, is);
+  ReadScalarFromStream(&nelem, is);
+
+  const std::uint64_t nbytes = elem_size * nelem;
+  TREELITE_CHECK_LE(nbytes, std::numeric_limits<std::streamoff>::max());  // NOLINT
+  is.seekg(static_cast<std::streamoff>(nbytes), std::ios::cur);
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 Tree<ThresholdType, LeafOutputType>::Tree(bool use_opt_field)
   : use_opt_field_(use_opt_field)
 {}
 
@@ -624,23 +609,23 @@
     dest->push_back(GetPyBufferFromArray(field, format));
   };
   SerializeTemplate(scalar_handler, primitive_array_handler, composite_array_handler);
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline void
-Tree<ThresholdType, LeafOutputType>::SerializeToFile(FILE* dest_fp) {
-  auto scalar_handler = [dest_fp](auto* field) {
-    WriteScalarToFile(field, dest_fp);
+Tree<ThresholdType, LeafOutputType>::SerializeToStream(std::ostream& os) {
+  auto scalar_handler = [&os](auto* field) {
+    WriteScalarToStream(field, os);
   };
-  auto primitive_array_handler = [dest_fp](auto* field) {
-    WriteArrayToFile(field, dest_fp);
+  auto primitive_array_handler = [&os](auto* field) {
+    WriteArrayToStream(field, os);
   };
-  auto composite_array_handler = [dest_fp](auto* field, const char* format) {
-    WriteArrayToFile(field, dest_fp);
+  auto composite_array_handler = [&os](auto* field, const char* format) {
+    WriteArrayToStream(field, os);
   };
   SerializeTemplate(scalar_handler, primitive_array_handler, composite_array_handler);
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline std::vector<PyBufferFrame>::iterator
 Tree<ThresholdType, LeafOutputType>::InitFromPyBuffer(std::vector<PyBufferFrame>::iterator it) {
@@ -656,23 +641,23 @@
   };
   DeserializeTemplate(scalar_handler, array_handler, skip_opt_field_handler);
   return new_it;
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline void
-Tree<ThresholdType, LeafOutputType>::DeserializeFromFile(FILE* src_fp) {
-  auto scalar_handler = [src_fp](auto* field) {
-    ReadScalarFromFile(field, src_fp);
+Tree<ThresholdType, LeafOutputType>::DeserializeFromStream(std::istream& is) {
+  auto scalar_handler = [&is](auto* field) {
+    ReadScalarFromStream(field, is);
   };
-  auto array_handler = [src_fp](auto* field) {
-    ReadArrayFromFile(field, src_fp);
+  auto array_handler = [&is](auto* field) {
+    ReadArrayFromStream(field, is);
   };
-  auto skip_opt_field_handler = [src_fp]() {
-    SkipOptFieldInFile(src_fp);
+  auto skip_opt_field_handler = [&is]() {
+    SkipOptFieldInStream(is);
   };
   DeserializeTemplate(scalar_handler, array_handler, skip_opt_field_handler);
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline void Tree<ThresholdType, LeafOutputType>::Node::Init() {
   std::memset(this, 0, sizeof(Node));
@@ -976,24 +961,24 @@
   };
   header_primitive_field_handler(&num_tree_);
   SerializeTemplate(header_primitive_field_handler, header_composite_field_handler, tree_handler);
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline void
-ModelImpl<ThresholdType, LeafOutputType>::SerializeToFileImpl(FILE* dest_fp) {
-  num_tree_ = static_cast<uint64_t>(this->trees.size());
-  auto header_primitive_field_handler = [dest_fp](auto* field) {
-    WriteScalarToFile(field, dest_fp);
+ModelImpl<ThresholdType, LeafOutputType>::SerializeToStreamImpl(std::ostream& os) {
+  num_tree_ = static_cast<std::uint64_t>(this->trees.size());
+  auto header_primitive_field_handler = [&os](auto* field) {
+    WriteScalarToStream(field, os);
   };
-  auto header_composite_field_handler = [dest_fp](auto* field, const char* format) {
-    WriteScalarToFile(field, dest_fp);
+  auto header_composite_field_handler = [&os](auto* field, const char* format) {
+    WriteScalarToStream(field, os);
   };
-  auto tree_handler = [dest_fp](Tree<ThresholdType, LeafOutputType>& tree) {
-    tree.SerializeToFile(dest_fp);
+  auto tree_handler = [&os](Tree<ThresholdType, LeafOutputType>& tree) {
+    tree.SerializeToStream(os);
   };
   header_primitive_field_handler(&num_tree_);
   SerializeTemplate(header_primitive_field_handler, header_composite_field_handler, tree_handler);
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline std::vector<PyBufferFrame>::iterator
@@ -1028,27 +1013,27 @@
   TREELITE_CHECK_EQ(num_tree_, this->trees.size());
 
   return new_it;
 }
 
 template <typename ThresholdType, typename LeafOutputType>
 inline void
-ModelImpl<ThresholdType, LeafOutputType>::DeserializeFromFileImpl(FILE* src_fp) {
-  ReadScalarFromFile(&num_tree_, src_fp);
+ModelImpl<ThresholdType, LeafOutputType>::DeserializeFromStreamImpl(std::istream& is) {
+  ReadScalarFromStream(&num_tree_, is);
 
-  auto header_field_handler = [src_fp](auto* field) {
-    ReadScalarFromFile(field, src_fp);
+  auto header_field_handler = [&is](auto* field) {
+    ReadScalarFromStream(field, is);
   };
 
-  auto skip_opt_field_handler = [src_fp]() {
-    SkipOptFieldInFile(src_fp);
+  auto skip_opt_field_handler = [&is]() {
+    SkipOptFieldInStream(is);
   };
 
-  auto tree_handler = [src_fp](Tree<ThresholdType, LeafOutputType>& tree) {
-    tree.DeserializeFromFile(src_fp);
+  auto tree_handler = [&is](Tree<ThresholdType, LeafOutputType>& tree) {
+    tree.DeserializeFromStream(is);
   };
 
   DeserializeTemplate(num_tree_, header_field_handler, tree_handler, skip_opt_field_handler);
   TREELITE_CHECK_EQ(num_tree_, this->trees.size());
 }
 
 inline void InitParamAndCheck(ModelParam* param,
```

### Comparing `treelite-3.2.0/treelite/include/treelite/typeinfo.h` & `treelite-3.3.0/treelite/include/treelite/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/libpath.py` & `treelite-3.3.0/treelite/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/serialize/__main__.py` & `treelite-3.3.0/treelite/serialize/__main__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/__init__.py` & `treelite-3.3.0/treelite/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/common.py` & `treelite-3.3.0/treelite/sklearn/common.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/gbm_classifier.py` & `treelite-3.3.0/treelite/sklearn/gbm_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/gbm_multi_classifier.py` & `treelite-3.3.0/treelite/sklearn/gbm_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/gbm_regressor.py` & `treelite-3.3.0/treelite/sklearn/gbm_regressor.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/importer.py` & `treelite-3.3.0/treelite/sklearn/importer.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/rf_classifier.py` & `treelite-3.3.0/treelite/sklearn/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/rf_multi_classifier.py` & `treelite-3.3.0/treelite/sklearn/rf_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/sklearn/rf_regressor.py` & `treelite-3.3.0/treelite/sklearn/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/CMakeLists.txt` & `treelite-3.3.0/treelite/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/annotator.cc` & `treelite-3.3.0/treelite/src/annotator.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/c_api/c_api.cc` & `treelite-3.3.0/treelite/src/c_api/c_api.cc`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 #include <treelite/math.h>
 #include <treelite/gtil.h>
 #include <treelite/logging.h>
 #include <numeric>
 #include <memory>
 #include <algorithm>
 #include <fstream>
+#include <sstream>
 #include <string>
-#include <cstdio>
 #include <cstddef>
 
 using namespace treelite;
 
 namespace {
 
 /*! \brief entry to to easily hold returning information */
@@ -307,28 +307,70 @@
       threshold, default_left, value, n_node_samples, gain, baseline_prediction);
   *out = static_cast<ModelHandle>(model.release());
   API_END();
 }
 
 int TreeliteSerializeModel(const char* filename, ModelHandle handle) {
   API_BEGIN();
-  FILE* fp = std::fopen(filename, "wb");
-  TREELITE_CHECK(fp) << "Failed to open file '" << filename << "'";
-  auto* model_ = static_cast<Model*>(handle);
-  model_->SerializeToFile(fp);
-  std::fclose(fp);
+  TREELITE_LOG(WARNING)
+      << "TreeliteSerializeModel() is deprecated; "
+      << "please use TreeliteSerializeModelToFile() instead";
+  return TreeliteSerializeModelToFile(handle, filename);
   API_END();
 }
 
 int TreeliteDeserializeModel(const char* filename, ModelHandle* out) {
   API_BEGIN();
-  FILE* fp = std::fopen(filename, "rb");
-  TREELITE_CHECK(fp) << "Failed to open file '" << filename << "'";
-  std::unique_ptr<Model> model = Model::DeserializeFromFile(fp);
-  std::fclose(fp);
+  TREELITE_LOG(WARNING)
+      << "TreeliteDeserializeModel() is deprecated; "
+      << "please use TreeliteDeserializeModelFromFile() instead";
+  return TreeliteDeserializeModelFromFile(filename, out);
+  API_END();
+}
+
+int TreeliteSerializeModelToFile(ModelHandle handle, const char* filename) {
+  API_BEGIN();
+  std::ofstream ofs(filename, std::ios::out | std::ios::binary);
+  TREELITE_CHECK(ofs) << "Failed to open file '" << filename << "'";
+  ofs.exceptions(std::ios::failbit | std::ios::badbit);  // throw exception on failure
+  auto* model_ = static_cast<Model*>(handle);
+  model_->SerializeToStream(ofs);
+  API_END();
+}
+
+int TreeliteDeserializeModelFromFile(const char* filename, ModelHandle* out) {
+  API_BEGIN();
+  std::ifstream ifs(filename, std::ios::in | std::ios::binary);
+  TREELITE_CHECK(ifs) << "Failed to open file '" << filename << "'";
+  ifs.exceptions(std::ios::failbit | std::ios::badbit);  // throw exception on failure
+  std::unique_ptr<Model> model = Model::DeserializeFromStream(ifs);
+  *out = static_cast<ModelHandle>(model.release());
+  API_END();
+}
+
+int TreeliteSerializeModelToBytes(ModelHandle handle, const char** out_bytes,
+                                  size_t* out_bytes_len) {
+  API_BEGIN();
+  std::ostringstream oss;
+  oss.exceptions(std::ios::failbit | std::ios::badbit);  // throw exception on failure
+  auto* model_ = static_cast<Model*>(handle);
+  model_->SerializeToStream(oss);
+
+  std::string& ret_str = TreeliteAPIThreadLocalStore::Get()->ret_str;
+  ret_str = oss.str();
+  *out_bytes = ret_str.data();
+  *out_bytes_len = ret_str.length();
+  API_END();
+}
+
+int TreeliteDeserializeModelFromBytes(const char* bytes, size_t bytes_len, ModelHandle* out) {
+  API_BEGIN();
+  std::istringstream iss(std::string(bytes, bytes_len));
+  iss.exceptions(std::ios::failbit | std::ios::badbit);  // throw exception on failure
+  std::unique_ptr<Model> model = Model::DeserializeFromStream(iss);
   *out = static_cast<ModelHandle>(model.release());
   API_END();
 }
 
 int TreeliteConcatenateModelObjects(const ModelHandle* objs, size_t len,
                                     ModelHandle* out) {
   API_BEGIN();
```

### Comparing `treelite-3.2.0/treelite/src/c_api/c_api_common.cc` & `treelite-3.3.0/treelite/src/c_api/c_api_common.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/c_api/c_api_error.cc` & `treelite-3.3.0/treelite/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/c_api/c_api_runtime.cc` & `treelite-3.3.0/treelite/src/c_api/c_api_runtime.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/ast.h` & `treelite-3.3.0/treelite/src/compiler/ast/ast.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/build.cc` & `treelite-3.3.0/treelite/src/compiler/ast/build.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/builder.h` & `treelite-3.3.0/treelite/src/compiler/ast/builder.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/dump.cc` & `treelite-3.3.0/treelite/src/compiler/ast/dump.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/fold_code.cc` & `treelite-3.3.0/treelite/src/compiler/ast/fold_code.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/is_categorical_array.cc` & `treelite-3.3.0/treelite/src/compiler/ast/is_categorical_array.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/load_data_counts.cc` & `treelite-3.3.0/treelite/src/compiler/ast/load_data_counts.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/quantize.cc` & `treelite-3.3.0/treelite/src/compiler/ast/quantize.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast/split.cc` & `treelite-3.3.0/treelite/src/compiler/ast/split.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast_native.cc` & `treelite-3.3.0/treelite/src/compiler/ast_native.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/ast_native.h` & `treelite-3.3.0/treelite/src/compiler/ast_native.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/common/categorical_bitmap.h` & `treelite-3.3.0/treelite/src/compiler/common/categorical_bitmap.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/common/code_folding_util.h` & `treelite-3.3.0/treelite/src/compiler/common/code_folding_util.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/common/format_util.h` & `treelite-3.3.0/treelite/src/compiler/common/format_util.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/compiler.cc` & `treelite-3.3.0/treelite/src/compiler/compiler.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/elf/elf_formatter.cc` & `treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/elf/elf_formatter.h` & `treelite-3.3.0/treelite/src/compiler/elf/elf_formatter.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/failsafe.cc` & `treelite-3.3.0/treelite/src/compiler/failsafe.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/failsafe.h` & `treelite-3.3.0/treelite/src/compiler/failsafe.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/native/code_folder_template.h` & `treelite-3.3.0/treelite/src/compiler/native/code_folder_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/native/header_template.h` & `treelite-3.3.0/treelite/src/compiler/native/header_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/native/main_template.h` & `treelite-3.3.0/treelite/src/compiler/native/main_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/native/pred_transform.h` & `treelite-3.3.0/treelite/src/compiler/native/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/native/qnode_template.h` & `treelite-3.3.0/treelite/src/compiler/native/qnode_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/native/typeinfo_ctypes.h` & `treelite-3.3.0/treelite/src/compiler/native/typeinfo_ctypes.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/pred_transform.cc` & `treelite-3.3.0/treelite/src/compiler/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/compiler/pred_transform.h` & `treelite-3.3.0/treelite/src/compiler/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/data.cc` & `treelite-3.3.0/treelite/src/data.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/filesystem.cc` & `treelite-3.3.0/treelite/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/builder.cc` & `treelite-3.3.0/treelite/src/frontend/builder.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/json_importer.cc` & `treelite-3.3.0/treelite/src/frontend/json_importer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/lightgbm.cc` & `treelite-3.3.0/treelite/src/frontend/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/sklearn.cc` & `treelite-3.3.0/treelite/src/frontend/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/xgboost/xgboost.h` & `treelite-3.3.0/treelite/src/frontend/xgboost/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/xgboost/xgboost_json.h` & `treelite-3.3.0/treelite/src/frontend/xgboost/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/xgboost.cc` & `treelite-3.3.0/treelite/src/frontend/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/xgboost_json.cc` & `treelite-3.3.0/treelite/src/frontend/xgboost_json.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/frontend/xgboost_util.cc` & `treelite-3.3.0/treelite/src/frontend/xgboost_util.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/gtil/config.cc` & `treelite-3.3.0/treelite/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/gtil/pred_transform.cc` & `treelite-3.3.0/treelite/src/gtil/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/gtil/pred_transform.h` & `treelite-3.3.0/treelite/src/gtil/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/gtil/predict.cc` & `treelite-3.3.0/treelite/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/json_serializer.cc` & `treelite-3.3.0/treelite/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/logging.cc` & `treelite-3.3.0/treelite/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/model_concat.cc` & `treelite-3.3.0/treelite/src/model_concat.cc`

 * *Files 12% similar despite different names*

```diff
@@ -13,32 +13,35 @@
 
 namespace treelite {
 
 std::unique_ptr<Model> ConcatenateModelObjects(const std::vector<const Model*>& objs) {
   if (objs.empty()) {
     return std::unique_ptr<Model>();
   }
-  return objs[0]->Dispatch([&objs](const auto& first_model_obj) {
+  const TypeInfo threshold_type = objs[0]->GetThresholdType();
+  const TypeInfo leaf_output_type = objs[0]->GetLeafOutputType();
+  return objs[0]->Dispatch([&objs, threshold_type, leaf_output_type](const auto& first_model_obj) {
     using ModelType = std::remove_const_t<std::remove_reference_t<decltype(first_model_obj)>>;
-    std::unique_ptr<ModelType> concatenated_model = std::make_unique<ModelType>();
+    std::unique_ptr<Model> concatenated_model = Model::Create(threshold_type, leaf_output_type);
+    auto* concatenated_model_concrete = dynamic_cast<ModelType*>(concatenated_model.get());
     for (std::size_t i = 0; i < objs.size(); ++i) {
       auto* casted = dynamic_cast<const ModelType*>(objs[i]);
       if (casted) {
         std::transform(casted->trees.begin(), casted->trees.end(),
-                       std::back_inserter(concatenated_model->trees),
+                       std::back_inserter(concatenated_model_concrete->trees),
                        [](const auto& tree) { return tree.Clone(); });
       } else {
         TREELITE_LOG(FATAL) << "Model object at index " << i
           << " has a different type than the first model object (at index 0)";
       }
     }
     /* Copy model metadata */
     concatenated_model->num_feature = first_model_obj.num_feature;
     concatenated_model->task_type = first_model_obj.task_type;
     concatenated_model->average_tree_output = first_model_obj.average_tree_output;
     concatenated_model->task_param = first_model_obj.task_param;
     concatenated_model->param = first_model_obj.param;
-    return std::unique_ptr<Model>(concatenated_model.release());
+    return concatenated_model;
   });
 }
 
 }  // namespace treelite
```

### Comparing `treelite-3.2.0/treelite/src/predictor/predictor.cc` & `treelite-3.3.0/treelite/src/predictor/predictor.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/predictor/thread_pool/spsc_queue.h` & `treelite-3.3.0/treelite/src/predictor/thread_pool/spsc_queue.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/predictor/thread_pool/thread_pool.h` & `treelite-3.3.0/treelite/src/predictor/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/serializer.cc` & `treelite-3.3.0/treelite/src/serializer.cc`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
  * \file serializer.cc
  * \brief Implementation for serialization related functions
  * \author Hyunsu Cho
  */
 
 #include <treelite/tree.h>
 #include <treelite/error.h>
+#include <iostream>
 
 namespace treelite {
 
 std::vector<PyBufferFrame>
 Model::GetPyBuffer() {
   std::vector<PyBufferFrame> buffer;
   auto header_primitive_field_handler = [&buffer](auto* field) {
@@ -40,37 +41,37 @@
   model->patch_ver_ = patch_ver;
   std::size_t num_frame = std::distance(it, frames.end());
   model->InitFromPyBuffer(it, num_frame);
   return model;
 }
 
 void
-Model::SerializeToFile(FILE* dest_fp) {
-  auto header_primitive_field_handler = [dest_fp](auto* field) {
-    WriteScalarToFile(field, dest_fp);
+Model::SerializeToStream(std::ostream& os) {
+  auto header_primitive_field_handler = [&os](auto* field) {
+    WriteScalarToStream(field, os);
   };
   SerializeTemplate(header_primitive_field_handler);
-  this->SerializeToFileImpl(dest_fp);
+  this->SerializeToStreamImpl(os);
 }
 
 std::unique_ptr<Model>
-Model::DeserializeFromFile(FILE* src_fp) {
+Model::DeserializeFromStream(std::istream& is) {
   TypeInfo threshold_type, leaf_output_type;
   int idx = 0;
-  auto header_primitive_field_handler = [src_fp](auto* field) {
-    ReadScalarFromFile(field, src_fp);
+  auto header_primitive_field_handler = [&is](auto* field) {
+    ReadScalarFromStream(field, is);
   };
-  int32_t major_ver;
-  int32_t minor_ver;
-  int32_t patch_ver;
+  std::int32_t major_ver;
+  std::int32_t minor_ver;
+  std::int32_t patch_ver;
   DeserializeTemplate(header_primitive_field_handler, major_ver, minor_ver, patch_ver,
     threshold_type, leaf_output_type);
 
   std::unique_ptr<Model> model = Model::Create(threshold_type, leaf_output_type);
   model->major_ver_ = major_ver;
   model->minor_ver_ = minor_ver;
   model->patch_ver_ = patch_ver;
-  model->DeserializeFromFileImpl(src_fp);
+  model->DeserializeFromStreamImpl(is);
   return model;
 }
 
 }  // namespace treelite
```

### Comparing `treelite-3.2.0/treelite/src/threading_utils/parallel_for.h` & `treelite-3.3.0/treelite/src/threading_utils/parallel_for.h`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/src/typeinfo.cc` & `treelite-3.3.0/treelite/src/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite/util.py` & `treelite-3.3.0/treelite/util.py`

 * *Files identical despite different names*

### Comparing `treelite-3.2.0/treelite.egg-info/PKG-INFO` & `treelite-3.3.0/treelite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite
-Version: 3.2.0
+Version: 3.3.0
 Summary: Treelite: model compiler for decision trees
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite-3.2.0/treelite.egg-info/SOURCES.txt` & `treelite-3.3.0/treelite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

