# Comparing `tmp/autogluon.core-0.7.1b20230427.tar.gz` & `tmp/autogluon.core-0.7.1b20230428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.1b20230427.tar", last modified: Thu Apr 27 09:03:55 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.1b20230428.tar", last modified: Fri Apr 28 09:03:58 2023, max compression
```

## Comparing `autogluon.core-0.7.1b20230427.tar` & `autogluon.core-0.7.1b20230428.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.981448 autogluon.core-0.7.1b20230427/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-27 09:03:55.981448 autogluon.core-0.7.1b20230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:03:55.981448 autogluon.core-0.7.1b20230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.969453 autogluon.core-0.7.1b20230427/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.969453 autogluon.core-0.7.1b20230427/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27098 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.973451 autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94065 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59618 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40090 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.977450 autogluon.core-0.7.1b20230427/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.981448 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.981448 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.981448 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-27 09:03:38.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:03:55.969453 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:03:55.000000 autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.508342 autogluon.core-0.7.1b20230428/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:03:58.508342 autogluon.core-0.7.1b20230428/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.492342 autogluon.core-0.7.1b20230428/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.496342 autogluon.core-0.7.1b20230428/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.496342 autogluon.core-0.7.1b20230428/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.496342 autogluon.core-0.7.1b20230428/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.496342 autogluon.core-0.7.1b20230428/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.496342 autogluon.core-0.7.1b20230428/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29490 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94028 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.500342 autogluon.core-0.7.1b20230428/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.504342 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-28 09:03:36.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:03:58.496342 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:03:58.000000 autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.1b20230427/PKG-INFO` & `autogluon.core-0.7.1b20230428/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230427
+Version: 0.7.1b20230428
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230427/setup.py` & `autogluon.core-0.7.1b20230428/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/constants.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/dataset.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/executors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import copy
 import logging
 import math
 import os
+import pandas as pd
 import time
 
 from abc import ABC, abstractmethod
-from typing import Optional, List, Dict, Union, Callable
+from typing import Any, Optional, List, Dict, Union, Callable, Tuple
 from autogluon.common.utils.resource_utils import ResourceManager
+from autogluon.common.utils.s3_utils import is_s3_url
 
 from .constants import RAY_BACKEND, CUSTOM_BACKEND
 from .exceptions import EmptySearchSpace
 from .. import Space
 from ..ray.resources_calculator import ResourceCalculator
 from ..scheduler.scheduler_factory import scheduler_factory
+from ..utils.savers import save_pkl
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ..models import AbstractModel
 
 
@@ -189,14 +192,19 @@
                 num_jobs_in_parallel_with_mem = total_memory_available // model_estimate_memory_usage
 
             num_jobs_in_parallel_with_cpu = num_cpus // minimum_model_num_cpus
             num_jobs_in_parallel_with_gpu = math.inf
             if minimum_model_num_gpus > 0:
                 num_jobs_in_parallel_with_gpu = num_gpus // minimum_model_num_gpus
             num_jobs_in_parallel = min(num_jobs_in_parallel_with_mem, num_jobs_in_parallel_with_cpu, num_jobs_in_parallel_with_gpu)
+            if k_fold is not None and k_fold > 0:
+                max_models = self.hyperparameter_tune_kwargs.get("num_trials", math.inf) * k_fold
+                num_jobs_in_parallel = min(num_jobs_in_parallel, max_models)
+            system_num_cpu = ResourceManager.get_cpu_count()
+            system_num_gpu = ResourceManager.get_gpu_count_all()
             if model_base != initialized_model:
                 # bagged model
                 if num_jobs_in_parallel // k_fold < 1:
                     # We can only train 1 trial in parallel
                     num_trials_in_parallel = 1
                 else:
                     num_trials_in_parallel = num_jobs_in_parallel // k_fold
@@ -208,22 +216,26 @@
             else:
                 num_trials = self.hyperparameter_tune_kwargs.get('num_trials', math.inf)
                 if self.executor_type == 'custom':
                     # custom backend runs sequentially
                     num_jobs_in_parallel = 1
                 cpu_per_trial = int(num_cpus // min(num_jobs_in_parallel, num_trials))
                 gpu_per_trial = num_gpus / min(num_jobs_in_parallel, num_trials)
-                
+            # In distributed setting, a single trial could be scheduled with resources that's more than a single node causing hanging
+            # Force it to be less than the current node. This works under the assumption that all nodes are of the same type
+            cpu_per_trial = min(cpu_per_trial, system_num_cpu)
+            gpu_per_trial = min(gpu_per_trial, system_num_gpu)
+            
             self.hyperparameter_tune_kwargs['resources_per_trial'] = {
                 'num_cpus': cpu_per_trial,
                 'num_gpus': gpu_per_trial
             }
 
         self.resources = dict(num_gpus=num_gpus, num_cpus=num_cpus)
-    
+
     @abstractmethod
     def validate_search_space(
             self,
             search_space: dict,
             model_name: str,
         ):
         """
@@ -233,14 +245,59 @@
         ----------
         search_space
             Search space provided to the experiment.
         model_name
             The model name of the hpo experiment is tuning. This is only used for logging purpose
         """
         raise NotImplementedError
+
+    def prepare_data(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        X_val: pd.DataFrame,
+        y_val: pd.Series,
+        path_prefix: str
+    ) -> Tuple[str, str]:
+        """
+        Prepare data as pickle files for hpo trials.
+        If path_prefix is a s3 url, will store to s3. Otherwise, store in local disk
+        
+        Parameters
+        ----------
+        X: pd.DataFrame
+            Training data
+        y: pd.Series
+            Training label
+        X_val: pd.DataFrame
+            Validation data
+        y_val: pd.Series
+            Validation label
+        path_prefix: str
+            path prefix to store the data artifacts
+        
+        Return
+        ------
+        Tuple[str, str]:
+            Path to both the training and validation data
+        """
+        def save_data(data: Any, path_prefix: str, filename: str) -> str:
+            if is_s3_url(path_prefix):
+                path = path_prefix + filename if path_prefix.endswith("/") else path_prefix + f"/{filename}"
+            else:
+                path = os.path.join(path_prefix, filename)
+            save_pkl.save(path=path, object=data, verbose=False)
+            return path
+
+        dataset_train_filename = 'dataset_train.pkl'
+        dataset_val_filename = 'dataset_val.pkl'
+        train_path = save_data(data=(X, y), path_prefix=path_prefix, filename=dataset_train_filename)
+        val_path = save_data(data=(X_val, y_val), path_prefix=path_prefix, filename=dataset_val_filename)
+
+        return train_path, val_path
     
     @abstractmethod
     def execute(self, **kwargs):
         """Execute the experiment"""
         raise NotImplementedError
     
     @abstractmethod
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import shutil
 
+from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.utils.try_import import try_import_ray
 try_import_ray()  # try import ray before importing the remaining contents so we can give proper error messages
 import ray
 
 from autogluon.common.utils.resource_utils import ResourceManager
 from abc import ABC, abstractmethod
 from typing import Optional, Callable, Union, List
@@ -232,32 +233,36 @@
     )
     scheduler = _get_scheduler(
         hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
         supported_schedulers=ray_tune_adapter.get_supported_schedulers()
     )
 
     if not ray.is_initialized():
-        ray.init(
-            log_to_driver=False,
-            runtime_env={"env_vars": {"PL_DISABLE_FORK": "1"}},  # https://github.com/ray-project/ray/issues/28197
-            logging_level=logging.ERROR,  # https://github.com/ray-project/ray/issues/29216
-            **total_resources
-        )
+        if DistributedContext.is_distributed_mode():
+            ray.init(address="auto")
+        else:
+            ray.init(
+                log_to_driver=False,
+                runtime_env={"env_vars": {"PL_DISABLE_FORK": "1"}},  # https://github.com/ray-project/ray/issues/28197
+                logging_level=logging.ERROR,  # https://github.com/ray-project/ray/issues/29216
+                **total_resources
+            )
 
     resources_per_trial = hyperparameter_tune_kwargs.get('resources_per_trial', None)
     resources_per_trial = ray_tune_adapter.get_resources_per_trial(
         total_resources=total_resources,
         num_samples=num_samples,
         resources_per_trial=resources_per_trial,
         minimum_gpu_per_trial=minimum_gpu_per_trial,
         minimum_cpu_per_trial=minimum_cpu_per_trial,
         model_estimate_memory_usage=model_estimate_memory_usage,
         wrap_resources_per_job_into_placement_group=trainable_is_parallel,
     )
     resources_per_trial = _validate_resources_per_trial(resources_per_trial)
+    logger.debug(f"resources_per_trial to be dispatched by ray tune: {resources_per_trial}")
     ray_tune_adapter.resources_per_trial = resources_per_trial
     trainable_args = ray_tune_adapter.trainable_args_update_method(trainable_args)
     
     original_path = os.getcwd()
     save_dir = os.path.normpath(save_dir)
     if tune_config_kwargs is None:
         tune_config_kwargs = dict()
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from autogluon.common.utils.try_import import try_import_ray
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.utils import setup_outputdir
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.log_utils import DuplicateFilter
 from autogluon.common.utils.resource_utils import ResourceManager, RayResourceManager
 from autogluon.common.utils.resource_utils import get_resource_manager
+from autogluon.common.utils.distribute_utils import DistributedContext
 
 from .model_trial import model_trial, skip_hpo
 from ._tags import _DEFAULT_CLASS_TAGS, _DEFAULT_TAGS
 from ... import metrics, Space
 from ...constants import AG_ARG_PREFIX, AG_ARGS_FIT, BINARY, REGRESSION, QUANTILE, REFIT_FULL_SUFFIX, OBJECTIVES_TO_NORMALIZE
 from ...data.label_cleaner import LabelCleaner, LabelCleanerMulticlassToBinary
 from ...hpo.exceptions import EmptySearchSpace
@@ -1372,23 +1373,21 @@
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(self, X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
 
         # Use absolute path here because ray tune will change the working directory
         self.set_contexts(os.path.abspath(self.path) + os.path.sep)
-        directory = self.path  # also create model directory if it doesn't exist
-        # TODO: This will break on S3. Use tabular/utils/savers for datasets, add new function
-        dataset_train_filename = 'dataset_train.pkl'
-        train_path = os.path.join(directory, dataset_train_filename)
-        save_pkl.save(path=train_path, object=(X, y))
-
-        dataset_val_filename = 'dataset_val.pkl'
-        val_path = os.path.join(directory, dataset_val_filename)
-        save_pkl.save(path=val_path, object=(X_val, y_val))
+
+        directory = self.path
+        os.makedirs(directory, exist_ok=True)
+        data_path = directory
+        if DistributedContext.is_distributed_mode():
+            data_path = DistributedContext.get_util_path()
+        train_path, val_path = hpo_executor.prepare_data(X=X, y=y, X_val=X_val, y_val=y_val, path_prefix=data_path)
 
         model_cls = self.__class__
         init_params = self.get_params()
         # We set soft time limit to avoid trials being terminated directly by ray tune
         trial_soft_time_limit = None
         if hpo_executor.time_limit is not None:
             trial_soft_time_limit = max(hpo_executor.time_limit * 0.9, hpo_executor.time_limit - 5)  # 5 seconds max for buffer
@@ -1437,14 +1436,16 @@
             except FileNotFoundError:
                 pass
 
         return hpo_results
     
     def _get_hpo_backend(self):
         """Choose which backend(Ray or Custom) to use for hpo"""
+        if DistributedContext.is_distributed_mode():
+            return RAY_BACKEND
         return CUSTOM_BACKEND
 
     def _get_default_hpo_executor(self) -> HpoExecutor:
         backend = self._get_model_base()._get_hpo_backend()  # If ensemble, will use the base model to determine backend
         if backend == RAY_BACKEND:
             try:
                 try_import_ray()
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1135,23 +1135,20 @@
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
 
         # Use absolute path here because ray tune will change the working directory
         self.set_contexts(os.path.abspath(self.path) + os.path.sep)
-        directory = self.path  # also create model directory if it doesn't exist
-        # TODO: This will break on S3. Use tabular/utils/savers for datasets, add new function
-        dataset_train_filename = 'dataset_train.pkl'
-        train_path = os.path.join(directory, dataset_train_filename)
-        save_pkl.save(path=train_path, object=(X, y))
-
-        dataset_val_filename = 'dataset_val.pkl'
-        val_path = os.path.join(directory, dataset_val_filename)
-        save_pkl.save(path=val_path, object=(X_val, y_val))
+        directory = self.path
+        os.makedirs(directory, exist_ok=True)
+        data_path = directory
+        if DistributedContext.is_distributed_mode():
+            data_path = DistributedContext.get_util_path()
+        train_path, val_path = hpo_executor.prepare_data(X=X, y=y, X_val=X_val, y_val=y_val, path_prefix=data_path)
 
         model_cls = self.__class__
         init_params = copy.deepcopy(self.get_params())
         model_base = self._get_model_base()
 
         if not inspect.isclass(model_base):
             init_params['model_base'] = init_params['model_base'].__class__
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,16 @@
     kwargs_fold: Dict[str, Any],
     head_node_id: str,
     model_sync_path: Optional[str] = None
 ):
     import ray  # ray must be present
     node_id = ray.get_runtime_context().get_node_id()
     is_head_node = node_id == head_node_id
+    logger.debug(f"head node: {is_head_node}")
+    logger.debug(f"executing fold on node {node_id}")
     logger.log(10, 'ray worker training')
     time_start_fold = time.time()
     fold, folds_finished, folds_left, \
         folds_to_fit, is_last_fold, \
         model_name_suffix = FoldFittingStrategy._get_fold_properties(fold_ctx)
     train_index, val_index = fold
     fold_model = copy.deepcopy(model_base)
@@ -516,14 +518,15 @@
         )
 
     def after_all_folds_scheduled(self):
         if not self.ray.is_initialized():
             ray_init_args = self._get_ray_init_args()
             self.ray.init(**ray_init_args)
         head_node_id = self.ray.get_runtime_context().get_node_id()
+        logger.debug(f"Dispatching folds on node {head_node_id}")
         job_refs = []
         job_fold_map = {}
         # prepare shared data
         X, y, X_pseudo, y_pseudo = self._prepare_data()
         model_base_ref = self.ray.put(self.model_base)
         time_limit_fold = self._get_fold_time_limit()
         # spread the task
@@ -628,16 +631,20 @@
         if self.sample_weight is not None:
             if is_pseudo:
                 # TODO: Add support for sample_weight when pseudo is present
                 raise Exception('Sample weights given, but not used due to pseudo labelled data being given.')
             else:
                 kwargs_fold['sample_weight'] = self.sample_weight[train_index]
                 kwargs_fold['sample_weight_val'] = self.sample_weight[val_index]
-        return self._ray_fit.options(**resources) \
-            .remote(
+        pg = self.ray.util.get_current_placement_group()
+        return self._ray_fit.options(
+            **resources,
+            scheduling_strategy=self.ray.util.scheduling_strategies.PlacementGroupSchedulingStrategy(
+                placement_group=pg
+            )).remote(
                 model_base=model_base_ref,
                 bagged_ensemble_model_path=self.bagged_ensemble_model.path,
                 X=X_ref,
                 y=y_ref,
                 X_pseudo=X_pseudo_ref,
                 y_pseudo=y_pseudo_ref,
                 fold_ctx=fold_ctx_ref,
@@ -810,15 +817,15 @@
         pass
     
     
 class ParallelLocalFoldFittingStrategy(ParallelFoldFittingStrategy):
     
     def _get_ray_init_args(self):
         ray_init_args = dict(
-            log_to_driver=True,
+            log_to_driver=False,
             logging_level=logging.ERROR,
             num_cpus=self.num_cpus
         )
         if self.num_gpus > 0:
             ray_init_args['num_gpus'] = self.num_gpus
         return ray_init_args
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/ray/resources_calculator.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,19 @@
         """
         When doing parallel training inside parallel trials, Ray requires to provide placement group for resource scheduling
         We wrap a group where the resource requirement is 0 because the trial only spread the task and doesn't require too much resources.
         """
         from ray import tune
         num_cpus = resources_per_job.get('cpu', 0)
         num_gpus = resources_per_job.get('gpu', 0)
-        return tune.PlacementGroupFactory([{'CPU': 0.0}] + [{'CPU': num_cpus, 'GPU': num_gpus}])
+        # The head bundle doesn't actually require resources.
+        # This memory constraint is a hack (1024 is a random number, unit is bytes) to trick ray to schedule bundles on the same node
+        # Currently we force the trial and its underlying folds being trained on the same node to avoid synchronization
+        # TODO: consider seperate the sub-bundle of folding so they can be scheduled on seperate nodes
+        return tune.PlacementGroupFactory([{"memory": 1024}, {'CPU': num_cpus, 'GPU': num_gpus}], strategy="STRICT_PACK")
 
 
 class CpuResourceCalculator(ResourceCalculator):
 
     @property
     def calc_type(self):
         return 'cpu'
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/space.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.1b20230428/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230427
+Version: 0.7.1b20230428
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230427/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.1b20230428/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

