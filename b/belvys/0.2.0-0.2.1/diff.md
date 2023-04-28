# Comparing `tmp/belvys-0.2.0.tar.gz` & `tmp/belvys-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belvys-0.2.0.tar", last modified: Fri Apr 28 09:38:45 2023, max compression
+gzip compressed data, was "belvys-0.2.1.tar", last modified: Fri Apr 28 14:58:00 2023, max compression
```

## Comparing `belvys-0.2.0.tar` & `belvys-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.059462 belvys-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 09:38:31.000000 belvys-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 09:38:31.000000 belvys-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 09:38:45.059462 belvys-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 09:38:31.000000 belvys-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.063462 belvys-0.2.0/belvys/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 09:38:45.063462 belvys-0.2.0/belvys/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_api_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_api_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_structure_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/example_structure_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-28 09:38:31.000000 belvys-0.2.0/belvys/tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.059462 belvys-0.2.0/belvys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:38:44.000000 belvys-0.2.0/belvys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:38:45.000000 belvys-0.2.0/belvys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 09:38:31.000000 belvys-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 09:38:45.059462 belvys-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 09:38:31.000000 belvys-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:38:45.059462 belvys-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 09:38:31.000000 belvys-0.2.0/tests/test_liveconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 09:38:31.000000 belvys-0.2.0/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-04-28 09:38:31.000000 belvys-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:58:00.218225 belvys-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 14:57:47.000000 belvys-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 14:57:47.000000 belvys-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 14:58:00.218225 belvys-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 14:57:47.000000 belvys-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:58:00.218225 belvys-0.2.1/belvys/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 14:58:00.218225 belvys-0.2.1/belvys/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/example_api_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/example_api_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/example_structure_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/example_structure_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-28 14:57:47.000000 belvys-0.2.1/belvys/tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:58:00.218225 belvys-0.2.1/belvys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 14:58:00.000000 belvys-0.2.1/belvys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 14:58:00.000000 belvys-0.2.1/belvys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:58:00.000000 belvys-0.2.1/belvys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:57:59.000000 belvys-0.2.1/belvys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 14:58:00.000000 belvys-0.2.1/belvys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 14:58:00.000000 belvys-0.2.1/belvys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 14:57:47.000000 belvys-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 14:58:00.218225 belvys-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 14:57:47.000000 belvys-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:58:00.218225 belvys-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 14:57:47.000000 belvys-0.2.1/tests/test_liveconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 14:57:47.000000 belvys-0.2.1/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-04-28 14:57:47.000000 belvys-0.2.1/versioneer.py
```

### Comparing `belvys-0.2.0/LICENSE` & `belvys-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/PKG-INFO` & `belvys-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.2.0
+Version: 0.2.1
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.2.0/README.rst` & `belvys-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys/adjustment.py` & `belvys-0.2.1/belvys/adjustment.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys/api.py` & `belvys-0.2.1/belvys/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 
         return cls(auth, req)
 
 
 class Api:
     """A class to interact with a Belvis Rest API server."""
 
+    __slots__ = ["_retry", "_server", "_tenant", "_cache", "_filepath", "_access"]
+
     @classmethod
     def from_file(cls, filepath: Union[str, pathlib.Path]) -> Api:
         """Load api data from file.
 
         Parameters
         ----------
         filepath : Union[str, pathlib.Path]
```

### Comparing `belvys-0.2.0/belvys/example.py` & `belvys-0.2.1/belvys/example.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys/example_api_complex.yaml` & `belvys-0.2.1/belvys/example_api_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys/example_structure_basic.yaml` & `belvys-0.2.1/belvys/example_structure_basic.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys/example_structure_complex.yaml` & `belvys-0.2.1/belvys/example_structure_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys/structure.py` & `belvys-0.2.1/belvys/structure.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 self._assert_valid_ref(r)
         else:
             raise AssertionError(
                 f"Incorrect type for ``ref``: expected str or Iterable; got {type(ref)}."
             )
 
 
-@dataclass
+@dataclass(frozen=True)
 class Structure:
     """Structure of the belvis database; which portfolios and timeseries are of interest.
 
     Parameters
     ----------
     freq : str
         Frequency of the spot market, which is also the shortest frequency that is of
@@ -131,21 +131,23 @@
             else:
                 return tsname_tree
         else:
             return [self._expand_tree(ts) for ts in tsname_tree]
 
     def __post_init__(self):
         # Finish initialisation.
-        self.portfolios = Portfolios(**self.portfolios)
+        portfolios = Portfolios(**self.portfolios)
+        object.__setattr__(self, "portfolios", portfolios)  # because frozen
 
         # Ensure pflines part is correct.
-        self.pflines = {
+        pflines = {
             pflineid: self._expand_tree(tsname_tree)
             for pflineid, tsname_tree in self.pflines.items()
         }
+        object.__setattr__(self, "pflines", pflines)  # because frozen
 
         # Assert corrections part is valid.
         for pfid, pflinesdict in self.corrections.items():
             assert pfid in self.portfolios.original  # must override existing portfolio
             for pfline, ref in pflinesdict.items():
                 if ref is None:
                     assert pfline in self.pflines.keys()
@@ -184,31 +186,31 @@
 
         Returns
         -------
         TsTree
             Names of timeseries that must be fetched.
         """
         if pfid not in (avail := self.available_pfids(True)):
-            raise ValueError(f"``pfid`` must one of {', '.join(avail)}.")
-
-        # Use correction, if it exists.
-        tsname_tree = self.corrections.get(pfid, {}).get(pflineid, "notfound")
-        if tsname_tree is None:
             raise ValueError(
-                f"The portfolio line ({pflineid}) does not exists for this portfolio ({pfid})."
+                f"The portfolio id ({pfid}) does not exist in this Structure instance;"
+                f" ``pfid`` must be one of {', '.join(avail)}."
             )
-        elif tsname_tree != "notfound":
+        if pflineid not in (avail := self.available_pflineids(pfid)):
+            raise ValueError(
+                f"The portfolio line ({pflineid}) does not exists for this portfolio ({pfid});"
+                f" ``pflineid`` must be one of {', '.join(avail)}."
+            )
+
+        # Use correction, if a correction is defined for this pfid and pflineid.
+        tsname_tree = self.corrections.get(pfid, {}).get(pflineid, "notfound")
+        if tsname_tree != "notfound":
             return create_tstree(pfid, tsname_tree)
 
         # If not, use default.
-        tsname_tree = self.pflines.get(pflineid, None)
-        if tsname_tree is None:
-            raise ValueError(
-                f"The portfolio line ({pflineid}) does not exists for this portfolio ({pfid})."
-            )
+        tsname_tree = self.pflines.get(pflineid, None)  # key should always exist
         return create_tstree(pfid, tsname_tree)
 
     def tstree_price(self, priceid: str) -> TsTree:
         """Timeseries that must be fetched to get the wanted price.
 
         Parameters
         ----------
@@ -255,26 +257,29 @@
             Id of portfolio. May be original or synthetic.
 
         Returns
         -------
         Iterable[str]
             List of original portfolio ids.
         """
+        if pfid not in (avail := self.available_pfids()):
+            raise ValueError(
+                f"The portfolio id ({pfid}) does not exist in this Structure instance;"
+                f" ``pfid`` must be one of {', '.join(avail)}."
+            )
+
         if pfid in self.portfolios.original:
             return [pfid]
-        elif pfid in self.portfolios.synthetic:
-            pfids = []
-            for child_pfid in self.portfolios.synthetic[pfid]:
-                for pfid in self.to_original_pfids(child_pfid):
-                    pfids.append(pfid)
-            return pfids
-        raise ValueError(
-            f"Could not find portfolio id {pfid} in configuration for this tenant; "
-            f"expected one of {', '.join((*self.portfolios.original, *self.portfolios.synthetic))}."
-        )
+
+        # pfid in self.portfolios.sythetic
+        original_pfids = []
+        for child_pfid in self.portfolios.synthetic[pfid]:
+            for original_pfid in self.to_original_pfids(child_pfid):
+                original_pfids.append(original_pfid)
+        return original_pfids
 
     def available_pflineids(self, pfid: str) -> Iterable[str]:
         """All available portfolio line ids for a given portfolio.
 
         Parameters
         ----------
         pfid : str
```

### Comparing `belvys-0.2.0/belvys/tenant.py` & `belvys-0.2.1/belvys/tenant.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/belvys.egg-info/PKG-INFO` & `belvys-0.2.1/belvys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.2.0
+Version: 0.2.1
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.2.0/belvys.egg-info/SOURCES.txt` & `belvys-0.2.1/belvys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/setup.py` & `belvys-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/tests/test_liveconnection.py` & `belvys-0.2.1/tests/test_liveconnection.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/tests/test_structure.py` & `belvys-0.2.1/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.0/versioneer.py` & `belvys-0.2.1/versioneer.py`

 * *Files identical despite different names*

