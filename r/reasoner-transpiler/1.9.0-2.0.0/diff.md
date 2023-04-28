# Comparing `tmp/reasoner-transpiler-1.9.0.tar.gz` & `tmp/reasoner-transpiler-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-transpiler-1.9.0.tar", last modified: Mon Sep 13 15:21:25 2021, max compression
+gzip compressed data, was "reasoner-transpiler-2.0.0.tar", last modified: Fri Apr 28 13:36:01 2023, max compression
```

## Comparing `reasoner-transpiler-1.9.0.tar` & `reasoner-transpiler-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-13 15:21:25.551744 reasoner-transpiler-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)      292 2021-09-13 15:21:25.551744 reasoner-transpiler-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      941 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-13 15:21:25.551744 reasoner-transpiler-1.9.0/reasoner_transpiler/
--rw-r--r--   0 runner    (1001) docker     (116)       41 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/reasoner_transpiler/attribute_types.json
--rw-r--r--   0 runner    (1001) docker     (116)     6338 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/reasoner_transpiler/cypher.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/reasoner_transpiler/cypher_expression.py
--rw-r--r--   0 runner    (1001) docker     (116)    11457 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/reasoner_transpiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (116)     8780 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/reasoner_transpiler/nesting.py
--rw-r--r--   0 runner    (1001) docker     (116)     2440 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/reasoner_transpiler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-13 15:21:25.551744 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      292 2021-09-13 15:21:25.000000 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      477 2021-09-13 15:21:25.000000 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-09-13 15:21:25.000000 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-09-13 15:21:25.000000 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-09-13 15:21:25.000000 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-09-13 15:21:25.000000 reasoner-transpiler-1.9.0/reasoner_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-09-13 15:21:25.551744 reasoner-transpiler-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      551 2021-09-13 15:21:23.000000 reasoner-transpiler-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:36:01.074276 reasoner-transpiler-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 13:36:01.074276 reasoner-transpiler-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:36:01.070276 reasoner-transpiler-2.0.0/reasoner_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/attribute_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/cypher_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/nesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:36:01.070276 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:36:01.074276 reasoner-transpiler-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/setup.py
```

### Comparing `reasoner-transpiler-1.9.0/README.md` & `reasoner-transpiler-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-1.9.0/reasoner_transpiler/cypher.py` & `reasoner-transpiler-2.0.0/reasoner_transpiler/cypher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools for compiling QGraph into Cypher query."""
+import copy
 from functools import reduce
 import json
 from operator import and_
 from pathlib import Path
 
 from . import cypher_expression
 from .matching import match_query
@@ -16,14 +17,19 @@
     "category",
 ]
 RESERVED_EDGE_PROPS = [
     "id",
     "predicate",
 ]
 
+EDGE_SOURCE_PROPS = [
+    "biolink:aggregator_knowledge_source",
+    "biolink:primary_knowledge_source"
+]
+
 def nest_op(operator, *args):
     """Generate a nested set of operations from a flat expression."""
     if len(args) > 2:
         return [operator, args[0], nest_op(operator, *args[1:])]
     else:
         return [operator, *args]
 
@@ -68,18 +74,21 @@
             "WHERE ni IS NOT null "
             "| {{id: ni}}]"
         ).format(
             qnode_id,
         ) if qnode.get("is_set", False) else
         (
             "`{0}`: (CASE "
-            "WHEN `{0}` IS NOT NULL THEN [{{id: `{0}`.id}}] "
+            "WHEN `{0}` IS NOT NULL THEN [{{id: `{0}`.id{1}}}] "
             "ELSE [] "
             "END)"
-        ).format(qnode_id)
+        ).format(
+            qnode_id,
+            f", qnode_id: `{qnode_id}_superclass`.id" if f"{qnode_id}_superclass" in qnodes else "",
+        )
         for qnode_id, qnode in qnodes.items()
         if qnode.get("_return", True)
     ]
     edge_bindings = [
         (
             "`{0}`: [ei IN collect(DISTINCT toString(id(`{0}`))) "
             "WHERE ei IS NOT null "
@@ -104,15 +113,15 @@
     ]
     kedges = [
         "collect(DISTINCT `{0}`)".format(qedge_id)
         for qedge_id, qedge in qedges.items()
         if qedge.get("_return", True)
     ]
     assemble_clause = (
-        "WITH {{node_bindings: {{{0}}}, edge_bindings: {{{1}}}}} AS result, "
+        "WITH {{node_bindings: {{{0}}}, analyses: [{{edge_bindings: {{{1}}}}}]}} AS result, "
         "{{nodes: {2}, edges: {3}}} AS knowledge_graph"
     ).format(
         ", ".join(node_bindings) or "",
         ", ".join(edge_bindings) or "",
         " + ".join(knodes) or "[]",
         " + ".join(kedges) or "[]",
     )
@@ -141,23 +150,28 @@
             "[key], \"NA\"), value: n[key]}]}]), "
         )
         if qnodes else
         "nodes: [], "
     )
     aggregate_clause += (
         (
-            "edges: apoc.map.fromLists("
+            "edges: apoc.map.fromLists(" + (
+            "[e IN collect(DISTINCT kedge) | toString(ID(e)) ], " if kwargs.get("relationship_id", "property") == "internal" else
             "[e IN collect(DISTINCT kedge) | e.id], "
+            ) +
             "[e IN collect(DISTINCT kedge) | {"
             "predicate: type(e), subject: startNode(e).id, object: endNode(e).id, "
             "attributes: [key in apoc.coll.subtract(keys(e), "
-            + cypher_expression.dumps(RESERVED_EDGE_PROPS) +
+            + cypher_expression.dumps(RESERVED_EDGE_PROPS + EDGE_SOURCE_PROPS) +
             ") | {original_attribute_name: key, attribute_type_id: COALESCE("
             + cypher_expression.dumps(ATTRIBUTE_TYPES) +
-            "[key], \"NA\"), value: e[key]}]}])"
+            "[key], \"NA\"), value: e[key]}]," +
+            "sources: [key IN " + cypher_expression.dumps(EDGE_SOURCE_PROPS) +" | "
+            " {resource_id: e[key] , resource_role: key }]"
+            "}])"
         )
         if kedges else
         "edges: []"
     )
     aggregate_clause += "} AS knowledge_graph"
     clauses.append(aggregate_clause)
 
@@ -178,14 +192,15 @@
 
 
 def get_query(qgraph, **kwargs):
     """Generate a Cypher query to extract the answer maps for a question.
 
     Returns the query as a string.
     """
+    qgraph = copy.deepcopy(qgraph)
     clauses = []
     query = transpile_compound(qgraph, **kwargs)
     clauses.extend(query.compile())
     where_clause = query.where_clause()
     if where_clause:
         if not clauses[-1].startswith("WITH"):
             clauses.append(query.with_clause())
```

### Comparing `reasoner-transpiler-1.9.0/reasoner_transpiler/cypher_expression.py` & `reasoner-transpiler-2.0.0/reasoner_transpiler/cypher_expression.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-1.9.0/reasoner_transpiler/nesting.py` & `reasoner-transpiler-2.0.0/reasoner_transpiler/nesting.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-1.9.0/reasoner_transpiler/util.py` & `reasoner-transpiler-2.0.0/reasoner_transpiler/util.py`

 * *Files identical despite different names*

