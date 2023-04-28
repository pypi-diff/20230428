# Comparing `tmp/cylp-0.91.5.tar.gz` & `tmp/cylp-0.91.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylp-0.91.5.tar", last modified: Sat Mar 26 19:54:40 2022, max compression
+gzip compressed data, was "cylp-0.91.6.tar", last modified: Fri Apr 21 03:30:11 2023, max compression
```

## Comparing `cylp-0.91.5.tar` & `cylp-0.91.6.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.833649 cylp-0.91.5/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-26 19:54:24.000000 cylp-0.91.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    13918 2022-03-26 19:54:24.000000 cylp-0.91.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-03-26 19:54:24.000000 cylp-0.91.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7259 2022-03-26 19:54:40.833649 cylp-0.91.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6798 2022-03-26 19:54:24.000000 cylp-0.91.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.821649 cylp-0.91.5/cylp/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.825649 cylp-0.91.5/cylp/cpp/
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/CbcCompareUser.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/CbcCompareUser.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/CyClpSimplex_api.h
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICbc.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICbc.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICbcModel.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICbcModel.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICbcNode.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICbcNode.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICglCutGeneratorBase.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICglCutGeneratorBase.h
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpDualRowPivotBase.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpDualRowPivotBase.h
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpPackedMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpPackedMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivot.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivot.h
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivotBase.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivotBase.h
--rw-r--r--   0 runner    (1001) docker     (121)    46601 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpSimplex.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8786 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpSimplex.hpp
--rw-r--r--   0 runner    (1001) docker     (121)   114708 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpSimplexPrimal.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8186 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpSimplexPrimal.hpp
--rw-r--r--   0 runner    (1001) docker     (121)   116485 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpSimplexPrimal_Wolfe.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IClpSimplexPrimal_Wolfe.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinIndexedVector.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinIndexedVector.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4851 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinMP.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinMP.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinModel.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7225 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinMpsIO.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinMpsIO.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinPackedMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/ICoinPackedMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IOsiCuts.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cpp/IOsiCuts.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.829649 cylp-0.91.5/cylp/cy/
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCbcModel.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10148 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCbcModel.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCbcNode.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCbcNode.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCgl.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCgl.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCglCutGeneratorBase.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCglCutGeneratorBase.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCglTreeInfo.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCglTreeInfo.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3891 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyClpDualRowPivotBase.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3392 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyClpDualRowPivotBase.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyClpPrimalColumnPivotBase.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyClpPrimalColumnPivotBase.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    13665 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyClpSimplex.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    78023 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyClpSimplex.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinIndexedVector.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinIndexedVector.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinModel.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5408 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinModel.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinMpsIO.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6769 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinMpsIO.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinPackedMatrix.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCoinPackedMatrix.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCutGeneratorPythonBase.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyCutGeneratorPythonBase.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyDantzigPivot.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyDantzigPivot.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyDualPivotPythonBase.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyDualPivotPythonBase.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyOsiCuts.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyOsiCuts.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyOsiSolverInterface.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyOsiSolverInterface.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyPEPivot.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyPEPivot.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyPivotPythonBase.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyPivotPythonBase.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CySolve.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyTest.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyWolfePivot.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/CyWolfePivot.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-03-26 19:54:24.000000 cylp-0.91.5/cylp/cy/createCythonInterface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.829649 cylp-0.91.5/cylp/py/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/Constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/PySolve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.829649 cylp-0.91.5/cylp/py/QP/
--rw-r--r--   0 runner    (1001) docker     (121)    12396 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/QP/GQP.py
--rw-r--r--   0 runner    (1001) docker     (121)    59071 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/QP/QP.py
--rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/QP/QPGen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/QP/QPSReader.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/QP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.829649 cylp-0.91.5/cylp/py/mip/
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/mip/CyLPCutGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/mip/GomoryCutGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/mip/NodeCompareBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/mip/SimpleNodeCompare.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/mip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.829649 cylp-0.91.5/cylp/py/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)    41053 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/modeling/CyLPModel.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6947 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/modeling/test_modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.829649 cylp-0.91.5/cylp/py/pivots/
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/DantzigPivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/DualDantzigPivot.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/DualPivotPythonBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/LIFOPivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/MostFrequentPivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/PivotPythonBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     4670 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/PositiveEdgePivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     5281 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/PositiveEdgeWolfePivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/WolfePivot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8884 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/WolfePivotPE.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/pivots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/test_PySolve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.833649 cylp-0.91.5/cylp/py/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5072 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/utils/readSetcovering.py
--rw-r--r--   0 runner    (1001) docker     (121)    19307 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/utils/sparseUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-03-26 19:54:25.000000 cylp-0.91.5/cylp/py/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 19:54:40.821649 cylp-0.91.5/cylp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7259 2022-03-26 19:54:40.000000 cylp-0.91.5/cylp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-03-26 19:54:40.000000 cylp-0.91.5/cylp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 19:54:40.000000 cylp-0.91.5/cylp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 19:54:39.000000 cylp-0.91.5/cylp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-26 19:54:40.000000 cylp-0.91.5/cylp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-26 19:54:40.000000 cylp-0.91.5/cylp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-03-26 19:54:25.000000 cylp-0.91.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-26 19:54:40.833649 cylp-0.91.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    17997 2022-03-26 19:54:25.000000 cylp-0.91.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.393189 cylp-0.91.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-21 03:29:59.000000 cylp-0.91.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-21 03:29:59.000000 cylp-0.91.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 03:29:59.000000 cylp-0.91.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-21 03:30:11.393189 cylp-0.91.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-21 03:29:59.000000 cylp-0.91.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.361189 cylp-0.91.6/cylp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.373189 cylp-0.91.6/cylp/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/CbcCompareUser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/CbcCompareUser.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/CyClpSimplex_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICbc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICbc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICbcModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICbcModel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICbcNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICbcNode.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICglCutGeneratorBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICglCutGeneratorBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpDualRowPivotBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpDualRowPivotBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpPackedMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpPackedMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivotBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivotBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46601 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpSimplex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpSimplex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   114708 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpSimplexPrimal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpSimplexPrimal.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   116485 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpSimplexPrimal_Wolfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IClpSimplexPrimal_Wolfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinIndexedVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinIndexedVector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinMP.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinMP.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinModel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinMpsIO.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinMpsIO.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinPackedMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/ICoinPackedMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IOsiCuts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cpp/IOsiCuts.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.385189 cylp-0.91.6/cylp/cy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCbcModel.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCbcModel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCbcNode.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCbcNode.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCgl.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCgl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCglCutGeneratorBase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCglCutGeneratorBase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCglTreeInfo.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCglTreeInfo.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyClpDualRowPivotBase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyClpDualRowPivotBase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyClpPrimalColumnPivotBase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyClpPrimalColumnPivotBase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyClpSimplex.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    78023 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyClpSimplex.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinIndexedVector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinIndexedVector.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinModel.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinModel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinMpsIO.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinMpsIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinPackedMatrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCoinPackedMatrix.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCutGeneratorPythonBase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyCutGeneratorPythonBase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyDantzigPivot.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyDantzigPivot.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyDualPivotPythonBase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyDualPivotPythonBase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyOsiCuts.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyOsiCuts.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyOsiSolverInterface.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyOsiSolverInterface.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyPEPivot.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyPEPivot.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyPivotPythonBase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyPivotPythonBase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CySolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyTest.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyWolfePivot.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/CyWolfePivot.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/cy/createCythonInterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.385189 cylp-0.91.6/cylp/py/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/PySolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.385189 cylp-0.91.6/cylp/py/QP/
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/QP/GQP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59071 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/QP/QP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/QP/QPGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/QP/QPSReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/QP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.389189 cylp-0.91.6/cylp/py/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/mip/CyLPCutGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/mip/GomoryCutGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/mip/NodeCompareBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/mip/SimpleNodeCompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/mip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.389189 cylp-0.91.6/cylp/py/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    41053 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/modeling/CyLPModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/modeling/test_modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.393189 cylp-0.91.6/cylp/py/pivots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/DantzigPivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/DualDantzigPivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/DualPivotPythonBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/LIFOPivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/MostFrequentPivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/PivotPythonBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/PositiveEdgePivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/PositiveEdgeWolfePivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/WolfePivot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/WolfePivotPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/pivots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/test_PySolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.393189 cylp-0.91.6/cylp/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/utils/readSetcovering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/utils/sparseUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-21 03:29:59.000000 cylp-0.91.6/cylp/py/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:30:11.361189 cylp-0.91.6/cylp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-21 03:30:11.000000 cylp-0.91.6/cylp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 03:30:11.000000 cylp-0.91.6/cylp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:30:11.000000 cylp-0.91.6/cylp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:30:11.000000 cylp-0.91.6/cylp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 03:30:11.000000 cylp-0.91.6/cylp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 03:30:11.000000 cylp-0.91.6/cylp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-21 03:29:59.000000 cylp-0.91.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:30:11.393189 cylp-0.91.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    18199 2023-04-21 03:29:59.000000 cylp-0.91.6/setup.py
```

### Comparing `cylp-0.91.5/LICENSE` & `cylp-0.91.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/PKG-INFO` & `cylp-0.91.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cylp
-Version: 0.91.5
+Version: 0.91.6
 Summary: A Python interface for CLP, CBC, and CGL
 Home-page: https://github.com/coin-or/cylp
 Author: Mehdi Towhidi (mehdi.towhidi@gerad.ca), Dominique Orban (dominique.orban@gerad.ca)
 Author-email: mehdi.towhidi@gerad.ca
 Maintainer: Ted Ralphs
 Maintainer-email: ted@lehigh.edu
 License: Eclipse Public License
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 CyLP
 ====
 
@@ -43,27 +42,51 @@
 ------------------------------------------
 
 On Windows, a binary wheel is available and it is not necessary to install Cbc.
 Just do::
 
     $ python -m pip install cylp
 
+On Linux/macOS: Installation as a binary wheel
+---------------------------------------------------------
+
+Binary wheels are available for Linux and some versions of OS X 
+for some versions of Python. To see if there is a wheel available
+for your platform, you can browse 
+
+https://pypi.org/project/cylp/#files
+
+or just try::
+
+    $ python -m pip install cylp
+
+In case this fails, it is most likely that there is no wheel for your platform.
+If you are on Linux, this can probably be addressed by switching to 
+a supported Python version with, e.g., conda::
+
+    $ conda create -n cylp python=3.9
+    $ conda activate cylp
+    
+If all else fails, it is easy to install from source, but Cbc must be 
+installed first, as detailed below. The easiest route for this is to use
+conda.
+
 On Linux/macOS with conda: Installation from source
 ---------------------------------------------------
 
 CyLP depends on `NumPy <https://numpy.org>`_ and `Cython <https://cython.org/>`_
 as prerequisites for building from source (`build-system requires`).
 You will also need to install binaries for Cbc. The version should be 2.10 (recommended) or earlier 
 (current master branch of Cbc will not work with this version of CyLP).
 
 The following commands will create and activate a new conda environment with all
 these prerequisites installed::
 
-    $ conda create -n cbc coin-or-cbc cython numpy pkg-config scipy -c conda-forge
-    $ conda activate cbc
+    $ conda create -n cylp coin-or-cbc cython numpy pkg-config scipy -c conda-forge
+    $ conda activate cylp
 
 Now you can install CyLP from PyPI::
 
     $ pip install --no-build-isolation cylp
 
 (The option `--no-build-isolation` ensures that `cylp` uses the Python packages
 installed by conda in the build phase.)
@@ -76,17 +99,19 @@
 -------------------------------------------------
 
 First of all, you will need to install binaries for Cbc. The version should be 2.10 (recommended) or earlier 
 (current master branch of Cbc will not work with this version of CyLP).
 You can install Cbc by either by installing with your system's package manager, by downloading pre-built binaries,
 or by building yourself from source using `coinbrew <https://github.com/coin-or/coinbrew>`_.
 
-1. To install Cbc in Linux, the easiest way is to use a package manager. Install `coinor-libcbc-dev` on Ubuntu/Debian 
-   or `coin-or-Cbc-devel` on Fedora.
-    
+1. To install Cbc in Linux, the easiest way is to use a package manager. Install
+   `coinor-libcbc-dev` on Ubuntu/Debian or `coin-or-Cbc-devel` on Fedora, or the
+   `corresponding package on your distribution
+   <https://doc.sagemath.org/html/en/reference/spkg/cbc.html#equivalent-system-packages>`_.
+
 #. On macOS, it is easiest to install Cbc with homebrew:
          
    ``$ brew install cbc pkg-config``
 
 You should no longer need to build Cbc from source on any platform unless for some reason, none of the
 above recipes applies to you. If you do need to build from source, please go to the `Cbc <https://github.com/coin-or/Cbc>`_
 project page and follow the instructions there. After building and installing, make sure to 
@@ -203,9 +228,7 @@
 #. Sherbrooke university hospital (Centre hospitalier universitaire de Sherbrooke): CyLP is used for nurse scheduling.
 #. Maisonneuve-Rosemont hospital (L'hôpital HMR): CyLP is used for  physician scheduling with preferences.
 #. Lehigh University: CyLP is used to teach mixed-integer cuts.
 #. IBM T. J. Watson research center
 #. Saarland University, Germany
 
 
-
-
```

### Comparing `cylp-0.91.5/README.rst` & `cylp-0.91.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -28,27 +28,51 @@
 ------------------------------------------
 
 On Windows, a binary wheel is available and it is not necessary to install Cbc.
 Just do::
 
     $ python -m pip install cylp
 
+On Linux/macOS: Installation as a binary wheel
+---------------------------------------------------------
+
+Binary wheels are available for Linux and some versions of OS X 
+for some versions of Python. To see if there is a wheel available
+for your platform, you can browse 
+
+https://pypi.org/project/cylp/#files
+
+or just try::
+
+    $ python -m pip install cylp
+
+In case this fails, it is most likely that there is no wheel for your platform.
+If you are on Linux, this can probably be addressed by switching to 
+a supported Python version with, e.g., conda::
+
+    $ conda create -n cylp python=3.9
+    $ conda activate cylp
+    
+If all else fails, it is easy to install from source, but Cbc must be 
+installed first, as detailed below. The easiest route for this is to use
+conda.
+
 On Linux/macOS with conda: Installation from source
 ---------------------------------------------------
 
 CyLP depends on `NumPy <https://numpy.org>`_ and `Cython <https://cython.org/>`_
 as prerequisites for building from source (`build-system requires`).
 You will also need to install binaries for Cbc. The version should be 2.10 (recommended) or earlier 
 (current master branch of Cbc will not work with this version of CyLP).
 
 The following commands will create and activate a new conda environment with all
 these prerequisites installed::
 
-    $ conda create -n cbc coin-or-cbc cython numpy pkg-config scipy -c conda-forge
-    $ conda activate cbc
+    $ conda create -n cylp coin-or-cbc cython numpy pkg-config scipy -c conda-forge
+    $ conda activate cylp
 
 Now you can install CyLP from PyPI::
 
     $ pip install --no-build-isolation cylp
 
 (The option `--no-build-isolation` ensures that `cylp` uses the Python packages
 installed by conda in the build phase.)
@@ -61,17 +85,19 @@
 -------------------------------------------------
 
 First of all, you will need to install binaries for Cbc. The version should be 2.10 (recommended) or earlier 
 (current master branch of Cbc will not work with this version of CyLP).
 You can install Cbc by either by installing with your system's package manager, by downloading pre-built binaries,
 or by building yourself from source using `coinbrew <https://github.com/coin-or/coinbrew>`_.
 
-1. To install Cbc in Linux, the easiest way is to use a package manager. Install `coinor-libcbc-dev` on Ubuntu/Debian 
-   or `coin-or-Cbc-devel` on Fedora.
-    
+1. To install Cbc in Linux, the easiest way is to use a package manager. Install
+   `coinor-libcbc-dev` on Ubuntu/Debian or `coin-or-Cbc-devel` on Fedora, or the
+   `corresponding package on your distribution
+   <https://doc.sagemath.org/html/en/reference/spkg/cbc.html#equivalent-system-packages>`_.
+
 #. On macOS, it is easiest to install Cbc with homebrew:
          
    ``$ brew install cbc pkg-config``
 
 You should no longer need to build Cbc from source on any platform unless for some reason, none of the
 above recipes applies to you. If you do need to build from source, please go to the `Cbc <https://github.com/coin-or/Cbc>`_
 project page and follow the instructions there. After building and installing, make sure to
```

### Comparing `cylp-0.91.5/cylp/cpp/CbcCompareUser.cpp` & `cylp-0.91.6/cylp/cpp/CbcCompareUser.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/CbcCompareUser.hpp` & `cylp-0.91.6/cylp/cpp/CbcCompareUser.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/CyClpSimplex_api.h` & `cylp-0.91.6/cylp/cpp/CyClpSimplex_api.h`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICbc.cpp` & `cylp-0.91.6/cylp/cpp/ICbc.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICbc.hpp` & `cylp-0.91.6/cylp/cpp/ICbc.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICbcModel.cpp` & `cylp-0.91.6/cylp/cpp/ICbcModel.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICbcModel.hpp` & `cylp-0.91.6/cylp/cpp/ICbcModel.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICglCutGeneratorBase.cpp` & `cylp-0.91.6/cylp/cpp/ICglCutGeneratorBase.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICglCutGeneratorBase.h` & `cylp-0.91.6/cylp/cpp/ICglCutGeneratorBase.h`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpDualRowPivotBase.cpp` & `cylp-0.91.6/cylp/cpp/IClpDualRowPivotBase.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpDualRowPivotBase.h` & `cylp-0.91.6/cylp/cpp/IClpDualRowPivotBase.h`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpPackedMatrix.cpp` & `cylp-0.91.6/cylp/cpp/IClpPackedMatrix.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpPackedMatrix.hpp` & `cylp-0.91.6/cylp/cpp/IClpPackedMatrix.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivot.cpp` & `cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivot.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivot.h` & `cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivot.h`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivotBase.cpp` & `cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivotBase.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpPrimalColumnPivotBase.h` & `cylp-0.91.6/cylp/cpp/IClpPrimalColumnPivotBase.h`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpSimplex.cpp` & `cylp-0.91.6/cylp/cpp/IClpSimplex.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpSimplex.hpp` & `cylp-0.91.6/cylp/cpp/IClpSimplex.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpSimplexPrimal.cpp` & `cylp-0.91.6/cylp/cpp/IClpSimplexPrimal.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpSimplexPrimal.hpp` & `cylp-0.91.6/cylp/cpp/IClpSimplexPrimal.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpSimplexPrimal_Wolfe.cpp` & `cylp-0.91.6/cylp/cpp/IClpSimplexPrimal_Wolfe.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IClpSimplexPrimal_Wolfe.hpp` & `cylp-0.91.6/cylp/cpp/IClpSimplexPrimal_Wolfe.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinIndexedVector.cpp` & `cylp-0.91.6/cylp/cpp/ICoinIndexedVector.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinMP.cpp` & `cylp-0.91.6/cylp/cpp/ICoinMP.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinMP.hpp` & `cylp-0.91.6/cylp/cpp/ICoinMP.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinModel.hpp` & `cylp-0.91.6/cylp/cpp/ICoinModel.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinMpsIO.cpp` & `cylp-0.91.6/cylp/cpp/ICoinMpsIO.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinMpsIO.hpp` & `cylp-0.91.6/cylp/cpp/ICoinMpsIO.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinPackedMatrix.cpp` & `cylp-0.91.6/cylp/cpp/ICoinPackedMatrix.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/ICoinPackedMatrix.hpp` & `cylp-0.91.6/cylp/cpp/ICoinPackedMatrix.hpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cpp/IOsiCuts.cpp` & `cylp-0.91.6/cylp/cpp/IOsiCuts.cpp`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCbcModel.pxd` & `cylp-0.91.6/cylp/cy/CyCbcModel.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCbcModel.pyx` & `cylp-0.91.6/cylp/cy/CyCbcModel.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCbcNode.pyx` & `cylp-0.91.6/cylp/cy/CyCbcNode.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCgl.pxd` & `cylp-0.91.6/cylp/cy/CyCgl.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCgl.pyx` & `cylp-0.91.6/cylp/cy/CyCgl.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCglCutGeneratorBase.pxd` & `cylp-0.91.6/cylp/cy/CyCglCutGeneratorBase.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCglCutGeneratorBase.pyx` & `cylp-0.91.6/cylp/cy/CyCglCutGeneratorBase.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyClpDualRowPivotBase.pxd` & `cylp-0.91.6/cylp/cy/CyClpDualRowPivotBase.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyClpDualRowPivotBase.pyx` & `cylp-0.91.6/cylp/cy/CyClpDualRowPivotBase.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyClpPrimalColumnPivotBase.pxd` & `cylp-0.91.6/cylp/cy/CyClpPrimalColumnPivotBase.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyClpPrimalColumnPivotBase.pyx` & `cylp-0.91.6/cylp/cy/CyClpPrimalColumnPivotBase.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyClpSimplex.pxd` & `cylp-0.91.6/cylp/cy/CyClpSimplex.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyClpSimplex.pyx` & `cylp-0.91.6/cylp/cy/CyClpSimplex.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinIndexedVector.pxd` & `cylp-0.91.6/cylp/cy/CyCoinIndexedVector.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinIndexedVector.pyx` & `cylp-0.91.6/cylp/cy/CyCoinIndexedVector.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinModel.pxd` & `cylp-0.91.6/cylp/cy/CyCoinModel.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinModel.pyx` & `cylp-0.91.6/cylp/cy/CyCoinModel.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinMpsIO.pxd` & `cylp-0.91.6/cylp/cy/CyCoinMpsIO.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinMpsIO.pyx` & `cylp-0.91.6/cylp/cy/CyCoinMpsIO.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinPackedMatrix.pxd` & `cylp-0.91.6/cylp/cy/CyCoinPackedMatrix.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCoinPackedMatrix.pyx` & `cylp-0.91.6/cylp/cy/CyCoinPackedMatrix.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCutGeneratorPythonBase.pxd` & `cylp-0.91.6/cylp/cy/CyCutGeneratorPythonBase.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyCutGeneratorPythonBase.pyx` & `cylp-0.91.6/cylp/cy/CyCutGeneratorPythonBase.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyDantzigPivot.pxd` & `cylp-0.91.6/cylp/cy/CyDantzigPivot.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyDantzigPivot.pyx` & `cylp-0.91.6/cylp/cy/CyDantzigPivot.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyDualPivotPythonBase.pxd` & `cylp-0.91.6/cylp/cy/CyDualPivotPythonBase.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyDualPivotPythonBase.pyx` & `cylp-0.91.6/cylp/cy/CyDualPivotPythonBase.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyOsiCuts.pxd` & `cylp-0.91.6/cylp/cy/CyOsiCuts.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyOsiCuts.pyx` & `cylp-0.91.6/cylp/cy/CyOsiCuts.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyOsiSolverInterface.pxd` & `cylp-0.91.6/cylp/cy/CyOsiSolverInterface.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyOsiSolverInterface.pyx` & `cylp-0.91.6/cylp/cy/CyOsiSolverInterface.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyPEPivot.pxd` & `cylp-0.91.6/cylp/cy/CyPEPivot.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyPEPivot.pyx` & `cylp-0.91.6/cylp/cy/CyPEPivot.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyPivotPythonBase.pxd` & `cylp-0.91.6/cylp/cy/CyPivotPythonBase.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyPivotPythonBase.pyx` & `cylp-0.91.6/cylp/cy/CyPivotPythonBase.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyTest.pyx` & `cylp-0.91.6/cylp/cy/CyTest.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyWolfePivot.pxd` & `cylp-0.91.6/cylp/cy/CyWolfePivot.pxd`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/CyWolfePivot.pyx` & `cylp-0.91.6/cylp/cy/CyWolfePivot.pyx`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/__init__.py` & `cylp-0.91.6/cylp/cy/__init__.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/cy/createCythonInterface.py` & `cylp-0.91.6/cylp/cy/createCythonInterface.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/PySolve.py` & `cylp-0.91.6/cylp/py/PySolve.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/QP/GQP.py` & `cylp-0.91.6/cylp/py/QP/GQP.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/QP/QP.py` & `cylp-0.91.6/cylp/py/QP/QP.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/QP/QPGen.py` & `cylp-0.91.6/cylp/py/QP/QPGen.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/QP/QPSReader.py` & `cylp-0.91.6/cylp/py/QP/QPSReader.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/mip/GomoryCutGenerator.py` & `cylp-0.91.6/cylp/py/mip/GomoryCutGenerator.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/mip/NodeCompareBase.py` & `cylp-0.91.6/cylp/py/mip/NodeCompareBase.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/mip/SimpleNodeCompare.py` & `cylp-0.91.6/cylp/py/mip/SimpleNodeCompare.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/modeling/CyLPModel.py` & `cylp-0.91.6/cylp/py/modeling/CyLPModel.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/modeling/test_modeling.py` & `cylp-0.91.6/cylp/py/modeling/test_modeling.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/DantzigPivot.py` & `cylp-0.91.6/cylp/py/pivots/DantzigPivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/DualDantzigPivot.py` & `cylp-0.91.6/cylp/py/pivots/DualDantzigPivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/LIFOPivot.py` & `cylp-0.91.6/cylp/py/pivots/LIFOPivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/MostFrequentPivot.py` & `cylp-0.91.6/cylp/py/pivots/MostFrequentPivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/PivotPythonBase.py` & `cylp-0.91.6/cylp/py/pivots/PivotPythonBase.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/PositiveEdgePivot.py` & `cylp-0.91.6/cylp/py/pivots/PositiveEdgePivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/PositiveEdgeWolfePivot.py` & `cylp-0.91.6/cylp/py/pivots/PositiveEdgeWolfePivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/WolfePivot.py` & `cylp-0.91.6/cylp/py/pivots/WolfePivot.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/pivots/WolfePivotPE.py` & `cylp-0.91.6/cylp/py/pivots/WolfePivotPE.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/test_PySolve.py` & `cylp-0.91.6/cylp/py/test_PySolve.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/utils/readSetcovering.py` & `cylp-0.91.6/cylp/py/utils/readSetcovering.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/utils/sparseUtil.py` & `cylp-0.91.6/cylp/py/utils/sparseUtil.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp/py/utils/util.py` & `cylp-0.91.6/cylp/py/utils/util.py`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/cylp.egg-info/PKG-INFO` & `cylp-0.91.6/cylp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cylp
-Version: 0.91.5
+Version: 0.91.6
 Summary: A Python interface for CLP, CBC, and CGL
 Home-page: https://github.com/coin-or/cylp
 Author: Mehdi Towhidi (mehdi.towhidi@gerad.ca), Dominique Orban (dominique.orban@gerad.ca)
 Author-email: mehdi.towhidi@gerad.ca
 Maintainer: Ted Ralphs
 Maintainer-email: ted@lehigh.edu
 License: Eclipse Public License
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 CyLP
 ====
 
@@ -43,27 +42,51 @@
 ------------------------------------------
 
 On Windows, a binary wheel is available and it is not necessary to install Cbc.
 Just do::
 
     $ python -m pip install cylp
 
+On Linux/macOS: Installation as a binary wheel
+---------------------------------------------------------
+
+Binary wheels are available for Linux and some versions of OS X 
+for some versions of Python. To see if there is a wheel available
+for your platform, you can browse 
+
+https://pypi.org/project/cylp/#files
+
+or just try::
+
+    $ python -m pip install cylp
+
+In case this fails, it is most likely that there is no wheel for your platform.
+If you are on Linux, this can probably be addressed by switching to 
+a supported Python version with, e.g., conda::
+
+    $ conda create -n cylp python=3.9
+    $ conda activate cylp
+    
+If all else fails, it is easy to install from source, but Cbc must be 
+installed first, as detailed below. The easiest route for this is to use
+conda.
+
 On Linux/macOS with conda: Installation from source
 ---------------------------------------------------
 
 CyLP depends on `NumPy <https://numpy.org>`_ and `Cython <https://cython.org/>`_
 as prerequisites for building from source (`build-system requires`).
 You will also need to install binaries for Cbc. The version should be 2.10 (recommended) or earlier 
 (current master branch of Cbc will not work with this version of CyLP).
 
 The following commands will create and activate a new conda environment with all
 these prerequisites installed::
 
-    $ conda create -n cbc coin-or-cbc cython numpy pkg-config scipy -c conda-forge
-    $ conda activate cbc
+    $ conda create -n cylp coin-or-cbc cython numpy pkg-config scipy -c conda-forge
+    $ conda activate cylp
 
 Now you can install CyLP from PyPI::
 
     $ pip install --no-build-isolation cylp
 
 (The option `--no-build-isolation` ensures that `cylp` uses the Python packages
 installed by conda in the build phase.)
@@ -76,17 +99,19 @@
 -------------------------------------------------
 
 First of all, you will need to install binaries for Cbc. The version should be 2.10 (recommended) or earlier 
 (current master branch of Cbc will not work with this version of CyLP).
 You can install Cbc by either by installing with your system's package manager, by downloading pre-built binaries,
 or by building yourself from source using `coinbrew <https://github.com/coin-or/coinbrew>`_.
 
-1. To install Cbc in Linux, the easiest way is to use a package manager. Install `coinor-libcbc-dev` on Ubuntu/Debian 
-   or `coin-or-Cbc-devel` on Fedora.
-    
+1. To install Cbc in Linux, the easiest way is to use a package manager. Install
+   `coinor-libcbc-dev` on Ubuntu/Debian or `coin-or-Cbc-devel` on Fedora, or the
+   `corresponding package on your distribution
+   <https://doc.sagemath.org/html/en/reference/spkg/cbc.html#equivalent-system-packages>`_.
+
 #. On macOS, it is easiest to install Cbc with homebrew:
          
    ``$ brew install cbc pkg-config``
 
 You should no longer need to build Cbc from source on any platform unless for some reason, none of the
 above recipes applies to you. If you do need to build from source, please go to the `Cbc <https://github.com/coin-or/Cbc>`_
 project page and follow the instructions there. After building and installing, make sure to 
@@ -203,9 +228,7 @@
 #. Sherbrooke university hospital (Centre hospitalier universitaire de Sherbrooke): CyLP is used for nurse scheduling.
 #. Maisonneuve-Rosemont hospital (L'hôpital HMR): CyLP is used for  physician scheduling with preferences.
 #. Lehigh University: CyLP is used to teach mixed-integer cuts.
 #. IBM T. J. Watson research center
 #. Saarland University, Germany
 
 
-
-
```

### Comparing `cylp-0.91.5/cylp.egg-info/SOURCES.txt` & `cylp-0.91.6/cylp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cylp-0.91.5/pyproject.toml` & `cylp-0.91.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # Use --no-third-party to avoid linking in GLPK.
 # The resulting binary would not be distributable.
 before-all = """
   apt-get install --yes wget || yum install -y wget || brew install bash coreutils
   wget https://raw.githubusercontent.com/coin-or/coinbrew/master/coinbrew
   sed -i.bak '/invoke_make/s/install/-j1 install/' coinbrew
   chmod +x coinbrew
-  ./coinbrew build Cbc@2.10.7 --no-third-party --parallel-jobs 16 --prefix=$(pwd)/local --verbosity 4 || echo ignoring errors
+  ./coinbrew build Cbc@2.10.10 --no-third-party --parallel-jobs 16 --prefix=$(pwd)/local --verbosity 4 || echo ignoring errors
 """
 environment = { PATH="$(pwd)/local/bin:$PATH", LD_LIBRARY_PATH="$(pwd)/local/lib:$LD_LIBRARY_PATH", PKG_CONFIG_PATH="$(pwd)/local/lib/pkgconfig:$PKG_CONFIG_PATH" }
 skip = ["pp*-macosx*", "*-musllinux*"]
```

### Comparing `cylp-0.91.5/setup.py` & `cylp-0.91.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,26 +47,29 @@
         # Do not need CoinDir
         pass
     else:
         CoinDir = os.environ['COIN_INSTALL_DIR']
 except:
     # If user didn't supply location, then try pkg-config
     try:
-        flags = (check_output(['pkg-config', '--libs', 'cbc'])
-                 .strip().decode('utf-8'))
-        libs = [flag[2:] for flag in flags.split()
-                if flag.startswith('-l')]
-        libDirs = [flag[2:] for flag in flags.split()
-                   if flag.startswith('-L')]
-        flags = (check_output(['pkg-config', '--cflags', 'cbc'])
-                 .strip().decode('utf-8'))
-        incDirs = [flag[2:] for flag in flags.split() if
-                   flag.startswith('-I')]
+        for p in ['cbc','cgl','osi-clp','clp','osi','coinutils']:
+            flags = (check_output(['pkg-config', '--libs', p])
+                     .strip().decode('utf-8'))
+            for flag in flags.split():
+                if flag.startswith('-l') and flag[2:] not in libs:
+                    libs.append(flag[2:]) 
+                if flag.startswith('-L') and flag[2:] not in libDirs:
+                    libDirs.append(flag[2:]) 
+            flags = (check_output(['pkg-config', '--cflags', p])
+                     .strip().decode('utf-8'))
+            for flag in flags.split():
+                if flag.startswith('-I') and flag[2:] not in incDirs:
+                    incDirs.append(flag[2:]) 
     except:
-        # If pkg-config fails, then look for an installed Cbc 
+        # If pkg-config fails, then look for an installed Cbc
         try:
             location = dirname(
                 check_output(['which', 'cbc']).strip()).decode('utf-8')
             CoinDir = abspath(join(location, ".."))
         except:
             #Otherwise, raise an exception
             raise Exception('''
```

