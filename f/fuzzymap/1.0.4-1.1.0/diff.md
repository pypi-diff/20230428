# Comparing `tmp/fuzzymap-1.0.4.tar.gz` & `tmp/fuzzymap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzymap-1.0.4.tar", last modified: Sat Dec  3 11:41:29 2022, max compression
+gzip compressed data, was "fuzzymap-1.1.0.tar", last modified: Fri Apr 28 09:35:37 2023, max compression
```

## Comparing `fuzzymap-1.0.4.tar` & `fuzzymap-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 11:41:29.888637 fuzzymap-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2022-12-03 11:41:17.000000 fuzzymap-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2022-12-03 11:41:29.888637 fuzzymap-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2022-12-03 11:41:17.000000 fuzzymap-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 11:41:29.888637 fuzzymap-1.0.4/fuzzymap/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-03 11:41:17.000000 fuzzymap-1.0.4/fuzzymap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2022-12-03 11:41:17.000000 fuzzymap-1.0.4/fuzzymap/fuzzymap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 11:41:29.888637 fuzzymap-1.0.4/fuzzymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2022-12-03 11:41:29.000000 fuzzymap-1.0.4/fuzzymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-03 11:41:29.000000 fuzzymap-1.0.4/fuzzymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 11:41:29.000000 fuzzymap-1.0.4/fuzzymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-03 11:41:29.000000 fuzzymap-1.0.4/fuzzymap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-03 11:41:29.000000 fuzzymap-1.0.4/fuzzymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 11:41:29.888637 fuzzymap-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-03 11:41:17.000000 fuzzymap-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/fuzzymap/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/fuzzymap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/fuzzymap/fuzzymap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/fuzzymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:35:37.000000 fuzzymap-1.1.0/fuzzymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 09:35:37.259618 fuzzymap-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 09:35:25.000000 fuzzymap-1.1.0/setup.py
```

### Comparing `fuzzymap-1.0.4/LICENSE` & `fuzzymap-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzymap-1.0.4/PKG-INFO` & `fuzzymap-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,62 @@
-Metadata-Version: 2.1
-Name: fuzzymap
-Version: 1.0.4
-Summary: Python dictionary with a FUZZY key-matching opportunity
-Home-page: https://github.com/pysnippet/fuzzymap
-Author: Artyom Vancyan
-Author-email: artyom@pysnippet.org
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FuzzyMap <img src="https://github.com/pysnippet.png" align="right" height="64" />
+# Fuzzy Map <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/fuzzymap.svg)](https://pypi.org/project/fuzzymap/)
-[![License](https://img.shields.io/pypi/l/fuzzymap.svg)](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
-
-## What is FuzzyMap?
-
-`FuzzyMap` is a polymorph Python dictionary. This kind of dictionary returns the value of the exact key if there is such
-a key. Otherwise, it will return the value of the most similar key satisfying the given ratio. The same mechanism works
-when setting a new or replacing an old key in the dictionary. If the key is not found and does not match any of the keys
-by the given ratio, it returns `None`.
-
-## How does it work?
-
-Suppose you have scraped data from multiple sources that do not have a unique identifier, and you want to compare the
-values of the items having the same identifiers. Sure there will be found a field that mostly has an equivalent value
-at each source. And you can use that field to identify the corresponding items of other sources' data.
-
-## Let's look at the following example
-
-There is a live data parser that collects the coefficients of football matches from different bookmakers at once, then
-calculates and logs the existing forks. Many bookmakers change the name of the teams to be incomparable with names on
-other sites.
+[![License](https://img.shields.io/pypi/l/fuzzymap.svg?color=blue)](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpysnippet%2Ffuzzymap?ref=badge_shield)
+[![Tests](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/fuzzymap/actions/workflows/tests.yml)
+
+## What is the Fuzzy Map?
+
+The Fuzzy Map is a polymorph Python dictionary that always returns the value of the closest similar key. This kind of
+dictionary returns the value of the exact key if there is such a key. Otherwise, it will return the value of the most
+similar key satisfying the given ratio. The exact mechanism works when setting a new or replacing an old key in the
+dictionary. If the key is not found and does not match any of the keys by the given ratio, it returns none.
+
+## Usage with a real-world example
+
+A live data parser collects the coefficients of sports games from different bookmakers at once, and then an analyzer
+tries to find the existing forks. Different bookmakers use different names for the same games. Some of them use the full
+names, and others use names with a partial abbreviation that makes the analyzer's job harder to find and compare the
+coefficients of the same game. Rather this could be hard without `FuzzyMap` that can find the game using the name used
+in one of the sources.
 
 ```python
 from fuzzymap import FuzzyMap
 
-src1 = {
+source_1 = {
     'Rapid Wien - First Vienna': {'w1': 1.93, 'x': 2.32, 'w2': 7.44},
     'Al Bourj - Al Nejmeh': {'w1': 26, 'x': 11.5, 'w2': 1.05},
-    # hundreds of other teams' data
+    # hundreds of other games' data
 }
 
-src2 = FuzzyMap({
+source_2 = FuzzyMap({
     'Bourj FC - Nejmeh SC Beirut': {'w1': 32, 'x': 12, 'w2': 1.05},
     'SK Rapid Wien - First Vienna FC': {'w1': 1.97, 'x': 2.3, 'w2': 8.2},
-    # hundreds of other teams' data
+    # hundreds of other games' data
 })
 
-for team, coefs1 in src1.items():
-    coefs2 = src2[team]
+for game, odds1 in source_1.items():
+    odds2 = source_2[game]
 
-    # coefs1 = {"w1": 1.93, "x": 2.32, "w2": 7.44}
-    # coefs2 = {"w1": 1.97, "x": 2.3, "w2": 8.2}
-    handle_fork(coefs1, coefs2)
+    # odds1 = {"w1": 1.93, "x": 2.32, "w2": 7.44}
+    # odds2 = {"w1": 1.97, "x": 2.3, "w2": 8.2}
+    handle_fork(odds1, odds2)
 ```
 
-With a human brain, it is not difficult to identify that "Rapid Wien - First Vienna" and "SK Rapid Wien - First Vienna
-FC" matches are the same. In the above example, the `src2` is defined as `FuzzyMap`, it makes its keys fuzzy-matchable,
-and we can get an item corresponding to the key of `src1`. See the below graph demonstrating the associations of
-`FuzzyMap` keys.
-
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/44609997/205437148-4fb3d7bd-1fe9-4ce8-8321-d7aef9488e37.svg" height="400" />
-</p>
+In this code example, `source_1` and `source_2` are the dictionary of game and coefficients key-value pairs parsed from
+different sources. And converting the `source_2` dictionary to the `FuzzyMap` dictionary makes it able to find the
+corresponding game using the game's key used in the `source_1` dictionary.
+
+```mermaid
+graph LR
+    src1team1[Rapid Wien - First Vienna] --> src1coefs1["{'w1': 1.93, 'x': 2.32, 'w2': 7.44}"]
+    src1team2[Al Bourj - Al Nejmeh] --> src1coefs2["{'w1': 26, 'x': 11.5, 'w2': 1.05}"]
+    src2team1[SK Rapid Wien - First Vienna FC] --> src2coefs1["{'w1': 1.97, 'x': 2.3, 'w2': 8.2}"]
+    src2team2[Bourj FC - Nejmeh SC Beirut] --> src2coefs2["{'w1': 32, 'x': 12, 'w2': 1.05}"]
+    src1team1 --> src2coefs1
+    src1team2 --> src2coefs2
+```
 
 ## License
 
-Copyright (C) 2022 Artyom Vancyan. [GPLv2](LICENSE)
+Copyright (C) 2022 Artyom Vancyan. [GPLv2](https://github.com/pysnippet/fuzzymap/blob/master/LICENSE)
```

### Comparing `fuzzymap-1.0.4/fuzzymap/__init__.py` & `fuzzymap-1.1.0/fuzzymap/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 __all__ = ('FuzzyMap',)
+__version__ = '1.1.0'
```

### Comparing `fuzzymap-1.0.4/fuzzymap/fuzzymap.py` & `fuzzymap-1.1.0/fuzzymap/fuzzymap.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     does  not  match  any of the keys by the given ratio, it returns `None`.
     """
 
     # set the minimum percent of the
     # diff between the compared keys
     ratio = 60
 
-    def closest_key(self, key):
+    def _closest_key(self, key):
         """Returns the closest key matched by the given ratio"""
 
         if len(self):
             # Calculate matching coefficient of each key via fuzz.ratio
             coefficients = {k: fuzz.ratio(k, key) for k in self.keys()}
             matching = max(coefficients, key=lambda k: coefficients[k])
             if coefficients[matching] >= self.ratio:
@@ -31,11 +31,11 @@
 
     def get(self, key, default=None):
         """Invokes the __getitem__ to keep the `FuzzyMap` behavior"""
 
         return self[key] or default
 
     def __missing__(self, key):
-        return super().get(self.closest_key(key))
+        return super().get(self._closest_key(key))
 
     def __setitem__(self, key, value):
-        super().__setitem__(self.closest_key(key), value)
+        super().__setitem__(self._closest_key(key), value)
```

