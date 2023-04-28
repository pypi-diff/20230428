# Comparing `tmp/acro-0.0.6.tar.gz` & `tmp/acro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acro-0.0.6.tar", last modified: Sun Apr 16 19:05:49 2023, max compression
+gzip compressed data, was "acro-0.1.0.tar", last modified: Fri Apr 28 13:36:23 2023, max compression
```

## Comparing `acro-0.0.6.tar` & `acro-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.0.6/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3149 2023-04-16 19:05:49.689686 acro-0.0.6/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2247 2022-11-17 15:40:19.000000 acro-0.0.6/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/acro/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-03-13 11:57:55.000000 acro-0.0.6/acro/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28833 2023-04-16 18:48:41.000000 acro-0.0.6/acro/acro.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1006 2023-03-13 11:57:55.000000 acro-0.0.6/acro/default.yaml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11264 2023-04-16 18:48:41.000000 acro-0.0.6/acro/utils.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/acro.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3149 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      265 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-04-16 19:05:49.689686 acro-0.0.6/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-04-16 18:51:12.000000 acro-0.0.6/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.0.6/test/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9669 2023-04-16 18:48:41.000000 acro-0.0.6/test/test_initial.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-28 13:36:23.972102 acro-0.1.0/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.1.0/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3149 2023-04-28 13:36:23.972102 acro-0.1.0/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2247 2022-11-17 15:40:19.000000 acro-0.1.0/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-28 13:36:23.972102 acro-0.1.0/acro/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-03-13 11:57:55.000000 acro-0.1.0/acro/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    29746 2023-04-28 11:01:46.000000 acro-0.1.0/acro/acro.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-04-18 18:15:41.000000 acro-0.1.0/acro/default.yaml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11895 2023-04-28 11:01:46.000000 acro-0.1.0/acro/utils.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-28 13:36:23.972102 acro-0.1.0/acro.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3149 2023-04-28 13:36:23.000000 acro-0.1.0/acro.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      265 2023-04-28 13:36:23.000000 acro-0.1.0/acro.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-04-28 13:36:23.000000 acro-0.1.0/acro.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-04-28 13:36:23.000000 acro-0.1.0/acro.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-04-28 13:36:23.000000 acro-0.1.0/acro.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-04-28 13:36:23.972102 acro-0.1.0/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-04-28 13:27:48.000000 acro-0.1.0/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-28 13:36:23.972102 acro-0.1.0/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.1.0/test/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10759 2023-04-27 09:35:54.000000 acro-0.1.0/test/test_initial.py
```

### Comparing `acro-0.0.6/LICENSE` & `acro-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acro-0.0.6/PKG-INFO` & `acro-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.0.6
+Version: 0.1.0
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.0.6/README.md` & `acro-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `acro-0.0.6/acro/acro.py` & `acro-0.1.0/acro/acro.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             self.config = yaml.load(handle, Loader=yaml.loader.SafeLoader)
         logger.info("config: %s", self.config)
         # set globals needed for aggregation functions
         utils.THRESHOLD = self.config["safe_threshold"]
         utils.SAFE_PRATIO_P = self.config["safe_pratio_p"]
         utils.SAFE_NK_N = self.config["safe_nk_n"]
         utils.SAFE_NK_K = self.config["safe_nk_k"]
+        utils.CHECK_MISSING_VALUES = self.config["check_missing_values"]
 
     def finalise(self, filename: str = "results.json") -> dict:
         """Creates a results file for checking.
 
         Parameters
         ----------
         filename : str
@@ -89,15 +90,15 @@
         return self.results
 
     def __add_output(  # pylint: disable=too-many-arguments
         self,
         command: str,
         summary: str,
         outcome: DataFrame,
-        output: list[DataFrame],
+        output: str | list[DataFrame],
         comments: str = "",
     ) -> None:
         """Adds an output to the results dictionary.
 
         Parameters
         ----------
         command : str
@@ -262,14 +263,25 @@
                 masks["negative"] = negative
             # p-percent check
             masks["p-ratio"] = pd.crosstab(
                 index, columns, values, aggfunc=utils.agg_p_percent
             )
             # nk values check
             masks["nk-rule"] = pd.crosstab(index, columns, values, aggfunc=utils.agg_nk)
+            # check for missing values -- currently unsupported
+            if utils.CHECK_MISSING_VALUES:
+                masks["missing"] = pd.crosstab(
+                    index, columns, values, aggfunc=utils.agg_missing
+                )
+        # pd.crosstab returns nan for an empty cell
+        for name, mask in masks.items():
+            mask.fillna(value=1, inplace=True)
+            mask = mask.astype(int)
+            mask.replace({0: False, 1: True}, inplace=True)
+            masks[name] = mask
 
         table, outcome = utils.apply_suppression(table, masks)
         summary = utils.get_summary(masks)
         self.__add_output(command, summary, outcome, [table])
         return table
 
     def pivot_table(  # pylint: disable=too-many-arguments,too-many-locals
@@ -371,14 +383,20 @@
                 masks["negative"] = negative
             # p-percent check
             agg = [utils.agg_p_percent] * n_agg if n_agg > 1 else utils.agg_p_percent
             masks["p-ratio"] = pd.pivot_table(data, values, index, columns, aggfunc=agg)
             # nk values check
             agg = [utils.agg_nk] * n_agg if n_agg > 1 else utils.agg_nk
             masks["nk-rule"] = pd.pivot_table(data, values, index, columns, aggfunc=agg)
+            # check for missing values -- currently unsupported
+            if utils.CHECK_MISSING_VALUES:
+                agg = [utils.agg_missing] * n_agg if n_agg > 1 else utils.agg_missing
+                masks["missing"] = pd.pivot_table(
+                    data, values, index, columns, aggfunc=agg
+                )
 
         table, outcome = utils.apply_suppression(table, masks)
         summary = utils.get_summary(masks)
         self.__add_output(command, summary, outcome, [table])
         return table
 
     def __check_model_dof(self, name: str, model) -> str:
```

### Comparing `acro-0.0.6/acro/default.yaml` & `acro-0.1.0/acro/default.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 # params for n, k tes: largest n values account for less than k% of the total
 safe_nk_n: 2
 safe_nk_k: 0.90
 
 # parameter for p-ration test: sum of smallest N-2 values accounts for at least
 # p% of largest
 safe_pratio_p: 0.10
+
+# refuse checking for missing values
+check_missing_values: False
 ...
```

### Comparing `acro-0.0.6/acro/utils.py` & `acro-0.1.0/acro/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,42 +78,36 @@
     except FileExistsError:
         logger.info("Directory %s already exists", OUTPUT_DIRECTORY)
 
     # convert dataframes to json
     for output_id, output in outputs.items():
         if output["outcome"] is not None:
             output["outcome"] = output["outcome"].to_json()
-
         # save each output to a different file
         if not isinstance(output["output"], str):
             with open(
                 OUTPUT_DIRECTORY + f"{output_id}.csv",
                 mode="w",
                 newline="",
                 encoding="utf-8",
             ) as file:
                 for i, _ in enumerate(output["output"]):
                     file.write(output["output"][i].to_csv())
+                    file.write("\n")
             output["output"] = os.path.abspath(f"{OUTPUT_DIRECTORY}{output_id}.csv")
 
-    # write to disk
+    data = outputs
+    # load existing results
     if os.path.isfile(OUTPUT_DIRECTORY + filename):
-        with open(
-            OUTPUT_DIRECTORY + filename, "r+", newline="", encoding="utf-8"
-        ) as file:
+        with open(OUTPUT_DIRECTORY + filename, newline="", encoding="utf-8") as file:
             data = json.load(file)
             data.update(outputs)
-            file.seek(0)
-            json.dump(data, file, indent=4, sort_keys=False)
-
-    else:
-        with open(
-            OUTPUT_DIRECTORY + filename, "w", newline="", encoding="utf-8"
-        ) as file:
-            json.dump(outputs, file, indent=4, sort_keys=False)
+    # write to disk
+    with open(OUTPUT_DIRECTORY + filename, "w", newline="", encoding="utf-8") as file:
+        json.dump(data, file, indent=4, sort_keys=False)
 
 
 def finalise_excel(filename: str, results: dict) -> None:
     """Writes outputs to an excel spreadsheet.
 
     Parameters
     ----------
@@ -201,14 +195,30 @@
     -------
     bool
         Whether a negative value was found.
     """
     return vals.min() < 0
 
 
+def agg_missing(vals: Series) -> bool:
+    """Aggregation function that returns whether any values are missing.
+
+    Parameters
+    ----------
+    vals : Series
+        Series to check for missing values.
+
+    Returns
+    -------
+    bool
+        Whether a missing value was found.
+    """
+    return vals.isna().sum() != 0
+
+
 def agg_p_percent(vals: Series) -> bool:
     """Aggregation function that returns whether the p percent rule is violated.
 
     That is, the uncertainty (as a fraction) of the estimate that the second
     highest respondent can make of the highest value. Assuming there are n
     items in the series, they are first sorted in descending order and then we
     calculate the value p = (sum - N-2 highest values)/highest value. If all
@@ -276,22 +286,29 @@
     safe_df = table.copy()
     outcome_df = DataFrame().reindex_like(table)
     outcome_df.fillna("", inplace=True)
     # don't apply suppression if negatives are present
     if "negative" in masks:
         mask = masks["negative"]
         outcome_df[mask.values] = "negative"
+    # don't apply suppression if missing values are present
+    elif "missing" in masks:
+        mask = masks["missing"]
+        outcome_df[mask.values] = "missing"
     # apply suppression masks
     else:
         for name, mask in masks.items():
-            safe_df[mask.values] = np.NaN
-            tmp_df = DataFrame().reindex_like(outcome_df)
-            tmp_df.fillna("", inplace=True)
-            tmp_df[mask.values] = name + "; "
-            outcome_df += tmp_df
+            try:
+                safe_df[mask.values] = np.NaN
+                tmp_df = DataFrame().reindex_like(outcome_df)
+                tmp_df.fillna("", inplace=True)
+                tmp_df[mask.values] = name + "; "
+                outcome_df += tmp_df
+            except TypeError:
+                logger.warning("problem mask %s is not binary", name)
         outcome_df = outcome_df.replace({"": "ok"})
     logger.info("outcome_df:\n%s", outcome_df)
     return safe_df, outcome_df
 
 
 def get_summary(masks: dict[str, DataFrame]) -> str:
     """Returns a string summarising the suppression masks.
@@ -305,14 +322,16 @@
     -------
     str
         Summary of the suppression masks.
     """
     summary: str = ""
     if "negative" in masks:
         summary = "review; negative values found"
+    elif "missing" in masks:
+        summary = "review; missing values found"
     else:
         for name, mask in masks.items():
             n_cells = mask.to_numpy().sum()
             if n_cells > 0:
                 summary += f"{name}: {n_cells} cells suppressed; "
         if summary == "":
             summary = "pass"
```

### Comparing `acro-0.0.6/acro.egg-info/PKG-INFO` & `acro-0.1.0/acro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.0.6
+Version: 0.1.0
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.0.6/setup.py` & `acro-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="acro",
-    version="0.0.6",
+    version="0.1.0",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="ACRO: Tools for the Automatic Checking of Research Outputs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/ACRO",
```

### Comparing `acro-0.0.6/test/test_initial.py` & `acro-0.1.0/test/test_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This module contains unit tests."""
 
 import json
 import os
 
+import numpy as np
 import pandas as pd
 import pytest
 
-from acro import ACRO, add_constant
+from acro import ACRO, add_constant, utils
 
 # pylint: disable=redefined-outer-name
 
 
 @pytest.fixture
 def data() -> pd.DataFrame:
     """Load test data."""
@@ -277,7 +278,35 @@
     """Adding an unsupported output to the results dictionary test"""
     filename = "XandY.jfif"
     file_path = os.path.abspath(filename)
     acro.custom_output(filename)
     output: dict = acro.finalise()
     output_0 = list(output.keys())[0]
     assert output[output_0]["output"] == file_path
+
+
+def test_missing(data, acro):
+    """Pivot table and Crosstab with negative values."""
+    utils.CHECK_MISSING_VALUES = True
+    data.loc[0:10, "inc_grants"] = np.NaN
+    _ = acro.crosstab(
+        data.year, data.grant_type, values=data.inc_grants, aggfunc="mean"
+    )
+    _ = acro.pivot_table(
+        data, index=["grant_type"], values=["inc_grants"], aggfunc=["mean", "std"]
+    )
+    output: dict = acro.finalise()
+    correct_summary: str = "review; missing values found"
+    output_0 = list(output.keys())[0]
+    output_1 = list(output.keys())[1]
+    assert output[output_0]["summary"] == correct_summary
+    assert output[output_1]["summary"] == correct_summary
+
+
+def test_suppression_error(caplog):
+    """Apply suppression type error test."""
+    table_data = {"col1": [1, 2], "col2": [3, 4]}
+    mask_data = {"col1": [np.NaN, True], "col2": [True, True]}
+    table = pd.DataFrame(data=table_data)
+    masks = {"test": pd.DataFrame(data=mask_data)}
+    utils.apply_suppression(table, masks)
+    assert "problem mask test is not binary" in caplog.text
```

