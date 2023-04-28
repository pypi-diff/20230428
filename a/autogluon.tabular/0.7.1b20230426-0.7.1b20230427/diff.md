# Comparing `tmp/autogluon.tabular-0.7.1b20230426.tar.gz` & `tmp/autogluon.tabular-0.7.1b20230427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.1b20230426.tar", last modified: Wed Apr 26 09:04:16 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.7.1b20230427.tar", last modified: Thu Apr 27 09:04:09 2023, max compression
```

## Comparing `autogluon.tabular-0.7.1b20230426.tar` & `autogluon.tabular-0.7.1b20230427.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.474595 autogluon.tabular-0.7.1b20230426/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-26 09:04:16.474595 autogluon.tabular-0.7.1b20230426/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:04:16.474595 autogluon.tabular-0.7.1b20230426/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.442595 autogluon.tabular-0.7.1b20230426/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.450595 autogluon.tabular-0.7.1b20230426/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.450595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.450595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.450595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.454595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.454595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.454595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.454595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.454595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.454595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.458595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.462595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.462595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.462595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.462595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36321 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.462595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.466595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.466595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.466595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.466595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.466595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    37284 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.466595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   249695 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.470595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.474595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.474595 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-26 09:03:35.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:16.450595 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:04:16.000000 autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.305563 autogluon.tabular-0.7.1b20230427/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-27 09:04:09.305563 autogluon.tabular-0.7.1b20230427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:04:09.305563 autogluon.tabular-0.7.1b20230427/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.285563 autogluon.tabular-0.7.1b20230427/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.289563 autogluon.tabular-0.7.1b20230427/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.289563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.293563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36321 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.297563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37284 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.301563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   249695 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.305563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.305563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.305563 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-27 09:03:38.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:04:09.289563 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:04:09.000000 autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.7.1b20230426/PKG-INFO` & `autogluon.tabular-0.7.1b20230427/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230426
+Version: 0.7.1b20230427
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230426/setup.py` & `autogluon.tabular-0.7.1b20230427/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """ Default (fixed) hyperparameter values used in Gradient Boosting model. """
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 DEFAULT_NUM_BOOST_ROUND = 10000  # default for single training run
 
 
 def get_lgb_objective(problem_type):
     return {
         BINARY: 'binary',
         MULTICLASS: 'multiclass',
+        QUANTILE: 'quantile',
         REGRESSION: 'regression',
         SOFTCLASS: 'multiclass',
     }[problem_type]
 
 
 def get_param_baseline_custom(problem_type):
     if problem_type == BINARY:
```

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 import numpy as np
 from pandas import DataFrame, Series
 
 from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 from autogluon.core.models import AbstractModel
 from autogluon.core.models._utils import get_early_stopping_rounds
 from autogluon.common.utils.try_import import try_import_lightgbm
 
 from . import lgb_utils
 from .hyperparameters.parameters import get_param_baseline, get_lgb_objective, DEFAULT_NUM_BOOST_ROUND
 from .hyperparameters.searchspaces import get_default_searchspace
-from .lgb_utils import construct_dataset
+from .lgb_utils import construct_dataset, train_lgb_model
 
 warnings.filterwarnings("ignore", category=UserWarning, message="Starting from version")  # lightGBM brew libomp warning
 logger = logging.getLogger(__name__)
 
 
 # TODO: Save dataset to binary and reload for HPO. This will avoid the memory spike overhead when training each model and instead it will only occur once upon saving the dataset.
 class LGBModel(AbstractModel):
@@ -136,21 +136,35 @@
             reporter = kwargs.get('reporter', None)
             train_loss_name = self._get_train_loss_name() if reporter is not None else None
             if train_loss_name is not None:
                 if 'metric' not in params or params['metric'] == '':
                     params['metric'] = train_loss_name
                 elif train_loss_name not in params['metric']:
                     params['metric'] = f'{params["metric"]},{train_loss_name}'
+            # early stopping callback will be added later by QuantileBooster if problem_type==QUANTILE
+            early_stopping_callback_kwargs = dict(
+                stopping_rounds=early_stopping_rounds,
+                metrics_to_use=[('valid_set', stopping_metric_name)],
+                max_diff=None,
+                start_time=start_time,
+                time_limit=time_limit,
+                ignore_dart_warning=True,
+                verbose=False,
+                manual_stop_file=False,
+                reporter=reporter,
+                train_loss_name=train_loss_name,
+            )
             callbacks += [
                 # Note: Don't use self.params_aux['max_memory_usage_ratio'] here as LightGBM handles memory per iteration optimally.  # TODO: Consider using when ratio < 1.
-                early_stopping_custom(early_stopping_rounds, metrics_to_use=[('valid_set', stopping_metric_name)], max_diff=None, start_time=start_time, time_limit=time_limit,
-                                      ignore_dart_warning=True, verbose=False, manual_stop_file=False, reporter=reporter, train_loss_name=train_loss_name),
+                early_stopping_custom(**early_stopping_callback_kwargs)
             ]
             valid_names = ['valid_set'] + valid_names
             valid_sets = [dataset_val] + valid_sets
+        else:
+            early_stopping_callback_kwargs = None
         from lightgbm.callback import log_evaluation
         if log_period is not None:
             callbacks.append(log_evaluation(period=log_period))
 
         seed_val = params.pop('seed_value', 0)
         train_params = {
             'params': params,
@@ -165,55 +179,56 @@
         else:
             if 'metric' not in train_params['params'] or train_params['params']['metric'] == '':
                 train_params['params']['metric'] = stopping_metric
             elif stopping_metric not in train_params['params']['metric']:
                 train_params['params']['metric'] = f'{train_params["params"]["metric"]},{stopping_metric}'
         if self.problem_type == SOFTCLASS:
             train_params['fobj'] = lgb_utils.softclass_lgbobj
+        elif self.problem_type == QUANTILE:
+            train_params['params']['quantile_levels'] = self.quantile_levels
         if seed_val is not None:
             train_params['params']['seed'] = seed_val
             random.seed(seed_val)
             np.random.seed(seed_val)
 
         # Train LightGBM model:
-        import lightgbm as lgb
         from lightgbm.basic import LightGBMError
         with warnings.catch_warnings():
             # Filter harmless warnings introduced in lightgbm 3.0, future versions plan to remove: https://github.com/microsoft/LightGBM/issues/3379
             warnings.filterwarnings('ignore', message='Overriding the parameters from Reference Dataset.')
             warnings.filterwarnings('ignore', message='categorical_column in param dict is overridden.')
             try:
-                self.model = lgb.train(**train_params)
+                self.model = train_lgb_model(early_stopping_callback_kwargs=early_stopping_callback_kwargs, **train_params)
             except LightGBMError:
                 if train_params['params'].get('device', 'cpu') != 'gpu':
                     raise
                 else:
                     logger.warning('Warning: GPU mode might not be installed for LightGBM, GPU training raised an exception. Falling back to CPU training...'
                                    'Refer to LightGBM GPU documentation: https://github.com/Microsoft/LightGBM/tree/master/python-package#build-gpu-version'
                                    'One possible method is:'
                                    '\tpip uninstall lightgbm -y'
                                    '\tpip install lightgbm --install-option=--gpu'
                                    )
                     train_params['params']['device'] = 'cpu'
-                    self.model = lgb.train(**train_params)
+                    self.model = train_lgb_model(early_stopping_callback_kwargs=early_stopping_callback_kwargs, **train_params)
             retrain = False
             if train_params['params'].get('boosting_type', '') == 'dart':
                 if dataset_val is not None and dart_retrain and (self.model.best_iteration != num_boost_round):
                     retrain = True
                     if time_limit is not None:
                         time_left = time_limit + start_time - time.time()
                         if time_left < 0.5 * time_limit:
                             retrain = False
                     if retrain:
                         logger.log(15, f"Retraining LGB model to optimal iterations ('dart' mode).")
                         train_params.pop('callbacks', None)
                         train_params.pop('valid_sets', None)
                         train_params.pop('valid_names', None)
                         train_params['num_boost_round'] = self.model.best_iteration
-                        self.model = lgb.train(**train_params)
+                        self.model = train_lgb_model(**train_params)
                     else:
                         logger.log(15, f"Not enough time to retrain LGB model ('dart' mode)...")
 
         if dataset_val is not None and not retrain:
             self.params_trained['num_boost_round'] = self.model.best_iteration
         else:
             self.params_trained['num_boost_round'] = self.model.current_iteration()
@@ -320,29 +335,29 @@
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             valid_raw_types=[R_BOOL, R_INT, R_FLOAT, R_CATEGORY],
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
-    
+
     def _is_gpu_lgbm_installed(self):
         # Taken from https://github.com/microsoft/LightGBM/issues/3939
         try_import_lightgbm()
         import lightgbm
         try:
             data = np.random.rand(50, 2)
             label = np.random.randint(2, size=50)
             train_data = lightgbm.Dataset(data, label=label)
             params = {'device': 'gpu'}
             gbm = lightgbm.train(params, train_set=train_data, verbose=-1)
             return True
         except Exception as e:
             return False
-    
+
     def get_minimum_resources(self, is_gpu_available=False):
         minimum_resources = {
             'num_cpus': 1,
         }
         if is_gpu_available and self._is_gpu_lgbm_installed():
             minimum_resources['num_gpus'] = 0.5
         return minimum_resources
```

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     CAT=60,
     custom=0,
 )
 
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
 
 # FIXME: v0.7 : Remove this, it is a hack. Model classes should define what problem types they support instead of using this
-DEFAULT_QUANTILE_MODEL = ['DUMMY', 'RF', 'XT', 'FASTAI', 'NN_TORCH', 'ENS_WEIGHTED', 'CAT']  # TODO: OTHERS will be added
+DEFAULT_QUANTILE_MODEL = ['DUMMY', 'RF', 'XT', 'FASTAI', 'NN_TORCH', 'ENS_WEIGHTED', 'CAT', 'GBM']  # TODO: OTHERS will be added
 
 MODEL_TYPES = dict(
     RF=RFModel,
     XT=XTModel,
     KNN=KNNModel,
     GBM=LGBModel,
     CAT=CatBoostModel,
```

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.7.1b20230427/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230426
+Version: 0.7.1b20230427
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230426/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.7.1b20230427/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

