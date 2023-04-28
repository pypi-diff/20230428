# Comparing `tmp/py3gpp-0.1.6.tar.gz` & `tmp/py3gpp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3gpp-0.1.6.tar", last modified: Wed Apr 26 07:31:26 2023, max compression
+gzip compressed data, was "py3gpp-0.1.7.tar", last modified: Fri Apr 28 07:09:56 2023, max compression
```

## Comparing `py3gpp-0.1.6.tar` & `py3gpp-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.019804 py3gpp-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-26 07:31:09.000000 py3gpp-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 07:31:26.019804 py3gpp-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 07:31:09.000000 py3gpp-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.015803 py3gpp-0.1.6/py3gpp/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.015803 py3gpp-0.1.6/py3gpp/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/CommonConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/DMRSConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/PDSCHConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/PDSCHPTRSConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrCarrierConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrNumerologyConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrPDSCHConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrPDSCHDMRSConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrPDSCHPTRSConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrChannelEstimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrEqualizeMMSE.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrExtractResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrOFDMDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrOFDMInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrOFDMModulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCH.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHPRBS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHPTRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHPTRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPRBS.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPSS.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPolarDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrRateRecoverPolar.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrResourceGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSSS.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSetResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSymbolDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSymbolModulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrTimingEstimate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.015803 py3gpp-0.1.6/py3gpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 07:31:09.000000 py3gpp-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:31:26.019804 py3gpp-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 07:31:09.000000 py3gpp-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.019804 py3gpp-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrPDSCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrPDSCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrPDSCHPTRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrRateRecoverPolar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.764460 py3gpp-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-28 07:09:38.000000 py3gpp-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-28 07:09:56.764460 py3gpp-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-28 07:09:38.000000 py3gpp-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.760460 py3gpp-0.1.7/py3gpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.760460 py3gpp-0.1.7/py3gpp/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/CommonConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/DMRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/PDSCHConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/PDSCHPTRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrCarrierConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrNumerologyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrPDSCHConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrPDSCHDMRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrPDSCHPTRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrChannelEstimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrEqualizeMMSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrExtractResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrOFDMDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrOFDMInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrOFDMModulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPolarDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrRateRecoverPolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrResourceGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSetResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSymbolDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSymbolModulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrTimingEstimate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.760460 py3gpp-0.1.7/py3gpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 07:09:38.000000 py3gpp-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:09:56.764460 py3gpp-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 07:09:38.000000 py3gpp-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.764460 py3gpp-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrRateRecoverPolar.py
```

### Comparing `py3gpp-0.1.6/LICENSE` & `py3gpp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/PKG-INFO` & `py3gpp-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.1.6
+Version: 0.1.7
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.1.6/README.md` & `py3gpp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/__init__.py` & `py3gpp-0.1.7/py3gpp/__init__.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/CommonConfig.py` & `py3gpp-0.1.7/py3gpp/configs/CommonConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/DMRSConfigBase.py` & `py3gpp-0.1.7/py3gpp/configs/DMRSConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/PDSCHConfigBase.py` & `py3gpp-0.1.7/py3gpp/configs/PDSCHConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/PDSCHPTRSConfigBase.py` & `py3gpp-0.1.7/py3gpp/configs/PDSCHPTRSConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/nrCarrierConfig.py` & `py3gpp-0.1.7/py3gpp/configs/nrCarrierConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .nrNumerologyConfig import nrNumerologyConfig
 
 class nrCarrierConfig(nrNumerologyConfig):
-        def __init__(self):
-            self._NCellID = 1
-            self._NSizeGrid = 52
-            self._NStartGrid = 0
-            self._NSlot = 0
-            self._NFrame = 0
+        def __init__(self, NCellID = 1, NSizeGrid = 52, NStartGrid = 0, NSlot = 0, NFrame = 0, SubcarrierSpacing = 15):
+            self._NCellID = NCellID
+            self._NSizeGrid = NSizeGrid
+            self._NStartGrid = NStartGrid
+            self._NSlot = NSlot
+            self._NFrame = NFrame
+            self.SubcarrierSpacing = SubcarrierSpacing
 
         @property
         def SymbolsPerSlot(self):
             if self.CyclicPrefix == "normal":
                 return 14
             else:
                 return 12
```

### Comparing `py3gpp-0.1.6/py3gpp/configs/nrNumerologyConfig.py` & `py3gpp-0.1.7/py3gpp/configs/nrNumerologyConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/nrPDSCHConfig.py` & `py3gpp-0.1.7/py3gpp/configs/nrPDSCHConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/configs/nrPDSCHDMRSConfig.py` & `py3gpp-0.1.7/py3gpp/configs/nrPDSCHDMRSConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/helper.py` & `py3gpp-0.1.7/py3gpp/helper.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrBCHDecode.py` & `py3gpp-0.1.7/py3gpp/nrBCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrCRCEncode.py` & `py3gpp-0.1.7/py3gpp/nrCRCEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrChannelEstimate.py` & `py3gpp-0.1.7/py3gpp/nrChannelEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrOFDMDemodulate.py` & `py3gpp-0.1.7/py3gpp/nrOFDMDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrOFDMModulate.py` & `py3gpp-0.1.7/py3gpp/nrOFDMModulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from py3gpp.configs import nrCarrierConfig
+from py3gpp.configs.nrCarrierConfig import nrCarrierConfig
 from py3gpp.nrOFDMInfo import nrOFDMInfo
 
 # TODO: implement windowing
 def nrOFDMModulate(
     carrier=None, grid=None, scs=None, initialNSlot=0, CyclicPrefix="normal", Nfft=None, SampleRate=None, Windowing=None
 ):
     info = {}
```

### Comparing `py3gpp-0.1.6/py3gpp/nrPBCH.py` & `py3gpp-0.1.7/py3gpp/nrPBCH.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrPBCHDMRSIndices.py` & `py3gpp-0.1.7/py3gpp/nrPBCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrPDSCHDMRS.py` & `py3gpp-0.1.7/py3gpp/nrPDSCHDMRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrPDSCHDMRSIndices.py` & `py3gpp-0.1.7/py3gpp/nrPDSCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrPDSCHPTRS.py` & `py3gpp-0.1.7/py3gpp/nrPDSCHPTRS.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,72 +5,85 @@
 
 from py3gpp.nrPRBS import nrPRBS
 from py3gpp.nrSymbolModulate import nrSymbolModulate
 from py3gpp.configs.nrPDSCHConfig import nrPDSCHConfig
 from py3gpp.configs.nrCarrierConfig import nrCarrierConfig
 from py3gpp.nrPDSCHDMRS import PDSCHDMRSSyms
 
-def nrPDSCHPTRS(cfg: nrPDSCHConfig, carrier: nrCarrierConfig):
-    raise NotImplementedError("no ready yet")
+def nrPDSCHPTRS(carrier: nrCarrierConfig, cfg: nrPDSCHConfig):
     if cfg.EnablePTRS == 0:
         return []
 
+    bwp_size = cfg.NRBSize * cfg.NSizeBWP
+
+    # Generates first DMRS symbol (l0)
+    n_scid = 0
+    dmrs_occupied_syms = PDSCHDMRSSyms(cfg)
+    cinit_dmrs = PDSCHPTRScinit(carrier.SymbolsPerSlot, carrier.NSlot, dmrs_occupied_syms[0], cfg.DMRS.NIDNSCID, n_scid)
+    dmrs_prbs = nrPRBS(cinit_dmrs, bwp_size)
+    dmrs_sym = nrSymbolModulate(dmrs_prbs, "QPSK")
+
+    # Form PTRS symbols from DMRS l0 sequency
+    ptrs_prb_set = PTRSPRBSet(cfg)
+
+    ptrs_sym = np.array([dmrs_sym[x] for x in ptrs_prb_set])
+
+    ptrs_occupied_syms = PDSCHPTRSSyms(carrier, cfg)
+
+    return np.tile(ptrs_sym, len(ptrs_occupied_syms))
+
+
+def PTRSPRBSet(cfg: nrPDSCHConfig):
+    # Align with frequency offset based on DMRS type
+    if cfg.DMRS.DMRSConfigurationType == 1:
+        dmrs_ref_table = np.array([0, 2, 6, 8])
+    else:
+        dmrs_ref_table = np.array([0, 2, 4, 6])
+    kRE_idx = int(cfg.PTRS.REOffset, 2)
+    dmrsRef = dmrs_ref_table[kRE_idx]
+
+    Nrb_mod_Kptrs = len(cfg.PRBSet) % cfg.PTRS.FrequencyDensity
+    if Nrb_mod_Kptrs == 0:
+        kRBref = cfg.RNTI % cfg.PTRS.FrequencyDensity
+    else:
+        kRBref = cfg.RNTI % Nrb_mod_Kptrs
+
     if cfg.DMRS.DMRSConfigurationType == 1:
         n_dmrs_per_re = 6
     else:
         n_dmrs_per_re = 4
-    n_dmrs_bits_re = 2*n_dmrs_per_re
 
-    dmrs_begin = n_dmrs_bits_re * min(cfg.PRBSet)
-    dmrs_end = n_dmrs_bits_re * (max(cfg.PRBSet)+1)
-    dmrs_size = n_dmrs_bits_re * cfg.NSizeBWP
+    prb_set = np.array(cfg.PRBSet[kRBref::cfg.PTRS.FrequencyDensity])
+    prb_set = (prb_set*n_dmrs_per_re)+dmrsRef//2
 
-    n_scid = 0
-
-    occupied_syms = PDSCHDMRSSyms(cfg)
-
-    # Start generation for every symbol
-    n_symb = occupied_syms[0]
-    cinit_dmrs = PDSCHPTRScinit(carrier.SymbolsPerSlot, carrier.NSlot, n_symb, cfg.DMRS.NIDNSCID, n_scid)
-    dmrs_prbs = nrPRBS(cinit_dmrs, dmrs_size)
-
-    # Cut DMRS PRBS sequency
-    dmrs_prbs = dmrs_prbs[dmrs_begin:dmrs_end]
-    dmrs_syms = nrSymbolModulate(dmrs_prbs, "QPSK")
-
-    # Form PTRS symbols from DMRS l0 sequency
-    # TODO
+    return prb_set
 
-    return []
 
 # LUT for PTRS occupied symbols positions
 def PDSCHPTRSSyms(carrier: nrCarrierConfig, cfg: nrPDSCHConfig):
     # First get DMRS symbols
     dmrs_syms = PDSCHDMRSSyms(cfg)
     # Then calculate positions of PTRS
     A_pos = cfg.DMRS.DMRSTypeAPosition
     td = cfg.PTRS.TimeDensity
 
     ptrs_cnt = td-1
     occupied_syms = np.array([], dtype=int)
     for i in range(cfg.SymbolAllocation[0], carrier.SymbolsPerSlot):
         if i == A_pos:
-            # print(i, 'flag A position')
             ptrs_cnt = 0
             continue
 
         if i in dmrs_syms:
-            # print(i, 'flag DMRS')
             ptrs_cnt = 0
             continue
 
         ptrs_cnt += 1
 
         if ptrs_cnt == td:
-            # print(i, ptrs_cnt, 'mark')
             occupied_syms = np.append(occupied_syms, i)
             ptrs_cnt = 0
 
     return occupied_syms
 
 def PDSCHPTRScinit(sps, n_slot, n_symb, NIDSCID, n_scid):
-    return 2**17 * (sps * n_slot + n_symb + 1) * (2*NIDSCID + 1) + 2*NIDSCID + n_scid
+    return 2**17 * (sps * n_slot + n_symb + 1) * (2*NIDSCID + 1) + 2*NIDSCID + n_scid
```

### Comparing `py3gpp-0.1.6/py3gpp/nrPDSCHPTRSIndices.py` & `py3gpp-0.1.7/py3gpp/nrPDSCHPTRSIndices.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,27 +24,24 @@
 
     Nrb_mod_Kptrs = len(cfg.PRBSet) % cfg.PTRS.FrequencyDensity
     if Nrb_mod_Kptrs == 0:
         kRBref = cfg.RNTI % cfg.PTRS.FrequencyDensity
     else:
         kRBref = cfg.RNTI % Nrb_mod_Kptrs
     kRBref *= cfg.NRBSize
-    # print(kRBref, kREref)
 
     # Move to BWP offset and the rest frequency offsets
     ptrs_begin = frame_begin + kREref + kRBref
 
     # Calculate PTRS positions in every occupied symbol. Frequency position,
     # for every 2 or 4 RBs
     occupied_res = np.array(list(range(ptrs_begin, frame_end, (cfg.PTRS.FrequencyDensity*12))))
-    # print(occupied_res)
 
     # Calculates occupied symbols numbers. Time positions
     occupied_syms = PDSCHPTRSSyms(carrier, cfg)
-    # print(occupied_syms)
 
-    ptrs_indices = np.array([])
-    for idx, sym in enumerate(occupied_syms):
-        sym_offset = sym*frame_size
-        ptrs_indices = np.append(ptrs_indices, (occupied_res + sym_offset))
+    # Move PTRS indices to occupied symbols
+    ptrs_indices = np.array([occupied_res+(sym*frame_size) for sym in occupied_syms])
+    if len(ptrs_indices) > 0:
+        ptrs_indices = np.concatenate(ptrs_indices, axis=None)
 
     return ptrs_indices
```

### Comparing `py3gpp-0.1.6/py3gpp/nrPolarDecode.py` & `py3gpp-0.1.7/py3gpp/nrPolarDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrRateRecoverPolar.py` & `py3gpp-0.1.7/py3gpp/nrRateRecoverPolar.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrSSS.py` & `py3gpp-0.1.7/py3gpp/nrSSS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrSymbolDemodulate.py` & `py3gpp-0.1.7/py3gpp/nrSymbolDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp/nrSymbolModulate.py` & `py3gpp-0.1.7/py3gpp/nrSymbolModulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
         assert not (len(databits) % 8), "length of databits must be multiple of 8"
         res_arr = np.zeros((len(databits)//8), dtype=(complex))
         chunks = np.array_split(databits, len(databits)//8)
         for idx, sample in enumerate(chunks):
             res_arr[idx] = ( (1-2*sample[0]) * (8-(1-2*sample[2]) * (4-(1-2*sample[4]) * (2-(1-2*sample[6])))) ) + 1j*( (1-2*sample[1]) * (8-(1-2*sample[3]) * (4-(1-2*sample[5]) * (2-(1-2*sample[7])))) )
         res_arr = [x/np.sqrt(170) for x in res_arr]
 
-    return res_arr
+    return np.array(res_arr)
```

### Comparing `py3gpp-0.1.6/py3gpp/nrTimingEstimate.py` & `py3gpp-0.1.7/py3gpp/nrTimingEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/py3gpp.egg-info/PKG-INFO` & `py3gpp-0.1.7/py3gpp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.1.6
+Version: 0.1.7
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.1.6/py3gpp.egg-info/SOURCES.txt` & `py3gpp-0.1.7/py3gpp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,9 +50,10 @@
 py3gpp/configs/nrPDSCHDMRSConfig.py
 py3gpp/configs/nrPDSCHPTRSConfig.py
 tests/test_nrBCHDecode.py
 tests/test_nrCRCDecode.py
 tests/test_nrCRCEncode.py
 tests/test_nrPDSCHDMRS.py
 tests/test_nrPDSCHDMRSIndices.py
+tests/test_nrPDSCHPTRS.py
 tests/test_nrPDSCHPTRSIndices.py
 tests/test_nrRateRecoverPolar.py
```

### Comparing `py3gpp-0.1.6/pyproject.toml` & `py3gpp-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     {name = "Benjamin Menküc", email = "benjamin@menkuec.de"},
 ]
 description = "Functions for 5G NR signal processing"
 name = "py3gpp"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `py3gpp-0.1.6/tests/test_nrBCHDecode.py` & `py3gpp-0.1.7/tests/test_nrBCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/tests/test_nrCRCDecode.py` & `py3gpp-0.1.7/tests/test_nrCRCDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/tests/test_nrPDSCHDMRS.py` & `py3gpp-0.1.7/tests/test_nrPDSCHDMRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/tests/test_nrPDSCHDMRSIndices.py` & `py3gpp-0.1.7/tests/test_nrPDSCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/tests/test_nrPDSCHPTRSIndices.py` & `py3gpp-0.1.7/tests/test_nrPDSCHPTRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.6/tests/test_nrRateRecoverPolar.py` & `py3gpp-0.1.7/tests/test_nrRateRecoverPolar.py`

 * *Files identical despite different names*

