# Comparing `tmp/cluster_experiments-0.6.2.tar.gz` & `tmp/cluster_experiments-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.6.2.tar", last modified: Fri Apr 14 13:10:47 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.6.3.tar", last modified: Fri Apr 28 14:01:07 2023, max compression
```

## Comparing `cluster_experiments-0.6.2.tar` & `cluster_experiments-0.6.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.810590 cluster_experiments-0.6.2/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.2/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.2/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-14 13:10:47.809940 cluster_experiments-0.6.2/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.769650 cluster_experiments-0.6.2/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.2/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17228 2023-03-01 11:45:41.000000 cluster_experiments-0.6.2/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.2/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.2/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17759 2023-04-12 08:53:42.000000 cluster_experiments-0.6.2/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.2/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.775126 cluster_experiments-0.6.2/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1071 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-04-14 13:10:47.810785 cluster_experiments-0.6.2/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1133 2023-04-14 13:06:22.000000 cluster_experiments-0.6.2/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.780835 cluster_experiments-0.6.2/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.2/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.786200 cluster_experiments-0.6.2/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.2/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.790848 cluster_experiments-0.6.2/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 13:06:22.000000 cluster_experiments-0.6.2/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.2/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.792850 cluster_experiments-0.6.2/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.801560 cluster_experiments-0.6.2/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.2/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5239 2023-04-12 09:19:03.000000 cluster_experiments-0.6.2/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.2/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.808841 cluster_experiments-0.6.2/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.2/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.2/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.2/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.2/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1324 2022-10-21 09:42:28.000000 cluster_experiments-0.6.2/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.883882 cluster_experiments-0.6.3/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.3/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.3/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-28 14:01:07.883206 cluster_experiments-0.6.3/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-16 08:27:58.000000 cluster_experiments-0.6.3/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.807871 cluster_experiments-0.6.3/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.3/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.3/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.6.3/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.3/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.3/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17760 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.3/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.817867 cluster_experiments-0.6.3/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-04-28 14:01:07.000000 cluster_experiments-0.6.3/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-04-28 14:01:07.884106 cluster_experiments-0.6.3/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-04-28 14:00:38.000000 cluster_experiments-0.6.3/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.828481 cluster_experiments-0.6.3/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.3/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.833027 cluster_experiments-0.6.3/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.3/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.838031 cluster_experiments-0.6.3/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.6.3/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.3/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.841395 cluster_experiments-0.6.3/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.864424 cluster_experiments-0.6.3/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.3/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.6.3/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.3/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.3/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-28 14:01:07.881544 cluster_experiments-0.6.3/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-04-05 14:50:51.000000 cluster_experiments-0.6.3/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.3/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.3/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.3/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.3/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.3/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.3/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.3/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.6.3/tests/utils.py
```

### Comparing `cluster_experiments-0.6.2/LICENSE` & `cluster_experiments-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/README.md` & `cluster_experiments-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments/__init__.py` & `cluster_experiments-0.6.3/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments/cupac.py` & `cluster_experiments-0.6.3/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.6.3/cluster_experiments/experiment_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,27 @@
             cov_type=self.cov_type,
             cov_kwds={"groups": self._get_cluster_column(df)},
         )
         if verbose:
             print(results_ols.summary())
         return results_ols.pvalues[self.treatment_col]
 
+    def analysis_point_estimate(self, df: pd.DataFrame, verbose: bool = False) -> float:
+        """Returns the point estimate of the analysis
+        Arguments:
+            df: dataframe containing the data to analyze
+            verbose (Optional): bool, prints the regression summary if True
+        """
+        # Keep in mind that the point estimate of the OLS is the same as the ClusteredOLS
+        results_ols = sm.OLS.from_formula(
+            self.formula,
+            data=df,
+        ).fit()
+        return results_ols.params[self.treatment_col]
+
 
 class TTestClusteredAnalysis(ExperimentAnalysis):
     """
     Class to run T-test analysis on aggregated data
 
     Arguments:
         cluster_cols: list of columns to use as clusters
@@ -489,25 +502,38 @@
         self.target_col = target_col
         self.treatment = treatment
         self.treatment_col = treatment_col
         self.covariates = covariates or []
         self.regressors = [self.treatment_col] + self.covariates
         self.formula = f"{self.target_col} ~ {' + '.join(self.regressors)}"
 
+    def fit_ols(self, df: pd.DataFrame) -> sm.GEE:
+        """Returns the fitted OLS model"""
+        return sm.OLS.from_formula(self.formula, data=df).fit()
+
     def analysis_pvalue(self, df: pd.DataFrame, verbose: bool = False) -> float:
         """Returns the p-value of the analysis
         Arguments:
             df: dataframe containing the data to analyze
             verbose (Optional): bool, prints the regression summary if True
         """
-        results_ols = sm.OLS.from_formula(self.formula, data=df).fit()
+        results_ols = self.fit_ols(df=df)
         if verbose:
             print(results_ols.summary())
         return results_ols.pvalues[self.treatment_col]
 
+    def analysis_point_estimate(self, df: pd.DataFrame, verbose: bool = False) -> float:
+        """Returns the point estimate of the analysis
+        Arguments:
+            df: dataframe containing the data to analyze
+            verbose (Optional): bool, prints the regression summary if True
+        """
+        results_ols = self.fit_ols(df=df)
+        return results_ols.params[self.treatment_col]
+
     @classmethod
     def from_config(cls, config):
         """Creates an OLSAnalysis object from a PowerConfig object"""
         return cls(
             target_col=config.target_col,
             treatment_col=config.treatment_col,
             treatment=config.treatment,
```

### Comparing `cluster_experiments-0.6.2/cluster_experiments/perturbator.py` & `cluster_experiments-0.6.3/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments/power_analysis.py` & `cluster_experiments-0.6.3/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments/power_config.py` & `cluster_experiments-0.6.3/cluster_experiments/power_config.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments/random_splitter.py` & `cluster_experiments-0.6.3/cluster_experiments/random_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     """
     Splits randomly using clusters and time column
 
     It is a clustered splitter but one of the cluster columns is obtained by truncating the time column to the switch frequency.
 
     Arguments:
         time_col: Name of the column with the time variable.
-        switch_frequency: Frequency to switch treatments. Uses pandas frequency aliases: https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
+        switch_frequency: Frequency to switch treatments. Uses pandas frequency aliases (https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases)
         cluster_cols: List of columns to use as clusters
         treatments: list of treatments
         treatment_col: Name of the column with the treatment variable.
         splitter_weights: weights to use for the splitter, should have the same length as treatments, each weight should correspond to an element in treatments
 
     Usage:
     ```python
```

### Comparing `cluster_experiments-0.6.2/cluster_experiments/washover.py` & `cluster_experiments-0.6.3/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.6.3/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.6.3/cluster_experiments.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 scikit-learn>=1.0.0
 tqdm>=4.0.0
 numpy>=1.20.0
 
 [dev]
 pytest>=5.4.3
 black==22.12.0
-flake8>=3.8.3
+ruff==0.0.261
 mktestdocs>=0.2.0
 pytest-cov>=2.10.1
 pytest-sugar>=0.9.4
 pytest-slow-last>=0.1.3
 coverage
 pytest-reportlog
 pytest-duration-insights
+pytest-clarity
+pytest-xdist
 pip>=22.2.2
 statsmodels>=0.13.2
 pandas>=1.2.0
 scikit-learn>=1.0.0
 tqdm>=4.0.0
 numpy>=1.20.0
 pre-commit>=2.6.0
@@ -27,44 +29,52 @@
 twine
 tox
 mkdocs==1.3.0
 mkdocs-material==8.5.0
 mkdocstrings==0.18.0
 jinja2<3.1.0
 mkdocs-jupyter==0.22.0
+plotnine==0.8.0
+matplotlib==3.4.3
 
 [docs]
 mkdocs==1.3.0
 mkdocs-material==8.5.0
 mkdocstrings==0.18.0
 jinja2<3.1.0
 mkdocs-jupyter==0.22.0
+plotnine==0.8.0
+matplotlib==3.4.3
 
 [only-test]
 pytest>=5.4.3
 black==22.12.0
-flake8>=3.8.3
+ruff==0.0.261
 mktestdocs>=0.2.0
 pytest-cov>=2.10.1
 pytest-sugar>=0.9.4
 pytest-slow-last>=0.1.3
 coverage
 pytest-reportlog
 pytest-duration-insights
+pytest-clarity
+pytest-xdist
 
 [test]
 pytest>=5.4.3
 black==22.12.0
-flake8>=3.8.3
+ruff==0.0.261
 mktestdocs>=0.2.0
 pytest-cov>=2.10.1
 pytest-sugar>=0.9.4
 pytest-slow-last>=0.1.3
 coverage
 pytest-reportlog
 pytest-duration-insights
+pytest-clarity
+pytest-xdist
 pip>=22.2.2
 statsmodels>=0.13.2
 pandas>=1.2.0
 scikit-learn>=1.0.0
 tqdm>=4.0.0
 numpy>=1.20.0
```

### Comparing `cluster_experiments-0.6.2/setup.py` & `cluster_experiments-0.6.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,24 @@
     "tqdm>=4.0.0",
     "numpy>=1.20.0",
 ]
 
 only_test_packages = [
     "pytest>=5.4.3",
     "black==22.12.0",
-    "flake8>=3.8.3",
+    "ruff==0.0.261",
     "mktestdocs>=0.2.0",
     "pytest-cov>=2.10.1",
     "pytest-sugar>=0.9.4",
     "pytest-slow-last>=0.1.3",
     "coverage",
     "pytest-reportlog",
     "pytest-duration-insights",
+    "pytest-clarity",
+    "pytest-xdist",
 ]
 test_packages = only_test_packages + base_packages
 
 util_packages = [
     "pre-commit>=2.6.0",
     "ipykernel>=6.15.1",
     "twine",
@@ -32,21 +34,23 @@
 
 docs_packages = [
     "mkdocs==1.3.0",
     "mkdocs-material==8.5.0",
     "mkdocstrings==0.18.0",
     "jinja2<3.1.0",
     "mkdocs-jupyter==0.22.0",
+    "plotnine==0.8.0",
+    "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.6.2",
+    version="0.6.3",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.6.2/tests/analysis/test_analysis.py` & `cluster_experiments-0.6.3/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/cupac/test_aggregator.py` & `cluster_experiments-0.6.3/tests/cupac/test_aggregator.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 
 import pandas as pd
-from cluster_experiments.cupac import TargetAggregation
 
+from cluster_experiments.cupac import TargetAggregation
 from tests.examples import binary_df
 
 
 def split_x_y(binary_df: pd.DataFrame) -> Tuple[pd.DataFrame, pd.Series]:
     return binary_df.drop("target", axis=1), binary_df["target"]
```

### Comparing `cluster_experiments-0.6.2/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.6.3/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/examples.py` & `cluster_experiments-0.6.3/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.6.3/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/conftest.py` & `cluster_experiments-0.6.3/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.6.3/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.6.3/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.6.3/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.6.3/tests/power_analysis/test_power_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -160,26 +160,55 @@
     pw = PowerAnalysis.from_config(config)
     i = 0
     for _ in pw.simulate_pvalue(df, n_simulations=5):
         i += 1
     assert i == 5
 
 
-def test_point_estimates(df):
+def test_point_estimate_gee(df):
     config = PowerConfig(
         cluster_cols=["cluster", "date"],
         analysis="gee",
         perturbator="uniform",
         splitter="clustered",
         n_simulations=10,
         average_effect=5.0,
         alpha=0.05,
     )
     pw = PowerAnalysis.from_config(config)
-    for point_estimate in pw.simulate_point_estimate(df, n_simulations=5):
+    for point_estimate in pw.simulate_point_estimate(df, n_simulations=1):
+        assert point_estimate > 0.0
+
+
+def test_point_estimate_clustered_ols(df):
+    config = PowerConfig(
+        cluster_cols=["cluster", "date"],
+        analysis="ols_clustered",
+        perturbator="uniform",
+        splitter="clustered",
+        n_simulations=10,
+        average_effect=5.0,
+        alpha=0.05,
+    )
+    pw = PowerAnalysis.from_config(config)
+    for point_estimate in pw.simulate_point_estimate(df, n_simulations=1):
+        assert point_estimate > 0.0
+
+
+def test_point_estimate_ols(df):
+    config = PowerConfig(
+        analysis="ols_non_clustered",
+        perturbator="uniform",
+        splitter="non_clustered",
+        n_simulations=10,
+        average_effect=5.0,
+        alpha=0.05,
+    )
+    pw = PowerAnalysis.from_config(config)
+    for point_estimate in pw.simulate_point_estimate(df, n_simulations=1):
         assert point_estimate > 0.0
 
 
 def test_power_line(df):
     config = PowerConfig(
         analysis="ols_non_clustered",
         perturbator="uniform",
```

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.6.3/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.6.3/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/splitter/conftest.py` & `cluster_experiments-0.6.3/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/splitter/test_splitter.py` & `cluster_experiments-0.6.3/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.6.3/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/splitter/test_time_col.py` & `cluster_experiments-0.6.3/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/splitter/test_washover.py` & `cluster_experiments-0.6.3/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/test_docs.py` & `cluster_experiments-0.6.3/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/test_non_clustered.py` & `cluster_experiments-0.6.3/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.2/tests/utils.py` & `cluster_experiments-0.6.3/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 
 import pandas as pd
+
 from cluster_experiments.random_splitter import RandomSplitter
 
 
 def combine_columns(df, cols_list):
     # combines columns for testing the stratified splitter in case of multiple strata or clusters
     if len(cols_list) > 1:
         return df[cols_list].agg("-".join, axis=1)
```

