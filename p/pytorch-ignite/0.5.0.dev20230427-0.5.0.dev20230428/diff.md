# Comparing `tmp/pytorch-ignite-0.5.0.dev20230427.tar.gz` & `tmp/pytorch-ignite-0.5.0.dev20230428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.5.0.dev20230427.tar", last modified: Thu Apr 27 00:14:22 2023, max compression
+gzip compressed data, was "pytorch-ignite-0.5.0.dev20230428.tar", last modified: Fri Apr 28 00:15:39 2023, max compression
```

## Comparing `pytorch-ignite-0.5.0.dev20230427.tar` & `pytorch-ignite-0.5.0.dev20230428.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.918102 pytorch-ignite-0.5.0.dev20230427/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-27 00:14:22.918102 pytorch-ignite-0.5.0.dev20230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.906102 pytorch-ignite-0.5.0.dev20230427/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 00:10:38.000000 pytorch-ignite-0.5.0.dev20230427/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.906102 pytorch-ignite-0.5.0.dev20230427/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.906102 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.906102 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.910102 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    37623 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21622 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.910102 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.910102 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.910102 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.910102 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.914102 pytorch-ignite-0.5.0.dev20230427/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.914102 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44800 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    62888 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/handlers/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.914102 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.918102 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    24270 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/multilabel_confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.918102 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:14:22.918102 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-27 00:14:22.000000 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-27 00:14:22.000000 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:14:22.000000 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:14:22.000000 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 00:14:22.000000 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 00:14:22.000000 pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-27 00:14:22.918102 pytorch-ignite-0.5.0.dev20230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-27 00:10:11.000000 pytorch-ignite-0.5.0.dev20230427/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 00:11:11.000000 pytorch-ignite-0.5.0.dev20230428/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.905848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37623 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21622 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.905848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.913848 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44800 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62888 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24270 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/multilabel_confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 00:15:39.921848 pytorch-ignite-0.5.0.dev20230428/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/setup.py
```

### Comparing `pytorch-ignite-0.5.0.dev20230427/LICENSE` & `pytorch-ignite-0.5.0.dev20230428/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230428/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230427
+Version: 0.5.0.dev20230428
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch Core Team
 Author-email: soumith@pytorch.org
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.dev20230427/README.md` & `pytorch-ignite-0.5.0.dev20230428/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/base/mixins.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/engines/common.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/common.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/engines/tbptt.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/base_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/clearml_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/mlflow_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/neptune_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/tqdm_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/visdom_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/handlers/wandb_logger.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/average_precision.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/cohen_kappa.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/gpu_info.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/__init__.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/_base.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/mean_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/r2_score.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/contrib/metrics/roc_auc.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/auto.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/__init__.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/base.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/horovod.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/native.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/comp_models/xla.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/launcher.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/distributed/utils.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+from contextlib import contextmanager
 from functools import wraps
 from typing import Any, Callable, List, Mapping, Optional, Tuple, Union
 
 import torch
 
 from ignite.distributed.comp_models import (
     _SerialModel,
@@ -37,14 +38,15 @@
     "has_xla_support",
     "has_native_dist_support",
     "has_hvd_support",
     "sync",
     "registered_computation_models",
     "one_rank_only",
     "new_group",
+    "one_rank_first",
 ]
 
 _model = _SerialModel()
 
 _need_to_sync = True
 
 
@@ -631,7 +633,48 @@
             if with_barrier:
                 barrier()
             return ret
 
         return wrapper
 
     return _one_rank_only
+
+
+@contextmanager
+def one_rank_first(rank: int = 0, local: bool = False) -> Any:
+    """Context manager that ensures a specific rank runs first before others in a distributed
+    environment.
+
+    Args:
+        rank: rank of the process that should execute the code
+            block inside the context manager first. Default, 0.
+        local: flag to specify local rank or global rank.
+            If True ``rank`` argument will define a local rank to run first.
+            Default, False
+
+    Examples:
+        .. code-block:: python
+
+            def download_dataset():
+                ...
+
+            with idist.one_rank_first():
+                ds = download_dataset()
+
+            dp = ds[0]
+
+    .. versionadded:: 0.5.0
+    """
+
+    current_rank = get_local_rank() if local else get_rank()
+    size = get_nproc_per_node() if local else get_world_size()
+
+    if rank >= size or rank < 0:
+        raise ValueError(f"rank should be between 0 and {size - 1}, but given {rank}")
+
+    if current_rank != rank:
+        barrier()
+
+    yield
+
+    if current_rank == rank:
+        barrier()
```

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/engine/__init__.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/engine/deterministic.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/engine/engine.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/engine/events.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/engine/utils.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/checkpoint.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/early_stopping.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/ema_handler.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/state_param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/stores.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/terminate_on_nan.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/time_limit.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/handlers/timing.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/__init__.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/accumulation.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/accuracy.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/classification_report.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/epoch_metric.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/fbeta.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/frequency.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/fid.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/inception_score.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/gan/utils.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/loss.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/mean_pairwise_distance.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/metric.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/metrics_lambda.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/bleu.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/rouge.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/nlp/utils.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/precision.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/psnr.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/recall.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/root_mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/running_average.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/ssim.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/ignite/utils.py` & `pytorch-ignite-0.5.0.dev20230428/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/pyproject.toml` & `pytorch-ignite-0.5.0.dev20230428/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230427
+Version: 0.5.0.dev20230428
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch Core Team
 Author-email: soumith@pytorch.org
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.dev20230427/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/setup.cfg` & `pytorch-ignite-0.5.0.dev20230428/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230427/setup.py` & `pytorch-ignite-0.5.0.dev20230428/setup.py`

 * *Files identical despite different names*

