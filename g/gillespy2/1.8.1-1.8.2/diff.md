# Comparing `tmp/gillespy2-1.8.1.tar.gz` & `tmp/gillespy2-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/GillesPy2/GillesPy2/dist/.tmp-t3x395ew/gillespy2-1.8.1.tar", last modified: Tue Mar  7 20:19:56 2023, max compression
+gzip compressed data, was "/home/runner/work/GillesPy2/GillesPy2/dist/.tmp-kvxgmbhi/gillespy2-1.8.2.tar", last modified: Thu Apr 27 21:59:17 2023, max compression
```

## Comparing `gillespy2-1.8.1.tar` & `gillespy2-1.8.2.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-07 20:19:41.000000 gillespy2-1.8.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-03-07 20:19:41.000000 gillespy2-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-07 20:19:41.000000 gillespy2-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-03-07 20:19:56.000000 gillespy2-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-03-07 20:19:41.000000 gillespy2-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/assignmentrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/functiondefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/gillespyError.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/gillespySolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/jsonify.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/liveGraphing.py
--rw-r--r--   0 runner    (1001) docker     (123)    71057 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/raterule.py
--rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/sortableobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/species.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/core/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/sbml/
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/sbml/SBMLexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    18166 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/sbml/SBMLimport.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/sbml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/SConstruct
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/build_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/make.py
--rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/build/template_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/SConscript
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/SConscript
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode.h
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_ls.h
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_proj.h
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_spils.h
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/nvector_serial.h
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_band.h
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_direct.h
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_iterative.h
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_linearsolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_math.h
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nonlinearsolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector.h
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector_senswrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_version.h
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunlinsol_spgmr.h
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_band.h
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_dense.h
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_sparse.h
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunnonlinsol_newton.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/
--rw-r--r--   0 runner    (1001) docker     (123)   134746 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode.c
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_direct.c
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_fused_stubs.c
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    27452 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_io.c
--rw-r--r--   0 runner    (1001) docker     (123)    55908 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls.c
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_nls.c
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj.c
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_spils.c
--rw-r--r--   0 runner    (1001) docker     (123)    46445 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/nvector_serial.c
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_band.c
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_debug.h
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_iterative.c
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_linearsolver.c
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_math.c
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_matrix.c
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nonlinearsolver.c
--rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector.c
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector_senswrapper.c
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_band.c
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_dense.c
--rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_spgmr.c
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_band.c
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_dense.c
--rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_fixedpoint.c
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_newton.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/tau.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/tau.h
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/arg_parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/arg_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/model.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESimulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/SConscript
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASimulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/
--rw-r--r--   0 runner    (1001) docker     (123)    24559 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSimulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.h
--rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/SConscript
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSimulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template.h
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_defaults.h
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_opts.h
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_params.h
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/ode_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/ssa_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/tau_hybrid_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/cpp/tau_leaping_c_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/CLE_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/ode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/ssa_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    60703 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/tau_hybrid_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/numpy/tau_leaping_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/solvers/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/utilities/Tau.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/utilities/cpp_support_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/solvers/utilities/solverutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2/stochss/
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/stochss/StochSSexport.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-07 20:19:41.000000 gillespy2-1.8.1/gillespy2/stochss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 20:19:56.000000 gillespy2-1.8.1/gillespy2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-07 20:19:41.000000 gillespy2-1.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-07 20:19:56.000000 gillespy2-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-03-07 20:19:41.000000 gillespy2-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:19:56.000000 gillespy2-1.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_SBML.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_StochML.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_all_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_build_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_c_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_c_solver_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_c_solver_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_c_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_check_cpp_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_empty_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_example_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_hybrid_c_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_hybrid_event_round.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_hybrid_negative_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_hybrid_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_hybrid_solver_opioid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_jsonify.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_numpy_ssa_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_ode_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_ode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_pause_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_propensity_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_python_solver_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_run_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_simple_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_ssa_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_sys_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_tau_hybrid_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_tau_leaping_c_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_tau_leaping_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_telegraph_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-03-07 20:19:41.000000 gillespy2-1.8.1/test/test_variable_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-27 21:59:05.000000 gillespy2-1.8.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-27 21:59:05.000000 gillespy2-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 21:59:05.000000 gillespy2-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-04-27 21:59:17.000000 gillespy2-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-04-27 21:59:05.000000 gillespy2-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/assignmentrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/functiondefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/gillespyError.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/gillespySolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/liveGraphing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71746 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/raterule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/sortableobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/species.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/core/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/sbml/
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/sbml/SBMLexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/sbml/SBMLimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/sbml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/build_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/build/template_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/SConscript
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/SConscript
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_ls.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_proj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_spils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/nvector_serial.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_band.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_direct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_iterative.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_linearsolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_math.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nonlinearsolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector_senswrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunlinsol_spgmr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_band.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_dense.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_sparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunnonlinsol_newton.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   134746 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_direct.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_fused_stubs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27452 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_io.c
+-rw-r--r--   0 runner    (1001) docker     (123)    55908 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_nls.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_spils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46445 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/nvector_serial.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_band.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_iterative.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_linearsolver.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_math.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_matrix.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nonlinearsolver.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector_senswrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_band.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_dense.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_spgmr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_band.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_dense.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_fixedpoint.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_newton.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/tau.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/tau.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/arg_parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/arg_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/model.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESimulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/SConscript
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASimulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSimulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23070 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/SConscript
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSimulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_defaults.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_params.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/ode_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/ssa_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/tau_hybrid_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/cpp/tau_leaping_c_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/CLE_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/ode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/ssa_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63590 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/tau_hybrid_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/numpy/tau_leaping_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/solvers/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/utilities/Tau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/utilities/cpp_support_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/solvers/utilities/solverutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2/stochss/
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/stochss/StochSSexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 21:59:05.000000 gillespy2-1.8.2/gillespy2/stochss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:59:17.000000 gillespy2-1.8.2/gillespy2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 21:59:05.000000 gillespy2-1.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 21:59:17.000000 gillespy2-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-27 21:59:05.000000 gillespy2-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:59:17.000000 gillespy2-1.8.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_SBML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_StochML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_all_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_build_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_c_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_c_solver_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_c_solver_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_c_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_check_cpp_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_empty_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_example_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_hybrid_c_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_hybrid_event_round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_hybrid_negative_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_hybrid_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_hybrid_solver_opioid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_numpy_ssa_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_ode_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_ode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_pause_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_propensity_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_python_solver_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_simple_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_ssa_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_sys_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_tau_hybrid_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_tau_leaping_c_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_tau_leaping_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_telegraph_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-27 21:59:06.000000 gillespy2-1.8.2/test/test_variable_solvers.py
```

### Comparing `gillespy2-1.8.1/COPYRIGHT` & `gillespy2-1.8.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/LICENSE` & `gillespy2-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/PKG-INFO` & `gillespy2-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gillespy2
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python interface for Gillespie-style biochemical simulations
 Home-page: https://github.com/StochSS/GillesPy2
 Download-URL: https://pypi.org/project/gillespy2/#files
 Author: See AUTHORS
 Author-email: bdrawert@unca.edu
 Maintainer: See AUTHORS
 Maintainer-email: bdrawert@unca.edu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gillespy2 Version: 1.8.1 Summary: Python interface
+Metadata-Version: 2.1 Name: gillespy2 Version: 1.8.2 Summary: Python interface
 for Gillespie-style biochemical simulations Home-page: https://github.com/
 StochSS/GillesPy2 Download-URL: https://pypi.org/project/gillespy2/#files
 Author: See AUTHORS Author-email: bdrawert@unca.edu Maintainer: See AUTHORS
 Maintainer-email: bdrawert@unca.edu License: GPL Project-URL: Tracker, https://
 github.com/StochSS/GillesPy2/issues Project-URL: Source, https://github.com/
 StochSS/GillesPy2 Keywords: biochemical simulation,Gillespie
 algorithm,stochastic simulation,biology Classifier: Development Status :: 5 -
```

### Comparing `gillespy2-1.8.1/README.md` & `gillespy2-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/__init__.py` & `gillespy2-1.8.2/gillespy2/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/__version__.py` & `gillespy2-1.8.2/gillespy2/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # @file    __version__.py
 # @brief   GillesPy2 version info
 # @license Please see the file named LICENSE in the project directory
 # @website https://github.com/StochSS/GillesPy2
 # =============================================================================
 
 
-__version__      = '1.8.1'
+__version__      = '1.8.2'
 
 __title__        = 'GillesPy2'
 __description__  = 'Python interface for Gillespie-style biochemical simulations'
 __url__          = 'https://github.com/StochSS/GillesPy2'
 __download_url__ = 'https://pypi.org/project/gillespy2/#files'
 __author__       = 'See AUTHORS'
 __email__        = 'bdrawert@unca.edu'
```

### Comparing `gillespy2-1.8.1/gillespy2/core/__init__.py` & `gillespy2-1.8.2/gillespy2/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/assignmentrule.py` & `gillespy2-1.8.2/gillespy2/core/assignmentrule.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/cleanup.py` & `gillespy2-1.8.2/gillespy2/core/cleanup.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/events.py` & `gillespy2-1.8.2/gillespy2/core/events.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/functiondefinition.py` & `gillespy2-1.8.2/gillespy2/core/functiondefinition.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/gillespyError.py` & `gillespy2-1.8.2/gillespy2/core/gillespyError.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/gillespySolver.py` & `gillespy2-1.8.2/gillespy2/core/gillespySolver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/jsonify.py` & `gillespy2-1.8.2/gillespy2/core/jsonify.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/liveGraphing.py` & `gillespy2-1.8.2/gillespy2/core/liveGraphing.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/model.py` & `gillespy2-1.8.2/gillespy2/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,18 +67,22 @@
     """
 
     try:
         from gillespy2.sbml.SBMLimport import convert # pylint: disable=import-outside-toplevel
     except ImportError as err:
         raise ImportError('SBML conversion not imported successfully') from err
 
-    return convert(
+    (model,errs) =  convert(
         filename, model_name=name, gillespy_model=gillespy_model,
         report_silently_with_sbml_error=report_silently_with_sbml_error
     )
+    if model.tspan is None:
+        model.timespan(gillespy2.TimeSpan.linspace(t=1))
+
+    return (model, errs)
 
 
 def export_SBML(gillespy_model, filename=None):
     """
     GillesPy model to SBML converter
 
     :param gillespy_model: GillesPy model to be converted to SBML
@@ -210,14 +214,16 @@
             return '\n' + divider + header + divider
 
         print_string = self.name
         if len(self.listOfSpecies):
             print_string += decorate('Species')
             for species in sorted(self.listOfSpecies.values()):
                 print_string += '\n' + str(species)
+                if species.mode is not None:
+                    print_string += ' (' + species.mode + ')'
         if len(self.listOfParameters):
             print_string += decorate('Parameters')
             for parameter in sorted(self.listOfParameters.values()):
                 print_string += '\n' + str(parameter)
         if len(self.listOfReactions):
             print_string += decorate('Reactions')
             for reaction in sorted(self.listOfReactions.values()):
@@ -237,14 +243,16 @@
         if len(self.listOfFunctionDefinitions):
             print_string += decorate('Function Definitions')
             for func_def in sorted(self.listOfFunctionDefinitions.values()):
                 print_string += '\n' + str(func_def)
         if self.tspan is not None:
             print_string += decorate('Timespan')
             print_string += str(self.tspan)
+        else:
+            print_string += decorate('No Timespan found')
         return print_string
 
     def __getitem__(self, key):
         if isinstance(key, str):
             return self.get_element(key)
         if hasattr(self.__class__, "__missing__"):
             return self.__class__.__missing__(self, key)
@@ -1287,14 +1295,24 @@
                 if "CSolver" in solver.name and \
                     ("resume" in solver_args or "variables" in solver_args or "live_output" in solver_args):
                     sol_kwargs['variable'] = True
                 solver = solver(**sol_kwargs)
             except Exception as err:
                 raise SimulationError(f"{solver} is not a valid solver.  Reason Given: {err}.") from err
 
+        if "integrator" in solver_args:
+            raise SimulationError(
+                f"""
+                The integrator argument to run is only supported by the ODESolver.run method. To use the integrator use:
+
+                solver = gillespy2.ODESolver(model=model)
+                results = solver.run(integrator='{solver_args['integrator']}')
+                """
+            )
+
         try:
             return solver.run(t=t, increment=increment, timeout=timeout, **solver_args)
         except Exception as err:
             raise SimulationError(
                 f"argument 'solver={solver}' to run() failed.  Reason Given: {err}"
             ) from err
```

### Comparing `gillespy2-1.8.1/gillespy2/core/parameter.py` & `gillespy2-1.8.2/gillespy2/core/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,10 +117,10 @@
         if coverage in ("all", "expression"):
             if expression is None:
                 expression = self.expression
 
             if expression is None:
                 raise ParameterError("initial_value can't be None type.")
             if not isinstance(expression, str):
-                raise ParameterError("expression must be of type str, float, or int.")
+                raise ParameterError("expression must be of type str.")
             if expression == "":
                 raise ParameterError("expression can't be an empty string.")
```

### Comparing `gillespy2-1.8.1/gillespy2/core/raterule.py` & `gillespy2-1.8.2/gillespy2/core/raterule.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/reaction.py` & `gillespy2-1.8.2/gillespy2/core/reaction.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/results.py` & `gillespy2-1.8.2/gillespy2/core/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,55 +279,62 @@
 
             results = Results(results_list)
             if "type" in live_output_options.keys() and live_output_options['type'] == "graph":
                 results.plot()
             return results
         raise ValueError("number_of_trajectories must be non-negative and non-zero")
 
-    def to_csv(self, path=None, nametag=None, stamp=None):
+    def to_csv(self, path=".", nametag=None, stamp=None, postfix=".odf", verbose=False):
         """
         Outputs the Results to one or more .csv files in a new directory.
 
         :param nametag: allows the user to optionally "tag" the directory and included files. Defaults to the model
             name.
         :type nametag: str
 
         :param path: the location for the new directory and included files. Defaults to model location.
         :type path: str
 
         :param stamp: Allows the user to optionally "tag" the directory (not included files). Default is timestamp.
         :type stamp: str
+
+        :param verbose: Print useful informataion.
+        :type verbose: str
+
+        :returns: Path to the observed data files.
+        :rtype: str
         """
         if stamp is None:
             now = datetime.now()
             stamp = datetime.timestamp(now)
         if nametag is None:
             identifier = self._validate_title(show_title=True)
         else:
             identifier = nametag
-        if path is None:
-            directory = os.path.join(".", str(identifier)+str(stamp))
-        else:
-            directory = os.path.join(path, str(identifier)+str(stamp))
+
+        directory = os.path.join(path, f"{identifier}-{stamp}{postfix}")
+        if verbose:
+            print(f"Writing data to: {directory}")
         # multiple trajectories
         if isinstance(self.data, list):
-            os.mkdir(directory)
+            os.makedirs(directory)
             for i, trajectory in enumerate(self.data):  # write each CSV file
                 filename = os.path.join(directory, str(identifier)+str(i)+".csv")
                 field_names = []
                 for species in trajectory:  # build the header
                     field_names.append(species)
                 with open(filename, 'w', newline='', encoding="utf-8") as csv_file:
                     csv_writer = csv.writer(csv_file)
                     csv_writer.writerow(field_names)  # write the header
                     for j, _ in enumerate(trajectory['time']):  # write all lines of the CSV file
                         this_line=[]
                         for species in trajectory:  # build one line of the CSV file
                             this_line.append(trajectory[species][j])
                         csv_writer.writerow(this_line)  # write one line of the CSV file
+        return directory
 
     def plot(self, index=None, xaxis_label="Time", xscale='linear', yscale='linear', yaxis_label="Value",
              style="default", title=None, show_title=False, show_legend=True, multiple_graphs=False,
              included_species_list=[], save_png=False, figsize=(18, 10)):
         """
         Plots the Results using matplotlib.
```

### Comparing `gillespy2-1.8.1/gillespy2/core/sortableobject.py` & `gillespy2-1.8.2/gillespy2/core/sortableobject.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/species.py` & `gillespy2-1.8.2/gillespy2/core/species.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/core/timespan.py` & `gillespy2-1.8.2/gillespy2/core/timespan.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/sbml/SBMLexport.py` & `gillespy2-1.8.2/gillespy2/sbml/SBMLexport.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/sbml/SBMLimport.py` & `gillespy2-1.8.2/gillespy2/sbml/SBMLimport.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,29 @@
 except ImportError as err:
     raise ImportError('libsbml is required to convert SBML files for GillesPy.') from err
 
 import numpy as np
 
 import gillespy2
 from gillespy2.core.gillespyError import InvalidModelError, SBMLError
+from gillespy2.core import log
+
+PYTHON_RESERVED_WORDS = [
+    'False', 'def', 'if', 'raise',
+    'None', 'del', 'import', 'return',
+    'True', 'elif', 'in', 'try',
+    'and', 'else', 'is', 'while',
+    'as', 'except', 'lambda', 'with',
+    'assert', 'finally', 'nonlocal', 'yield',
+    'break', 'for', 'not',
+    'class', 'form', 'or',
+    'continue', 'global', 'pass',
+]
+PREFIX_INVALID_SBML_NAME = 'GPY2__' #'lambda' -> 'k_lambda'
+
 
 init_state = {'INF': np.inf, 'NaN': np.nan}
 postponed_evals = {}
 eval_globals = math.__dict__.copy()
 def piecewise(*args):
     args = list(args)
     sol = None
@@ -65,18 +80,24 @@
 
 def __get_math(formula):
     math_str = libsbml.formulaToL3String(formula)
     replacements = {
         r'\bln\b': 'log',
         r'\^': '**',
         r'\&\&': 'and',
-        r'\|\|': 'or'
+        r'\|\|': 'or',
         }
     for old, new in replacements.items():
         math_str = re.sub(old, new, math_str)
+    for rword in PYTHON_RESERVED_WORDS:
+        reg = r'\b' + rword + r'\b'
+        if re.search(reg, math_str):
+            sub = PREFIX_INVALID_SBML_NAME + rword
+            log.warning("'%s' is an invalid name in GillesPy2, changing to '%s'",rword,sub)
+            math_str = re.sub(reg, sub, math_str)
     return math_str
 
 def __get_species(sbml_model, gillespy_model, errors):
 
     for i in range(sbml_model.getNumSpecies()):
         species = sbml_model.getSpecies(i)
         name = species.getId()
@@ -106,14 +127,16 @@
             else: # Else convert population to concentration
                 postponed_evals[name] = f'{name} / {cid}'
                 value = population
 
         constant = species.getConstant()
         boundary_condition = species.getBoundaryCondition()
         is_negative = value < 0
+        if name in PYTHON_RESERVED_WORDS:
+            name =  PREFIX_INVALID_SBML_NAME + name
         gillespy_species = gillespy2.Species(name=name, initial_value=value,
                                                 allow_negative_populations=is_negative, mode=mode,
                                                 constant=constant, boundary_condition=boundary_condition)
         gillespy_model.add_species([gillespy_species])
         init_state[name] = value
 
 def __get_parameters(sbml_model, gillespy_model):
@@ -124,14 +147,16 @@
         if parameter.isSetValue():
             value = parameter.getValue()
         else:
             value = 0
         init_state[name] = value
 
         # GillesPy2 represents non-constant parameters as species
+        if name in PYTHON_RESERVED_WORDS:
+            name =  PREFIX_INVALID_SBML_NAME + name
         if parameter.isSetConstant():
             gillespy_parameter = gillespy2.Parameter(name=name, expression=value)
             gillespy_model.add_parameter([gillespy_parameter])
         else:
             gillespy_species = gillespy2.Species(name=name,initial_value=value)
             gillespy_model.add_species([gillespy_species])
 
@@ -143,14 +168,16 @@
             value = compartment.getSize()
         else:
             value = 1
 
         if name == "vol":
             gillespy_model.volume = value
         else:
+            if name in PYTHON_RESERVED_WORDS:
+                name =  PREFIX_INVALID_SBML_NAME + name
             gillespy_parameter = gillespy2.Parameter(name=name, expression=value)
             init_state[name] = value
             gillespy_model.add_parameter([gillespy_parameter])
 
 def __traverse_math(node, old_id, new_id):
     if node is None:
         return
@@ -174,20 +201,26 @@
     local_params = kinetic_law.getListOfLocalParameters()
     for i in range(kinetic_law.getNumLocalParameters()):
         local_param = local_params.get(i)
         old_id = local_param.getId()
         new_id = (f'{reaction.getId()}_{local_param.getId()}')
         __traverse_math(tree, old_id, new_id)
         local_param.setId(new_id)
-        gillespy_parameter = gillespy2.Parameter(name=new_id, expression=local_param.getValue())
+        name = new_id
+        if name in PYTHON_RESERVED_WORDS:
+            name =  PREFIX_INVALID_SBML_NAME + name
+        gillespy_parameter = gillespy2.Parameter(name=name, expression=local_param.getValue())
         gillespy_model.add_parameter([gillespy_parameter])
     for i in range(kinetic_law.getNumParameters()):
         param = params.get(i)
         if not param.getId() in gillespy_model.listOfParameters:
-            gillespy_parameter = gillespy2.Parameter(name=param.getId(), expression=param.getValue())
+            name = param.getId()
+            if name in PYTHON_RESERVED_WORDS:
+                name =  PREFIX_INVALID_SBML_NAME + name
+            gillespy_parameter = gillespy2.Parameter(name=name, expression=param.getValue())
             gillespy_model.add_parameter([gillespy_parameter])
     return tree
 
 def __get_reactions(sbml_model, gillespy_model, errors):
     # reactions
     for i in range(sbml_model.getNumReactions()):
         reaction = sbml_model.getReaction(i)
@@ -256,15 +289,18 @@
             rule_name = f"ar_{rule.getId()}"
 
         rule_variable = rule.getVariable()
         rule_string = __get_math(rule.getMath())
         if rule_variable in gillespy_model.listOfParameters:
             # Treat Non-Constant Parameters as Species
             value = gillespy_model.listOfParameters[rule_variable].expression
-            species = gillespy2.Species(name=rule_variable,
+            name = rule_variable
+            if name in PYTHON_RESERVED_WORDS:
+                name =  PREFIX_INVALID_SBML_NAME + name
+            species = gillespy2.Species(name=name,
                                         initial_value=value,
                                         allow_negative_populations=True,
                                         mode='continuous')
             gillespy_model.delete_parameter(rule_variable)
             gillespy_model.add_species([species])
 
         t = []
@@ -339,16 +375,19 @@
         gillespy_trigger = gillespy2.EventTrigger(
             expression=expression, initial_value=initial_value, persistent=persistent
         )
         assignments = event.getListOfEventAssignments()
         for assign in assignments:
             # Convert Non-Constant Parameter to Species
             if assign.getVariable() in gillespy_model.listOfParameters:
+                name = assign.getVariable()
+                if name in PYTHON_RESERVED_WORDS:
+                    name =  PREFIX_INVALID_SBML_NAME + name
                 gillespy_species = gillespy2.Species(
-                    name=assign.getVariable(),
+                    name=name,
                     initial_value=gillespy_model.listOfParameters[assign.getVariable()].expression,
                     mode='continuous', allow_negative_populations=True
                 )
                 gillespy_model.delete_parameter(assign.getVariable())
                 gillespy_model.add_species([gillespy_species])
 
             gillespy_assignment = gillespy2.EventAssignment(variable=assign.getVariable(),
@@ -371,15 +410,15 @@
         if assigned_value != assigned_value:
             assigned_value = expression
             postponed_evals[variable] = expression
 
         if variable in gillespy_model.listOfSpecies:
             gillespy_model.listOfSpecies[variable].initial_value = assigned_value
         elif variable in gillespy_model.listOfParameters:
-            gillespy_model.listOfParameters[variable].expression = assigned_value
+            gillespy_model.listOfParameters[variable].expression = str(assigned_value)
 
 def __resolve_evals(gillespy_model, init_state):
     while True:
         successful = []
         if len(postponed_evals):
             for var, expr in postponed_evals.items():
                 try:
@@ -395,14 +434,16 @@
                         gillespy_model.listOfParameters[var].value = assigned_value
         if len(successful) <= 0:
             break
         for var in successful:
             del postponed_evals[var]
 
 def convert(filename, model_name=None, gillespy_model=None, report_silently_with_sbml_error=False):
+
+
     sbml_model, errors = __read_sbml_model(filename)
 
     if sbml_model is None:
         if report_silently_with_sbml_error:
             return None, errors
         errs = '\n\t'.join(errors)
         raise SBMLError(f"SBML model import failed.  Reason Given: \n\t{errs}")
```

### Comparing `gillespy2-1.8.1/gillespy2/sbml/__init__.py` & `gillespy2-1.8.2/gillespy2/sbml/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/__init__.py` & `gillespy2-1.8.2/gillespy2/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/__init__.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/build/SConstruct` & `gillespy2-1.8.2/gillespy2/solvers/cpp/build/SConstruct`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/build/__init__.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/build/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/build/build_engine.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/build/build_engine.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/build/expression.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/build/expression.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/build/make.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/build/make.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/build/template_gen.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/build/template_gen.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/LICENSE` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/LICENSE`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/NOTICE` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/NOTICE`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/README.md` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/README.md`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_ls.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_ls.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_proj.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_proj.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_spils.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/cvode_spils.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/nvector_serial.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_band.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_band.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_config.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_config.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_direct.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_iterative.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_linearsolver.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_math.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_math.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_matrix.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nonlinearsolver.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector_senswrapper.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_nvector_senswrapper.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_types.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_types.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_version.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sundials_version.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunlinsol_spgmr.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunlinsol_spgmr.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_band.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_band.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_dense.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_sparse.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunmatrix_sparse.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/include/sunnonlinsol_newton.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/include/sunnonlinsol_newton.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_direct.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_direct.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_fused_stubs.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_fused_stubs.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_impl.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_impl.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_io.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_io.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls_impl.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_ls_impl.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_nls.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_nls.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj_impl.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_proj_impl.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_spils.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/cvode_spils.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/nvector_serial.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_band.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_debug.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_debug.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_iterative.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_linearsolver.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_linearsolver.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_math.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_matrix.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_matrix.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nonlinearsolver.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nonlinearsolver.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector_senswrapper.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sundials_nvector_senswrapper.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_band.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_band.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_dense.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_dense.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_spgmr.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunlinsol_spgmr.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_band.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_band.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_dense.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunmatrix_dense.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_fixedpoint.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_fixedpoint.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_newton.c` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Sundials/src/sunnonlinsol_newton.c`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/tau.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/tau.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/Tau/tau.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/Tau/tau.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/arg_parser.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/arg_parser.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/arg_parser.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/arg_parser.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/model.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/model.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/model.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/model.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESimulation.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESimulation.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/ODESolver.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ode_cpp_solver/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ode_cpp_solver/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASimulation.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASimulation.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/ssa_cpp_solver/SSASolver.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                     });
                 }
             }
         }
 
         // Helper method to flag reactions that can be processed deterministically (continuous change)
         // without exceeding the user-supplied tolerance
-        std::set<int> flag_det_rxns(
+        int flag_det_rxns(
                 std::vector<HybridReaction> &reactions,
                 std::vector<HybridSpecies> &species)
         {
             int num_reactions = reactions.size();
             int num_species = species.size();
             std::set<int> det_rxns;
 
@@ -333,15 +333,15 @@
                 }
 
                 if (rxn.mode == SimulationState::CONTINUOUS) {
                     det_rxns.insert(rxn_i);
                 }
             }
 
-            return det_rxns;
+            return det_rxns.size();
         }
 
         void partition_species(
                 double current_time,
                 std::vector<HybridReaction> &reactions,
                 std::vector<HybridSpecies> &species,
                 const std::vector<double> &propensity_values,
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/HybridModel.h`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                 INTEGRATOR_FAILED = 3,
                 INVALID_AFTER_SSA = 4,
                 NEGATIVE_STATE_NO_SSA_REACTION = 5,
                 NEGATIVE_STATE_AT_BEGINING_OF_STEP = 6,
             };
         };
 
-        std::set<int> flag_det_rxns(
+        int flag_det_rxns(
                 std::vector<HybridReaction> &reactions,
                 std::vector<HybridSpecies> &species);
 
         void partition_species(
                 double current_time,
                 std::vector<HybridReaction> &reactions,
                 std::vector<HybridSpecies> &species,
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSimulation.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSimulation.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 #include "sundials_types.h"  // defs. of realtype, sunindextype
 #include "sundials_math.h"  // contains the macros ABS, SUNSQR, EXP
 #include "TauHybridSolver.h"
 #include "HybridModel.h"
 #include "integrator.h"
 #include "tau.h"
 
+#include "template_defaults.h"
+
+
 static void silent_error_handler(int error_code, const char *module, const char *function_name,
                           char *message, void *eh_data);
 
 namespace Gillespy
 {
     static volatile bool interrupted = false;
     std::mt19937_64 generator;
@@ -48,16 +51,15 @@
         interrupted = true;
     })
 
     namespace TauHybrid
     {
         void CalculateSpeciesChangeAfterStep(IntegrationResults&result, int*population_changes,
          std::vector<double> current_state, std::set<unsigned int>&rxn_roots, 
-         std::set<int>&event_roots, HybridSimulation*simulation, URNGenerator&urn, 
-         int only_reaction_to_fire){
+         std::set<int>&event_roots, HybridSimulation*simulation, URNGenerator&urn){
             Model<double> &model = *(simulation->model);
             int num_species = model.number_species;
             int num_reactions = model.number_reactions;
             // 0-initialize our population_changes array.
             for (int p_i = 0; p_i < num_species; ++p_i) {
                 population_changes[p_i] = 0;
             }
@@ -84,20 +86,21 @@
                     // Temporary variable for the reaction's state.
                     // Does not get updated unless the changes are deemed valid.
                     double rxn_state = result.reactions[rxn_i];
                     double old_rxn_state = rxn_state;
 
                     if (simulation->reaction_state[rxn_i].mode == SimulationState::DISCRETE) {
                         unsigned int rxn_count = 0;
-                        if(only_reaction_to_fire > -1){
-                            if(only_reaction_to_fire == rxn_i){
-                                    rxn_state = log(urn.next());
-                                    rxn_count = 1;
-                            }
-                        }else if(rxn_state > 0){
+                        //if(only_reaction_to_fire > -1){
+                        //    if(only_reaction_to_fire == rxn_i){
+                        //            rxn_state = log(urn.next());
+                        //            rxn_count = 1;
+                        //    }
+                        //}else
+                        if(rxn_state > 0){
                             std::poisson_distribution<int> poisson(rxn_state);
                             rxn_count = 1 + poisson(generator);
                             rxn_state = log(urn.next());
 
                         }
                         if(rxn_count > 0){
                             for (int spec_i = 0; spec_i < num_species; ++spec_i) {
@@ -109,28 +112,32 @@
                 }
             }
         }
 
         bool TakeIntegrationStep(Integrator&sol, IntegrationResults&result, double *next_time, int*population_changes,
          std::vector<double> current_state, std::set<unsigned int>&rxn_roots, 
          std::set<int>&event_roots, HybridSimulation*simulation, URNGenerator&urn, 
-         int only_reaction_to_fire){
+         int num_det_rxns, int num_rate_rules){
             // Integration Step
+
+            // check to see if we can do a constant integration (no deterministic reactions or rate rules)
+
             // For deterministic reactions, the concentrations are updated directly.
             // For stochastic reactions, integration updates the rxn_offsets vector.
-            result = sol.integrate(next_time, event_roots, rxn_roots);
+            result = sol.integrate(next_time, event_roots, rxn_roots, num_det_rxns, num_rate_rules);
             if (sol.status == IntegrationStatus::BAD_STEP_SIZE)
             {
                 simulation->set_status(HybridSimulation::INTEGRATOR_FAILED);
                 return false;
-            } else {
-                // The integrator has, at this point, been validated.
-                // Any errors beyond this point is assumed to be a stochastic state failure.
-                CalculateSpeciesChangeAfterStep(result, population_changes, current_state, rxn_roots, event_roots, simulation, urn, only_reaction_to_fire);
             }
+
+
+            // The integrator has, at this point, been validated.
+            // Any errors beyond this point is assumed to be a stochastic state failure.
+            CalculateSpeciesChangeAfterStep(result, population_changes, current_state, rxn_roots, event_roots, simulation, urn);
             return true;
         }
 
 
 
 
         bool IsStateValidNonNegativeSpecies(int num_species, std::vector<double> current_state, std::vector<int> non_negative_species){  
@@ -167,25 +174,29 @@
             if (simulation == NULL)
             {
                 return;
             }
             GPY_INTERRUPT_INSTALL_HANDLER(signal_handler);
 
             Model<double> &model = *(simulation->model);
+            int num_rate_rules = 0;
             int num_species = model.number_species;
             int num_reactions = model.number_reactions;
             int num_trajectories = simulation->number_trajectories;
             std::unique_ptr<Species<double>[]> &species = model.species;
             bool use_root_finding = default_use_root_finding;
             bool in_event_handling = false;
             unsigned int neg_state_loop_cnt = 0;
 
             std::vector<int> non_negative_species;
 
             for (int spec = 0; spec < model.number_species; spec++) {
+                HybridSpecies *specO = &simulation->species_state[spec];
+                num_rate_rules += specO->diff_equation.rate_rules.size();
+
                 for (int r = 0; r < model.number_reactions; r++) {
                     if (model.reactions[r].products_change[spec] > 0 ||
                         model.reactions[r].reactants_change[spec] > 0) {
                         non_negative_species.push_back(model.species[spec].id);
                         break;// once we flagged it, skip to the next species
                     }
                 }
@@ -278,14 +289,20 @@
 
                 // Reset the parameters, they may be modified by an Event
                 double *s_vars = Reaction::s_variables.get();
                 for(int s_num_i=0; s_num_i < Reaction::s_num_variables; s_num_i++){
                     s_vars[s_num_i] = saved__s_variables[s_num_i];
                 }
 
+                // reset R_j values
+                double *curr_rxn_state = sol.get_reaction_state();
+                for (unsigned int rxn_j = 0; rxn_j < num_reactions; ++rxn_j) {
+                    curr_rxn_state[rxn_j] = log(urn.next()); 
+                }
+
 
                 while (!interrupted && !invalid_state && simulation->current_time < simulation->end_time)
                 {
                     // Compute current propensity values based on existing state.
                     double *curr_rxn_state = sol.get_reaction_state();
                     for (unsigned int rxn_j = 0; rxn_j < num_reactions; ++rxn_j)
                     {
@@ -309,33 +326,37 @@
                     if( ! IsStateValidNonNegativeSpecies(num_species, current_state, non_negative_species) ) {
                         // throw an error
                         simulation->set_status(HybridSimulation::NEGATIVE_STATE_AT_BEGINING_OF_STEP);
                         return;
                     }
 
                     // Expected tau step is determined.
-                    tau_step = select<double, double>(
-                            model,
-                            tau_args,
-                            tau_tol,
-                            simulation->current_time,
-                            save_time,
-                            sol.data.propensities,
-                            current_state
-                    );
+                    if(GPY_CONSTANT_TAU_STEPSIZE > 0){
+                        tau_step = GPY_CONSTANT_TAU_STEPSIZE;
+                    }else{
+                        tau_step = select<double, double>(
+                                model,
+                                tau_args,
+                                tau_tol,
+                                simulation->current_time,
+                                save_time,
+                                sol.data.propensities,
+                                current_state
+                        );
+                    }
                     partition_species(
                             simulation->current_time,
                             simulation->reaction_state,
                             simulation->species_state,
                             sol.data.propensities,
                             current_state,
                             tau_step,
                             tau_args
                     );
-                    flag_det_rxns(
+                    int num_det_rxns = flag_det_rxns(
                             simulation->reaction_state,
                             simulation->species_state
                     );
                     update_species_state(simulation->species_state, current_state);
                     create_differential_equations(simulation->species_state, simulation->reaction_state);
 
                     // Determine what the next time point is.
@@ -367,15 +388,15 @@
                             use_root_finding = default_use_root_finding;
                         }
                     }else{
                         sol.disable_root_finder();
                     }
 
 
-                    if(!TauHybrid::TakeIntegrationStep(sol, result, &next_time, population_changes, current_state, rxn_roots, event_roots, simulation, urn, -1)){
+                    if(!TauHybrid::TakeIntegrationStep(sol, result, &next_time, population_changes, current_state, rxn_roots, event_roots, simulation, urn, num_det_rxns, num_rate_rules)){
                         return;
                     }
 
                     // Check if we have gone negative
                     if (TauHybrid::IsStateNegativeCheck(num_species, population_changes, current_state, tau_args.reactants)) {
                         // If state is invalid, we took too agressive tau step and need to take a single SSA step forward
                         // Restore the solver to the intial step state
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/TauHybridSolver.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/hybrid_template.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -119,14 +119,55 @@
 {
     N_VDestroy_Serial(y);
     CVodeFree(&cvode_mem);
     SUNLinSolFree_SPGMR(solver);
     delete[] m_roots;
 }
 
+IntegrationResults Integrator::integrate_constant(double *t)
+{
+    // this function assumes no deterministic species or 
+    realtype *Y = N_VGetArrayPointer(y);
+    HybridSimulation *sim = data.simulation;
+    std::vector<HybridSpecies> *species = data.species_state;
+    std::vector<HybridReaction> *reactions = data.reaction_state;
+    std::vector<double> &propensities = data.propensities;
+    unsigned int num_species = sim->model->number_species;
+    unsigned int num_reactions = sim->model->number_reactions;
+    realtype propensity;
+    for (unsigned int rxn_i = 0; rxn_i < num_reactions; ++rxn_i)
+    {
+        HybridReaction rxn = (*reactions)[rxn_i];
+        switch (rxn.mode) {
+        case SimulationState::DISCRETE:
+            // Process stochastic reaction state by updating the root offset for each reaction.
+            propensity = rxn.ssa_propensity(Y);
+            propensities[rxn_i] = propensity;
+            break;
+
+        case SimulationState::CONTINUOUS:
+            break;
+        default:
+            break;
+        }
+    }
+
+    double tau = *t - this->t;
+    for (int rxn_i = 0; rxn_i < num_reactions; ++rxn_i){
+        NV_Ith_S(y, rxn_i+num_species) = NV_Ith_S(y, rxn_i+num_species) + propensities[rxn_i] * tau;
+    }
+    this->t = *t;
+
+    return {
+        NV_DATA_S(y),
+        NV_DATA_S(y) + num_species,
+        IntegrationStatus::OK
+    };
+}
+
 IntegrationResults Integrator::integrate(double *t)
 {
     int retcode = CVode(cvode_mem, *t, y, &this->t, CV_NORMAL);
     if (!validate(this, retcode ))
     {
         return { nullptr, nullptr, 0 };
     }
@@ -153,17 +194,23 @@
         // This gets initialized to a random negative offset, and gets "less negative"
         //   during the integration step.
         // After each integration step, the reaction_state is used to count stochastic reactions.
         NV_Ith_S(y0, rxn_i) = log(urn.next());
     }
 }
 
-IntegrationResults Integrator::integrate(double *t, std::set<int> &event_roots, std::set<unsigned int> &reaction_roots)
+IntegrationResults Integrator::integrate(double *t, std::set<int> &event_roots, std::set<unsigned int> &reaction_roots, int num_det_rxns, int num_rate_rules)
 {
-    IntegrationResults results = integrate(t);
+
+    IntegrationResults results;
+    if(num_det_rxns == 0 && num_rate_rules == 0 &&  data.active_triggers.size() == 0 && data.active_reaction_ids.size() == 0){
+        results = integrate_constant(t);
+    }else{
+        results = integrate(t);
+    }
     if (status != IntegrationStatus::OK) {
         return results;
     }
 
     // check to see if any root we found by the solver
     if( results.retcode == CV_ROOT_RETURN ){
         // find which roots were found and return them
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_hybrid_cpp_solver/integrator.h`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,16 @@
 		}
 		inline realtype *get_reaction_state()
 		{
 			return &N_VGetArrayPointer(y)[num_species];
 		}
 
         IntegrationResults integrate(double *t);
-        IntegrationResults integrate(double *t, std::set<int> &event_roots, std::set<unsigned int> &reaction_roots);
+        IntegrationResults integrate_constant(double *t);
+        IntegrationResults integrate(double *t, std::set<int> &event_roots, std::set<unsigned int> &reaction_roots, int num_det_rxns, int num_rate_rules);
         IntegratorData data;
 
         Integrator(HybridSimulation *simulation, Model<double> &model, URNGenerator urn, double reltol, double abstol);
         ~Integrator();
         void reset_model_vector();
     };
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/SConscript` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/SConscript`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSimulation.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSimulation.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 #include <iostream>
 #include <functional>
 #include <algorithm>
 
 #include "TauLeapingSolver.h"
 #include "tau.h"
 
+#include "template_defaults.h"
+
 namespace Gillespy
 {
     static volatile bool interrupted = false;
     std::mt19937_64 generator;
 
     GPY_INTERRUPT_HANDLER(signal_handler, {
         interrupted = true;
@@ -145,16 +147,19 @@
                     }
 
                     //calculate propensities for each step
                     for (unsigned int reaction_number = 0; reaction_number < simulation->model->number_reactions; reaction_number++)
                     {
                         propensity_values[reaction_number] = Reaction::propensity(reaction_number, current_state.data());
                     }
-
-                    tau_step = select(*(simulation->model), tau_args, tau_tol, simulation->current_time, save_time, propensity_values, current_state);
+                    if(GPY_CONSTANT_TAU_STEPSIZE > 0){
+                        tau_step = GPY_CONSTANT_TAU_STEPSIZE;
+                    }else{
+                        tau_step = select(*(simulation->model), tau_args, tau_tol, simulation->current_time, save_time, propensity_values, current_state);
+                    }
                     prev_curr_state = current_state;
                     double prev_curr_time = simulation->current_time;
                     int loop_cnt = 0;
 
                     while (true)
                     {
                         loop_cnt += 1;
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/tau_leaping_cpp_solver/TauLeapingSolver.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template.cpp` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template.cpp`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_defaults.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_defaults.h`

 * *Files 4% similar despite different names*

```diff
@@ -59,33 +59,40 @@
 #define GPY_SPECIES_NAMES
 #endif
 
 #ifndef GPY_REACTION_NAMES
 #define GPY_REACTION_NAMES
 #endif
 
+
+#ifndef GPY_CONSTANT_TAU_STEPSIZE
+#define GPY_CONSTANT_TAU_STEPSIZE 0 
+#endif
+
 // ===============================================================
 // ================ HYBRID SOLVER OPTION DEFAULTS ================
 // ===============================================================
 
 /* GPY_HYBRID_SPECIES_MODES: Default, user-provided flags for how each species is to be represented.
  * Populate each SPECIES_MODE() with two arguments: species ID and species mode.
  * Possible values for species mode are: DISCRETE / CONTINUOUS / DYNAMIC
  * 
  * 
  * #define GPY_HYBRID_SPECIES_MODES \
  * SPECIES_MODE(0, DISCRETE_MODE) \
  * SPECIES_MODE(1, CONTINUOUS_MODE) \
  * SPECIES_MODE(2, DYNAMIC_MODE)
  */
+
 #ifdef GPY_SOLVER_HYBRID
 
 #ifndef GPY_HYBRID_SPECIES_MODES
 #define GPY_HYBRID_SPECIES_MODES
 #endif
 
 #ifndef GPY_RATE_RULES
 #define GPY_RATE_RULES
 #endif
 
 #endif
 
+
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_definitions.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_definitions.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_base/template/template_params.h` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_base/template/template_params.h`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_decoder.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_decoder.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/c_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/ode_c_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/ode_c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/ssa_c_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/ssa_c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/tau_hybrid_c_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/tau_hybrid_c_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,29 @@
     along with ODE solvers to simulate ODE and Stochastic systems
     interchangeably or simultaneously.
     """
 
     name = "TauHybridCSolver"
     target = "hybrid"
 
+    def __init__(self, model = None, output_directory = None, delete_directory = True, resume=None, variable = False,  constant_tau_stepsize=None):
+
+        self.constant_tau_stepsize = constant_tau_stepsize
+        super().__init__(model=model, output_directory=output_directory, 
+                         delete_directory=delete_directory, resume=resume, variable=variable)
+
     class ErrorStatus(IntEnum):
         UNKNOWN = 1
         LOOP_OVER_INTEGRATE = 2
         INTEGRATOR_FAILED = 3
         INVALID_AFTER_SSA = 4
         NEGATIVE_STATE_NO_SSA_REACTION = 5
         NEGATIVE_STATE_AT_BEGINING_OF_STEP = 6
 
-    @classmethod
-    def __create_options(cls, sanitized_model: "SanitizedModel") -> "SanitizedModel":
+    def __create_options(self, sanitized_model: "SanitizedModel") -> "SanitizedModel":
         """
         Populate the given list of species modes into a set of template macro definitions.
         Generated options are specific to the Tau Hybrid solver,
         and get passed as custom definitions to the build engine.
 
         :param sanitized_model: Sanitized model containing sanitized species definitions.
         The GPY_HYBRID_SPECIES_MODES option will be set as an option for the model.
@@ -165,22 +170,33 @@
             RateRule,
         }
 
     @classmethod
     def get_supported_integrator_options(cls) -> "Set[str]":
         return { "rtol", "atol", "max_step" }
 
+
+
     def _build(self, model: "Union[Model, SanitizedModel]", simulation_name: str, variable: bool, debug: bool = False,
                custom_definitions=None) -> str:
         variable = variable or len(model.listOfEvents) > 0
-        sanitized_model = TauHybridCSolver.__create_options(SanitizedModel(model, variable=variable))
+        sanitized_model = self.__create_options(SanitizedModel(model, variable=variable))
         for rate_rule in model.listOfRateRules.values():
             sanitized_model.use_rate_rule(rate_rule)
+
+        # determine if a constant stepsize has been requested
+        if self.constant_tau_stepsize is not None:
+            sanitized_model.options['GPY_CONSTANT_TAU_STEPSIZE'] = str(float(self.constant_tau_stepsize))
+        else:
+            sanitized_model.options['GPY_CONSTANT_TAU_STEPSIZE'] = '0'
         return super()._build(sanitized_model, simulation_name, variable, debug)
 
+
+
+
     def _handle_return_code(self, return_code: "int") -> "int":
         if return_code == TauHybridCSolver.ErrorStatus.UNKNOWN:
             raise SimulationError("C++ solver failed (no error code given).")
         if return_code == TauHybridCSolver.ErrorStatus.LOOP_OVER_INTEGRATE:
             raise SimulationError("Loop over integrate exceeded, problem space is too stiff")
         if return_code == TauHybridCSolver.ErrorStatus.INTEGRATOR_FAILED:
             raise SimulationError("Sundials ODE solver failed with 'BAD_STEP_SIZE'")
@@ -266,18 +282,20 @@
             log.warning('model = gillespy2.model is deprecated. Future releases '
                         'of GillesPy2 may not support this feature.')
         if self.model is None:
             if model is None:
                 raise SimulationError("A model is required to run the simulation.")
             self._set_model(model=model)
 
+
         self.model.compile_prep()
         self.validate_model(self.model, model)
         self.validate_sbml_features(model=self.model)
 
+
         self.validate_tspan(increment=increment, t=t)
         if increment is None:
             increment = self.model.tspan[-1] - self.model.tspan[-2]
         if t is None:
             t = self.model.tspan[-1]
 
         # Validate parameters prior to running the model.
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/cpp/tau_leaping_c_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/cpp/tau_leaping_c_solver.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,38 +19,58 @@
 from gillespy2.solvers.utilities import solverutils as cutils
 from gillespy2.core import GillesPySolver, Model
 from gillespy2.core.gillespyError import *
 from gillespy2.core import Results 
 
 from .c_solver import CSolver, SimulationReturnCode
 
+from gillespy2.solvers.cpp.build.template_gen import SanitizedModel
+
+
 class TauLeapingCSolver(GillesPySolver, CSolver):
 
     """
     A Tau Leaping solver for GillesPy2 models.  This solver uses an algorithm that calculates
     multiple reactions in a single step over a given tau step size.  The change in propensities
     over this step are bounded by relative change in state, yielding greatly improved
     run-time performance with very little trade-off in accuracy.
     """
 
     name = "TauLeapingCSolver"
     target = "tau_leap"
 
+    def __init__(self, model = None, output_directory = None, delete_directory = True, resume=None, variable = False,  constant_tau_stepsize=None):
+
+        self.constant_tau_stepsize = constant_tau_stepsize
+        super().__init__(model=model, output_directory=output_directory, 
+                         delete_directory=delete_directory, resume=resume, variable=variable) 
+
+    def _build(self, model, simulation_name, variable, debug = False,
+               custom_definitions=None):
+        sanitized_model = SanitizedModel(model, variable=variable)
+        # determine if a constant stepsize has been requested
+        if self.constant_tau_stepsize is not None:
+            sanitized_model.options['GPY_CONSTANT_TAU_STEPSIZE'] = str(float(self.constant_tau_stepsize))
+        else:
+            sanitized_model.options['GPY_CONSTANT_TAU_STEPSIZE'] = '0'
+        return super()._build(sanitized_model, simulation_name, variable, debug)
+
+
     @classmethod
     def get_solver_settings(cls):
         """
         Returns a list of arguments supported by tau_leaping_c_solver.run.
         :returns: Tuple of strings, denoting all keyword argument for this solvers run() method.
         :rtype: tuple
         """
         return ('model', 't', 'number_of_trajectories', 'timeout', 'increment', 'seed', 'debug', 'profile')
 
     def run(self=None, model: Model = None, t: int = None, number_of_trajectories: int = 1, timeout: int = 0,
             increment: int = None, seed: int = None, debug: bool = False, profile: bool = False, variables={},
-            resume=None, live_output: str = None, live_output_options: dict = {}, tau_tol=0.03, **kwargs):
+            resume=None, live_output: str = None, live_output_options: dict = {}, tau_tol=0.03, constant_tau_stepsize=None, **kwargs):
 
         """
         :param model: The model on which the solver will operate. (Deprecated)
         :type model: gillespy2.Model
 
         :param t: End time of simulation.
         :type t: int
@@ -81,14 +101,16 @@
             "clear_output" specifies if display should be refreshed with each display.
         :type live_output_options:  dict
 
         :param tau_tol: Tolerance level for Tau leaping algorithm.  Larger tolerance values will
         result in larger tau steps. Default value is 0.03.
         :type tau_tol: float
 
+        :param constant_tau_stepsize: If set, overrides the automatic stepsize selection and uses the given
+                    value as the stepsize on each step.
         :returns: A result object containing the results of the simulation
         :rtype: gillespy2.Results
         """
 
         if self is None:
             # Post deprecation block
             # raise SimulationError("TauLeapingCSolver must be instantiated to run the simulation")
@@ -107,14 +129,16 @@
             log.warning('model = gillespy2.model is deprecated. Future releases '
                         'of GillesPy2 may not support this feature.')
         if self.model is None:
             if model is None:
                 raise SimulationError("A model is required to run the simulation.")
             self._set_model(model=model)
 
+        self.constant_tau_stepsize = constant_tau_stepsize
+
         self.model.compile_prep()
         self.validate_model(self.model, model)
         self.validate_sbml_features(model=self.model)
 
         self.validate_tspan(increment=increment, t=t)
         if increment is None:
             increment = self.model.tspan[-1] - self.model.tspan[-2]
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/numpy/CLE_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/numpy/CLE_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/numpy/__init__.py` & `gillespy2-1.8.2/gillespy2/solvers/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/numpy/ode_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/numpy/ode_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/numpy/ssa_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/numpy/ssa_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/numpy/tau_hybrid_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/numpy/tau_hybrid_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 from gillespy2.core.results import Results
 
 eval_globals = math.__dict__
 
 def __piecewise(*args):
     # Eval entry for piecewise functions
     args = list(args)
-    sol = None
+    solution = None
     if len(args) % 2:
         args.append(True)
     for i, arg in enumerate(args):
         if not i % 2:
             continue
         if arg:
-            sol = args[i - 1]
+            solution = args[i - 1]
             break
-    return sol
+    return solution
 
 
 def __xor(*args):
     # Eval entry for MathML xor function
     from operator import ixor
     from functools import reduce
     args = list(args)
@@ -69,15 +69,15 @@
     :type model: gillespy2.Model
     """
     name = "TauHybridSolver"
     rc = 0
     result = None
     stop_event = None
 
-    def __init__(self, model=None, profile_reactions=False):
+    def __init__(self, model=None, profile_reactions=False, constant_tau_stepsize=None):
         if model is None:
             raise SimulationError("A model is required to run the simulation.")
 
         name = 'TauHybridSolver'
         rc = 0
         self.model = copy.deepcopy(model)
         self.is_instantiated = True
@@ -89,14 +89,25 @@
                 self.profile_data[k] = []
         self.non_negative_species = set()
         for reaction, _ in model.listOfReactions.items():
             for key, value in model.listOfReactions[reaction].reactants.items():
                 self.non_negative_species.add(key.name)
             for key, value in model.listOfReactions[reaction].products.items():
                 self.non_negative_species.add(key.name)
+        self.constant_tau_stepsize = constant_tau_stepsize
+        # check if model should skip ODE integration step
+        self.pure_discrete = False
+        if len(self.model.listOfRateRules)==0:
+            self.pure_discrete = True
+            for species in self.model.listOfSpecies:
+                if self.model.listOfSpecies[species].mode != 'discrete':
+                    self.pure_discrete = False
+                    break
+
+
 
     def __save_state_to_output(self, curr_time, save_index, curr_state, species, 
                                 trajectory, save_times):
         """
         Helper function to save the curr_state to the trajectory output
         """
         
@@ -484,57 +495,101 @@
                             initial_state[a.variable.name] = eval(a.expression, {**eval_globals, **initial_state})
                             species_modified_by_events.append(a.variable.name)
                     else:
                         execution_time = eval(e.delay, {**eval_globals, **initial_state})
                         t0_delayed_events[e.name] = execution_time
         return t0_delayed_events, species_modified_by_events
 
-    def __update_stochastic_rxn_states(self, compiled_reactions, curr_state, only_update=None):
+    def __update_stochastic_rxn_states(self, propensities, tau_step, compiled_reactions, curr_state, only_update=None):
         """
         Helper method for updating the state of stochastic reactions.
 
         if 'only_update' is set to a reaction name, it will only reset that reaction, and only one firing
         """
 
         rxn_count = OrderedDict()
         species_modified = OrderedDict()
         # Update stochastic reactions
 
         for rxn in compiled_reactions:
             rxn_count[rxn] = 0
             if only_update is not None:  # for a single SSA step
                 if rxn == only_update:
-                    curr_state[rxn] = math.log(random.uniform(0, 1)) #set this value, needs to be <0
+                    curr_state[rxn] = math.log(np.random.uniform(0, 1)) #set this value, needs to be <0
                     rxn_count[rxn] = 1
-            else:  # for a normal Tau-step
-                while curr_state[rxn] > 0:
-                    rxn_count[rxn] += 1
-                    curr_state[rxn] += math.log(random.uniform(0, 1))
+            elif curr_state[rxn] > 0:
+                rxn_count[rxn] = 1 + np.random.poisson(curr_state[rxn])
+                curr_state[rxn] = math.log(np.random.uniform(0, 1))
+
             if rxn_count[rxn]:
                 for reactant in self.model.listOfReactions[rxn].reactants:
                     species_modified[reactant.name] = True
                     curr_state[reactant.name] -= self.model.listOfReactions[rxn].reactants[reactant] * rxn_count[rxn]
                 for product in self.model.listOfReactions[rxn].products:
                     species_modified[product.name] = True
                     curr_state[product.name] += self.model.listOfReactions[rxn].products[product] * rxn_count[rxn]
         return species_modified, rxn_count
 
-    def __integrate(self, integrator_options, curr_state, y0, curr_time,
+    def __integrate_constant(self, integrator_options, curr_state, y0, curr_time,
                     propensities, y_map, compiled_reactions,
                     active_rr, event_queue,
                     delayed_events, trigger_states,
                     event_sensitivity, tau_step ):
         """
+        Integreate one step, skip ODE integrator as all species are 
+        discrete.
+        """
+        tau_step = max(1e-6, tau_step)
+        next_tau = curr_time + tau_step
+        prev_time = curr_time
+        curr_state['t'] = curr_time
+        curr_state['time'] = curr_time
+        
+        event_times = {}
+        reaction_times = []
+        next_step, curr_time = self.__get_next_step(event_times, reaction_times,
+                                                    delayed_events,
+                                                    self.model.tspan[-1], next_tau)
+        curr_state['t'] = curr_time
+
+        tau_step2 = curr_time - prev_time
+
+        for rxn in compiled_reactions:
+            curr_state[rxn] = curr_state[rxn] + propensities[rxn]*tau_step2
+
+        return curr_time, tau_step2
+
+
+
+    def __integrate(self, integrator_options, curr_state, y0, curr_time,
+                    propensities, y_map, compiled_reactions,
+                    active_rr, event_queue,
+                    delayed_events, trigger_states,
+                    event_sensitivity, tau_step, det_rxn ):
+        """
         Helper function to perform the ODE integration of one step.  This
         method uses scipy.integrate.LSODA to get simulation data, and
         determines the next stopping point of the simulation. The state is
         updated and returned to __simulate along with curr_time and the
         solution object.
         """
-        max_step_size = self.model.tspan[1] - self.model.tspan[0] / 100
+        use_const = False
+        if self.pure_discrete:
+            use_const = True
+        elif len(self.model.listOfRateRules)==0:
+            use_const = True
+            for rxn in det_rxn:
+                if det_rxn[rxn]:
+                    use_const = False
+                    break
+
+        if use_const:
+            return self.__integrate_constant(integrator_options, curr_state, y0, curr_time,
+                            propensities, y_map, compiled_reactions, active_rr, event_queue,
+                            delayed_events, trigger_states, event_sensitivity, tau_step)
 
         from functools import partial
         events = self.model.listOfEvents.values()
         dense_output = False
         int_args = [curr_state, self.model.listOfSpecies, self.model.listOfReactions,
                     self.model.listOfRateRules,
                     propensities, y_map,
@@ -543,23 +598,35 @@
                     events,
                     self.model.listOfAssignmentRules]
         rhs = lambda t, y: TauHybridSolver.__f(t, y, *int_args)
         if 'min_step' in integrator_options:
             tau_step = max(integrator_options['min_step'], tau_step)
         else:
             tau_step = max(1e-6, tau_step)
-        next_tau = curr_time + tau_step
+        #next_tau = curr_time + tau_step
+        last_curr_time = curr_time
+
+        # Set curr time to next time a change occurs in the system outside of
+        # the standard ODE process.  Determine what kind of change this is,
+        # and set the curr_time of simulation to restart simulation after
+        # making the appropriate state changes.
+        event_times = {}
+        reaction_times = []
+        next_step, curr_time = self.__get_next_step(event_times, reaction_times,
+                                                    delayed_events,
+                                                    self.model.tspan[-1], curr_time + tau_step)
         curr_state['t'] = curr_time
         curr_state['time'] = curr_time
+        actual_tau_step = last_curr_time - curr_time
 
         # Integrate until end or tau is reached
         loop_count = 0
-        sol = LSODA(rhs, curr_time, y0, next_tau)
+        sol = LSODA(rhs, last_curr_time, y0, curr_time)
         counter = 0
-        while sol.t < next_tau:
+        while sol.t < curr_time:
             counter += 1
             sol.step()
 
 
         # Update states of all species based on changes made to species through
         # ODE processes.  This will update all species whose mode is set to
         # 'continuous', as well as 'dynamic' mode species which have been
@@ -576,24 +643,14 @@
                                                trigger_states, curr_time, curr_state)
         else:
             event_times = {}
 
         # Get next tau time
         reaction_times = []
         '''
-        # Set curr time to next time a change occurs in the system outside of
-        # the standard ODE process.  Determine what kind of change this is,
-        # and set the curr_time of simulation to restart simulation after
-        # making the appropriate state changes.
-        event_times = {}
-        reaction_times = []
-        next_step, curr_time = self.__get_next_step(event_times, reaction_times,
-                                                    delayed_events,
-                                                    self.model.tspan[-1], next_tau)
-        curr_state['t'] = curr_time
 
         # Stochastic Reactions are also fired through a root-finding method
         # which mirrors the standard SSA probability.  Since we are using
         # Tau-Leaping, rather than firing reactions based on a direct poisson
         # distribution from the propensity, we use that same poisson
         # distribution to select a random negative offset for the reaction
         # state, then integrate forward along with any deterministic
@@ -621,15 +678,15 @@
         # reached the designated time of execution, we add all currently
         # designated event assignments to a heap to be processed in Event
         # Priority order.
         elif next_step == 'delay':
             event = heapq.heappop(delayed_events)
             heapq.heappush(event_queue, (eval(self.model.listOfEvents[event[1]].priority), event[1]))
 
-        return sol, curr_time
+        return curr_time, actual_tau_step
 
 
     def __simulate_negative_state_check(self, curr_state):
             # check each species to see if they are negative
             for s in self.non_negative_species:
                 if curr_state[s] < 0:
                     raise SimulationError(f"Negative State detected at begining of step." \
@@ -645,15 +702,15 @@
                 err_message += f"'{s}' has negative state '{curr_state[s]}'"
         return (invalid_state, err_message)
 
     def __simulate(self, integrator_options, curr_state, y0, curr_time,
                    propensities, species, parameters, compiled_reactions,
                    active_rr, y_map, trajectory, save_times, save_index,
                    delayed_events, trigger_states, event_sensitivity,
-                   tau_step, debug, det_spec):
+                   tau_step, debug, det_spec, det_rxn):
         """
         Function to process simulation until next step, which can be a
         stochastic reaction firing, an event trigger or assignment, or end of
         simulation.
 
         :param curr_state: Contains all state variables for system at current time
         :type curr_state: dict
@@ -661,16 +718,14 @@
         :param curr_time: Represents current time
         :type curr_time: float
 
         :param save_times: Currently unreached save points
         :type save_times: list
 
         :returns: curr_state, curr_time, save_times, sol
-            sol - Python object returned from LSODA which contains all solution
-            data.
         """
 
         # first check if we have a valid state:
         self.__simulate_negative_state_check(curr_state)
         if curr_time == 0.0:
             # save state at beginning of simulation
             save_index = self.__save_state_to_output(
@@ -696,28 +751,28 @@
             for k in list(self.model.listOfSpecies)+list(self.model.listOfReactions):
                 self.profile_data[k].append(curr_state[k])
 
 
         # check each reaction to see if it is >=0. If we have taken a single SSA step, this could be >0 for the non-selected reactions, check if propensity is zero and reset if so
         for r in compiled_reactions.keys():
             if curr_state[r] >= 0 and propensities[r] == 0:
-                curr_state[r] = math.log(random.uniform(0, 1))
+                curr_state[r] = math.log(np.random.uniform(0, 1))
 
-        sol, curr_time = self.__integrate(integrator_options, curr_state,
+        curr_time, actual_tau_step = self.__integrate(integrator_options, curr_state,
                                           y0, curr_time, propensities, y_map,
                                           compiled_reactions,
                                           active_rr,
                                           event_queue,
                                           delayed_events,
                                           trigger_states,
                                           event_sensitivity,
-                                          tau_step
+                                          tau_step, det_rxn
                                           )
 
-        species_modified,rxn_count = self.__update_stochastic_rxn_states(compiled_reactions, curr_state)
+        species_modified,rxn_count = self.__update_stochastic_rxn_states(propensities, actual_tau_step, compiled_reactions, curr_state)
 
         # Occasionally, a tau step can result in an overly-aggressive
         # forward step and cause a species population to fall below 0,
         # which would result in an erroneous simulation.
         # We estimate the time to the first
         # stochatic reaction firing (assume constant propensities) and
         # simulate the ODE system until that time, fire that reaction
@@ -758,29 +813,29 @@
                     if min_tau is None or min_tau > rxn_times[rname]:
                         min_tau = rxn_times[rname]
                         rxn_selected = rname
             if rxn_selected is None: raise SimulationError(f"Negative State detected in step, and no reaction found to fire. error_message={invalid_err_message}")
 
             tau_step = min_tau #estimated time to the first stochatic reaction
 
-            sol, curr_time = self.__integrate(integrator_options, curr_state,
+            curr_time, actual_tau_step = self.__integrate(integrator_options, curr_state,
                                           y0, curr_time, propensities, y_map,
                                           compiled_reactions,
                                           active_rr,
                                           event_queue,
                                           delayed_events,
                                           trigger_states,
                                           event_sensitivity,
-                                          tau_step
+                                          tau_step, det_rxn
                                           )
 
             # only update the selected reaction
             first_rxn_count = copy.deepcopy(rxn_count)
             first_err_message = invalid_err_message
-            species_modified,rxn_count = self.__update_stochastic_rxn_states(compiled_reactions, curr_state, only_update=rxn_selected)
+            species_modified,rxn_count = self.__update_stochastic_rxn_states(propensities, actual_tau_step, compiled_reactions, curr_state, only_update=rxn_selected)
 
             (invalid_state, invalid_err_message) = self.__simulate_invalid_state_check(species_modified, curr_state, compiled_reactions)
             if invalid_state:
                 raise SimulationError(f"Negative State detected in step, after single SSA step. error_message={invalid_err_message}")
 
 
         save_index = self.__save_state_to_output(curr_time, save_index, curr_state, species, trajectory, save_times)
@@ -800,23 +855,23 @@
                                         event_queue, trigger_states, delayed_events)
                     event_cycle = True
                 elif not triggered:
                     curr_state[e.name] = False
 
         events_processed = self.__process_queued_events(event_queue, trigger_states, curr_state, det_spec)
 
-        return sol, curr_state, curr_time, save_times, save_index
+        return curr_state, curr_time, save_times, save_index
 
     def __set_seed(self, seed):
         # Set seed if supplied
         if seed is not None:
             if not isinstance(seed, int):
                 seed = int(seed)
             if seed > 0:
-                random.seed(seed)
+                np.random.seed(seed)
             else:
                 raise ModelError('seed must be a positive integer')
 
     def __set_recommended_ode_defaults(self, integrator_options):
         """
         Set some ODE solver defaults.  These values are chosen based on the
         precision required to successfully complete the SBML Test suite.
@@ -862,15 +917,15 @@
 
         # initialize species population state
         for s in self.model.listOfSpecies:
             curr_state[s] = self.model.listOfSpecies[s].initial_value
 
         # Set reactions to uniform random number
         for i, r in enumerate(self.model.listOfReactions):
-            curr_state[r] = math.log(random.uniform(0, 1))
+            curr_state[r] = math.log(np.random.uniform(0, 1))
             if debug:
                 print("Setting Random number ", curr_state[r], " for ", self.model.listOfReactions[r].name)
 
         # Initialize event last-fired times to 0
         for e_name in self.model.listOfEvents:
             curr_state[e_name] = 0
 
@@ -1009,14 +1064,15 @@
                 raise SimulationError("A model is required to run the simulation.")
             self.model = copy.deepcopy(model)
 
         self.model.compile_prep()
         self.validate_model(self.model, model)
         self.validate_sbml_features(model=self.model)
 
+
         self.validate_tspan(increment=increment, t=t)
         if increment is None:
             increment = self.model.tspan[-1] - self.model.tspan[-2]
         if t is None:
             t = self.model.tspan[-1]
 
         if timeout is not None and timeout > 0:
@@ -1191,14 +1247,19 @@
 
             trajectory = trajectory_base[trajectory_num]  # NumPy array containing this simulation's results
             propensities = OrderedDict()  # Propensities evaluated at current state
 
             curr_state[0] = initial_state.copy()
             curr_time[0] = 0  # Current Simulation Time
 
+            for i, r in enumerate(self.model.listOfReactions):
+                curr_state[0][r] = math.log(np.random.uniform(0, 1))
+                if debug:
+                    print("Setting Random number ", curr_state[0][r], " for ", self.model.listOfReactions[r].name)
+
             end_time = self.model.tspan[-1]  # End of Simulation time
             entry_pos = 1
             data = OrderedDict()  # Dictionary for results
             data['time'] = timeline  # All time entries
             save_index = 0
 
             # Record Highest Order reactant for each reaction and set error tolerance
@@ -1235,20 +1296,29 @@
                     break
                 # Get current propensities
                 for i, r in enumerate(self.model.listOfReactions):
                     try:
                         propensities[r] = eval(compiled_propensities[r], eval_globals, curr_state[0])
                         if curr_state[0][r] > 0 and propensities[r]==0:
                             # This is an edge case, that might happen after a single SSA step.
-                            curr_state[0][r] = math.log(random.uniform(0, 1))
+                            curr_state[0][r] = math.log(np.random.uniform(0, 1))
                     except Exception as e:
                         raise SimulationError('Error calculation propensity for {0}.\nReason: {1}\ncurr_state={2}'.format(r, e, curr_state))
 
                 # Calculate Tau statistics and select a good tau step
-                tau_step = Tau.select(HOR, reactants, mu_i, sigma_i, g_i, epsilon_i, tau_tol, critical_threshold, self.model, propensities, curr_state[0], curr_time[0], save_times[0])
+                if self.constant_tau_stepsize is None:
+                    tau_step = Tau.select(HOR, reactants, mu_i, sigma_i, g_i, epsilon_i, tau_tol, critical_threshold, self.model, propensities, curr_state[0], curr_time[0], save_times[0])
+                else:
+                    tau_step = self.constant_tau_stepsize
+                if debug:
+                    X = ''
+                    for k,v in curr_state[0].items():
+                        X+= f'{k}:{v:.2f} '
+                    print(f"t={curr_time[0]} tau={tau_step} curr_state={X}")
+
 
                 # Process switching if used
                 mn, sd, CV = self.__calculate_statistics(curr_time[0], propensities, curr_state[0], tau_step, det_spec)
 
                 # Calculate sd and CV for hybrid switching and flag deterministic reactions
                 deterministic_reactions = self.__flag_det_reactions(det_spec, det_rxn, dependencies)
 
@@ -1265,24 +1335,24 @@
                                                         dependencies, curr_state[0], det_spec, rr_sets)
 
                 # Create integration initial state vector
                 y0, y_map = self.__map_state(species, parameters,
                                              compiled_reactions, self.model.listOfEvents, curr_state[0])
 
                 # Run simulation to next step
-                sol, curr_state[0], curr_time[0], save_times, save_index = self.__simulate(integrator_options,
+                curr_state[0], curr_time[0], save_times, save_index = self.__simulate(integrator_options,
                                                                                curr_state[0], y0, curr_time[0],
                                                                                propensities, species,
                                                                                parameters, compiled_reactions,
                                                                                active_rr, y_map,
                                                                                trajectory, save_times, save_index,
                                                                                delayed_events,
                                                                                trigger_states,
                                                                                event_sensitivity, tau_step,
-                                                                               debug, det_spec)
+                                                                               debug, det_spec, det_rxn)
 
             # End of trajectory, format results
             data = {'time': timeline}
             for i in range(number_species):
                 data[species[i]] = trajectory[:, i + 1]
             simulation_data.append(data)
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/numpy/tau_leaping_solver.py` & `gillespy2-1.8.2/gillespy2/solvers/numpy/tau_leaping_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,26 +39,27 @@
 
     name = "TauLeapingSolver"
     rc = 0
     stop_event = None
     pause_event = None
     result = None
 
-    def __init__(self, model=None, debug=False):
+    def __init__(self, model=None, debug=False, constant_tau_stepsize=None):
         if model is None:
             raise SimulationError("A model is required to run the simulation.")
 
         name = "TauLeapingSolver"
         rc = 0
         stop_event = None
         pause_event = None
         result = None
         self.model = copy.deepcopy(model)
         self.debug = debug
         self.is_instantiated = True
+        self.constant_tau_stepsize = constant_tau_stepsize
 
     def __get_reactions(self, step, curr_state, curr_time, save_time, propensities, reactions):
         """
         Helper Function to get reactions fired from t to t+tau.  
         :returns: Three values:
             rxn_count - dict with key=Reaction channel value=number of times fired
             curr_state - dict containing all state variables for system at current time
@@ -138,15 +139,15 @@
 
         :param resume: Result of a previously run simulation, to be resumed.
         :type resume: gillespy2.Results
 
         :param tau_tol: Tolerance level for Tau leaping algorithm.  Larger tolerance values will
             result in larger tau steps. Default value is 0.03.
         :type tau_tol: float
-        
+
         :returns: A result object containing the results of the simulation.
         :rtype: gillespy2.Results
         """
         from gillespy2 import log
 
         if self is None:
             # Post deprecation block
@@ -158,14 +159,15 @@
 
                 You should use `gillespy2.Model.run(solver=TauLeapingSolver(model=gillespy2.Model))
                 Future releases of GillesPy2 may not support this feature.
                 """
             )
             self = TauLeapingSolver(model=model, debug=debug, profile=profile)
 
+
         if model is not None:
             log.warning('model = gillespy2.model is deprecated. Future releases '
                         'of GillesPy2 may not support this feature.')
         if self.model is None:
             if model is None:
                 raise SimulationError("A model is required to run the simulation.")
             self.model = copy.deepcopy(model)
@@ -396,15 +398,19 @@
                     for i, r in enumerate(self.model.listOfReactions):
                         propensities[r] = eval(compiled_propensities[r], curr_state[0])
                         propensity_sum += propensities[r]
 
                     tau_args = [HOR, reactants, mu_i, sigma_i, g_i, epsilon_i, tau_tol, critical_threshold,
                                 self.model, propensities, curr_state[0], curr_time[0], save_time]
 
-                    tau_step = Tau.select(*tau_args)
+                    if self.constant_tau_stepsize is None:
+                        tau_step = Tau.select(*tau_args)
+                        #print(f"t={curr_time[0]} tau={tau_step}")
+                    else:
+                        tau_step = self.constant_tau_stepsize
 
                     prev_start_state = start_state.copy()
                     prev_curr_state = curr_state[0].copy()
                     prev_curr_time = curr_time[0]
                     total_time[0] = curr_time[0]
 
                     loop_cnt = 0
```

### Comparing `gillespy2-1.8.1/gillespy2/solvers/utilities/Tau.py` & `gillespy2-1.8.2/gillespy2/solvers/utilities/Tau.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/utilities/__init__.py` & `gillespy2-1.8.2/gillespy2/solvers/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/utilities/cpp_support_test.py` & `gillespy2-1.8.2/gillespy2/solvers/utilities/cpp_support_test.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/solvers/utilities/solverutils.py` & `gillespy2-1.8.2/gillespy2/solvers/utilities/solverutils.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2/stochss/StochSSexport.py` & `gillespy2-1.8.2/gillespy2/stochss/StochSSexport.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+''' Module for exporting GillesPy2 model as StochSS Live! models. '''
 import ast
 import json
 
 from gillespy2.core.jsonify import ComplexJsonCoder
 
 def __add_events(model, events):
     for name, event in events.items():
@@ -51,16 +51,16 @@
         event['eventAssignments'].append(s_assignment)
 
 
 def __add_function_definitions(model, function_definitions):
     for name, function_definition in function_definitions.items():
         variables = function_definition.get_arg_string()
         expression = function_definition.function_string
-        function = "lambda({0}, {1})".format(variables, expression)
-        signature = "{0}({1})".format(name, variables)
+        function = f"lambda({variables}, {expression})"
+        signature = f"{name}({variables})"
 
         s_function_definition = {"compID":model['defaultID'],
                                  "name":name,
                                  "function":function,
                                  "expression":expression,
                                  "variables":variables,
                                  "signature":signature,
@@ -69,15 +69,15 @@
         model['defaultID'] += 1
 
 
 def __add_parameters(model, parameters):
     for name, parameter in parameters.items():
         try:
             expression = ast.literal_eval(parameter.expression)
-        except:
+        except Exception: # pylint: disable=broad-except
             expression = parameter.expression
         s_parameter = {"compID":model['defaultID'],
                        "name":name,
                        "expression":str(expression),
                        "annotation": ""}
         model['parameters'].append(s_parameter)
         model['defaultID'] += 1
@@ -181,15 +181,15 @@
 
 
 def __get_species(species, name):
     return list(filter(lambda specie: specie['name'] == name, species))[0]
 
 
 def __write_to_file(model, path):
-    with open(path, "w") as model_file:
+    with open(path, "w", encoding="utf-8") as model_file:
         json.dump(model, model_file, indent=4, sort_keys=True, cls=ComplexJsonCoder)
 
 
 def export(model, path=None, return_stochss_model=False):
     """
     GillesPy model to StochSS converter
 
@@ -203,33 +203,39 @@
     model.compile_prep()
 
     if path is None:
         path = f"{model.name}.mdl"
 
     if model.tspan is None:
         model_settings = {"endSim": 20, "timeStep": 0.05}
+    elif type(model.tspan).__name__ == "TimeSpan":
+        model_settings = {
+            "endSim": model.tspan.items[-1],
+            "timeStep": model.tspan.items[1] - model.tspan.items[0]
+        }
     else:
         model_settings = {
             "endSim": model.tspan[-1],
-            "timeStep": model.tspan[-1] / len(model.tspan)
+            "timeStep": model.tspan[1] - model.tspan[0]
         }
 
-    s_model = {"is_spatial": False,
-               "defaultID": 1,
-               "annotation": "",
-               "volume": model.volume,
-               "modelSettings": model_settings,
-                "species": [],
-                "initialConditions": [],
-                "parameters": [],
-                "reactions": [],
-                "rules": [],
-                "eventsCollection": [],
-                "functionDefinitions": []
-              }
+    s_model = {
+        "is_spatial": False,
+        "defaultID": 1,
+        "annotation": "",
+        "volume": model.volume,
+        "modelSettings": model_settings,
+        "species": [],
+        "initialConditions": [],
+        "parameters": [],
+        "reactions": [],
+        "rules": [],
+        "eventsCollection": [],
+        "functionDefinitions": []
+    }
 
     __add_species(model=s_model, species=model.get_all_species())
     __add_parameters(model=s_model, parameters=model.get_all_parameters())
     __add_reactions(model=s_model, reactions=model.get_all_reactions())
     __add_events(model=s_model, events=model.get_all_events())
     __add_rules(model=s_model, r_type='Rate Rule', rules=model.get_all_rate_rules())
     __add_rules(model=s_model, r_type='Assignment Rule', rules=model.get_all_assignment_rules())
```

### Comparing `gillespy2-1.8.1/gillespy2/stochss/__init__.py` & `gillespy2-1.8.2/gillespy2/stochss/__init__.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/gillespy2.egg-info/PKG-INFO` & `gillespy2-1.8.2/gillespy2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gillespy2
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python interface for Gillespie-style biochemical simulations
 Home-page: https://github.com/StochSS/GillesPy2
 Download-URL: https://pypi.org/project/gillespy2/#files
 Author: See AUTHORS
 Author-email: bdrawert@unca.edu
 Maintainer: See AUTHORS
 Maintainer-email: bdrawert@unca.edu
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gillespy2 Version: 1.8.1 Summary: Python interface
+Metadata-Version: 2.1 Name: gillespy2 Version: 1.8.2 Summary: Python interface
 for Gillespie-style biochemical simulations Home-page: https://github.com/
 StochSS/GillesPy2 Download-URL: https://pypi.org/project/gillespy2/#files
 Author: See AUTHORS Author-email: bdrawert@unca.edu Maintainer: See AUTHORS
 Maintainer-email: bdrawert@unca.edu License: GPL Project-URL: Tracker, https://
 github.com/StochSS/GillesPy2/issues Project-URL: Source, https://github.com/
 StochSS/GillesPy2 Keywords: biochemical simulation,Gillespie
 algorithm,stochastic simulation,biology Classifier: Development Status :: 5 -
```

### Comparing `gillespy2-1.8.1/gillespy2.egg-info/SOURCES.txt` & `gillespy2-1.8.2/gillespy2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/setup.py` & `gillespy2-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_SBML.py` & `gillespy2-1.8.2/test/test_SBML.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             import libsbml
         except ImportError:
             return
 
         model_path = os.path.join(os.path.dirname(__file__), "assets", "test_sbml.xml")
         sbml_model, errors = import_SBML(model_path)
         solver = ODESolver(model=sbml_model)
-        sbml_results = sbml_model.run(solver=solver, increment=0.05, t=20)
+        sbml_results = sbml_model.run(solver=solver)
 
     def test_sbml_string_replace(self):
         """
         Ensure that non-supported symbols are converted to supported symbols (such as ln -> log)
         """
         try:
             import libsbml
```

### Comparing `gillespy2-1.8.1/test/test_StochML.py` & `gillespy2-1.8.2/test/test_StochML.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_all_solvers.py` & `gillespy2-1.8.2/test/test_all_solvers.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_build_engine.py` & `gillespy2-1.8.2/test/test_build_engine.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_c_decode.py` & `gillespy2-1.8.2/test/test_c_decode.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_c_solver_integrators.py` & `gillespy2-1.8.2/test/test_c_solver_integrators.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_c_solver_perf.py` & `gillespy2-1.8.2/test/test_c_solver_perf.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_c_solvers.py` & `gillespy2-1.8.2/test/test_c_solvers.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_check_cpp_support.py` & `gillespy2-1.8.2/test/test_check_cpp_support.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_empty_model.py` & `gillespy2-1.8.2/test/test_empty_model.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_example_models.py` & `gillespy2-1.8.2/test/test_example_models.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_hybrid_c_events.py` & `gillespy2-1.8.2/test/test_hybrid_c_events.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_hybrid_event_round.py` & `gillespy2-1.8.2/test/test_hybrid_event_round.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_hybrid_negative_state.py` & `gillespy2-1.8.2/test/test_hybrid_negative_state.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_hybrid_solver.py` & `gillespy2-1.8.2/test/test_hybrid_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_hybrid_solver_opioid_model.py` & `gillespy2-1.8.2/test/test_hybrid_solver_opioid_model.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_jsonify.py` & `gillespy2-1.8.2/test/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_model.py` & `gillespy2-1.8.2/test/test_model.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_notebooks.py` & `gillespy2-1.8.2/test/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_numpy_ssa_solver.py` & `gillespy2-1.8.2/test/test_numpy_ssa_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_ode_c_solver.py` & `gillespy2-1.8.2/test/test_ode_c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_ode_solver.py` & `gillespy2-1.8.2/test/test_ode_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_pause_resume.py` & `gillespy2-1.8.2/test/test_pause_resume.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_propensity_parser.py` & `gillespy2-1.8.2/test/test_propensity_parser.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_python_solver_perf.py` & `gillespy2-1.8.2/test/test_python_solver_perf.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_results.py` & `gillespy2-1.8.2/test/test_results.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_run_output.py` & `gillespy2-1.8.2/test/test_run_output.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_simple_model.py` & `gillespy2-1.8.2/test/test_simple_model.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_ssa_c_solver.py` & `gillespy2-1.8.2/test/test_ssa_c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_sys_init.py` & `gillespy2-1.8.2/test/test_sys_init.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_tau_hybrid_c_solver.py` & `gillespy2-1.8.2/test/test_tau_hybrid_c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_tau_leaping_c_solver.py` & `gillespy2-1.8.2/test/test_tau_leaping_c_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_tau_leaping_solver.py` & `gillespy2-1.8.2/test/test_tau_leaping_solver.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_telegraph_model.py` & `gillespy2-1.8.2/test/test_telegraph_model.py`

 * *Files identical despite different names*

### Comparing `gillespy2-1.8.1/test/test_variable_solvers.py` & `gillespy2-1.8.2/test/test_variable_solvers.py`

 * *Files identical despite different names*

