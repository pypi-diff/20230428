# Comparing `tmp/bw_temporalis-0.3.0.tar.gz` & `tmp/bw_temporalis-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_temporalis-0.3.0.tar", last modified: Thu Apr 27 12:22:29 2023, max compression
+gzip compressed data, was "bw_temporalis-0.3.1.tar", last modified: Thu Apr 27 14:39:23 2023, max compression
```

## Comparing `bw_temporalis-0.3.0.tar` & `bw_temporalis-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.580768 bw_temporalis-0.3.0/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-23 13:14:37.000000 bw_temporalis-0.3.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       30 2023-04-23 13:14:37.000000 bw_temporalis-0.3.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     3028 2023-04-27 12:22:29.580854 bw_temporalis-0.3.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1955 2023-04-23 13:14:37.000000 bw_temporalis-0.3.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.578174 bw_temporalis-0.3.0/bw_temporalis/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-27 12:21:46.000000 bw_temporalis-0.3.0/bw_temporalis/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      316 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/bw_temporalis/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7804 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/bw_temporalis/lca.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.576874 bw_temporalis-0.3.0/bw_temporalis/lcia/
--rw-r--r--   0 chrismutel   (501) staff       (20)       60 2023-04-27 12:03:34.000000 bw_temporalis-0.3.0/bw_temporalis/lcia/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4538 2023-04-27 12:17:06.000000 bw_temporalis-0.3.0/bw_temporalis/lcia/climate.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5352 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/bw_temporalis/temporal_distribution.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6513 2023-04-27 12:06:28.000000 bw_temporalis-0.3.0/bw_temporalis/timeline.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1197 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/bw_temporalis/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.579572 bw_temporalis-0.3.0/bw_temporalis.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3028 2023-04-27 12:22:29.000000 bw_temporalis-0.3.0/bw_temporalis.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      642 2023-04-27 12:22:29.000000 bw_temporalis-0.3.0/bw_temporalis.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-27 12:22:29.000000 bw_temporalis-0.3.0/bw_temporalis.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 11:46:09.000000 bw_temporalis-0.3.0/bw_temporalis.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      175 2023-04-27 12:22:29.000000 bw_temporalis-0.3.0/bw_temporalis.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       37 2023-04-27 12:22:29.000000 bw_temporalis-0.3.0/bw_temporalis.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.577239 bw_temporalis-0.3.0/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-04-23 13:14:37.000000 bw_temporalis-0.3.0/docs/conf.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.578007 bw_temporalis-0.3.0/examples/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1500 2023-04-26 18:20:47.000000 bw_temporalis-0.3.0/examples/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4350 2023-04-26 18:20:47.000000 bw_temporalis-0.3.0/examples/ia.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6149 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/examples/inv.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-23 13:14:37.000000 bw_temporalis-0.3.0/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1754 2023-04-27 12:22:29.581742 bw_temporalis-0.3.0/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 12:22:29.580512 bw_temporalis-0.3.0/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     8567 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/tests/test_fixtures.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4585 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/tests/test_td.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3620 2023-04-27 11:45:54.000000 bw_temporalis-0.3.0/tests/test_timeline.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.125622 bw_temporalis-0.3.1/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-23 13:14:37.000000 bw_temporalis-0.3.1/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       30 2023-04-23 13:14:37.000000 bw_temporalis-0.3.1/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3028 2023-04-27 14:39:23.125689 bw_temporalis-0.3.1/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1955 2023-04-23 13:14:37.000000 bw_temporalis-0.3.1/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.124194 bw_temporalis-0.3.1/bw_temporalis/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-27 14:39:06.000000 bw_temporalis-0.3.1/bw_temporalis/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      316 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/bw_temporalis/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7804 2023-04-27 14:38:30.000000 bw_temporalis-0.3.1/bw_temporalis/lca.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.123237 bw_temporalis-0.3.1/bw_temporalis/lcia/
+-rw-r--r--   0 chrismutel   (501) staff       (20)       60 2023-04-27 12:03:34.000000 bw_temporalis-0.3.1/bw_temporalis/lcia/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4538 2023-04-27 12:17:06.000000 bw_temporalis-0.3.1/bw_temporalis/lcia/climate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5352 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/bw_temporalis/temporal_distribution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6513 2023-04-27 12:06:28.000000 bw_temporalis-0.3.1/bw_temporalis/timeline.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1197 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/bw_temporalis/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.124950 bw_temporalis-0.3.1/bw_temporalis.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3028 2023-04-27 14:39:23.000000 bw_temporalis-0.3.1/bw_temporalis.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      642 2023-04-27 14:39:23.000000 bw_temporalis-0.3.1/bw_temporalis.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-27 14:39:23.000000 bw_temporalis-0.3.1/bw_temporalis.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 11:46:09.000000 bw_temporalis-0.3.1/bw_temporalis.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      175 2023-04-27 14:39:23.000000 bw_temporalis-0.3.1/bw_temporalis.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       37 2023-04-27 14:39:23.000000 bw_temporalis-0.3.1/bw_temporalis.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.123471 bw_temporalis-0.3.1/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-04-23 13:14:37.000000 bw_temporalis-0.3.1/docs/conf.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.124042 bw_temporalis-0.3.1/examples/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1500 2023-04-26 18:20:47.000000 bw_temporalis-0.3.1/examples/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4350 2023-04-26 18:20:47.000000 bw_temporalis-0.3.1/examples/ia.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6149 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/examples/inv.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-23 13:14:37.000000 bw_temporalis-0.3.1/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1754 2023-04-27 14:39:23.126070 bw_temporalis-0.3.1/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 14:39:23.125470 bw_temporalis-0.3.1/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8567 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/tests/test_fixtures.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4585 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/tests/test_td.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3620 2023-04-27 11:45:54.000000 bw_temporalis-0.3.1/tests/test_timeline.py
```

### Comparing `bw_temporalis-0.3.0/LICENSE` & `bw_temporalis-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/PKG-INFO` & `bw_temporalis-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 0.3.0
+Version: 0.3.1
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.3.0/README.md` & `bw_temporalis-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/bw_temporalis/lca.py` & `bw_temporalis-0.3.1/bw_temporalis/lca.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     pass
 
 
 class TemporalisLCA:
     """
     Calculate an LCA using graph traversal, with edges using temporal distributions.
 
-    Edges with temporal distributions should store this information using `"temporal distributions"`:
+    Edges with temporal distributions should store this information using `"temporal_distributions"`:
 
     ```python
-        exchange["temporal distribution"] = bw_temporalis.TemporalDistribution(
+        exchange["temporal_distribution"] = bw_temporalis.TemporalDistribution(
             times=numpy.array([-2, -1, 0, 1, 2], dtype="timedelta64[D]"),
             values=numpy.ones(5)
         )
     ```
 
     Temporal distribution times must always have the data type `timedelta64[D]`. Not all edges need to have temporal distributions.
 
@@ -132,30 +132,30 @@
         while heap:
             _, td, node = heappop(heap)
             for flow in self.flow_mapping.get(node.unique_id, []):
                 for exchange in self.get_biosphere_exchanges(
                     flow.flow_datapackage_id, node.activity_datapackage_id
                 ):
                     value = (
-                        exchange.data.get("temporal distribution")
+                        exchange.data.get("temporal_distribution")
                         or exchange.data["amount"]
                     )
                     timeline.add_flow_temporal_distribution(
                         td=td * value,
                         flow=flow.flow_datapackage_id,
                         activity=node.activity_datapackage_id,
                     )
 
             for edge in self.edge_mapping[node.unique_id]:
                 exchange = self.get_technosphere_exchange(
                     input_id=self.nodes[edge.producer_id].activity_datapackage_id,
                     output_id=node.activity_datapackage_id,
                 )
                 value = (
-                    exchange.data.get("temporal distribution")
+                    exchange.data.get("temporal_distribution")
                     or exchange.data["amount"]
                 ) / node.reference_product_production_amount
                 producer = self.nodes[edge.producer_id]
                 heappush(
                     heap,
                     (
                         1 / node.cumulative_score,
@@ -179,16 +179,16 @@
 
     def get_biosphere_exchanges(self, flow_id: int, activity_id: int) -> Iterable[ED]:
         exchanges = self._exchange_iterator(flow_id, activity_id)
         if len(exchanges) > 1:
             total = sum(exc.data["amount"] for exc in exchanges)
             for exc in exchanges:
                 exc.data["amount"] /= total
-                if "temporal distribution" in exc.data:
-                    exc.data["temporal distribution"] /= total
+                if "temporal_distribution" in exc.data:
+                    exc.data["temporal_distribution"] /= total
                 yield exc
         else:
             yield from exchanges
 
     def get_technosphere_exchange(self, input_id: int, output_id: int) -> ED:
         exchanges = self._exchange_iterator(input_id, output_id)
         if len(exchanges) > 1:
```

### Comparing `bw_temporalis-0.3.0/bw_temporalis/lcia/climate.py` & `bw_temporalis-0.3.1/bw_temporalis/lcia/climate.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/bw_temporalis/temporal_distribution.py` & `bw_temporalis-0.3.1/bw_temporalis/temporal_distribution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/bw_temporalis/timeline.py` & `bw_temporalis-0.3.1/bw_temporalis/timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/bw_temporalis/utils.py` & `bw_temporalis-0.3.1/bw_temporalis/utils.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/bw_temporalis.egg-info/PKG-INFO` & `bw_temporalis-0.3.1/bw_temporalis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-temporalis
-Version: 0.3.0
+Version: 0.3.1
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.3.0/bw_temporalis.egg-info/SOURCES.txt` & `bw_temporalis-0.3.1/bw_temporalis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/docs/conf.py` & `bw_temporalis-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/examples/__init__.py` & `bw_temporalis-0.3.1/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/examples/ia.py` & `bw_temporalis-0.3.1/examples/ia.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/examples/inv.py` & `bw_temporalis-0.3.1/examples/inv.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/setup.cfg` & `bw_temporalis-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/tests/test_fixtures.py` & `bw_temporalis-0.3.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/tests/test_td.py` & `bw_temporalis-0.3.1/tests/test_td.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.3.0/tests/test_timeline.py` & `bw_temporalis-0.3.1/tests/test_timeline.py`

 * *Files identical despite different names*

