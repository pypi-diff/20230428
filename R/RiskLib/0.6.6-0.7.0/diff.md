# Comparing `tmp/RiskLib-0.6.6.tar.gz` & `tmp/RiskLib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLib-0.6.6.tar", last modified: Thu Apr 27 21:52:58 2023, max compression
+gzip compressed data, was "RiskLib-0.7.0.tar", last modified: Thu Apr 27 23:46:49 2023, max compression
```

## Comparing `RiskLib-0.6.6.tar` & `RiskLib-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:52:58.272259 RiskLib-0.6.6/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 21:52:58.271956 RiskLib-0.6.6/PKG-INFO
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:52:58.267712 RiskLib-0.6.6/RiskLib/
--rw-r--r--   0 ma_qh      (501) staff       (20)    16468 2023-04-27 21:30:12.000000 RiskLib-0.6.6/RiskLib/Option.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.6/RiskLib/VaR.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      204 2023-04-27 21:16:35.000000 RiskLib-0.6.6/RiskLib/__init__.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.6/RiskLib/calculation.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.6/RiskLib/cov_matrix.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.6/RiskLib/linear_regression.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1011 2023-04-27 21:14:16.000000 RiskLib-0.6.6/RiskLib/optimal_portfolio.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     8088 2023-04-27 20:59:27.000000 RiskLib-0.6.6/RiskLib/risk_parity.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     5280 2023-04-27 21:52:24.000000 RiskLib-0.6.6/RiskLib/simulation.py
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:52:58.271291 RiskLib-0.6.6/RiskLib.egg-info/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 21:52:58.000000 RiskLib-0.6.6/RiskLib.egg-info/PKG-INFO
--rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 21:52:58.000000 RiskLib-0.6.6/RiskLib.egg-info/SOURCES.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 21:52:58.000000 RiskLib-0.6.6/RiskLib.egg-info/dependency_links.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 21:52:58.000000 RiskLib-0.6.6/RiskLib.egg-info/requires.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 21:52:58.000000 RiskLib-0.6.6/RiskLib.egg-info/top_level.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 21:52:58.272344 RiskLib-0.6.6/setup.cfg
--rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 21:52:32.000000 RiskLib-0.6.6/setup.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 23:46:49.031931 RiskLib-0.7.0/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 23:46:49.031736 RiskLib-0.7.0/PKG-INFO
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 23:46:49.030643 RiskLib-0.7.0/RiskLib/
+-rw-r--r--   0 ma_qh      (501) staff       (20)    16468 2023-04-27 21:30:12.000000 RiskLib-0.7.0/RiskLib/Option.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.7.0/RiskLib/VaR.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 23:44:53.000000 RiskLib-0.7.0/RiskLib/__init__.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.7.0/RiskLib/calculation.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.7.0/RiskLib/cov_matrix.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.7.0/RiskLib/linear_regression.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1011 2023-04-27 21:14:16.000000 RiskLib-0.7.0/RiskLib/optimal_portfolio.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5605 2023-04-27 23:44:11.000000 RiskLib-0.7.0/RiskLib/risk_attribution.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     2641 2023-04-27 23:44:36.000000 RiskLib-0.7.0/RiskLib/risk_parity.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5280 2023-04-27 21:52:24.000000 RiskLib-0.7.0/RiskLib/simulation.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 23:46:49.031481 RiskLib-0.7.0/RiskLib.egg-info/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/PKG-INFO
+-rw-r--r--   0 ma_qh      (501) staff       (20)      391 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/SOURCES.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/dependency_links.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/requires.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 23:46:48.000000 RiskLib-0.7.0/RiskLib.egg-info/top_level.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 23:46:49.031997 RiskLib-0.7.0/setup.cfg
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 23:46:17.000000 RiskLib-0.7.0/setup.py
```

### Comparing `RiskLib-0.6.6/RiskLib/Option.py` & `RiskLib-0.7.0/RiskLib/Option.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.6/RiskLib/calculation.py` & `RiskLib-0.7.0/RiskLib/calculation.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.6/RiskLib/cov_matrix.py` & `RiskLib-0.7.0/RiskLib/cov_matrix.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.6/RiskLib/linear_regression.py` & `RiskLib-0.7.0/RiskLib/linear_regression.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.6/RiskLib/optimal_portfolio.py` & `RiskLib-0.7.0/RiskLib/optimal_portfolio.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.6/RiskLib/risk_parity.py` & `RiskLib-0.7.0/RiskLib/risk_attribution.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import numpy as np
 import pandas as pd
-from scipy.optimize import minimize
+
+def risk_contrib(w, covar):
+    risk_contrib = w * covar.dot(w) / np.sqrt(w.dot(covar).dot(w))
+    return risk_contrib
 
 def expost_attribution(w, upReturns):
     _stocks = list(upReturns.columns)
     n = upReturns.shape[0]
     pReturn = np.empty(n)
     weights = np.empty((n, len(w)))
     lastW = np.copy(w)
@@ -155,106 +158,8 @@
     assert np.isclose(np.sum(cSD), np.std(pReturn))
 
     # Add the Vol attribution to the output
     Expost_Attribution = pd.concat([Attribution, 
         pd.DataFrame({"Value": "Vol Attribution", **{newFactors[i]:cSD[i] for i in range(len(newFactors))}, "Portfolio":np.std(pReturn)}, index=[0])
     ])
 
-    return Expost_Attribution
-
-def vol_risk_parity(stockMeans, covar, b=None):
-    n = len(stockMeans)
-    
-    # Function for Portfolio Volatility
-    def pvol(w):
-        x = np.array(w)
-        return np.sqrt(x.dot(covar).dot(x))
-    
-    # Function for Component Standard Deviation
-    def pCSD(w, b=None, last = False):
-        x = np.array(w)
-        pVol = pvol(w)
-        csd = x * (covar.dot(x)) / pVol
-        if last:
-            return csd
-        if b is not None:
-            csd /= b
-        return csd
-    
-    # Sum Square Error of cSD
-    def sseCSD(w):
-        csd = pCSD(w, b)
-        mCSD = np.sum(csd) / n
-        dCsd = csd - mCSD
-        se = dCsd * dCsd
-        return 1.0e5 * np.sum(se) # Add a large multiplier for better convergence
-    
-    # Define the optimization problem
-    m = minimize(sseCSD, [1/n]*n, method='SLSQP', bounds=[(0, None)]*n, constraints={'type': 'eq', 'fun': lambda w: np.sum(w)-1})
-    
-    w = m.x
-    
-    # Compute RPWeights
-    RPWeights = pd.DataFrame({
-        'Weight': w,
-        'cEr': stockMeans * w,
-        'CSD': pCSD(w, b, True)
-    })
-    
-    return RPWeights
-
-
-def es_risk_parity(stock, stockMeans, simReturn, b=None):
-    # internal ES function
-    def _ES(*w):
-
-        def ES(a, alpha=0.05):
-            x = np.sort(a)
-            nup = int(np.ceil(a.size * alpha))
-            ndn = int(np.floor(a.size * alpha))
-            v = 0.5 * (x[nup] + x[ndn])
-            
-            es = np.mean(x[x <= v])
-            return -es
-        r = simReturn @ w
-        return ES(r)
-
-    # Function for the component ES
-    def CES(w, b=None, last = False):
-        x = list(w)
-        n = len(x)
-        ces = np.empty(n)
-        es = _ES(*x)
-        e = 1e-6
-        for i in range(n):
-            old = x[i]
-            x[i] = x[i] + e
-            ces[i] = old * (_ES(*x) - es) / e
-            x[i] = old
-        if last:
-            return ces
-        if b is not None:
-            ces /= b
-        return ces 
-
-    # SSE of the Component ES
-    def SSE_CES(*w):
-        ces = CES(*w,b)
-        ces = [x - sum(ces) / len(ces) for x in ces]
-        return 1e3 * (sum([x ** 2 for x in ces]))
-    
-    n = len(stock)
-    w0 = np.full(n, 1/n)
-    bounds = [(0, None)] * n
-    res = minimize(SSE_CES, w0, method='SLSQP', bounds=bounds, constraints=[{'type': 'eq', 'fun': lambda w: sum(w) - 1}])
-    w = res.x
-    
-    # Compute RPWeights
-    ES_RPWeights = pd.DataFrame({
-        'Stock': stock,
-        'Weight': w,
-        'cEr': stockMeans * w,
-        'CES': CES(w, b, True)
-    }).set_index('Stock')
-    
-    return ES_RPWeights
-
+    return Expost_Attribution
```

### Comparing `RiskLib-0.6.6/RiskLib/simulation.py` & `RiskLib-0.7.0/RiskLib/simulation.py`

 * *Files identical despite different names*

