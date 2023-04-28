# Comparing `tmp/gate_drift-0.1.4.tar.gz` & `tmp/gate_drift-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gate_drift-0.1.4.tar", max compression
+gzip compressed data, was "gate_drift-0.1.5.tar", max compression
```

## Comparing `gate_drift-0.1.4.tar` & `gate_drift-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-04-20 19:33:25.531694 gate_drift-0.1.4/LICENSE
--rw-r--r--   0        0        0     1965 2023-04-28 01:13:54.722939 gate_drift-0.1.4/README.md
--rw-r--r--   0        0        0      244 2023-04-27 01:03:41.538087 gate_drift-0.1.4/gate/__init__.py
--rw-r--r--   0        0        0    21635 2023-04-28 00:57:06.998900 gate_drift-0.1.4/gate/drift.py
--rw-r--r--   0        0        0     5223 2023-04-27 23:14:25.758176 gate_drift-0.1.4/gate/statistics.py
--rw-r--r--   0        0        0     4084 2023-04-28 00:57:06.780878 gate_drift-0.1.4/gate/summarize.py
--rw-r--r--   0        0        0    16145 2023-04-28 00:57:07.107493 gate_drift-0.1.4/gate/summary.py
--rw-r--r--   0        0        0     1051 2023-04-28 01:20:50.855647 gate_drift-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 gate_drift-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-20 19:33:25.531694 gate_drift-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1965 2023-04-28 01:23:05.642615 gate_drift-0.1.5/README.md
+-rw-r--r--   0        0        0      244 2023-04-28 01:23:05.646837 gate_drift-0.1.5/gate/__init__.py
+-rw-r--r--   0        0        0    21782 2023-04-28 17:32:12.262353 gate_drift-0.1.5/gate/drift.py
+-rw-r--r--   0        0        0     5223 2023-04-28 01:23:05.647200 gate_drift-0.1.5/gate/statistics.py
+-rw-r--r--   0        0        0     4084 2023-04-28 01:23:05.647333 gate_drift-0.1.5/gate/summarize.py
+-rw-r--r--   0        0        0    16145 2023-04-28 01:23:05.647498 gate_drift-0.1.5/gate/summary.py
+-rw-r--r--   0        0        0     1051 2023-04-28 17:33:44.094633 gate_drift-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 gate_drift-0.1.5/PKG-INFO
```

### Comparing `gate_drift-0.1.4/LICENSE` & `gate_drift-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.4/README.md` & `gate_drift-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.4/gate/drift.py` & `gate_drift-0.1.5/gate/drift.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,17 +152,18 @@
 
         The resulting dataframe has the following schema (column, statistic are
         indexes):
 
         - column: Name of the column
         - statistic: Name of the statistic
         - z-score: z-score of the column
-        - cluster: Cluster number of the column (if clustering was performed)
-        - z-score-cluster: z-score of the column in the cluster (if
-        clustering was performed)
+        - cluster: Cluster number that the column belongs to (if clustering was
+        performed)
+        - abs(z-score-cluster): absolute value of the average z-score of the
+        column in the cluster (if clustering was performed)
 
         Use the `drifted_columns` method first, since `drifted_columns`
         deduplicates columns.
 
         Args:
             sort_by_cluster_score (bool, optional):
                 Whether to sort by cluster z-score. Defaults to False.
@@ -187,28 +188,30 @@
         sorted_df.rename(columns={sorted_df.columns[0]: "z-score"}, inplace=True)
         sorted_df = sorted_df.rename_axis(["column", "statistic"])
 
         if self._clustered_features is not None:
             # Join the clustered features with the sorted_df
             # sorted_df.rename(index={"column": "cluster"}, inplace=True)
             sorted_df = sorted_df.rename_axis(["cluster", "statistic"]).reset_index()
-            sorted_df.rename(columns={"z-score": "z-score-cluster"}, inplace=True)
+            sorted_df.rename(columns={"z-score": "abs(z-score-cluster)"}, inplace=True)
 
             sorted_df = sorted_df.merge(
                 self._clustered_features,
                 on=["cluster", "statistic"],
                 how="left",
             )
 
             # Sort again
             if sort_by_cluster_score:
                 sorted_df = sorted_df.reindex(
-                    sorted_df[["z-score-cluster", "z-score"]]
+                    sorted_df[["abs(z-score-cluster)", "z-score"]]
                     .abs()
-                    .sort_values(by=["z-score-cluster", "z-score"], ascending=False)
+                    .sort_values(
+                        by=["abs(z-score-cluster)", "z-score"], ascending=False
+                    )
                     .index
                 )
                 sorted_df.set_index(["column", "statistic"], inplace=True)
 
         if len(self._embedding_columns) > 0 and average_embedding_columns:
             # Average the z-scores
             sorted_df.reset_index(inplace=True)
@@ -250,15 +253,15 @@
         resulting dataframe has the following schema (column is an
         index):
 
         - column: Name of the column
         - statistic: Name of the statistic
         - z-score: z-score of the column
         - cluster: Cluster number of the column (if clustering was performed)
-        - z-score-cluster: z-score of the column in the cluster (if
+        - abs(z-score-cluster): z-score of the column in the cluster (if
         clustering was performed)
 
         Args:
             limit (int, optional):
                 Limit for number of drifted columns to return. Defaults to 10.
             average_embedding_columns (bool, optional):
                 Whether to average statistics across embedding dimensions.
@@ -273,33 +276,33 @@
                 highest magnitude z-score is returned.
         """
         # Return a dataframe of the top limit columns that have drifted
         # Drop duplicate column names
         dd_results = self.drill_down(average_embedding_columns)
 
         if self._clustered_features is not None:
-            # Sort by z-score first, then z-score-cluster
+            # Sort by z-score first, then abs(z-score-cluster)
             dd_results = dd_results.reindex(
-                dd_results[["z-score", "z-score-cluster"]]
+                dd_results[["z-score", "abs(z-score-cluster)"]]
                 .abs()
-                .sort_values(by=["z-score", "z-score-cluster"], ascending=False)
+                .sort_values(by=["z-score", "abs(z-score-cluster)"], ascending=False)
                 .index
             )
 
         dd_results.reset_index(inplace=True)
 
         dd_results.drop_duplicates(subset=["column"], keep="first", inplace=True)
         dd_results.set_index("column", inplace=True)
 
         if self._clustered_features is not None:
             # Reorder columns
             dd_results = dd_results[
-                ["statistic", "z-score", "cluster", "z-score-cluster"]
+                ["statistic", "z-score", "cluster", "abs(z-score-cluster)"]
             ]
-            dd_results = dd_results[dd_results["z-score-cluster"].abs() > 0.0]
+            dd_results = dd_results[dd_results["abs(z-score-cluster)"].abs() > 0.0]
 
         return dd_results.head(limit)
 
 
 def name_to_ec(name: str, embedding_columns: typing.List[str]) -> str:
     """Converts a column name to an embedding column name.
```

### Comparing `gate_drift-0.1.4/gate/statistics.py` & `gate_drift-0.1.5/gate/statistics.py`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.4/gate/summarize.py` & `gate_drift-0.1.5/gate/summarize.py`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.4/gate/summary.py` & `gate_drift-0.1.5/gate/summary.py`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.4/pyproject.toml` & `gate_drift-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gate-drift"
-version = "0.1.4"
+version = "0.1.5"
 description = "Data drift detection tool for machine learning pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gate"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gate_drift-0.1.4/PKG-INFO` & `gate_drift-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gate-drift
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data drift detection tool for machine learning pipelines.
 License: MIT
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

