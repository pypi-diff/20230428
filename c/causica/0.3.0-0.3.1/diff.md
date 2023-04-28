# Comparing `tmp/causica-0.3.0.tar.gz` & `tmp/causica-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causica-0.3.0.tar", max compression
+gzip compressed data, was "causica-0.3.1.tar", max compression
```

## Comparing `causica-0.3.0.tar` & `causica-0.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1141 2023-04-27 12:56:49.952801 causica-0.3.0/LICENSE
--rw-r--r--   0        0        0     7092 2023-04-27 13:52:23.840044 causica-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.952801 causica-0.3.0/examples/__init__.py
--rw-r--r--   0        0        0    76973 2023-04-27 12:56:49.952801 causica-0.3.0/examples/csuite_example.ipynb
--rw-r--r--   0        0        0   530997 2023-04-27 13:52:23.850044 causica-0.3.0/examples/multi_investment_sales_attribution.ipynb
--rw-r--r--   0        0        0      760 2023-04-27 13:52:23.860045 causica-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.952801 causica-0.3.0/src/causica/__init__.py
--rw-r--r--   0        0        0      153 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/config/lightning/default_data.yaml
--rw-r--r--   0        0        0     1227 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/config/lightning/default_gaussian.yaml
--rw-r--r--   0        0        0     1225 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/config/lightning/default_spline.yaml
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/datasets/__init__.py
--rw-r--r--   0        0        0    12768 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/causica_dataset_format.py
--rw-r--r--   0        0        0     2642 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/interventional_data.py
--rw-r--r--   0        0        0     1230 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/datasets/loaded_expert_graph_container.py
--rw-r--r--   0        0        0     2454 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/datasets/standardizer.py
--rw-r--r--   0        0        0     1959 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/tensordict_utils.py
--rw-r--r--   0        0        0      307 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/datasets/variable_types.py
--rw-r--r--   0        0        0      891 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/__init__.py
--rw-r--r--   0        0        0      613 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/__init__.py
--rw-r--r--   0        0        0     3600 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/adjacency/adjacency_distributions.py
--rw-r--r--   0        0        0     8583 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
--rw-r--r--   0        0        0     3374 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/directed_acyclic.py
--rw-r--r--   0        0        0     7979 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/adjacency/enco.py
--rw-r--r--   0        0        0     3952 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/adjacency/gibbs_dag_prior.py
--rw-r--r--   0        0        0     4784 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/adjacency/three_way.py
--rw-r--r--   0        0        0      773 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/distribution_module.py
--rw-r--r--   0        0        0      649 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/gumbel_binary.py
--rw-r--r--   0        0        0      595 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/__init__.py
--rw-r--r--   0        0        0     3356 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/bernoulli.py
--rw-r--r--   0        0        0     3222 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/categorical.py
--rw-r--r--   0        0        0     7593 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/joint.py
--rw-r--r--   0        0        0     3389 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/noise.py
--rw-r--r--   0        0        0      112 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/spline/__init__.py
--rw-r--r--   0        0        0     6539 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
--rw-r--r--   0        0        0     4340 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/spline/rational_quadratic_transform.py
--rw-r--r--   0        0        0     8024 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/noise/spline/spline.py
--rw-r--r--   0        0        0     1736 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/distributions/noise/univariate_normal.py
--rw-r--r--   0        0        0     4058 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/sem_distribution.py
--rw-r--r--   0        0        0     3063 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/distributions/transforms.py
--rw-r--r--   0        0        0      516 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/fsspec_helpers.py
--rw-r--r--   0        0        0      310 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/functional_relationships/__init__.py
--rw-r--r--   0        0        0     4574 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/do_functional_relationships.py
--rw-r--r--   0        0        0     2330 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/functional_relationships.py
--rw-r--r--   0        0        0     9442 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/icgnn.py
--rw-r--r--   0        0        0     2949 2023-04-27 13:52:23.860045 causica-0.3.0/src/causica/functional_relationships/linear_functional_relationships.py
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/graph/__init__.py
--rw-r--r--   0        0        0      375 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/graph/dag_constraint.py
--rw-r--r--   0        0        0     2711 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/graph/evaluation_metrics.py
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/lightning/__init__.py
--rw-r--r--   0        0        0     3437 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/callbacks.py
--rw-r--r--   0        0        0      718 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/lightning/cli.py
--rw-r--r--   0        0        0        0 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/__init__.py
--rw-r--r--   0        0        0     3052 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/basic_data_module.py
--rw-r--r--   0        0        0     1143 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/deci_data_module.py
--rw-r--r--   0        0        0     7778 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/data_modules/variable_spec_data.py
--rw-r--r--   0        0        0      776 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/main.py
--rw-r--r--   0        0        0        0 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/modules/__init__.py
--rw-r--r--   0        0        0    12424 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/modules/deci_module.py
--rw-r--r--   0        0        0     2096 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/lightning/modules/variable_spec_module.py
--rw-r--r--   0        0        0     1289 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/mlflow_helpers.py
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/sem/__init__.py
--rw-r--r--   0        0        0     3711 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/sem/distribution_parameters_sem.py
--rw-r--r--   0        0        0     6175 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/sem/structural_equation_model.py
--rw-r--r--   0        0        0        0 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/training/__init__.py
--rw-r--r--   0        0        0    10903 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/training/auglag.py
--rw-r--r--   0        0        0     5286 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/training/evaluation.py
--rw-r--r--   0        0        0     8958 2023-04-27 13:52:23.870045 causica-0.3.0/src/causica/training/per_variable_metrics.py
--rw-r--r--   0        0        0     1169 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/training/training_callbacks.py
--rw-r--r--   0        0        0     1725 2023-04-27 12:56:49.962801 causica-0.3.0/src/causica/triangular_transformations.py
--rw-r--r--   0        0        0     7913 1970-01-01 00:00:00.000000 causica-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-04-28 09:33:29.796962 causica-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7092 2023-04-28 09:33:29.796962 causica-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.806962 causica-0.3.1/examples/__init__.py
+-rw-r--r--   0        0        0    76973 2023-04-28 09:33:29.806962 causica-0.3.1/examples/csuite_example.ipynb
+-rw-r--r--   0        0        0   530941 2023-04-28 10:07:03.298657 causica-0.3.1/examples/multi_investment_sales_attribution.ipynb
+-rw-r--r--   0        0        0      734 2023-04-28 10:07:03.308657 causica-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/config/lightning/default_data.yaml
+-rw-r--r--   0        0        0     1227 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/config/lightning/default_gaussian.yaml
+-rw-r--r--   0        0        0     1225 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/config/lightning/default_spline.yaml
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/__init__.py
+-rw-r--r--   0        0        0    12768 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/causica_dataset_format.py
+-rw-r--r--   0        0        0     2642 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/interventional_data.py
+-rw-r--r--   0        0        0     1230 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/loaded_expert_graph_container.py
+-rw-r--r--   0        0        0     2454 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/standardizer.py
+-rw-r--r--   0        0        0     1959 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/tensordict_utils.py
+-rw-r--r--   0        0        0      307 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/datasets/variable_types.py
+-rw-r--r--   0        0        0      891 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/__init__.py
+-rw-r--r--   0        0        0      613 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/__init__.py
+-rw-r--r--   0        0        0     3600 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/adjacency_distributions.py
+-rw-r--r--   0        0        0     8583 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
+-rw-r--r--   0        0        0     3374 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/directed_acyclic.py
+-rw-r--r--   0        0        0     7979 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/enco.py
+-rw-r--r--   0        0        0     3952 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/gibbs_dag_prior.py
+-rw-r--r--   0        0        0     4784 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/adjacency/three_way.py
+-rw-r--r--   0        0        0      773 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/distribution_module.py
+-rw-r--r--   0        0        0      649 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/gumbel_binary.py
+-rw-r--r--   0        0        0      595 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/noise/__init__.py
+-rw-r--r--   0        0        0     3356 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/bernoulli.py
+-rw-r--r--   0        0        0     3222 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/categorical.py
+-rw-r--r--   0        0        0     7593 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/noise/joint.py
+-rw-r--r--   0        0        0     3389 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/noise/noise.py
+-rw-r--r--   0        0        0      112 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/spline/__init__.py
+-rw-r--r--   0        0        0     6539 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
+-rw-r--r--   0        0        0     4340 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/spline/rational_quadratic_transform.py
+-rw-r--r--   0        0        0     8024 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/spline/spline.py
+-rw-r--r--   0        0        0     1736 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/distributions/noise/univariate_normal.py
+-rw-r--r--   0        0        0     4058 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/sem_distribution.py
+-rw-r--r--   0        0        0     3063 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/distributions/transforms.py
+-rw-r--r--   0        0        0      516 2023-04-28 09:33:29.806962 causica-0.3.1/src/causica/fsspec_helpers.py
+-rw-r--r--   0        0        0      310 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/functional_relationships/__init__.py
+-rw-r--r--   0        0        0     4574 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/functional_relationships/do_functional_relationships.py
+-rw-r--r--   0        0        0     2330 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/functional_relationships/functional_relationships.py
+-rw-r--r--   0        0        0     9442 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/functional_relationships/icgnn.py
+-rw-r--r--   0        0        0     2949 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/functional_relationships/linear_functional_relationships.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/graph/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/graph/dag_constraint.py
+-rw-r--r--   0        0        0     2711 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/graph/evaluation_metrics.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/callbacks.py
+-rw-r--r--   0        0        0      718 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/cli.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/data_modules/__init__.py
+-rw-r--r--   0        0        0     3052 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/data_modules/basic_data_module.py
+-rw-r--r--   0        0        0     1143 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/data_modules/deci_data_module.py
+-rw-r--r--   0        0        0     7778 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/data_modules/variable_spec_data.py
+-rw-r--r--   0        0        0      776 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/main.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/modules/__init__.py
+-rw-r--r--   0        0        0    12424 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/modules/deci_module.py
+-rw-r--r--   0        0        0     2096 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/lightning/modules/variable_spec_module.py
+-rw-r--r--   0        0        0     1289 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/mlflow_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/sem/__init__.py
+-rw-r--r--   0        0        0     3711 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/sem/distribution_parameters_sem.py
+-rw-r--r--   0        0        0     6175 2023-04-28 09:33:29.816961 causica-0.3.1/src/causica/sem/structural_equation_model.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:33:29.826961 causica-0.3.1/src/causica/training/__init__.py
+-rw-r--r--   0        0        0    10903 2023-04-28 09:33:29.826961 causica-0.3.1/src/causica/training/auglag.py
+-rw-r--r--   0        0        0     5286 2023-04-28 09:33:29.826961 causica-0.3.1/src/causica/training/evaluation.py
+-rw-r--r--   0        0        0     8958 2023-04-28 09:33:29.826961 causica-0.3.1/src/causica/training/per_variable_metrics.py
+-rw-r--r--   0        0        0     1169 2023-04-28 09:33:29.826961 causica-0.3.1/src/causica/training/training_callbacks.py
+-rw-r--r--   0        0        0     1725 2023-04-28 09:33:29.826961 causica-0.3.1/src/causica/triangular_transformations.py
+-rw-r--r--   0        0        0     7874 1970-01-01 00:00:00.000000 causica-0.3.1/PKG-INFO
```

### Comparing `causica-0.3.0/LICENSE` & `causica-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/README.md` & `causica-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/examples/csuite_example.ipynb` & `causica-0.3.1/examples/csuite_example.ipynb`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/examples/multi_investment_sales_attribution.ipynb` & `causica-0.3.1/examples/multi_investment_sales_attribution.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962968472734097%*

 * *Differences: {"'cells'": "{22: {'outputs': {1: {'data': {'application/vnd.jupyter.widget-view+json': "*

 * *            "{'model_id': '3cb2c2e020e2499dbbbc14ecab5b28d6'}}}}}, 25: {'source': {insert: [(1, "*

 * *            "'\\n'), (3, 'sem = sem_module().mode')], delete: [6, 5, 4, 3, 2]}}, 26: {'source': "*

 * *            "{insert: [(0, 'graph = nx.from_numpy_array(sem.graph.cpu().numpy(), "*

 * *            "create_using=nx.DiGraph)\\n')], delete: [0]}}, insert: [(36, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count' […]*

```diff
@@ -623,15 +623,15 @@
                         "20.1 K    Total params\n",
                         "0.081     Total estimated model params size (MB)\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a99ea13a85d64f278cb4be91b21c99d4",
+                            "model_id": "3cb2c2e020e2499dbbbc14ecab5b28d6",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Training: 0it [00:00, ?it/s]"
                         ]
                     },
@@ -686,20 +686,17 @@
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sem_module: SEMDistributionModule = torch.load(\"deci.pt\")\n",
+                "\n",
                 "# create a structural equation model using the most likely graph\n",
-                "sem = DistributionParametersSEM(\n",
-                "    graph=sem_module.adjacency_module().mode,\n",
-                "    func=sem_module.functional_relationships,\n",
-                "    noise_dist=sem_module.noise_module,\n",
-                ")"
+                "sem = sem_module().mode"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {},
             "outputs": [
@@ -711,15 +708,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "graph = nx.from_numpy_matrix(sem.graph.cpu().numpy(), create_using=nx.DiGraph)\n",
+                "graph = nx.from_numpy_array(sem.graph.cpu().numpy(), create_using=nx.DiGraph)\n",
                 "graph = nx.relabel_nodes(graph, dict(enumerate(data_module.dataset_train.keys())))\n",
                 "\n",
                 "fig, axis = plt.subplots(1, 1, figsize=(8, 8))\n",
                 "\n",
                 "for node, i in labels.items():\n",
                 "    axis.scatter(layout[node][0], layout[node][1], label=f\"{i}: {node}\")\n",
                 "axis.legend()\n",
@@ -892,14 +889,21 @@
                 "fig.suptitle(\"Comparison of Ground Truth ITEs with DECI estimates\")\n",
                 "for ax, treatment in zip(axes, revenue_estimated_ite.keys()):\n",
                 "    ax.scatter(revenue_estimated_ite[treatment], ground_truth_ites[treatment])\n",
                 "    ax.set_title(treatment)\n",
                 "    ax.set_xlabel(\"Estimated ITE ($)\")\n",
                 "    ax.set_ylabel(\"Ground Truth ITE ($)\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `causica-0.3.0/pyproject.toml` & `causica-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causica"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "causica", from = "src" },
     { include = "examples", from = "." },
 ]
@@ -13,16 +13,15 @@
 [tool.poetry.dependencies]
 python = "~3.10"
 azureml-mlflow = "^1.46.0"
 mlflow = "^2.0.0"
 numpy = "^1.22.4"
 pandas = "^1.4.2"
 tensorboard = "^2.9.0"
-pytorch-lightning = {version = "^2.0.0", extras= ["extra"]}
-jsonargparse = "<=4.20.0"
+pytorch-lightning = {version = "^1.9.0", extras= ["extra"]}
 dataclasses-json = "^0.5.7"
 types-PyYAML = "^6.0.12.2"
 tensordict = "^0.1.0"
 torch = "^2.0.0"
 numba = "^0.56.0"  # needed to make the build work
 
 [tool.poetry.dev-dependencies]
```

### Comparing `causica-0.3.0/src/causica/config/lightning/default_gaussian.yaml` & `causica-0.3.1/src/causica/config/lightning/default_gaussian.yaml`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/config/lightning/default_spline.yaml` & `causica-0.3.1/src/causica/config/lightning/default_spline.yaml`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/datasets/causica_dataset_format.py` & `causica-0.3.1/src/causica/datasets/causica_dataset_format.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/datasets/interventional_data.py` & `causica-0.3.1/src/causica/datasets/interventional_data.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/datasets/loaded_expert_graph_container.py` & `causica-0.3.1/src/causica/datasets/loaded_expert_graph_container.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/datasets/standardizer.py` & `causica-0.3.1/src/causica/datasets/standardizer.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/datasets/tensordict_utils.py` & `causica-0.3.1/src/causica/datasets/tensordict_utils.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/__init__.py` & `causica-0.3.1/src/causica/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/__init__.py` & `causica-0.3.1/src/causica/distributions/adjacency/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/adjacency_distributions.py` & `causica-0.3.1/src/causica/distributions/adjacency/adjacency_distributions.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/constrained_adjacency_distributions.py` & `causica-0.3.1/src/causica/distributions/adjacency/constrained_adjacency_distributions.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/directed_acyclic.py` & `causica-0.3.1/src/causica/distributions/adjacency/directed_acyclic.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/enco.py` & `causica-0.3.1/src/causica/distributions/adjacency/enco.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/gibbs_dag_prior.py` & `causica-0.3.1/src/causica/distributions/adjacency/gibbs_dag_prior.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/adjacency/three_way.py` & `causica-0.3.1/src/causica/distributions/adjacency/three_way.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/distribution_module.py` & `causica-0.3.1/src/causica/distributions/distribution_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/gumbel_binary.py` & `causica-0.3.1/src/causica/distributions/gumbel_binary.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/__init__.py` & `causica-0.3.1/src/causica/distributions/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/bernoulli.py` & `causica-0.3.1/src/causica/distributions/noise/bernoulli.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/categorical.py` & `causica-0.3.1/src/causica/distributions/noise/categorical.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/joint.py` & `causica-0.3.1/src/causica/distributions/noise/joint.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/noise.py` & `causica-0.3.1/src/causica/distributions/noise/noise.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py` & `causica-0.3.1/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/spline/rational_quadratic_transform.py` & `causica-0.3.1/src/causica/distributions/noise/spline/rational_quadratic_transform.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/spline/spline.py` & `causica-0.3.1/src/causica/distributions/noise/spline/spline.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/noise/univariate_normal.py` & `causica-0.3.1/src/causica/distributions/noise/univariate_normal.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/sem_distribution.py` & `causica-0.3.1/src/causica/distributions/sem_distribution.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/distributions/transforms.py` & `causica-0.3.1/src/causica/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/fsspec_helpers.py` & `causica-0.3.1/src/causica/fsspec_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/functional_relationships/do_functional_relationships.py` & `causica-0.3.1/src/causica/functional_relationships/do_functional_relationships.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/functional_relationships/functional_relationships.py` & `causica-0.3.1/src/causica/functional_relationships/functional_relationships.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/functional_relationships/icgnn.py` & `causica-0.3.1/src/causica/functional_relationships/icgnn.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/functional_relationships/linear_functional_relationships.py` & `causica-0.3.1/src/causica/functional_relationships/linear_functional_relationships.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/graph/evaluation_metrics.py` & `causica-0.3.1/src/causica/graph/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/callbacks.py` & `causica-0.3.1/src/causica/lightning/callbacks.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/cli.py` & `causica-0.3.1/src/causica/lightning/cli.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/data_modules/basic_data_module.py` & `causica-0.3.1/src/causica/lightning/data_modules/basic_data_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/data_modules/deci_data_module.py` & `causica-0.3.1/src/causica/lightning/data_modules/deci_data_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/data_modules/variable_spec_data.py` & `causica-0.3.1/src/causica/lightning/data_modules/variable_spec_data.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/main.py` & `causica-0.3.1/src/causica/lightning/main.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/modules/deci_module.py` & `causica-0.3.1/src/causica/lightning/modules/deci_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/lightning/modules/variable_spec_module.py` & `causica-0.3.1/src/causica/lightning/modules/variable_spec_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/mlflow_helpers.py` & `causica-0.3.1/src/causica/mlflow_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/sem/distribution_parameters_sem.py` & `causica-0.3.1/src/causica/sem/distribution_parameters_sem.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/sem/structural_equation_model.py` & `causica-0.3.1/src/causica/sem/structural_equation_model.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/training/auglag.py` & `causica-0.3.1/src/causica/training/auglag.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/training/evaluation.py` & `causica-0.3.1/src/causica/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/training/per_variable_metrics.py` & `causica-0.3.1/src/causica/training/per_variable_metrics.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/training/training_callbacks.py` & `causica-0.3.1/src/causica/training/training_callbacks.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/src/causica/triangular_transformations.py` & `causica-0.3.1/src/causica/triangular_transformations.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.0/PKG-INFO` & `causica-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: causica
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: azureml-mlflow (>=1.46.0,<2.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
-Requires-Dist: jsonargparse (<=4.20.0)
 Requires-Dist: mlflow (>=2.0.0,<3.0.0)
 Requires-Dist: numba (>=0.56.0,<0.57.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: pytorch-lightning[extra] (>=2.0.0,<3.0.0)
+Requires-Dist: pytorch-lightning[extra] (>=1.9.0,<2.0.0)
 Requires-Dist: tensorboard (>=2.9.0,<3.0.0)
 Requires-Dist: tensordict (>=0.1.0,<0.2.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: types-PyYAML (>=6.0.12.2,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 [![Causica CI Build](https://github.com/microsoft/causica/actions/workflows/ci-build.yml/badge.svg)](https://github.com/microsoft/causica/actions/workflows/ci-build.yml)
```

