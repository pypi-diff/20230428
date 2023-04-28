# Comparing `tmp/RiskLib-0.7.0.tar.gz` & `tmp/RiskLib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLib-0.7.0.tar", last modified: Thu Apr 27 23:46:49 2023, max compression
+gzip compressed data, was "RiskLib-0.7.1.tar", last modified: Fri Apr 28 02:10:24 2023, max compression
```

## Comparing `RiskLib-0.7.0.tar` & `RiskLib-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 23:46:49.031931 RiskLib-0.7.0/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 23:46:49.031736 RiskLib-0.7.0/PKG-INFO
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 23:46:49.030643 RiskLib-0.7.0/RiskLib/
--rw-r--r--   0 ma_qh      (501) staff       (20)    16468 2023-04-27 21:30:12.000000 RiskLib-0.7.0/RiskLib/Option.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.7.0/RiskLib/VaR.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 23:44:53.000000 RiskLib-0.7.0/RiskLib/__init__.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.7.0/RiskLib/calculation.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.7.0/RiskLib/cov_matrix.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.7.0/RiskLib/linear_regression.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1011 2023-04-27 21:14:16.000000 RiskLib-0.7.0/RiskLib/optimal_portfolio.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     5605 2023-04-27 23:44:11.000000 RiskLib-0.7.0/RiskLib/risk_attribution.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     2641 2023-04-27 23:44:36.000000 RiskLib-0.7.0/RiskLib/risk_parity.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     5280 2023-04-27 21:52:24.000000 RiskLib-0.7.0/RiskLib/simulation.py
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 23:46:49.031481 RiskLib-0.7.0/RiskLib.egg-info/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/PKG-INFO
--rw-r--r--   0 ma_qh      (501) staff       (20)      391 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/SOURCES.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/dependency_links.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/requires.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/top_level.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 23:46:49.031997 RiskLib-0.7.0/setup.cfg
--rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 23:46:17.000000 RiskLib-0.7.0/setup.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-28 02:10:24.288345 RiskLib-0.7.1/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-28 02:10:24.288153 RiskLib-0.7.1/PKG-INFO
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-28 02:10:24.286801 RiskLib-0.7.1/RiskLib/
+-rw-r--r--   0 ma_qh      (501) staff       (20)    16468 2023-04-27 21:30:12.000000 RiskLib-0.7.1/RiskLib/Option.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.7.1/RiskLib/VaR.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 23:44:53.000000 RiskLib-0.7.1/RiskLib/__init__.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.7.1/RiskLib/calculation.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.7.1/RiskLib/cov_matrix.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.7.1/RiskLib/linear_regression.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1648 2023-04-28 01:56:24.000000 RiskLib-0.7.1/RiskLib/optimal_portfolio.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5605 2023-04-27 23:44:11.000000 RiskLib-0.7.1/RiskLib/risk_attribution.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     2641 2023-04-27 23:44:36.000000 RiskLib-0.7.1/RiskLib/risk_parity.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5280 2023-04-27 21:52:24.000000 RiskLib-0.7.1/RiskLib/simulation.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-28 02:10:24.287919 RiskLib-0.7.1/RiskLib.egg-info/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-28 02:10:24.000000 RiskLib-0.7.1/RiskLib.egg-info/PKG-INFO
+-rw-r--r--   0 ma_qh      (501) staff       (20)      391 2023-04-28 02:10:24.000000 RiskLib-0.7.1/RiskLib.egg-info/SOURCES.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-28 02:10:24.000000 RiskLib-0.7.1/RiskLib.egg-info/dependency_links.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-28 02:10:24.000000 RiskLib-0.7.1/RiskLib.egg-info/requires.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-28 02:10:24.000000 RiskLib-0.7.1/RiskLib.egg-info/top_level.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-28 02:10:24.288406 RiskLib-0.7.1/setup.cfg
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-28 02:10:10.000000 RiskLib-0.7.1/setup.py
```

### Comparing `RiskLib-0.7.0/RiskLib/Option.py` & `RiskLib-0.7.1/RiskLib/Option.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.7.0/RiskLib/calculation.py` & `RiskLib-0.7.1/RiskLib/calculation.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.7.0/RiskLib/cov_matrix.py` & `RiskLib-0.7.1/RiskLib/cov_matrix.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.7.0/RiskLib/linear_regression.py` & `RiskLib-0.7.1/RiskLib/linear_regression.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.7.0/RiskLib/risk_attribution.py` & `RiskLib-0.7.1/RiskLib/risk_attribution.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.7.0/RiskLib/risk_parity.py` & `RiskLib-0.7.1/RiskLib/risk_parity.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.7.0/RiskLib/simulation.py` & `RiskLib-0.7.1/RiskLib/simulation.py`

 * *Files identical despite different names*

