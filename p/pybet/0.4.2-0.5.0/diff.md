# Comparing `tmp/pybet-0.4.2.tar.gz` & `tmp/pybet-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybet-0.4.2.tar", max compression
+gzip compressed data, was "pybet-0.5.0.tar", max compression
```

## Comparing `pybet-0.4.2.tar` & `pybet-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.4.2/LICENSE
--rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.4.2/pybet/__init__.py
--rw-r--r--   0        0        0     6745 2023-02-18 00:28:56.232325 pybet-0.4.2/pybet/market.py
--rw-r--r--   0        0        0    11292 2023-02-18 00:28:56.233330 pybet-0.4.2/pybet/odds.py
--rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.4.2/pybet/staking/__init__.py
--rw-r--r--   0        0        0     1141 2023-02-24 18:11:33.731147 pybet-0.4.2/pybet/staking/kelly.py
--rw-r--r--   0        0        0      936 2023-02-24 18:11:39.929657 pybet-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.4.2/README.md
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pybet-0.4.2/setup.py
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.5.0/LICENSE
+-rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.5.0/pybet/__init__.py
+-rw-r--r--   0        0        0     6745 2023-02-18 00:28:56.232325 pybet-0.5.0/pybet/market.py
+-rw-r--r--   0        0        0    11292 2023-02-18 00:28:56.233330 pybet-0.5.0/pybet/odds.py
+-rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.5.0/pybet/staking/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-27 22:41:50.387749 pybet-0.5.0/pybet/staking/kelly.py
+-rw-r--r--   0        0        0      936 2023-04-27 22:47:41.639108 pybet-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.5.0/README.md
+-rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.5.0/PKG-INFO
```

### Comparing `pybet-0.4.2/LICENSE` & `pybet-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybet-0.4.2/pybet/market.py` & `pybet-0.5.0/pybet/market.py`

 * *Files identical despite different names*

### Comparing `pybet-0.4.2/pybet/odds.py` & `pybet-0.5.0/pybet/odds.py`

 * *Files identical despite different names*

### Comparing `pybet-0.4.2/pybet/staking/kelly.py` & `pybet-0.5.0/pybet/staking/kelly.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from decimal import Decimal
 from ..odds import Odds
 
 
-def kelly(true_odds: Odds, market_odds: Odds, bank: Decimal) -> Decimal:
+def kelly(
+    true_odds: Odds,
+    market_odds: Odds,
+    bank: Decimal,
+    percentage_commission: Decimal = Decimal("0"),
+) -> Decimal:
     """Calculates the stake that should be placed according to the Kelly Criterion
     [https://en.wikipedia.org/wiki/Kelly_criterion], i.e. edge over odds
     for any given true odds at any given market odds for any given bank size
 
     :param true_odds: The calculated true odds of the selection
     :type true_odds: Odds
     :param market_odds: The odds currently available in the market
     :type market_odds: Odds
     :param bank: The bank available
     :type bank: Decimal
+    :param percentage_commission: The percentage commission applied to winnings
+    :type percentage_commission: Decimal
     :return: The stake to place according to the Kelly criterion
     :rtype: Decimal
 
 
     :Example:
         >>> kelly(Odds(4), Odds(5), 100)
         Decimal('6.25')
         >>> kelly(Odds(5), Odds(4), 100)
         Decimal('0.00')
     """
+    if not 0 <= percentage_commission <= 100:
+        raise ValueError("Commission must be between 0 and 100")
 
     p: Decimal = true_odds.to_probability()
     q: Decimal = 1 - p
-    odds: Decimal = market_odds.to_one()
+    odds: Decimal = market_odds.to_one() * Decimal(str(1 - percentage_commission / 100))
 
     edge: Decimal = (odds * p) - q
     kelly: Decimal = edge / odds
 
     stake: Decimal = round(bank * max(kelly, Decimal("0")), 2)
 
     return stake
```

### Comparing `pybet-0.4.2/pyproject.toml` & `pybet-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybet"
-version = "0.4.2"
+version = "0.5.0"
 description = "A library of betting utilities to assist with calculation of bets, stakes and markets"
 license = "GPL-3.0-only"
 authors = ["Robert Peacock <robertjamespeacock@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/peaky76/pybet"
 documentation = "https://pybet.readthedocs.io/"
 keywords = ["betting", "gambling"]
@@ -14,16 +14,16 @@
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
 auto-changelog = "^0.6.0"
+black = "^23.1.0"
 coverage = "^7.1.0"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
```

### Comparing `pybet-0.4.2/README.md` & `pybet-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pybet-0.4.2/PKG-INFO` & `pybet-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybet
-Version: 0.4.2
+Version: 0.5.0
 Summary: A library of betting utilities to assist with calculation of bets, stakes and markets
 Home-page: https://github.com/peaky76/pybet
 License: GPL-3.0-only
 Keywords: betting,gambling
 Author: Robert Peacock
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

