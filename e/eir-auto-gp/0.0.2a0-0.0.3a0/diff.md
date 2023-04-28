# Comparing `tmp/eir_auto_gp-0.0.2a0.tar.gz` & `tmp/eir_auto_gp-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eir_auto_gp-0.0.2a0.tar", max compression
+gzip compressed data, was "eir_auto_gp-0.0.3a0.tar", max compression
```

## Comparing `eir_auto_gp-0.0.2a0.tar` & `eir_auto_gp-0.0.3a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34523 2023-04-03 12:29:50.425420 eir_auto_gp-0.0.2a0/LICENSE
--rw-r--r--   0        0        0     3646 2023-04-03 12:29:50.425420 eir_auto_gp-0.0.2a0/README.md
--rw-r--r--   0        0        0        0 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/analysis/__init__.py
--rw-r--r--   0        0        0    15616 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/analysis/run_analysis.py
--rw-r--r--   0        0        0        0 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/__init__.py
--rw-r--r--   0        0        0     4051 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/configs.py
--rw-r--r--   0        0        0     9831 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/dl_feature_selection.py
--rw-r--r--   0        0        0     4568 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/gwas_feature_selection.py
--rw-r--r--   0        0        0    22261 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/run_modelling.py
--rw-r--r--   0        0        0        0 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/common.py
--rw-r--r--   0        0        0    13889 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/converge.py
--rw-r--r--   0        0        0     4024 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/genotype.py
--rw-r--r--   0        0        0    17349 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/gwas_pre_selection.py
--rw-r--r--   0        0        0     1286 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/tabular.py
--rw-r--r--   0        0        0    15604 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/run.py
--rw-r--r--   0        0        0        0 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/eir_auto_gp/utils/utils.py
--rw-r--r--   0        0        0      863 2023-04-03 12:29:50.433420 eir_auto_gp-0.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     4701 1970-01-01 00:00:00.000000 eir_auto_gp-0.0.2a0/setup.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 eir_auto_gp-0.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-28 15:05:51.356097 eir_auto_gp-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0     3808 2023-04-28 15:05:51.356097 eir_auto_gp-0.0.3a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/analysis/__init__.py
+-rw-r--r--   0        0        0    15616 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/analysis/run_analysis.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/__init__.py
+-rw-r--r--   0        0        0     4051 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/configs.py
+-rw-r--r--   0        0        0    13841 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/dl_feature_selection.py
+-rw-r--r--   0        0        0     4568 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/gwas_feature_selection.py
+-rw-r--r--   0        0        0    22272 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/run_modelling.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/common.py
+-rw-r--r--   0        0        0    14349 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/converge.py
+-rw-r--r--   0        0        0     4024 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/genotype.py
+-rw-r--r--   0        0        0    17378 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/gwas_pre_selection.py
+-rw-r--r--   0        0        0     1286 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/tabular.py
+-rw-r--r--   0        0        0    15845 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/run.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-28 15:05:51.364097 eir_auto_gp-0.0.3a0/eir_auto_gp/utils/utils.py
+-rw-r--r--   0        0        0      863 2023-04-28 15:05:51.368098 eir_auto_gp-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 eir_auto_gp-0.0.3a0/setup.py
+-rw-r--r--   0        0        0     4274 1970-01-01 00:00:00.000000 eir_auto_gp-0.0.3a0/PKG-INFO
```

### Comparing `eir_auto_gp-0.0.2a0/LICENSE` & `eir_auto_gp-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `eir_auto_gp-0.0.2a0/README.md` & `eir_auto_gp-0.0.3a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # EIR-auto-GP
 
 <p align="center">
-  <img src="docs/source/_static/img/eir-auto-gp-logo.svg" alt="Eir Auto GP Logo">
+  <img src="docs/source/_static/img/eir-auto-gp-logo.svg" alt="EIR auto GP Logo">
 </p>
 
 <p align="center">
   <a href="LICENSE" alt="License">
         <img src="https://img.shields.io/badge/License-APGL-5B2D5B.svg" />
   </a>
   
@@ -54,14 +54,20 @@
 
 ## Usage
 
 Please refer to the [Documentation](https://eir-auto-gp.readthedocs.io/en/latest/) for examples and information.
 
 ## Workflow
 
+The rough workflow can be visualized as follows:
+
+<p align="center">
+  <img src="docs/source/_static/img/eir_auto_gp.svg" alt="EIR auto GP Workflow">
+</p>
+
 1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK files and `.csv` label file, preparing the data for model training and evaluation.
 2. Train/test split: The processed data is automatically split into training and testing sets, with the option of manually specifying splits.
 3. Training: Configurable number of training runs are set up and executed using EIR's deep learning models.
 4. SNP feature selection: GWAS based feature selection, deep learning-based feature selection with Bayesian optimization, and mixed strategies are supported.
 5. Test set prediction: Predictions are made on the test set using all training run folds.
 6. Ensemble prediction: An ensemble prediction is created from the individual predictions.
 7. Results analysis: Performance metrics, visualizations, and analysis are generated to assess the model's performance.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # EIR-auto-GP
-                              [Eir Auto GP Logo]
+                              [EIR auto GP Logo]
 [https://img.shields.io/badge/License-APGL-5B2D5B.svg] [https://img.shields.io/
  badge/python-3.10-blue.svg] [https://img.shields.io/pypi/v/eir-auto-gp.svg]
    [https://codecov.io/gh/arnor-sigurdsson/EIR-auto-GP/branch/master/graph/
               badge.svg?token=PODL2J83Y0] [Documentation_Status]
 `EIR-auto-GP`: Automated genomic prediction (GP) using deep learning models
 with EIR. **WARNING**: This project is in alpha phase. Expect backwards
 incompatible changes and API changes. ## Overview EIR-auto-GP is a
@@ -16,26 +16,28 @@
 Takes care of launching a configurable number of deep learning training runs. -
 SNP-based feature selection based on GWAS, deep learning-based attributions,
 and a combination of both. - Ensemble prediction from multiple training runs. -
 Analysis and visualization of results. ## Installation First, ensure that
 [plink2](https://www.cog-genomics.org/plink/2.0/) is installed and available in
 your `PATH`. Then, install `EIR-auto-GP` using `pip`: `pip install eir-auto-gp`
 ## Usage Please refer to the [Documentation](https://eir-auto-
-gp.readthedocs.io/en/latest/) for examples and information. ## Workflow 1. Data
-processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK files and
-`.csv` label file, preparing the data for model training and evaluation. 2.
-Train/test split: The processed data is automatically split into training and
-testing sets, with the option of manually specifying splits. 3. Training:
-Configurable number of training runs are set up and executed using EIR's deep
-learning models. 4. SNP feature selection: GWAS based feature selection, deep
-learning-based feature selection with Bayesian optimization, and mixed
-strategies are supported. 5. Test set prediction: Predictions are made on the
-test set using all training run folds. 6. Ensemble prediction: An ensemble
-prediction is created from the individual predictions. 7. Results analysis:
-Performance metrics, visualizations, and analysis are generated to assess the
-model's performance. ## Citation If you use `EIR-auto-GP` in a scientific
-publication, we would appreciate if you could use the following citation: ```
-@article{sigurdsson2021deep, title={Deep integrative models for large-scale
-human genomics}, author={Sigurdsson, Arnor Ingi and Westergaard, David and
-Winther, Ole and Lund, Ole and Brunak, S{\o}ren and Vilhjalmsson, Bjarni J and
-Rasmussen, Simon}, journal={bioRxiv}, year={2021}, publisher={Cold Spring
-Harbor Laboratory} } ```
+gp.readthedocs.io/en/latest/) for examples and information. ## Workflow The
+rough workflow can be visualized as follows:
+                            [EIR auto GP Workflow]
+1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK
+files and `.csv` label file, preparing the data for model training and
+evaluation. 2. Train/test split: The processed data is automatically split into
+training and testing sets, with the option of manually specifying splits. 3.
+Training: Configurable number of training runs are set up and executed using
+EIR's deep learning models. 4. SNP feature selection: GWAS based feature
+selection, deep learning-based feature selection with Bayesian optimization,
+and mixed strategies are supported. 5. Test set prediction: Predictions are
+made on the test set using all training run folds. 6. Ensemble prediction: An
+ensemble prediction is created from the individual predictions. 7. Results
+analysis: Performance metrics, visualizations, and analysis are generated to
+assess the model's performance. ## Citation If you use `EIR-auto-GP` in a
+scientific publication, we would appreciate if you could use the following
+citation: ``` @article{sigurdsson2021deep, title={Deep integrative models for
+large-scale human genomics}, author={Sigurdsson, Arnor Ingi and Westergaard,
+David and Winther, Ole and Lund, Ole and Brunak, S{\o}ren and Vilhjalmsson,
+Bjarni J and Rasmussen, Simon}, journal={bioRxiv}, year={2021}, publisher={Cold
+Spring Harbor Laboratory} } ```
```

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/analysis/run_analysis.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/analysis/run_analysis.py`

 * *Files identical despite different names*

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/configs.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/configs.py`

 * *Files identical despite different names*

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/gwas_feature_selection.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/gwas_feature_selection.py`

 * *Files identical despite different names*

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/modelling/run_modelling.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/modelling/run_modelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
     feature_selection_config: Dict[str, Any],
     modelling_config: Dict[str, Any],
 ) -> ModelInjectionParams:
     compute_attributions = False
 
     fs = feature_selection_config["feature_selection"]
     n_act_folds = feature_selection_config["n_dl_feature_selection_setup_folds"]
-    if task == "train" and fs in ("dl", "gwas->dl") and fold < n_act_folds:
+    if task == "train" and fs in ("dl", "gwas->dl", "dl+gwas") and fold < n_act_folds:
         compute_attributions = True
 
     weighted_sampling_columns = None
     if modelling_config["output_cat_columns"]:
         weighted_sampling_columns = ["all"]
 
     feature_selection_tasks = feature_selection_config["feature_selection"]
```

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/converge.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/converge.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     genotype_data_path = luigi.Parameter()
     label_file_path = luigi.Parameter()
     data_output_folder = luigi.Parameter()
     output_format = luigi.Parameter()
     output_name = luigi.Parameter()
     pre_split_folder = luigi.Parameter()
     freeze_validation_set = luigi.BoolParameter()
-    only_data = luigi.Parameter()
+    only_data = luigi.BoolParameter()
 
     def requires(self):
         """
         Will require 3 tasks:
             - genotype processing,
             - label file processing.
 
@@ -166,14 +166,17 @@
 
 def _id_setup_wrapper(
     output_root: Path,
     common_ids_to_keep: Sequence[str],
     freeze_validation_set: bool,
     pre_split_folder: Optional[str] = None,
 ):
+    valid_path = None
+    valid_path_exists = False
+
     if pre_split_folder is not None:
         pre_split_folder = Path(pre_split_folder)
         logger.info("Using pre-split folder: %s", pre_split_folder)
 
         train_path = pre_split_folder / "train_ids.txt"
         if not train_path.exists():
             raise FileNotFoundError(f"Could not find train IDs file: {train_path}")
@@ -187,33 +190,43 @@
         )
 
         test_ids = (
             pd.read_csv(test_path, header=None).astype(str).squeeze("columns").tolist()
         )
 
         valid_path = pre_split_folder / "valid_ids.txt"
-        freeze_validation_set = valid_path.exists() and freeze_validation_set
+        valid_path_exists = valid_path.exists()
 
     else:
         logger.info("Generating train+valid and test IDs.")
 
         train_ids, test_ids = _split_ids(all_ids=common_ids_to_keep)
 
     valid_ids = []
     if freeze_validation_set:
-        logger.info("Creating new frozen validation set.")
+        if not valid_path_exists:
+            logger.info("Creating new frozen validation set.")
+
+            batch_size = get_batch_size(samples_per_epoch=len(train_ids))
+            valid_size = get_dynamic_valid_size(
+                num_samples_per_epoch=len(train_ids),
+                batch_size=batch_size,
+            )
+            train_ids, valid_ids = _split_ids(
+                all_ids=train_ids, valid_or_test_size=valid_size
+            )
+        else:
+            logger.info("Using frozen validation set from %s.", valid_path)
+            valid_ids = (
+                pd.read_csv(valid_path, header=None)
+                .astype(str)
+                .squeeze("columns")
+                .tolist()
+            )
 
-        batch_size = get_batch_size(samples_per_epoch=len(train_ids))
-        valid_size = get_dynamic_valid_size(
-            num_samples_per_epoch=len(train_ids),
-            batch_size=batch_size,
-        )
-        train_ids, valid_ids = _split_ids(
-            all_ids=train_ids, valid_or_test_size=valid_size
-        )
         _save_ids_to_text_file(
             ids=valid_ids, path=output_root / "ids" / "valid_ids.txt"
         )
 
     _save_ids_to_text_file(ids=train_ids, path=output_root / "ids" / "train_ids.txt")
     _save_ids_to_text_file(ids=test_ids, path=output_root / "ids" / "test_ids.txt")
 
@@ -248,17 +261,21 @@
             len(all_ids) - len(common_ids),
         )
         return list(common_ids)
 
     return list(all_ids)
 
 
-def gather_ids_from_csv_file(file_path: Path):
+def gather_ids_from_csv_file(file_path: Path, drop_nas: bool = False):
     logger.debug("Gathering IDs from %s.", file_path)
-    df = pd.read_csv(file_path, usecols=["ID"])
+    df = pd.read_csv(filepath_or_buffer=file_path)
+
+    if drop_nas:
+        df = df.dropna(how="any", axis=0)
+
     all_ids = tuple(df["ID"].astype(str))
 
     return all_ids
 
 
 def _split_ids(
     all_ids: Sequence[str], valid_or_test_size: float | int = 0.1
```

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/genotype.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/genotype.py`

 * *Files identical despite different names*

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/gwas_pre_selection.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/gwas_pre_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,17 @@
     return snps_to_keep
 
 
 def gather_all_ids(fam_file_path: str | Path, label_file_path: str | Path) -> list[str]:
     df_fam = _read_fam(fam_path=fam_file_path)
     genotype_ids = set(df_fam[1].astype(str))
 
-    labelled_ids = set(gather_ids_from_csv_file(file_path=label_file_path))
+    labelled_ids = set(
+        gather_ids_from_csv_file(file_path=label_file_path, drop_nas=True)
+    )
 
     common_ids_to_keep = set().union(genotype_ids, labelled_ids)
     common_ids = genotype_ids.intersection(labelled_ids)
 
     logger.info(
         "Keeping %d common IDs among %d total (difference: %d).",
         len(common_ids),
```

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/preprocess/tabular.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/preprocess/tabular.py`

 * *Files identical despite different names*

### Comparing `eir_auto_gp-0.0.2a0/eir_auto_gp/run.py` & `eir_auto_gp-0.0.3a0/eir_auto_gp/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         dest="freeze_validation_set",
         action="store_false",
     )
 
     parser.add_argument(
         "--feature_selection",
         default="gwas->dl",
-        choices=["dl", "gwas", "gwas->dl", None],
+        choices=["dl", "gwas", "gwas->dl", "dl+gwas", None],
         required=False,
         help="What kind of feature selection strategy to use for SNP selection:\n"
         "  - If None, no feature selection is performed.\n"
         "  - If 'dl', feature selection is performed using DL feature importance,\n"
         "    and the top SNPs are selected iteratively using Bayesian optimization.\n"
         "  - If 'gwas', feature selection is performed using GWAS p-values,\n"
         "    as specified by the --gwas_p_value_threshold parameter.\n"
@@ -405,19 +405,28 @@
     return cl_args_copy
 
 
 def _add_pre_split_folder_if_present(cl_args: argparse.Namespace) -> argparse.Namespace:
     cl_args_copy = copy(cl_args)
     genotype_path = Path(cl_args_copy.genotype_data_path)
 
-    if (genotype_path / "ids").exists():
+    id_path = genotype_path / "ids"
+    if id_path.exists():
         cl_args_copy.pre_split_folder = str(genotype_path / "ids")
+
+        found_files = [
+            i.name
+            for i in id_path.iterdir()
+            if i.is_file() and i.name.endswith(".txt") and "_plink" not in i.name
+        ]
+
         logger.info(
-            f"Found pre-split folder {cl_args_copy.pre_split_folder}. "
-            f"in root genotype folder. Using those for train/test split."
+            f"Found pre-split folder '{cl_args_copy.pre_split_folder}'. "
+            f"in root genotype folder. "
+            f"Using files: {found_files} for respective splits."
         )
 
     return cl_args_copy
 
 
 def build_data_config(cl_args: argparse.Namespace) -> Dict[str, Any]:
     data_keys = [
```

### Comparing `eir_auto_gp-0.0.2a0/pyproject.toml` & `eir_auto_gp-0.0.3a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "EIR-auto-GP"
-version = "0.0.2-alpha"
+version = "0.0.3-alpha"
 description = ""
 authors = ["Arnor Sigurdsson <arnor-sigurdsson@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "eir_auto_gp"}]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
```

### Comparing `eir_auto_gp-0.0.2a0/setup.py` & `eir_auto_gp-0.0.3a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 entry_points = \
 {'console_scripts': ['eirautogp = eir_auto_gp.run:main',
                      'eirautogwas = '
                      'eir_auto_gp.preprocess.gwas_pre_selection:main']}
 
 setup_kwargs = {
     'name': 'eir-auto-gp',
-    'version': '0.0.2a0',
+    'version': '0.0.3a0',
     'description': '',
-    'long_description': '# EIR-auto-GP\n\n<p align="center">\n  <img src="docs/source/_static/img/eir-auto-gp-logo.svg" alt="Eir Auto GP Logo">\n</p>\n\n<p align="center">\n  <a href="LICENSE" alt="License">\n        <img src="https://img.shields.io/badge/License-APGL-5B2D5B.svg" />\n  </a>\n  \n  <a href="https://www.python.org/downloads/" alt="Python">\n        <img src="https://img.shields.io/badge/python-3.10-blue.svg" />\n  </a>\n  \n  <a href="https://pypi.org/project/eir-auto-gp/" alt="Python">\n        <img src="https://img.shields.io/pypi/v/eir-auto-gp.svg" />\n  </a>\n  \n  \n  <a href="https://codecov.io/gh/arnor-sigurdsson/EIR-auto-GP" > \n        <img src="https://codecov.io/gh/arnor-sigurdsson/EIR-auto-GP/branch/master/graph/badge.svg?token=PODL2J83Y0"/> \n  </a>\n  \n  <a href=\'https://eir-auto-gp.readthedocs.io\'>\n    <img src=\'https://readthedocs.org/projects/eir-auto-gp/badge/?version=latest\' alt=\'Documentation Status\' />\n  </a>\n      \n  \n</p>\n\n`EIR-auto-GP`: Automated genomic prediction (GP) using deep learning models with EIR.\n\n**WARNING**: This project is in alpha phase. Expect backwards incompatible changes and API changes.\n\n## Overview\n\nEIR-auto-GP is a comprehensive framework for genomic prediction (GP) tasks, built on top of the [EIR](https://github.com/arnor-sigurdsson/EIR) deep learning framework. EIR-auto-GP streamlines the process of preparing data, training, and evaluating models on genomic data, automating much of the process from raw input files to results analysis. Key features include:\n\n- Support for `.bed/.bim/.fam` PLINK files as input data.\n- Automated data processing and train/test splitting.\n- Takes care of launching a configurable number of deep learning training runs.\n- SNP-based feature selection based on GWAS, deep learning-based attributions, and a combination of both.\n- Ensemble prediction from multiple training runs.\n- Analysis and visualization of results.\n\n## Installation\n\nFirst, ensure that [plink2](https://www.cog-genomics.org/plink/2.0/) is installed and available in your `PATH`. \n\nThen, install `EIR-auto-GP` using `pip`:\n\n`pip install eir-auto-gp`\n\n## Usage\n\nPlease refer to the [Documentation](https://eir-auto-gp.readthedocs.io/en/latest/) for examples and information.\n\n## Workflow\n\n1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK files and `.csv` label file, preparing the data for model training and evaluation.\n2. Train/test split: The processed data is automatically split into training and testing sets, with the option of manually specifying splits.\n3. Training: Configurable number of training runs are set up and executed using EIR\'s deep learning models.\n4. SNP feature selection: GWAS based feature selection, deep learning-based feature selection with Bayesian optimization, and mixed strategies are supported.\n5. Test set prediction: Predictions are made on the test set using all training run folds.\n6. Ensemble prediction: An ensemble prediction is created from the individual predictions.\n7. Results analysis: Performance metrics, visualizations, and analysis are generated to assess the model\'s performance.\n\n## Citation\n\nIf you use `EIR-auto-GP` in a scientific publication, we would appreciate if you could use the following citation:\n\n```\n@article{sigurdsson2021deep,\n  title={Deep integrative models for large-scale human genomics},\n  author={Sigurdsson, Arnor Ingi and Westergaard, David and Winther, Ole and Lund, Ole and Brunak, S{\\o}ren and Vilhjalmsson, Bjarni J and Rasmussen, Simon},\n  journal={bioRxiv},\n  year={2021},\n  publisher={Cold Spring Harbor Laboratory}\n}\n```\n',
+    'long_description': '# EIR-auto-GP\n\n<p align="center">\n  <img src="docs/source/_static/img/eir-auto-gp-logo.svg" alt="EIR auto GP Logo">\n</p>\n\n<p align="center">\n  <a href="LICENSE" alt="License">\n        <img src="https://img.shields.io/badge/License-APGL-5B2D5B.svg" />\n  </a>\n  \n  <a href="https://www.python.org/downloads/" alt="Python">\n        <img src="https://img.shields.io/badge/python-3.10-blue.svg" />\n  </a>\n  \n  <a href="https://pypi.org/project/eir-auto-gp/" alt="Python">\n        <img src="https://img.shields.io/pypi/v/eir-auto-gp.svg" />\n  </a>\n  \n  \n  <a href="https://codecov.io/gh/arnor-sigurdsson/EIR-auto-GP" > \n        <img src="https://codecov.io/gh/arnor-sigurdsson/EIR-auto-GP/branch/master/graph/badge.svg?token=PODL2J83Y0"/> \n  </a>\n  \n  <a href=\'https://eir-auto-gp.readthedocs.io\'>\n    <img src=\'https://readthedocs.org/projects/eir-auto-gp/badge/?version=latest\' alt=\'Documentation Status\' />\n  </a>\n      \n  \n</p>\n\n`EIR-auto-GP`: Automated genomic prediction (GP) using deep learning models with EIR.\n\n**WARNING**: This project is in alpha phase. Expect backwards incompatible changes and API changes.\n\n## Overview\n\nEIR-auto-GP is a comprehensive framework for genomic prediction (GP) tasks, built on top of the [EIR](https://github.com/arnor-sigurdsson/EIR) deep learning framework. EIR-auto-GP streamlines the process of preparing data, training, and evaluating models on genomic data, automating much of the process from raw input files to results analysis. Key features include:\n\n- Support for `.bed/.bim/.fam` PLINK files as input data.\n- Automated data processing and train/test splitting.\n- Takes care of launching a configurable number of deep learning training runs.\n- SNP-based feature selection based on GWAS, deep learning-based attributions, and a combination of both.\n- Ensemble prediction from multiple training runs.\n- Analysis and visualization of results.\n\n## Installation\n\nFirst, ensure that [plink2](https://www.cog-genomics.org/plink/2.0/) is installed and available in your `PATH`. \n\nThen, install `EIR-auto-GP` using `pip`:\n\n`pip install eir-auto-gp`\n\n## Usage\n\nPlease refer to the [Documentation](https://eir-auto-gp.readthedocs.io/en/latest/) for examples and information.\n\n## Workflow\n\nThe rough workflow can be visualized as follows:\n\n<p align="center">\n  <img src="docs/source/_static/img/eir_auto_gp.svg" alt="EIR auto GP Workflow">\n</p>\n\n1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK files and `.csv` label file, preparing the data for model training and evaluation.\n2. Train/test split: The processed data is automatically split into training and testing sets, with the option of manually specifying splits.\n3. Training: Configurable number of training runs are set up and executed using EIR\'s deep learning models.\n4. SNP feature selection: GWAS based feature selection, deep learning-based feature selection with Bayesian optimization, and mixed strategies are supported.\n5. Test set prediction: Predictions are made on the test set using all training run folds.\n6. Ensemble prediction: An ensemble prediction is created from the individual predictions.\n7. Results analysis: Performance metrics, visualizations, and analysis are generated to assess the model\'s performance.\n\n## Citation\n\nIf you use `EIR-auto-GP` in a scientific publication, we would appreciate if you could use the following citation:\n\n```\n@article{sigurdsson2021deep,\n  title={Deep integrative models for large-scale human genomics},\n  author={Sigurdsson, Arnor Ingi and Westergaard, David and Winther, Ole and Lund, Ole and Brunak, S{\\o}ren and Vilhjalmsson, Bjarni J and Rasmussen, Simon},\n  journal={bioRxiv},\n  year={2021},\n  publisher={Cold Spring Harbor Laboratory}\n}\n```\n',
     'author': 'Arnor Sigurdsson',
     'author_email': 'arnor-sigurdsson@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -2,17 +2,17 @@
 ['eir_auto_gp', 'eir_auto_gp.analysis', 'eir_auto_gp.modelling',
 'eir_auto_gp.preprocess', 'eir_auto_gp.utils'] package_data = \ {'': ['*']}
 install_requires = \ ['eir-dl>=0.1.31a0,<0.2.0', 'plink-
 pipelines>=0.1.5a0,<0.2.0', 'qmplot>=0.3.2,<0.4.0', 'scikit-
 optimize>=0.9.0,<0.10.0'] entry_points = \ {'console_scripts': ['eirautogp =
 eir_auto_gp.run:main', 'eirautogwas = '
 'eir_auto_gp.preprocess.gwas_pre_selection:main']} setup_kwargs = { 'name':
-'eir-auto-gp', 'version': '0.0.2a0', 'description': '', 'long_description': '#
+'eir-auto-gp', 'version': '0.0.3a0', 'description': '', 'long_description': '#
 EIR-auto-GP\n\n
-                            \n [Eir Auto GP Logo]\n
+                            \n [EIR auto GP Logo]\n
 \n\n
 \n \n_[https://img.shields.io/badge/License-APGL-5B2D5B.svg]\n\n \n \n_[https:/
 /img.shields.io/badge/python-3.10-blue.svg]\n\n \n \n_[https://img.shields.io/
  pypi/v/eir-auto-gp.svg]\n\n \n \n \n_[https://codecov.io/gh/arnor-sigurdsson/
 EIR-auto-GP/branch/master/graph/badge.svg?token=PODL2J83Y0]_\n\n \n \n_'_/>\n\n
                                      \n \n
 \n\n`EIR-auto-GP`: Automated genomic prediction (GP) using deep learning models
@@ -28,31 +28,33 @@
 runs.\n- SNP-based feature selection based on GWAS, deep learning-based
 attributions, and a combination of both.\n- Ensemble prediction from multiple
 training runs.\n- Analysis and visualization of results.\n\n##
 Installation\n\nFirst, ensure that [plink2](https://www.cog-genomics.org/plink/
 2.0/) is installed and available in your `PATH`. \n\nThen, install `EIR-auto-
 GP` using `pip`:\n\n`pip install eir-auto-gp`\n\n## Usage\n\nPlease refer to
 the [Documentation](https://eir-auto-gp.readthedocs.io/en/latest/) for examples
-and information.\n\n## Workflow\n\n1. Data processing: EIR-auto-GP processes
-the input `.bed/.bim/.fam` PLINK files and `.csv` label file, preparing the
-data for model training and evaluation.\n2. Train/test split: The processed
-data is automatically split into training and testing sets, with the option of
-manually specifying splits.\n3. Training: Configurable number of training runs
-are set up and executed using EIR\'s deep learning models.\n4. SNP feature
-selection: GWAS based feature selection, deep learning-based feature selection
-with Bayesian optimization, and mixed strategies are supported.\n5. Test set
-prediction: Predictions are made on the test set using all training run
-folds.\n6. Ensemble prediction: An ensemble prediction is created from the
-individual predictions.\n7. Results analysis: Performance metrics,
-visualizations, and analysis are generated to assess the model\'s
-performance.\n\n## Citation\n\nIf you use `EIR-auto-GP` in a scientific
-publication, we would appreciate if you could use the following citation:
-\n\n```\n@article{sigurdsson2021deep,\n title={Deep integrative models for
-large-scale human genomics},\n author={Sigurdsson, Arnor Ingi and Westergaard,
-David and Winther, Ole and Lund, Ole and Brunak, S{\\o}ren and Vilhjalmsson,
-Bjarni J and Rasmussen, Simon},\n journal={bioRxiv},\n year={2021},\n
-publisher={Cold Spring Harbor Laboratory}\n}\n```\n', 'author': 'Arnor
-Sigurdsson', 'author_email': 'arnor-sigurdsson@users.noreply.github.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.10.0,<4.0.0', } setup
-(**setup_kwargs)
+and information.\n\n## Workflow\n\nThe rough workflow can be visualized as
+follows:\n\n
+                          \n [EIR auto GP Workflow]\n
+\n\n1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK
+files and `.csv` label file, preparing the data for model training and
+evaluation.\n2. Train/test split: The processed data is automatically split
+into training and testing sets, with the option of manually specifying
+splits.\n3. Training: Configurable number of training runs are set up and
+executed using EIR\'s deep learning models.\n4. SNP feature selection: GWAS
+based feature selection, deep learning-based feature selection with Bayesian
+optimization, and mixed strategies are supported.\n5. Test set prediction:
+Predictions are made on the test set using all training run folds.\n6. Ensemble
+prediction: An ensemble prediction is created from the individual
+predictions.\n7. Results analysis: Performance metrics, visualizations, and
+analysis are generated to assess the model\'s performance.\n\n## Citation\n\nIf
+you use `EIR-auto-GP` in a scientific publication, we would appreciate if you
+could use the following citation:\n\n```\n@article{sigurdsson2021deep,\n title=
+{Deep integrative models for large-scale human genomics},\n author={Sigurdsson,
+Arnor Ingi and Westergaard, David and Winther, Ole and Lund, Ole and Brunak, S
+{\\o}ren and Vilhjalmsson, Bjarni J and Rasmussen, Simon},\n journal=
+{bioRxiv},\n year={2021},\n publisher={Cold Spring Harbor
+Laboratory}\n}\n```\n', 'author': 'Arnor Sigurdsson', 'author_email': 'arnor-
+sigurdsson@users.noreply.github.com', 'maintainer': 'None', 'maintainer_email':
+'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'entry_points': entry_points,
+'python_requires': '>=3.10.0,<4.0.0', } setup(**setup_kwargs)
```

### Comparing `eir_auto_gp-0.0.2a0/PKG-INFO` & `eir_auto_gp-0.0.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eir-auto-gp
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: 
 Author: Arnor Sigurdsson
 Author-email: arnor-sigurdsson@users.noreply.github.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,15 +13,15 @@
 Requires-Dist: qmplot (>=0.3.2,<0.4.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # EIR-auto-GP
 
 <p align="center">
-  <img src="docs/source/_static/img/eir-auto-gp-logo.svg" alt="Eir Auto GP Logo">
+  <img src="docs/source/_static/img/eir-auto-gp-logo.svg" alt="EIR auto GP Logo">
 </p>
 
 <p align="center">
   <a href="LICENSE" alt="License">
         <img src="https://img.shields.io/badge/License-APGL-5B2D5B.svg" />
   </a>
   
@@ -70,14 +70,20 @@
 
 ## Usage
 
 Please refer to the [Documentation](https://eir-auto-gp.readthedocs.io/en/latest/) for examples and information.
 
 ## Workflow
 
+The rough workflow can be visualized as follows:
+
+<p align="center">
+  <img src="docs/source/_static/img/eir_auto_gp.svg" alt="EIR auto GP Workflow">
+</p>
+
 1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK files and `.csv` label file, preparing the data for model training and evaluation.
 2. Train/test split: The processed data is automatically split into training and testing sets, with the option of manually specifying splits.
 3. Training: Configurable number of training runs are set up and executed using EIR's deep learning models.
 4. SNP feature selection: GWAS based feature selection, deep learning-based feature selection with Bayesian optimization, and mixed strategies are supported.
 5. Test set prediction: Predictions are made on the test set using all training run folds.
 6. Ensemble prediction: An ensemble prediction is created from the individual predictions.
 7. Results analysis: Performance metrics, visualizations, and analysis are generated to assess the model's performance.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: eir-auto-gp Version: 0.0.2a0 Summary: Author: Arnor
+Metadata-Version: 2.1 Name: eir-auto-gp Version: 0.0.3a0 Summary: Author: Arnor
 Sigurdsson Author-email: arnor-sigurdsson@users.noreply.github.com Requires-
 Python: >=3.10.0,<4.0.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: eir-dl (>=0.1.31a0,<0.2.0) Requires-
 Dist: plink-pipelines (>=0.1.5a0,<0.2.0) Requires-Dist: qmplot (>=0.3.2,<0.4.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0) Description-Content-Type:
 text/markdown # EIR-auto-GP
-                              [Eir Auto GP Logo]
+                              [EIR auto GP Logo]
 [https://img.shields.io/badge/License-APGL-5B2D5B.svg] [https://img.shields.io/
  badge/python-3.10-blue.svg] [https://img.shields.io/pypi/v/eir-auto-gp.svg]
    [https://codecov.io/gh/arnor-sigurdsson/EIR-auto-GP/branch/master/graph/
               badge.svg?token=PODL2J83Y0] [Documentation_Status]
 `EIR-auto-GP`: Automated genomic prediction (GP) using deep learning models
 with EIR. **WARNING**: This project is in alpha phase. Expect backwards
 incompatible changes and API changes. ## Overview EIR-auto-GP is a
@@ -23,26 +23,28 @@
 Takes care of launching a configurable number of deep learning training runs. -
 SNP-based feature selection based on GWAS, deep learning-based attributions,
 and a combination of both. - Ensemble prediction from multiple training runs. -
 Analysis and visualization of results. ## Installation First, ensure that
 [plink2](https://www.cog-genomics.org/plink/2.0/) is installed and available in
 your `PATH`. Then, install `EIR-auto-GP` using `pip`: `pip install eir-auto-gp`
 ## Usage Please refer to the [Documentation](https://eir-auto-
-gp.readthedocs.io/en/latest/) for examples and information. ## Workflow 1. Data
-processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK files and
-`.csv` label file, preparing the data for model training and evaluation. 2.
-Train/test split: The processed data is automatically split into training and
-testing sets, with the option of manually specifying splits. 3. Training:
-Configurable number of training runs are set up and executed using EIR's deep
-learning models. 4. SNP feature selection: GWAS based feature selection, deep
-learning-based feature selection with Bayesian optimization, and mixed
-strategies are supported. 5. Test set prediction: Predictions are made on the
-test set using all training run folds. 6. Ensemble prediction: An ensemble
-prediction is created from the individual predictions. 7. Results analysis:
-Performance metrics, visualizations, and analysis are generated to assess the
-model's performance. ## Citation If you use `EIR-auto-GP` in a scientific
-publication, we would appreciate if you could use the following citation: ```
-@article{sigurdsson2021deep, title={Deep integrative models for large-scale
-human genomics}, author={Sigurdsson, Arnor Ingi and Westergaard, David and
-Winther, Ole and Lund, Ole and Brunak, S{\o}ren and Vilhjalmsson, Bjarni J and
-Rasmussen, Simon}, journal={bioRxiv}, year={2021}, publisher={Cold Spring
-Harbor Laboratory} } ```
+gp.readthedocs.io/en/latest/) for examples and information. ## Workflow The
+rough workflow can be visualized as follows:
+                            [EIR auto GP Workflow]
+1. Data processing: EIR-auto-GP processes the input `.bed/.bim/.fam` PLINK
+files and `.csv` label file, preparing the data for model training and
+evaluation. 2. Train/test split: The processed data is automatically split into
+training and testing sets, with the option of manually specifying splits. 3.
+Training: Configurable number of training runs are set up and executed using
+EIR's deep learning models. 4. SNP feature selection: GWAS based feature
+selection, deep learning-based feature selection with Bayesian optimization,
+and mixed strategies are supported. 5. Test set prediction: Predictions are
+made on the test set using all training run folds. 6. Ensemble prediction: An
+ensemble prediction is created from the individual predictions. 7. Results
+analysis: Performance metrics, visualizations, and analysis are generated to
+assess the model's performance. ## Citation If you use `EIR-auto-GP` in a
+scientific publication, we would appreciate if you could use the following
+citation: ``` @article{sigurdsson2021deep, title={Deep integrative models for
+large-scale human genomics}, author={Sigurdsson, Arnor Ingi and Westergaard,
+David and Winther, Ole and Lund, Ole and Brunak, S{\o}ren and Vilhjalmsson,
+Bjarni J and Rasmussen, Simon}, journal={bioRxiv}, year={2021}, publisher={Cold
+Spring Harbor Laboratory} } ```
```

