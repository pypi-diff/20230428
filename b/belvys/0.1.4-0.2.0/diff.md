# Comparing `tmp/belvys-0.1.4.tar.gz` & `tmp/belvys-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belvys-0.1.4.tar", last modified: Tue Dec 13 19:03:32 2022, max compression
+gzip compressed data, was "belvys-0.2.0.tar", last modified: Fri Apr 28 09:38:45 2023, max compression
```

## Comparing `belvys-0.1.4.tar` & `belvys-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:03:32.235447 belvys-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2022-12-13 19:03:22.000000 belvys-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:03:22.000000 belvys-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-13 19:03:32.235447 belvys-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2022-12-13 19:03:22.000000 belvys-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:03:32.235447 belvys-0.1.4/belvys/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-13 19:03:32.235447 belvys-0.1.4/belvys/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16379 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/example_api_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/example_api_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/example_structure_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/example_structure_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2022-12-13 19:03:22.000000 belvys-0.1.4/belvys/tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:03:32.235447 belvys-0.1.4/belvys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-13 19:03:32.000000 belvys-0.1.4/belvys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-13 19:03:32.000000 belvys-0.1.4/belvys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 19:03:32.000000 belvys-0.1.4/belvys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 19:03:31.000000 belvys-0.1.4/belvys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-13 19:03:32.000000 belvys-0.1.4/belvys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-13 19:03:32.000000 belvys-0.1.4/belvys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-13 19:03:22.000000 belvys-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-13 19:03:32.235447 belvys-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-13 19:03:22.000000 belvys-0.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81464 2022-12-13 19:03:22.000000 belvys-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.059462 belvys-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 09:38:31.000000 belvys-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 09:38:31.000000 belvys-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 09:38:45.059462 belvys-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 09:38:31.000000 belvys-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.063462 belvys-0.2.0/belvys/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 09:38:45.063462 belvys-0.2.0/belvys/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_api_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_api_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_structure_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_structure_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.059462 belvys-0.2.0/belvys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:38:44.000000 belvys-0.2.0/belvys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 09:38:31.000000 belvys-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 09:38:45.059462 belvys-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 09:38:31.000000 belvys-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.059462 belvys-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 09:38:31.000000 belvys-0.2.0/tests/test_liveconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 09:38:31.000000 belvys-0.2.0/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-04-28 09:38:31.000000 belvys-0.2.0/versioneer.py
```

### Comparing `belvys-0.1.4/LICENSE` & `belvys-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/PKG-INFO` & `belvys-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.1.4
+Version: 0.2.0
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.1.4/README.rst` & `belvys-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/adjustment.py` & `belvys-0.2.0/belvys/adjustment.py`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/api.py` & `belvys-0.2.0/belvys/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,16 @@
         elif self._retry is True:
             # Authentication might have expired, or maybe has never been done before. Try once.
             self._retry = False
             self.access.authenticate()
             return self.query(url)  # retry.
         else:
             raise RuntimeError(
-                f"Request to url {url} failed; server response: {response}."
+                f"Request to url {url} failed; server response: {response or '(None)'}"
+                f" (status code {response.status_code})."
             )
 
     def metadata(self, tsid: int) -> Dict:
         """Get information about timeseries.
 
         Parameters
         ----------
```

### Comparing `belvys-0.1.4/belvys/example.py` & `belvys-0.2.0/belvys/example.py`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/example_api_complex.yaml` & `belvys-0.2.0/belvys/example_api_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/example_structure_basic.yaml` & `belvys-0.2.0/belvys/example_structure_basic.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/example_structure_complex.yaml` & `belvys-0.2.0/belvys/example_structure_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/structure.py` & `belvys-0.2.0/belvys/structure.py`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/belvys/tenant.py` & `belvys-0.2.0/belvys/tenant.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,23 +119,47 @@
         elif isinstance(ts_tree, Iterable):  # Must be after Dict
             for branch in ts_tree:
                 self._fetch_series(branch, ts_left, ts_right, **kwargs)
 
     def _pfline(self, ts_tree: TsTree) -> pf.PfLine:
         """Create a portfolio line from the data stored in the ts_tree series."""
 
-        # MultiPfLine.
+        # NestedPfLine.
 
         if isinstance(ts_tree, Dict):
             children = {}
             for name, subtree in ts_tree.items():
                 children[name] = self._pfline(subtree)
+
+            # Turn all revenue-only pflines into complete pflines.
+            children = {
+                name: child | pf.Q_(0.0, "MW")
+                if child.kind is pf.Kind.REVENUE
+                else child
+                for name, child in children.items()
+            }
             return pf.PfLine(children)
 
-        # SinglePfLine.
+            # TODO: use code below once portfolyo allows for NestedPfLine | 0 MW.
+            kinds = set([child.kind for child in children.values()])
+            if len(kinds) == 1:
+                return pf.PfLine(children)
+
+            def make_complete(pfl: pf.PfLine):
+                if pfl.kind in (pf.Kind.REVENUE, pf.Kind.PRICE):
+                    return pfl | pf.Q_(0, "MW")
+                elif pfl.kind is pf.Kind.VOLUME:
+                    return pfl | pf.Q_(0, "Eur/MWh")
+                return pfl  # pfl.kind is pf.Kind.COMPLETE
+
+            return pf.PfLine(
+                {name: make_complete(child) for name, child in children.items()}
+            )
+
+        # FlatPfLine.
 
         tss = [ts_tree] if isinstance(ts_tree, Ts) else ts_tree
         # Collect the timeseries values from Belvis.
         series_by_dimension = defaultdict(list)
         for ts in tss:
             s = ts.series  # series as returned by api.
             # Here we make corrections for design decisions in our Belvis database.
@@ -230,18 +254,15 @@
         for pfid in self.structure.to_original_pfids(pfid):
             ts_tree = self.structure.tstree_pfline(pfid, pflineid)
             self._fetch_series(ts_tree, ts_left, ts_right, missing2zero=missing2zero)
             ts_trees.append(ts_tree)
         if debug:
             return ts_trees
         # Turn into portfolio line.
-        pflines = []
-        for ts_tree in ts_trees:
-            pflines.append(self._pfline(ts_tree))
-        return sum(pflines)
+        return sum([self._pfline(ts_tree) for ts_tree in ts_trees])
 
     def price_pfl(
         self,
         priceid: str,
         ts_left: pd.Timestamp,
         ts_right: pd.Timestamp,
         missing2zero: bool = True,
```

### Comparing `belvys-0.1.4/belvys.egg-info/PKG-INFO` & `belvys-0.2.0/belvys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.1.4
+Version: 0.2.0
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.1.4/belvys.egg-info/SOURCES.txt` & `belvys-0.2.0/belvys.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,8 +18,10 @@
 belvys/structure.py
 belvys/tenant.py
 belvys.egg-info/PKG-INFO
 belvys.egg-info/SOURCES.txt
 belvys.egg-info/dependency_links.txt
 belvys.egg-info/not-zip-safe
 belvys.egg-info/requires.txt
-belvys.egg-info/top_level.txt
+belvys.egg-info/top_level.txt
+tests/test_liveconnection.py
+tests/test_structure.py
```

### Comparing `belvys-0.1.4/setup.py` & `belvys-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `belvys-0.1.4/versioneer.py` & `belvys-0.2.0/versioneer.py`

 * *Files identical despite different names*

