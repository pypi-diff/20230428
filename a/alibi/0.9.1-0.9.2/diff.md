# Comparing `tmp/alibi-0.9.1.tar.gz` & `tmp/alibi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alibi-0.9.1.tar", last modified: Mon Mar 13 15:27:47 2023, max compression
+gzip compressed data, was "alibi-0.9.2.tar", last modified: Fri Apr 28 13:44:02 2023, max compression
```

## Comparing `alibi-0.9.1.tar` & `alibi-0.9.2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.257276 alibi-0.9.1/
--rw-r--r--   0 janis     (1000) janis     (1000)    11354 2023-03-13 15:25:40.000000 alibi-0.9.1/LICENSE
--rw-r--r--   0 janis     (1000) janis     (1000)       58 2023-03-13 15:25:40.000000 alibi-0.9.1/MANIFEST.in
--rw-r--r--   0 janis     (1000) janis     (1000)    20875 2023-03-13 15:27:47.257276 alibi-0.9.1/PKG-INFO
--rw-r--r--   0 janis     (1000) janis     (1000)    19975 2023-03-13 15:25:40.000000 alibi-0.9.1/README.md
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.240610 alibi-0.9.1/alibi/
--rw-r--r--   0 janis     (1000) janis     (1000)      187 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/api/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/api/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7096 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/api/defaults.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6960 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/api/interfaces.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/api/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/api/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2793 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/api/tests/test_interfaces.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/confidence/
--rw-r--r--   0 janis     (1000) janis     (1000)      251 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/confidence/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18571 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/confidence/model_linearity.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/confidence/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/confidence/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8326 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/confidence/tests/test_model_linearity.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2174 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/confidence/tests/test_trustscore.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8214 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/confidence/trustscore.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/data/
--rw-r--r--   0 janis     (1000) janis     (1000)   116015 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/data/cats.tar.gz
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/datasets/
--rw-r--r--   0 janis     (1000) janis     (1000)      451 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/datasets/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12968 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/datasets/default.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1037 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/datasets/tensorflow.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.243943 alibi-0.9.1/alibi/datasets/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/datasets/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4559 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/datasets/tests/test_datasets.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1608 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/exceptions.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/
--rw-r--r--   0 janis     (1000) janis     (1000)     2230 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    29966 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/ale.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/anchors/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    35887 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/anchor_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4371 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/anchor_explanation.py
--rw-r--r--   0 janis     (1000) janis     (1000)    28092 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/anchor_image.py
--rw-r--r--   0 janis     (1000) janis     (1000)    49305 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/anchor_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12848 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/anchor_tabular_distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)    24277 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/anchor_text.py
--rw-r--r--   0 janis     (1000) janis     (1000)    27155 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/language_model_text_sampler.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16961 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/anchors/text_samplers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/backends/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4211 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    39363 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/cfrl_tabular.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/backends/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17765 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/pytorch/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6141 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/pytorch/cfrl_tabular.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/backends/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    19783 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/tensorflow/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6379 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/backends/tensorflow/cfrl_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    35265 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/cem.py
--rw-r--r--   0 janis     (1000) janis     (1000)    66499 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/cfproto.py
--rw-r--r--   0 janis     (1000) janis     (1000)    44884 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    23850 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/cfrl_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    27167 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/counterfactual.py
--rw-r--r--   0 janis     (1000) janis     (1000)    55064 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/integrated_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)    73245 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/partial_dependence.py
--rw-r--r--   0 janis     (1000) janis     (1000)    39164 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/pd_variance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    45135 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/permutation_importance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    80284 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/shap_wrappers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/similarity/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/similarity/backends/
--rw-r--r--   0 janis     (1000) janis     (1000)     1301 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/backends/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.247276 alibi-0.9.1/alibi/explainers/similarity/backends/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/backends/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4724 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/backends/pytorch/base.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.250610 alibi-0.9.1/alibi/explainers/similarity/backends/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/backends/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4312 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/backends/tensorflow/base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7001 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12715 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/grad.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2654 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/similarity/metrics.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.250610 alibi-0.9.1/alibi/explainers/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    11006 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17481 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_ale.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2938 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_anchor_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7874 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_anchor_image.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16247 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_anchor_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18774 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_anchor_text.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1572 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_cem.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6681 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_cfproto.py
--rw-r--r--   0 janis     (1000) janis     (1000)    20718 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_cfrl.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4900 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_counterfactual.py
--rw-r--r--   0 janis     (1000) janis     (1000)    37074 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_integrated_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)    42674 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_partial_dependence.py
--rw-r--r--   0 janis     (1000) janis     (1000)    28620 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_pd_variance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    23539 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_permutation_importance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    65433 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_shap_wrappers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/explainers/tests/test_simiarlity/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_simiarlity/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5894 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_simiarlity/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5864 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_simiarlity/test_backends.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17977 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
--rw-r--r--   0 janis     (1000) janis     (1000)     9302 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3086 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/explainers/tests/utils.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/models/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/models/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)      477 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2748 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3094 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8134 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/cfrl_models.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4952 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/metrics.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12988 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/model.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/models/pytorch/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1767 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/tests/test_actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)      647 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/tests/test_autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3778 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/tests/test_cfrl_models.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1847 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/tests/test_metrics.py
--rw-r--r--   0 janis     (1000) janis     (1000)    21220 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/pytorch/tests/test_model.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/models/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)      486 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2913 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3378 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8692 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/cfrl_models.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/models/tensorflow/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1655 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/tests/test_actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)      643 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/tests/test_autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3708 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/models/tensorflow/tests/test_cfrl_models.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/prototypes/
--rw-r--r--   0 janis     (1000) janis     (1000)      250 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/prototypes/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    32709 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/prototypes/protoselect.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.253943 alibi-0.9.1/alibi/prototypes/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/prototypes/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    11674 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/prototypes/tests/test_protoselect.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3195 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/prototypes/tests/test_utils.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15554 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/saving.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.257276 alibi-0.9.1/alibi/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)      622 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/tests/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7261 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/tests/test_dep_management.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17618 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/tests/test_saving.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1033 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/tests/test_utils.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4809 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/tests/utils.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.257276 alibi-0.9.1/alibi/utils/
--rw-r--r--   0 janis     (1000) janis     (1000)     1276 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5000 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/approximation_methods.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2652 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/data.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3592 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/discretizer.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12076 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/distance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    31339 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)      582 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/distributions.py
--rw-r--r--   0 janis     (1000) janis     (1000)      513 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/download.py
--rw-r--r--   0 janis     (1000) janis     (1000)      320 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/frameworks.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2915 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4666 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/kernel.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15255 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/lang_model.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4718 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/mapping.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5365 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/missing_optional_dependency.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.257276 alibi-0.9.1/alibi/utils/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)      194 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/mocked_opt_dep.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1014 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_data.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3193 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_distance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15565 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1631 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2855 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_import_optional.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1103 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_mapping.py
--rw-r--r--   0 janis     (1000) janis     (1000)      398 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tests/test_misc.py
--rw-r--r--   0 janis     (1000) janis     (1000)      919 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/tf.py
--rw-r--r--   0 janis     (1000) janis     (1000)    22959 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/visualization.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1707 2023-03-13 15:25:40.000000 alibi-0.9.1/alibi/utils/wrappers.py
--rw-r--r--   0 janis     (1000) janis     (1000)      212 2023-03-13 15:26:04.000000 alibi-0.9.1/alibi/version.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-03-13 15:27:47.240610 alibi-0.9.1/alibi.egg-info/
--rw-r--r--   0 janis     (1000) janis     (1000)    20875 2023-03-13 15:27:47.000000 alibi-0.9.1/alibi.egg-info/PKG-INFO
--rw-r--r--   0 janis     (1000) janis     (1000)     5394 2023-03-13 15:27:47.000000 alibi-0.9.1/alibi.egg-info/SOURCES.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-03-13 15:27:47.000000 alibi-0.9.1/alibi.egg-info/dependency_links.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-03-13 15:27:47.000000 alibi-0.9.1/alibi.egg-info/not-zip-safe
--rw-r--r--   0 janis     (1000) janis     (1000)      650 2023-03-13 15:27:47.000000 alibi-0.9.1/alibi.egg-info/requires.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        6 2023-03-13 15:27:47.000000 alibi-0.9.1/alibi.egg-info/top_level.txt
--rw-r--r--   0 janis     (1000) janis     (1000)     2066 2023-03-13 15:27:47.260610 alibi-0.9.1/setup.cfg
--rw-r--r--   0 janis     (1000) janis     (1000)     2938 2023-03-13 15:25:40.000000 alibi-0.9.1/setup.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.075916 alibi-0.9.2/
+-rw-r--r--   0 janis     (1000) janis     (1000)    11354 2023-04-28 13:41:02.000000 alibi-0.9.2/LICENSE
+-rw-r--r--   0 janis     (1000) janis     (1000)       58 2023-04-28 13:41:02.000000 alibi-0.9.2/MANIFEST.in
+-rw-r--r--   0 janis     (1000) janis     (1000)    20875 2023-04-28 13:44:02.079249 alibi-0.9.2/PKG-INFO
+-rw-r--r--   0 janis     (1000) janis     (1000)    19975 2023-04-28 13:41:02.000000 alibi-0.9.2/README.md
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.045915 alibi-0.9.2/alibi/
+-rw-r--r--   0 janis     (1000) janis     (1000)      187 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/api/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     7096 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/defaults.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6960 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/interfaces.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/api/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2793 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/api/tests/test_interfaces.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/confidence/
+-rw-r--r--   0 janis     (1000) janis     (1000)      251 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    18571 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/model_linearity.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/confidence/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8326 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/tests/test_model_linearity.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2174 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/tests/test_trustscore.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8214 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/confidence/trustscore.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/data/
+-rw-r--r--   0 janis     (1000) janis     (1000)   116015 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/data/cats.tar.gz
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/datasets/
+-rw-r--r--   0 janis     (1000) janis     (1000)      451 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12968 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/default.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1037 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/tensorflow.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.049249 alibi-0.9.2/alibi/datasets/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4559 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/datasets/tests/test_datasets.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1813 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/exceptions.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.052582 alibi-0.9.2/alibi/explainers/
+-rw-r--r--   0 janis     (1000) janis     (1000)     2230 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    29966 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/ale.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/anchors/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    35805 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4371 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_explanation.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    28092 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_image.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    49286 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12848 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_tabular_distributed.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    24277 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/anchor_text.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    27223 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/language_model_text_sampler.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    16961 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/anchors/text_samplers.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/backends/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4211 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    39363 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/cfrl_tabular.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/backends/pytorch/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/pytorch/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    17765 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6141 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_tabular.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/backends/tensorflow/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/tensorflow/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    19783 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6379 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    35265 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cem.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    66499 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cfproto.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    44884 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cfrl_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    23850 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/cfrl_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    27167 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/counterfactual.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    56445 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/integrated_gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    73613 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/partial_dependence.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    39164 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/pd_variance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    45135 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/permutation_importance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    80284 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/shap_wrappers.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/similarity/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/similarity/backends/
+-rw-r--r--   0 janis     (1000) janis     (1000)     1321 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.055916 alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4753 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/base.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.059249 alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4341 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8837 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    13302 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/grad.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2654 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/similarity/metrics.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/explainers/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    11006 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/conftest.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    17481 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_ale.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2582 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_base.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     7874 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_image.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    16247 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_tabular.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    18774 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_anchor_text.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1572 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_cem.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     6681 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_cfproto.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    20718 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_cfrl.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4900 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_counterfactual.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    37074 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_integrated_gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    42674 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_partial_dependence.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    28620 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_pd_variance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    23539 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_permutation_importance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    65433 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_shap_wrappers.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5894 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/conftest.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5864 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_backends.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    17977 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     9302 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3086 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/explainers/tests/utils.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/models/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/__init__.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.062582 alibi-0.9.2/alibi/models/pytorch/
+-rw-r--r--   0 janis     (1000) janis     (1000)      477 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2748 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3094 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8134 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/cfrl_models.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4952 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/metrics.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12988 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/model.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.065916 alibi-0.9.2/alibi/models/pytorch/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1767 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      647 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3778 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_cfrl_models.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1847 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_metrics.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    21220 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/pytorch/tests/test_model.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.065916 alibi-0.9.2/alibi/models/tensorflow/
+-rw-r--r--   0 janis     (1000) janis     (1000)      486 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2913 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3378 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     8692 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/cfrl_models.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.065916 alibi-0.9.2/alibi/models/tensorflow/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1655 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/test_actor_critic.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      643 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/test_autoencoder.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3708 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/models/tensorflow/tests/test_cfrl_models.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.069249 alibi-0.9.2/alibi/prototypes/
+-rw-r--r--   0 janis     (1000) janis     (1000)      250 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    32709 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/protoselect.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.069249 alibi-0.9.2/alibi/prototypes/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    11674 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/tests/test_protoselect.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3195 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/prototypes/tests/test_utils.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    16242 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/saving.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.072583 alibi-0.9.2/alibi/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      622 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/conftest.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     7261 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/test_dep_management.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    18797 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/test_saving.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1033 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/test_utils.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4809 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/tests/utils.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.075916 alibi-0.9.2/alibi/utils/
+-rw-r--r--   0 janis     (1000) janis     (1000)     1276 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5000 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/approximation_methods.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2652 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/data.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3592 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/discretizer.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    12076 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/distance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    31339 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/distributed.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      582 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/distributions.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      513 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/download.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      320 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/frameworks.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2915 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4666 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/kernel.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    15255 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/lang_model.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     4718 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/mapping.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     5365 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/missing_optional_dependency.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.075916 alibi-0.9.2/alibi/utils/tests/
+-rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/__init__.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      194 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/mocked_opt_dep.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1014 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_data.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     3193 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_distance.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    15565 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_distributed.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1631 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_gradients.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     2855 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_import_optional.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1103 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_mapping.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      398 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tests/test_misc.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      919 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/tf.py
+-rw-r--r--   0 janis     (1000) janis     (1000)    22959 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/visualization.py
+-rw-r--r--   0 janis     (1000) janis     (1000)     1707 2023-04-28 13:41:02.000000 alibi-0.9.2/alibi/utils/wrappers.py
+-rw-r--r--   0 janis     (1000) janis     (1000)      212 2023-04-28 13:41:49.000000 alibi-0.9.2/alibi/version.py
+drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-04-28 13:44:02.045915 alibi-0.9.2/alibi.egg-info/
+-rw-r--r--   0 janis     (1000) janis     (1000)    20875 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/PKG-INFO
+-rw-r--r--   0 janis     (1000) janis     (1000)     5394 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/SOURCES.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/dependency_links.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/not-zip-safe
+-rw-r--r--   0 janis     (1000) janis     (1000)      649 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/requires.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)        6 2023-04-28 13:44:01.000000 alibi-0.9.2/alibi.egg-info/top_level.txt
+-rw-r--r--   0 janis     (1000) janis     (1000)     2066 2023-04-28 13:44:02.079249 alibi-0.9.2/setup.cfg
+-rw-r--r--   0 janis     (1000) janis     (1000)     2937 2023-04-28 13:41:02.000000 alibi-0.9.2/setup.py
```

### Comparing `alibi-0.9.1/LICENSE` & `alibi-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/PKG-INFO` & `alibi-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.1
+Version: 0.9.2
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alibi Version: 0.9.1 Summary: Algorithms for
+Metadata-Version: 2.1 Name: alibi Version: 0.9.2 Summary: Algorithms for
 monitoring and explaining machine learning models Home-page: https://
 github.com/SeldonIO/alibi Author: Seldon Technologies Ltd. Author-email:
 hello@seldon.io License: Apache 2.0 Classifier: Intended Audience :: Science/
 Research Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `alibi-0.9.1/README.md` & `alibi-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/api/defaults.py` & `alibi-0.9.2/alibi/api/defaults.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/api/interfaces.py` & `alibi-0.9.2/alibi/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/api/tests/test_interfaces.py` & `alibi-0.9.2/alibi/api/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/confidence/model_linearity.py` & `alibi-0.9.2/alibi/confidence/model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/confidence/tests/test_model_linearity.py` & `alibi-0.9.2/alibi/confidence/tests/test_model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/confidence/tests/test_trustscore.py` & `alibi-0.9.2/alibi/confidence/tests/test_trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/confidence/trustscore.py` & `alibi-0.9.2/alibi/confidence/trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/data/cats.tar.gz` & `alibi-0.9.2/alibi/data/cats.tar.gz`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/datasets/default.py` & `alibi-0.9.2/alibi/datasets/default.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/datasets/tensorflow.py` & `alibi-0.9.2/alibi/datasets/tensorflow.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/datasets/tests/test_datasets.py` & `alibi-0.9.2/alibi/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/exceptions.py` & `alibi-0.9.2/alibi/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,7 +48,15 @@
     This exception is raised whenever a compulsory call to a `fit` method has not been carried out.
     """
 
     def __init__(self, object_name: str):
         super().__init__(
             f"This {object_name} instance is not fitted yet. Call 'fit' with appropriate arguments first."
         )
+
+
+class SerializationError(AlibiException):
+    """
+    This exception is raised whenever an explainer cannot be serialized.
+    """
+    def __init__(self, message: str):
+        super().__init__(message)
```

### Comparing `alibi-0.9.1/alibi/explainers/__init__.py` & `alibi-0.9.2/alibi/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/ale.py` & `alibi-0.9.2/alibi/explainers/ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/anchors/anchor_base.py` & `alibi-0.9.2/alibi/explainers/anchors/anchor_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,16 +454,14 @@
         n_samples = data.shape[0]
 
         current_idx = self.state['current_idx']
         idxs = range(current_idx, current_idx + n_samples)
         self.state['t_idx'][anchor].update(idxs)
         self.state['t_nsamples'][anchor] += n_samples
         self.state['t_positives'][anchor] += labels.sum()
-        if coverage > -1:
-            self.state['t_coverage'][anchor] = coverage
         self.state['t_covered_true'][anchor] = covered_true
         self.state['t_covered_false'][anchor] = covered_false
         self.state['data'][idxs] = data
         self.state['labels'][idxs] = labels
         self.state['current_idx'] += n_samples
 
         if self.state['current_idx'] >= self.state['data'].shape[0] - max(self.margin, n_samples):
```

### Comparing `alibi-0.9.1/alibi/explainers/anchors/anchor_explanation.py` & `alibi-0.9.2/alibi/explainers/anchors/anchor_explanation.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/anchors/anchor_image.py` & `alibi-0.9.2/alibi/explainers/anchors/anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/anchors/anchor_tabular.py` & `alibi-0.9.2/alibi/explainers/anchors/anchor_tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -908,17 +908,18 @@
         Parameters
         ----------
         explanation
             Dict with anchors and additional metadata.
         """
 
         anchor_idxs = explanation['feature']
-        explanation['names'] = []
-        explanation['feature'] = [self.enc2feat_idx[idx] for idx in anchor_idxs]
         ordinal_ranges = {self.enc2feat_idx[idx]: [float('-inf'), float('inf')] for idx in anchor_idxs}
+        explanation['feature'] = list(ordinal_ranges.keys())
+        explanation['names'] = []
+
         for idx in set(anchor_idxs) - self.cat_lookup.keys():
             feat_id = self.enc2feat_idx[idx]  # feature col. id
             if 0 in self.ord_lookup[idx]:  # tells if the feature in X falls in a higher or lower bin
                 ordinal_ranges[feat_id][1] = min(
                     ordinal_ranges[feat_id][1], max(list(self.ord_lookup[idx]))
                 )
             else:
```

### Comparing `alibi-0.9.1/alibi/explainers/anchors/anchor_tabular_distributed.py` & `alibi-0.9.2/alibi/explainers/anchors/anchor_tabular_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/anchors/anchor_text.py` & `alibi-0.9.2/alibi/explainers/anchors/anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/anchors/language_model_text_sampler.py` & `alibi-0.9.2/alibi/explainers/anchors/language_model_text_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,14 +628,15 @@
             top_k_logits = (top_k_logits / temperature) if use_proba else (top_k_logits * 0)
 
             # Sample indices
             ids_k = tf.reshape(tf.random.categorical(top_k_logits, 1), shape=-1)
 
             # replace masked tokens with the sampled one
             tokens[masked_rows, masked_cols] = tf.gather(top_k_tokens, ids_k, batch_dims=1)
+            tokens_plus['input_ids'] = tf.convert_to_tensor(tokens)
         return tokens, data
 
     def set_data_type(self) -> None:
         """
         Working with `numpy` arrays of strings requires setting the data type to avoid
         truncating examples. This function estimates the longest sentence expected
         during the sampling process, which is used to set the number of characters
```

### Comparing `alibi-0.9.1/alibi/explainers/anchors/text_samplers.py` & `alibi-0.9.2/alibi/explainers/anchors/text_samplers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/backends/cfrl_base.py` & `alibi-0.9.2/alibi/explainers/backends/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/backends/cfrl_tabular.py` & `alibi-0.9.2/alibi/explainers/backends/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/backends/pytorch/cfrl_base.py` & `alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/backends/pytorch/cfrl_tabular.py` & `alibi-0.9.2/alibi/explainers/backends/pytorch/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/backends/tensorflow/cfrl_base.py` & `alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/backends/tensorflow/cfrl_tabular.py` & `alibi-0.9.2/alibi/explainers/backends/tensorflow/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/cem.py` & `alibi-0.9.2/alibi/explainers/cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/cfproto.py` & `alibi-0.9.2/alibi/explainers/cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/cfrl_base.py` & `alibi-0.9.2/alibi/explainers/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/cfrl_tabular.py` & `alibi-0.9.2/alibi/explainers/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/counterfactual.py` & `alibi-0.9.2/alibi/explainers/counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/integrated_gradients.py` & `alibi-0.9.2/alibi/explainers/integrated_gradients.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import logging
 import string
 import warnings
+from enum import Enum
 from typing import Callable, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import tensorflow as tf
 
 from alibi.api.defaults import DEFAULT_DATA_INTGRAD, DEFAULT_META_INTGRAD
 from alibi.api.interfaces import Explainer, Explanation
@@ -775,19 +776,30 @@
         logger.warning("It looks like you are passing a model with a scalar output and target is set to `None`."
                        "If your model is a regression model this will produce correct attributions. If your model "
                        "is a classification model, targets for each datapoint must be defined. "
                        "Not defining the target may lead to incorrect values for the attributions."
                        "Targets can be either the true classes or the classes predicted by the model.")
 
 
+class LayerState(str, Enum):
+    UNSPECIFIED = 'unspecified'
+    NON_SERIALIZABLE = 'non-serializable'
+    CALLABLE = 'callable'
+
+
 class IntegratedGradients(Explainer):
 
     def __init__(self,
                  model: tf.keras.Model,
-                 layer: Optional[tf.keras.layers.Layer] = None,
+                 layer: Optional[
+                     Union[
+                         Callable[[tf.keras.Model], tf.keras.layers.Layer],
+                         tf.keras.layers.Layer
+                     ]
+                 ] = None,
                  target_fn: Optional[Callable] = None,
                  method: str = "gausslegendre",
                  n_steps: int = 50,
                  internal_batch_size: int = 100
                  ) -> None:
         """
         An implementation of the integrated gradients method for `tensorflow` models.
@@ -795,16 +807,18 @@
         For details of the method see the original paper: https://arxiv.org/abs/1703.01365 .
 
         Parameters
         ----------
         model
             `tensorflow` model.
         layer
-            Layer with respect to which the gradients are calculated.
-            If not provided, the gradients are calculated with respect to the input.
+            A layer or a function having as parameter the model and returning a layer with respect to which the
+            gradients are calculated. If not provided, the gradients are calculated with respect to the input.
+            To guarantee saving and loading of the explainer, the layer has to be specified as a callable which
+            returns a layer given the model. E.g. ``lambda model: model.layers[0].embeddings``.
         target_fn
             A scalar function that is applied to the predictions of the model.
             This can be used to specify which scalar output the attributions should be calculated for.
             This can be particularly useful if the desired output is not known before calling the model
             (e.g. explaining the `argmax` output for a probabilistic classifier, in this case we could pass
             ``target_fn=partial(np.argmax, axis=1)``).
         method
@@ -825,26 +839,41 @@
         if self.model.inputs is None:
             self._has_inputs = False
         else:
             self._has_inputs = True
 
         if layer is None:
             self.orig_call: Optional[Callable] = None
-            layer_num: Optional[int] = 0
-        else:
+            self.layer = None
+            layer_meta: Union[int, str] = LayerState.UNSPECIFIED.value
+
+        elif isinstance(layer, tf.keras.layers.Layer):
             self.orig_call = layer.call
+            self.layer = layer
+
             try:
-                layer_num = model.layers.index(layer)
+                layer_meta = model.layers.index(layer)
             except ValueError:
-                logger.info("Layer not in the list of model.layers")
-                layer_num = None
+                layer_meta = LayerState.NON_SERIALIZABLE.value
+                logger.warning('Layer not in the list of `model.layers`. Passing the layer directly would not '
+                               'permit the serialization of the explainer. This is due to nested layers. To permit '
+                               'the serialization of the explainer, provide the layer as a callable which returns '
+                               'the layer given the model.')
+
+        elif callable(layer):
+            self.layer = layer(self.model)
+            self.orig_call = self.layer.call
+            self.callable_layer = layer
+            layer_meta = LayerState.CALLABLE.value
+
+        else:
+            raise TypeError(f'Unsupported layer type. Received {type(layer)}.')
 
-        params['layer'] = layer_num
+        params['layer'] = layer_meta
         self.meta['params'].update(params)
-        self.layer = layer
         self.n_steps = n_steps
         self.method = method
         self.internal_batch_size = internal_batch_size
 
         self._is_list: Optional[bool] = None
         self._is_np: Optional[bool] = None
         self.orig_dummy_input: Optional[Union[list, np.ndarray]] = None
```

### Comparing `alibi-0.9.1/alibi/explainers/partial_dependence.py` & `alibi-0.9.2/alibi/explainers/partial_dependence.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,14 +502,25 @@
             feature_values=feature_values,
             ice_values=ice_values,
             pd_values=pd_values,
             feature_deciles=feature_deciles,
         )
         return Explanation(meta=copy.deepcopy(self.meta), data=data)
 
+    def reset_predictor(self, predictor: Union[Callable[[np.ndarray], np.ndarray], BaseEstimator]) -> None:
+        """
+        Resets the predictor function or tree-based `sklearn` estimator.
+
+        Parameters
+        ----------
+        predictor
+            New predictor function or tree-based `sklearn` estimator.
+        """
+        self.predictor = predictor
+
 
 class PartialDependence(PartialDependenceBase):
     """ Black-box implementation of partial dependence for tabular datasets.
     Supports multiple feature interactions. """
 
     def __init__(self,
                  predictor: Callable[[np.ndarray], np.ndarray],
```

### Comparing `alibi-0.9.1/alibi/explainers/pd_variance.py` & `alibi-0.9.2/alibi/explainers/pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/permutation_importance.py` & `alibi-0.9.2/alibi/explainers/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/shap_wrappers.py` & `alibi-0.9.2/alibi/explainers/shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/similarity/backends/__init__.py` & `alibi-0.9.2/alibi/explainers/similarity/backends/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Union, Type
+from typing import Type, Union
 
-from alibi.utils.frameworks import has_pytorch, has_tensorflow, Framework
+from alibi.utils.frameworks import Framework, has_pytorch, has_tensorflow
 
 if has_pytorch:
     # import pytorch backend
-    from alibi.explainers.similarity.backends.pytorch.base import _PytorchBackend
+    from alibi.explainers.similarity.backends.pytorch.base import \
+        _PytorchBackend
 
 if has_tensorflow:
     # import tensorflow backend
-    from alibi.explainers.similarity.backends.tensorflow.base import _TensorFlowBackend
+    from alibi.explainers.similarity.backends.tensorflow.base import \
+        _TensorFlowBackend
 
 
 def _select_backend(backend: Framework = Framework.TENSORFLOW) \
         -> Union[Type['_TensorFlowBackend'], Type['_PytorchBackend']]:
     """
     Selects the backend according to the `backend` flag.
```

### Comparing `alibi-0.9.1/alibi/explainers/similarity/backends/pytorch/base.py` & `alibi-0.9.2/alibi/explainers/similarity/backends/pytorch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """`pytorch` backend for similarity explainers.
 
 Methods unique to the `pytorch` backend are defined here. The interface this class defines syncs with the `tensorflow`
 backend in order to ensure that the similarity methods only require to match this interface.
 """
 
-from typing import Callable, Union, Optional
+from typing import Any, Callable, List, Optional, Union
 
 import numpy as np
-import torch.nn as nn
 import torch
+import torch.nn as nn
 
 
 class _PytorchBackend:
     device: Optional[torch.device] = None  # device used by `pytorch` backend
 
     @staticmethod
     def get_grads(
             model: nn.Module,
-            X: torch.Tensor,
+            X: Union[torch.Tensor, List[Any]],
             Y: torch.Tensor,
             loss_fn: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
     ) -> np.ndarray:
         """
         Computes the gradients of the loss function with respect to the model's parameters for a single training and
         target pair.
```

### Comparing `alibi-0.9.1/alibi/explainers/similarity/backends/tensorflow/base.py` & `alibi-0.9.2/alibi/explainers/similarity/backends/tensorflow/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """`tensorflow` backend for similarity explainers.
 
 Methods unique to the `tensorflow` backend are defined here. The interface this class defines syncs with the `pytorch`
 backend in order to ensure that the similarity methods only require to match this interface.
 """
 
-from typing import Callable, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow import keras
 
 
 class _TensorFlowBackend:
     device: Optional[str] = None  # device used by `tensorflow` backend
 
     @staticmethod
     def get_grads(
             model: keras.Model,
-            X: tf.Tensor,
+            X: Union[tf.Tensor, List[Any]],
             Y: tf.Tensor,
             loss_fn: Callable[[tf.Tensor, tf.Tensor], tf.Tensor],
     ) -> np.ndarray:
         """
         Computes the gradients of the loss function with respect to the model's parameters for a single training and
         target pair.
```

### Comparing `alibi-0.9.1/alibi/explainers/similarity/base.py` & `alibi-0.9.2/alibi/explainers/similarity/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from abc import ABC
-from typing import TYPE_CHECKING, Callable, Union, Tuple, Optional
-from typing_extensions import Literal
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Union
 
 import numpy as np
-from tqdm import tqdm
-
 from alibi.api.interfaces import Explainer
 from alibi.explainers.similarity.backends import _select_backend
-from alibi.utils.frameworks import Framework
+from alibi.utils.frameworks import Framework, has_pytorch, has_tensorflow
+from alibi.utils.missing_optional_dependency import import_optional
+from tqdm import tqdm
+from typing_extensions import Literal
+
+_TfTensor = import_optional('tensorflow', ['Tensor'])
+_PtTensor = import_optional('torch', ['Tensor'])
 
 if TYPE_CHECKING:
     import tensorflow
     import torch
 
 
 class BaseSimilarityExplainer(Explainer, ABC):
@@ -59,15 +62,15 @@
         self.precompute_grads = precompute_grads
         self.verbose = verbose
 
         meta = {} if meta is None else meta
         super().__init__(meta=meta)
 
     def fit(self,
-            X_train: np.ndarray,
+            X_train: Union[np.ndarray, List[Any]],
             Y_train: np.ndarray) -> "Explainer":
         """Fit the explainer. If ``self.precompute_grads == True`` then the gradients are precomputed and stored.
 
         Parameters
         ----------
         X_train
             Training data.
@@ -75,45 +78,67 @@
             Training labels.
 
         Returns
         -------
         self
             Returns self.
         """
-        self.X_train: np.ndarray = X_train
-        self.Y_train: np.ndarray = Y_train
-        self.X_dims: Tuple = self.X_train.shape[1:]
-        self.Y_dims: Tuple = self.Y_train.shape[1:]
-        self.grad_X_train: np.ndarray = np.array([])
+        self.X_train = X_train
+        self.Y_train = Y_train
+        self.X_dims = self.X_train.shape[1:] if isinstance(self.X_train, np.ndarray) else None
+        self.Y_dims = self.Y_train.shape[1:]
+        self.grad_X_train = np.array([])
 
         # compute and store gradients
         if self.precompute_grads:
             grads = []
+            X: Union[np.ndarray, List[Any]]
             for X, Y in tqdm(zip(self.X_train, self.Y_train), disable=not self.verbose):
-                grad_X_train = self._compute_grad(X[None], Y[None])
+                grad_X_train = self._compute_grad(self._format(X), Y[None])
                 grads.append(grad_X_train[None])
+
             self.grad_X_train = np.concatenate(grads, axis=0)
         return self
 
+    @staticmethod
+    def _is_tensor(x: Any) -> bool:
+        """Checks if an obejct is a tensor."""
+        if has_tensorflow and isinstance(x, _TfTensor):
+            return True
+        if has_pytorch and isinstance(x, _PtTensor):
+            return True
+        if isinstance(x, np.ndarray):
+            return True
+        return False
+
+    @staticmethod
+    def _format(x: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, Any]'
+                ) -> 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, List[Any]]':
+        """Adds batch dimension."""
+        if BaseSimilarityExplainer._is_tensor(x):
+            return x[None]
+        return [x]
+
     def _verify_fit(self) -> None:
         """Verify that the explainer has been fitted.
 
         Raises
         ------
         ValueError
             If the explainer has not been fitted.
         """
-
         if not hasattr(self, 'X_train') or not hasattr(self, 'Y_train'):
             raise ValueError('Training data not set. Call `fit` and pass training data first.')
 
     def _match_shape_to_data(self,
-                             data: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]',
-                             target_type: Literal['X', 'Y']) -> 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]':
-        """Verify the shape of `data` against the shape of the training data.
+                             data: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, Any, List[Any]]',
+                             target_type: Literal['X', 'Y']
+                             ) -> 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, List[Any]]':
+        """
+        Verify the shape of `data` against the shape of the training data.
 
         Used to ensure input is correct shape for gradient methods implemented in the backends. `data` will be the
         features or label of the instance being explained. If the `data` is not a batch, reshape to be a single batch
         element. i.e. if training data shape is `(3, 28, 28)` and data shape is `(3, 28, 28)` we reshape data to
         `(1, 3, 28, 28)`.
 
         Parameters
@@ -127,44 +152,60 @@
 
         Raises
         ------
         ValueError
             If the shape of `data` does not match the shape of the training data, or fit has not been called prior to
             calling this method.
         """
+        if self._is_tensor(data):
+            return self._match_shape_to_data_tensor(data, target_type)
+        return self._match_shape_to_data_any(data)
+
+    def _match_shape_to_data_tensor(self,
+                                    data: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]',
+                                    target_type: Literal['X', 'Y']
+                                    ) -> 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]':
+        """ Verify the shape of `data` against the shape of the training data for tensor like data."""
         target_shape = getattr(self, f'{target_type}_dims')
         if data.shape == target_shape:
             data = data[None]
         if data.shape[1:] != target_shape:
             raise ValueError((f'Input `{target_type}` has shape {data.shape[1:]}'
                               f' but training data has shape {target_shape}'))
         return data
 
+    @staticmethod
+    def _match_shape_to_data_any(data: Union[Any, List[Any]]) -> list:
+        """ Ensures that any other data type is a list."""
+        if isinstance(data, list):
+            return data
+        return [data]
+
     def _compute_adhoc_similarity(self, grad_X: np.ndarray) -> np.ndarray:
         """
         Computes the similarity between the gradients of the test instances and all the training instances. The method
         performs the computation of the gradients of the training instance on the fly without storing them in memory.
 
         parameters
         ----------
         grad_X
             Gradients of the test instances.
         """
-        scores = np.zeros((grad_X.shape[0], self.X_train.shape[0]))
+        scores = np.zeros((len(grad_X), len(self.X_train)))
+        X: Union[np.ndarray, List[Any]]
         for i, (X, Y) in tqdm(enumerate(zip(self.X_train, self.Y_train)), disable=not self.verbose):
-            grad_X_train = self._compute_grad(X[None], Y[None])
+            grad_X_train = self._compute_grad(self._format(X), Y[None])
             scores[:, i] = self.sim_fn(grad_X, grad_X_train[None])[:, 0]
         return scores
 
     def _compute_grad(self,
-                      X: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]',
+                      X: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, List[Any]]',
                       Y: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]') \
             -> np.ndarray:
         """Computes predictor parameter gradients and returns a flattened `numpy` array."""
-
         X = self.backend.to_tensor(X) if isinstance(X, np.ndarray) else X
         Y = self.backend.to_tensor(Y) if isinstance(Y, np.ndarray) else Y
         return self.backend.get_grads(self.predictor, X, Y, self.loss_fn)
 
     def reset_predictor(self, predictor: 'Union[tensorflow.keras.Model, torch.nn.Module]') -> None:
         """Resets the predictor to the given predictor.
```

### Comparing `alibi-0.9.1/alibi/explainers/similarity/grad.py` & `alibi-0.9.2/alibi/explainers/similarity/grad.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Gradient-based explainer.
 
 This module implements the gradient-based explainers grad-dot and grad-cos.
 """
 
 import copy
-from typing import TYPE_CHECKING, Callable, Optional, Union, Dict, Tuple
-from typing_extensions import Literal
-from enum import Enum
 import warnings
+from enum import Enum
+from typing import (TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple,
+                    Union)
 
 import numpy as np
-
-from alibi.api.interfaces import Explanation
+from alibi.api.defaults import DEFAULT_DATA_SIM, DEFAULT_META_SIM
+from alibi.api.interfaces import Explainer, Explanation
 from alibi.explainers.similarity.base import BaseSimilarityExplainer
-from alibi.explainers.similarity.metrics import dot, cos, asym_dot
-from alibi.api.defaults import DEFAULT_META_SIM, DEFAULT_DATA_SIM
+from alibi.explainers.similarity.metrics import asym_dot, cos, dot
 from alibi.utils import _get_options_string
 from alibi.utils.frameworks import Framework
-from alibi.api.interfaces import Explainer
+from typing_extensions import Literal
 
 if TYPE_CHECKING:
     import tensorflow
     import torch
 
 
 class Task(str, Enum):
@@ -136,15 +135,15 @@
                            " This might be because your model has layers that track statistics using non-trainable "
                            "parameters such as batch normalization layers. In this case, you don't need to worry. "
                            "Otherwise it's because you have set some parameters to be non-trainable and alibi is "
                            "letting you know.")
             warnings.warn(warning_msg)
 
     def fit(self,
-            X_train: np.ndarray,
+            X_train: Union[np.ndarray, List[Any]],
             Y_train: np.ndarray) -> "Explainer":
         """Fit the explainer.
 
         The `GradientSimilarity` explainer requires the model gradients over the training data. In the explain method
         it compares them to the model gradients for the test instance(s). If ``precompute_grads=True`` on
         initialization then the gradients are precomputed here and stored. This will speed up the explain method call
         but storing the gradients may not be feasible for large models.
@@ -161,15 +160,15 @@
         self
             Returns self.
         """
         return super().fit(X_train, Y_train)
 
     def _preprocess_args(
             self,
-            X: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]',
+            X: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, Any, List[Any]]',
             Y: 'Optional[Union[np.ndarray, tensorflow.Tensor, torch.Tensor]]' = None) \
             -> 'Union[Tuple[torch.Tensor, torch.Tensor], Tuple[tensorflow.Tensor, tensorflow.Tensor]]':
         """Formats `X`, `Y` for explain method.
 
         Parameters
         ----------
         X
@@ -201,28 +200,29 @@
         if isinstance(Y, np.ndarray):
             Y = self.backend.to_tensor(Y)
 
         return X, Y
 
     def explain(
             self,
-            X: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor]',
+            X: 'Union[np.ndarray, tensorflow.Tensor, torch.Tensor, Any, List[Any]]',
             Y: 'Optional[Union[np.ndarray, tensorflow.Tensor, torch.Tensor]]' = None) -> "Explanation":
         """Explain the predictor's predictions for a given input.
 
         Computes the similarity score between the inputs and the training set. Returns an explainer object
         containing the scores, the indices of the training set instances sorted by descending similarity and the
         most similar and least similar instances of the data set for the input. Note that the input may be a single
         instance or a batch of instances.
 
         Parameters
         ----------
         X
-            `X` can be a `numpy` array, `tensorflow` tensor, or `pytorch` tensor of the same shape as the training data
-            with or without a leading batch dimension. If the batch dimension is missing it's added.
+            `X` can be a `numpy` array, `tensorflow` tensor, `pytorch` tensor of the same shape as the training data
+            or a list of objects, with or without a leading batch dimension. If the batch dimension is missing it's
+            added.
         Y
             `Y` can be a `numpy` array, `tensorflow` tensor or a `pytorch` tensor. In the case of a regression task, the
             `Y` argument must be present. If the task is classification then `Y` defaults to the model prediction.
 
         Returns
         -------
         `Explanation` object containing the ordered similarity scores for the test instance(s) with additional \
@@ -245,15 +245,15 @@
         ValueError
             If the fit method has not been called prior to calling this method.
         """
         self._verify_fit()
         X, Y = self._preprocess_args(X, Y)
         test_grads = []
         for x, y in zip(X, Y):
-            test_grads.append(self._compute_grad(x[None], y[None])[None])
+            test_grads.append(self._compute_grad(self._format(x), y[None])[None])
         grads_X_test = np.concatenate(np.array(test_grads), axis=0)
         if not self.precompute_grads:
             scores = self._compute_adhoc_similarity(grads_X_test)
         else:
             scores = self.sim_fn(grads_X_test, self.grad_X_train)
         return self._build_explanation(scores)
 
@@ -263,15 +263,28 @@
         Parameters
         ----------
         scores
             The scores for each of the instances in the data set computed by the similarity method.
         """
         data = copy.deepcopy(DEFAULT_DATA_SIM)
         sorted_score_indices = np.argsort(scores)[:, ::-1]
-        broadcast_indices = np.expand_dims(sorted_score_indices, axis=tuple(range(2, len(self.X_train[None].shape))))
+        most_similar: Union[np.ndarray, List[Any]]
+        least_similar: Union[np.ndarray, List[Any]]
+
+        if isinstance(self.X_train, np.ndarray):
+            broadcast_indices = np.expand_dims(
+                sorted_score_indices,
+                axis=tuple(range(2, len(self.X_train[None].shape)))
+            )
+            most_similar = np.take_along_axis(self.X_train[None], broadcast_indices[:, :5], axis=1)
+            least_similar = np.take_along_axis(self.X_train[None], broadcast_indices[:, -1:-6:-1], axis=1)
+        else:
+            most_similar = [[self.X_train[i] for i in ssi[:5]] for ssi in sorted_score_indices]
+            least_similar = [[self.X_train[i] for i in ssi[-1:-6:-1]] for ssi in sorted_score_indices]
+
         data.update(
             scores=np.take_along_axis(scores, sorted_score_indices, axis=1),
             ordered_indices=sorted_score_indices,
-            most_similar=np.take_along_axis(self.X_train[None], broadcast_indices[:, :5], axis=1),
-            least_similar=np.take_along_axis(self.X_train[None], broadcast_indices[:, -1:-6:-1], axis=1),
+            most_similar=most_similar,
+            least_similar=least_similar
         )
         return Explanation(meta=self.meta, data=data)
```

### Comparing `alibi-0.9.1/alibi/explainers/similarity/metrics.py` & `alibi-0.9.2/alibi/explainers/similarity/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/conftest.py` & `alibi-0.9.2/alibi/explainers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_ale.py` & `alibi-0.9.2/alibi/explainers/tests/test_ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_anchor_base.py` & `alibi-0.9.2/alibi/explainers/tests/test_anchor_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
                          ids='clf=rf_{}'.format,
                          )
 @pytest.mark.parametrize('at_defaults', (0.9, 0.95), indirect=True)
 def test_anchor_base_beam(rf_classifier, at_defaults, at_iris_explainer):
     # inputs
     n_anchors_to_sample = 6
     coverage_samples = 500
-    dummy_coverage = - 0.55  # used to test coverage updates on sampling
 
     X_test, explainer, predict_fn, predict_type = at_iris_explainer
     explain_defaults = at_defaults
     threshold = explain_defaults['desired_confidence']
     explanation = explainer.explain(X_test[0], threshold=threshold, **explain_defaults)
     anchor_beam = explainer.mab
 
@@ -33,23 +32,18 @@
     to_sample = []
     for _ in range(n_anchors_to_sample):
         anchor_len = np.random.randint(0, anchor_max_len)
         anchor = np.random.choice(anchor_features, anchor_len, replace=False)
         to_sample.append(tuple(anchor))
     to_sample = list(set(to_sample))
     current_state = deepcopy(anchor_beam.state)
-    for anchor in to_sample:
-        if anchor not in current_state['t_nsamples']:
-            anchor_beam.state['t_coverage'][anchor] = dummy_coverage
     pos, total = anchor_beam.draw_samples(to_sample, explain_defaults['batch_size'])
     for p, t, anchor in zip(pos, total, to_sample):
         assert anchor_beam.state['t_nsamples'][anchor] == current_state['t_nsamples'][anchor] + t
         assert anchor_beam.state['t_positives'][anchor] == current_state['t_positives'][anchor] + p
-        if anchor:  # empty anchor has dummy coverage
-            assert anchor_beam.state['t_coverage'][anchor] != dummy_coverage
 
     # testing resampling works
     # by sampling all features, we are guaranteed that partial anchors might not exist
     feat_set = tuple(range(anchor_max_len))
     pos, total = anchor_beam.draw_samples([feat_set], explain_defaults['batch_size'])
     assert 'placeholder' not in explanation['raw']['examples']
     assert -1 not in explanation['raw']['coverage']
```

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_anchor_image.py` & `alibi-0.9.2/alibi/explainers/tests/test_anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_anchor_tabular.py` & `alibi-0.9.2/alibi/explainers/tests/test_anchor_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_anchor_text.py` & `alibi-0.9.2/alibi/explainers/tests/test_anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_cem.py` & `alibi-0.9.2/alibi/explainers/tests/test_cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_cfproto.py` & `alibi-0.9.2/alibi/explainers/tests/test_cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_cfrl.py` & `alibi-0.9.2/alibi/explainers/tests/test_cfrl.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_counterfactual.py` & `alibi-0.9.2/alibi/explainers/tests/test_counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_integrated_gradients.py` & `alibi-0.9.2/alibi/explainers/tests/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_partial_dependence.py` & `alibi-0.9.2/alibi/explainers/tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_pd_variance.py` & `alibi-0.9.2/alibi/explainers/tests/test_pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_permutation_importance.py` & `alibi-0.9.2/alibi/explainers/tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_shap_wrappers.py` & `alibi-0.9.2/alibi/explainers/tests/test_shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_simiarlity/conftest.py` & `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_simiarlity/test_backends.py` & `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_backends.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py` & `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py` & `alibi-0.9.2/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/explainers/tests/utils.py` & `alibi-0.9.2/alibi/explainers/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/actor_critic.py` & `alibi-0.9.2/alibi/models/pytorch/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/autoencoder.py` & `alibi-0.9.2/alibi/models/pytorch/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/cfrl_models.py` & `alibi-0.9.2/alibi/models/pytorch/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/metrics.py` & `alibi-0.9.2/alibi/models/pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/model.py` & `alibi-0.9.2/alibi/models/pytorch/model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/tests/test_actor_critic.py` & `alibi-0.9.2/alibi/models/pytorch/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/tests/test_autoencoder.py` & `alibi-0.9.2/alibi/models/pytorch/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/tests/test_cfrl_models.py` & `alibi-0.9.2/alibi/models/pytorch/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/tests/test_metrics.py` & `alibi-0.9.2/alibi/models/pytorch/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/pytorch/tests/test_model.py` & `alibi-0.9.2/alibi/models/pytorch/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/tensorflow/actor_critic.py` & `alibi-0.9.2/alibi/models/tensorflow/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/tensorflow/autoencoder.py` & `alibi-0.9.2/alibi/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/tensorflow/cfrl_models.py` & `alibi-0.9.2/alibi/models/tensorflow/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/tensorflow/tests/test_actor_critic.py` & `alibi-0.9.2/alibi/models/tensorflow/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/tensorflow/tests/test_autoencoder.py` & `alibi-0.9.2/alibi/models/tensorflow/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/models/tensorflow/tests/test_cfrl_models.py` & `alibi-0.9.2/alibi/models/tensorflow/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/prototypes/protoselect.py` & `alibi-0.9.2/alibi/prototypes/protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/prototypes/tests/test_protoselect.py` & `alibi-0.9.2/alibi/prototypes/tests/test_protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/prototypes/tests/test_utils.py` & `alibi-0.9.2/alibi/prototypes/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/saving.py` & `alibi-0.9.2/alibi/saving.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import json
+import numbers
 import os
 from pathlib import Path
 import sys
 from typing import Callable, TYPE_CHECKING, Union
 import warnings
 
 import dill
@@ -119,29 +120,38 @@
         explainer = dill.load(f)
     explainer.reset_predictor(predictor)
     return explainer
 
 
 def _load_IntegratedGradients(path: Union[str, os.PathLike], predictor: 'Union[tensorflow.keras.Model]',
                               meta: dict) -> 'IntegratedGradients':
-    layer_num = meta['params']['layer']
-    if layer_num == 0:
-        layer = None
-    else:
-        layer = predictor.layers[layer_num]
-
+    from alibi.explainers.integrated_gradients import LayerState
     with open(Path(path, 'explainer.dill'), 'rb') as f:
         explainer = dill.load(f)
+
     explainer.reset_predictor(predictor)
-    explainer.layer = layer
+    layer_meta = meta['params']['layer']
+
+    if layer_meta == LayerState.CALLABLE:
+        explainer.layer = explainer.callable_layer(predictor)
+    elif isinstance(layer_meta, numbers.Integral):
+        explainer.layer = predictor.layers[layer_meta]
 
     return explainer
 
 
 def _save_IntegratedGradients(explainer: 'IntegratedGradients', path: Union[str, os.PathLike]) -> None:
+    from alibi.explainers.integrated_gradients import LayerState
+    from alibi.exceptions import SerializationError
+
+    if explainer.meta['params']['layer'] == LayerState.NON_SERIALIZABLE:
+        raise SerializationError('The layer provided in the explainer initialization cannot be serialized. This is due '
+                                 'to nested layers. To permit the serialization of the explainer, provide the layer as '
+                                 'a callable which returns the layer given the model.')
+
     model = explainer.model
     layer = explainer.layer
     explainer.model = explainer.layer = None
     with open(Path(path, 'explainer.dill'), 'wb') as f:
         dill.dump(explainer, f, recurse=True)
     explainer.model = model
     explainer.layer = layer
```

### Comparing `alibi-0.9.1/alibi/tests/conftest.py` & `alibi-0.9.2/alibi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/tests/test_dep_management.py` & `alibi-0.9.2/alibi/tests/test_dep_management.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/tests/test_saving.py` & `alibi-0.9.2/alibi/tests/test_saving.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numbers
 import sys
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 from pytest_lazyfixture import lazy_fixture
 from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
@@ -16,14 +17,15 @@
     AnchorText,
     IntegratedGradients,
     KernelShap,
     TreeShap,
     CounterfactualRLTabular,
     GradientSimilarity
 )
+from alibi.explainers.integrated_gradients import LayerState
 from alibi.saving import load_explainer
 from alibi_testing.data import get_adult_data, get_iris_data, get_movie_sentiment_data
 import alibi_testing
 from alibi.utils.download import spacy_model
 from alibi.explainers.tests.utils import predict_fcn
 
 
@@ -137,17 +139,28 @@
 @pytest.fixture(scope='module')
 def ale_explainer(iris_data, lr_classifier):
     ale = ALE(predictor=lr_classifier.predict_proba,
               feature_names=iris_data['metadata']['feature_names'])
     return ale
 
 
-@pytest.fixture(scope='module')
-def ig_explainer(iris_data, ffn_classifier):
-    ig = IntegratedGradients(model=ffn_classifier)
+@pytest.fixture(scope='module',
+                params=[LayerState.UNSPECIFIED, LayerState.CALLABLE, 1])
+def ig_explainer(request, iris_data, ffn_classifier):
+    layer_meta = request.param
+
+    if layer_meta == LayerState.CALLABLE:
+        def layer(model):
+            return model.layers[1]
+    elif isinstance(layer_meta, numbers.Integral):
+        layer = ffn_classifier.layers[layer_meta]
+    else:
+        layer = None
+
+    ig = IntegratedGradients(model=ffn_classifier, layer=layer)
     return ig
 
 
 def mnist_segmentation_fn(image, size=(4, 7)):
     segments = np.zeros([image.shape[0], image.shape[1]])
     row_idx, col_idx = np.where(segments == 0)
     for i, j in zip(row_idx, col_idx):
@@ -310,16 +323,35 @@
     exp0 = ig_explainer.explain(X, target=target)
 
     with tempfile.TemporaryDirectory() as temp_dir:
         ig_explainer.save(temp_dir)
         ig_explainer1 = load_explainer(temp_dir, predictor=ffn_classifier)
 
         assert isinstance(ig_explainer1, IntegratedGradients)
+
+        # need to remove the layer entry since it can be a callable.
+        # Although the callable are identical, they have different addresses in memory
+        layer = ig_explainer.meta['params']['layer']
+        layer1 = ig_explainer1.meta['params']['layer']
+        del ig_explainer.meta['params']['layer']
+        del ig_explainer1.meta['params']['layer']
+
+        # compare metadata
         assert ig_explainer.meta == ig_explainer1.meta
 
+        # compare layers
+        if callable(layer):
+            assert layer.__code__ == layer1.__code__
+        else:
+            assert layer == layer1
+
+        # insert layers back in case the `ig_explainer` will be used in the future
+        ig_explainer.meta['params']['layer'] = layer
+        ig_explainer1.meta['params']['layer'] = layer1
+
         exp1 = ig_explainer.explain(X, target=target)
         assert exp0.meta == exp1.meta
 
         # IG is deterministic
         assert np.all(exp0.attributions[0] == exp1.attributions[0])
```

### Comparing `alibi-0.9.1/alibi/tests/test_utils.py` & `alibi-0.9.2/alibi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/tests/utils.py` & `alibi-0.9.2/alibi/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/__init__.py` & `alibi-0.9.2/alibi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/approximation_methods.py` & `alibi-0.9.2/alibi/utils/approximation_methods.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/data.py` & `alibi-0.9.2/alibi/utils/data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/discretizer.py` & `alibi-0.9.2/alibi/utils/discretizer.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/distance.py` & `alibi-0.9.2/alibi/utils/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/distributed.py` & `alibi-0.9.2/alibi/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/distributions.py` & `alibi-0.9.2/alibi/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/download.py` & `alibi-0.9.2/alibi/utils/download.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/gradients.py` & `alibi-0.9.2/alibi/utils/gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/kernel.py` & `alibi-0.9.2/alibi/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/lang_model.py` & `alibi-0.9.2/alibi/utils/lang_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/mapping.py` & `alibi-0.9.2/alibi/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/missing_optional_dependency.py` & `alibi-0.9.2/alibi/utils/missing_optional_dependency.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tests/test_data.py` & `alibi-0.9.2/alibi/utils/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tests/test_distance.py` & `alibi-0.9.2/alibi/utils/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tests/test_distributed.py` & `alibi-0.9.2/alibi/utils/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tests/test_gradients.py` & `alibi-0.9.2/alibi/utils/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tests/test_import_optional.py` & `alibi-0.9.2/alibi/utils/tests/test_import_optional.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tests/test_mapping.py` & `alibi-0.9.2/alibi/utils/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/tf.py` & `alibi-0.9.2/alibi/utils/tf.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/visualization.py` & `alibi-0.9.2/alibi/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi/utils/wrappers.py` & `alibi-0.9.2/alibi/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi.egg-info/PKG-INFO` & `alibi-0.9.2/alibi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.1
+Version: 0.9.2
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alibi Version: 0.9.1 Summary: Algorithms for
+Metadata-Version: 2.1 Name: alibi Version: 0.9.2 Summary: Algorithms for
 monitoring and explaining machine learning models Home-page: https://
 github.com/SeldonIO/alibi Author: Seldon Technologies Ltd. Author-email:
 hello@seldon.io License: Apache 2.0 Classifier: Intended Audience :: Science/
 Research Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `alibi-0.9.1/alibi.egg-info/SOURCES.txt` & `alibi-0.9.2/alibi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/alibi.egg-info/requires.txt` & `alibi-0.9.2/alibi.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 numpy<2.0.0,>=1.16.2
-pandas<2.0.0,>=0.23.3
+pandas<3.0.0,>=1.0.0
 scikit-learn<2.0.0,>=1.0.0
 spacy[lookups]<4.0.0,>=2.0.0
 blis<0.8.0
-scikit-image<0.20,>=0.17.2
+scikit-image<0.21,>=0.17.2
 requests<3.0.0,>=2.21.0
 Pillow<10.0,>=5.4.1
-attrs<23.0.0,>=19.2.0
+attrs<24.0.0,>=19.2.0
 scipy<2.0.0,>=1.1.0
 matplotlib<4.0.0,>=3.0.0
 typing-extensions>=3.7.4.3
 dill<0.4.0,>=0.3.0
 transformers<5.0.0,>=4.7.0
 tqdm<5.0.0,>=4.28.1
 
 [all]
 ray<3.0.0,>=0.8.7
 shap<0.42.0,>=0.40.0
 numba!=0.54.0,<0.57.0,>=0.50.0
-tensorflow!=2.6.0,!=2.6.1,<2.11.0,>=2.0.0
+tensorflow!=2.6.0,!=2.6.1,<2.13.0,>=2.0.0
 torch<2.0.0,>=1.9.0
 
 [ray]
 ray<3.0.0,>=0.8.7
 
 [shap]
 shap<0.42.0,>=0.40.0
 numba!=0.54.0,<0.57.0,>=0.50.0
 
 [tensorflow]
-tensorflow!=2.6.0,!=2.6.1,<2.11.0,>=2.0.0
+tensorflow!=2.6.0,!=2.6.1,<2.13.0,>=2.0.0
 
 [torch]
 torch<2.0.0,>=1.9.0
```

### Comparing `alibi-0.9.1/setup.cfg` & `alibi-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `alibi-0.9.1/setup.py` & `alibi-0.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 extras_require = {
     'ray': ['ray>=0.8.7, <3.0.0'],
     # shap is separated due to build issues, see https://github.com/slundberg/shap/pull/1802
     'shap': [
         'shap>=0.40.0, <0.42.0',  # versioning: https://github.com/SeldonIO/alibi/issues/333
         'numba>=0.50.0, !=0.54.0, <0.57.0',  # Avoid 0.54 due to: https://github.com/SeldonIO/alibi/issues/466
     ],
-    'tensorflow': ['tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.11.0'],
+    'tensorflow': ['tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.13.0'],
     'torch': ['torch>=1.9.0, <2.0.0'],
     'all': [
         'ray>=0.8.7, <3.0.0',
         'shap>=0.40.0, <0.42.0',
         'numba>=0.50.0, !=0.54.0, <0.57.0',
-        'tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.11.0',
+        'tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.13.0',
         'torch>=1.9.0, <2.0.0'
     ]
 }
 
 if __name__ == '__main__':
     setup(name='alibi',
           author='Seldon Technologies Ltd.',
@@ -39,22 +39,22 @@
           license="Apache 2.0",
           packages=find_packages(),
           include_package_data=True,
           python_requires='>=3.7',
           # lower bounds based on Debian Stable versions where available
           install_requires=[
               'numpy>=1.16.2, <2.0.0',
-              'pandas>=0.23.3, <2.0.0',
+              'pandas>=1.0.0, <3.0.0',
               'scikit-learn>=1.0.0, <2.0.0',
               'spacy[lookups]>=2.0.0, <4.0.0',
               'blis<0.8.0',  # Windows memory issues https://github.com/explosion/thinc/issues/771
-              'scikit-image>=0.17.2, <0.20',  # introduced `start_label` argument for `slic`
+              'scikit-image>=0.17.2, <0.21',  # introduced `start_label` argument for `slic`
               'requests>=2.21.0, <3.0.0',
               'Pillow>=5.4.1, <10.0',
-              'attrs>=19.2.0, <23.0.0',
+              'attrs>=19.2.0, <24.0.0',
               'scipy>=1.1.0, <2.0.0',
               'matplotlib>=3.0.0, <4.0.0',
               'typing-extensions>=3.7.4.3',
               'dill>=0.3.0, <0.4.0',
               'transformers>=4.7.0, <5.0.0',
               'tqdm>=4.28.1, <5.0.0',
           ],
```

