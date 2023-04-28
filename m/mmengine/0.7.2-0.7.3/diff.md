# Comparing `tmp/mmengine-0.7.2.tar.gz` & `tmp/mmengine-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.7.2.tar", last modified: Thu Apr  6 10:33:28 2023, max compression
+gzip compressed data, was "dist/mmengine-0.7.3.tar", last modified: Fri Apr 28 07:14:41 2023, max compression
```

## Comparing `mmengine-0.7.2.tar` & `mmengine-0.7.3.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-06 10:31:51.000000 mmengine-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-04-06 10:33:28.000000 mmengine-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-04-06 10:31:51.000000 mmengine-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44065 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33957 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42761 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26650 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27397 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    63458 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    25764 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)    99454 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53052 2023-04-06 10:31:51.000000 mmengine-0.7.2/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-04-06 10:33:27.000000 mmengine-0.7.2/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-06 10:33:28.000000 mmengine-0.7.2/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:33:27.000000 mmengine-0.7.2/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-06 10:33:27.000000 mmengine-0.7.2/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 10:33:27.000000 mmengine-0.7.2/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-06 10:33:28.000000 mmengine-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-06 10:31:51.000000 mmengine-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 07:13:18.000000 mmengine-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-04-28 07:14:41.000000 mmengine-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-04-28 07:13:18.000000 mmengine-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33957 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27397 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63458 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25968 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30321 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24176 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100487 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30072 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-04-28 07:13:18.000000 mmengine-0.7.3/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 07:14:41.000000 mmengine-0.7.3/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 07:14:41.000000 mmengine-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-28 07:13:18.000000 mmengine-0.7.3/setup.py
```

### Comparing `mmengine-0.7.2/PKG-INFO` & `mmengine-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.7.2
+Version: 0.7.3
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -84,17 +84,22 @@
         
            - Defines the training process just like playing with Legos.
            - Provides rich components and strategies.
            - Complete controls on the training process with different levels of APIs.
         
         ## What's New
         
-        v0.7.2 was released on 2023-04-06.
+        v0.7.3 was released on 2023-04-28.
         
-        Read [Changelog](./docs/en/notes/changelog.md#v071-04062023) for more details.
+        ### Highlights
+        
+        - Support using MLflow to record experiment data
+        - Support registering callable objects to the registry
+        
+        Read [Changelog](./docs/en/notes/changelog.md#v073-04282023) for more details.
         
         ## Installation
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
         
@@ -333,32 +338,32 @@
         This project is released under the [Apache 2.0 license](LICENSE).
         
         ## Projects in OpenMMLab
         
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-        - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
+        - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+        - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
         - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
         - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
         - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
         - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
         - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
         - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
         - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
         - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
         - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
         - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
         - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+        - [Playground](https://github.com/open-mmlab/playground): A central hub for gathering and showcasing amazing projects built upon OpenMMLab.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mmengine-0.7.2/README.md` & `mmengine-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,22 @@
 
    - Defines the training process just like playing with Legos.
    - Provides rich components and strategies.
    - Complete controls on the training process with different levels of APIs.
 
 ## What's New
 
-v0.7.2 was released on 2023-04-06.
+v0.7.3 was released on 2023-04-28.
 
-Read [Changelog](./docs/en/notes/changelog.md#v071-04062023) for more details.
+### Highlights
+
+- Support using MLflow to record experiment data
+- Support registering callable objects to the registry
+
+Read [Changelog](./docs/en/notes/changelog.md#v073-04282023) for more details.
 
 ## Installation
 
 Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
 
 Install MMEngine
 
@@ -325,25 +330,25 @@
 This project is released under the [Apache 2.0 license](LICENSE).
 
 ## Projects in OpenMMLab
 
 - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
 - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
 - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-- [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
+- [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+- [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
 - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+- [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
 - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
 - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-- [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
 - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
 - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
 - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
 - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
 - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
 - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
 - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-- [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
 - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+- [Playground](https://github.com/open-mmlab/playground): A central hub for gathering and showcasing amazing projects built upon OpenMMLab.
```

### Comparing `mmengine-0.7.2/mmengine/analysis/complexity_analysis.py` & `mmengine-0.7.3/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/analysis/jit_analysis.py` & `mmengine-0.7.3/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/analysis/jit_handles.py` & `mmengine-0.7.3/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/analysis/print_helper.py` & `mmengine-0.7.3/mmengine/analysis/print_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 # Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved.
 # Modified from
 # https://github.com/facebookresearch/fvcore/blob/main/fvcore/nn/print_model_statistics.py
 
 from collections import defaultdict
-from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import torch
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from torch import nn
 
+from mmengine.utils import is_tuple_of
 from .complexity_analysis import (ActivationAnalyzer, FlopAnalyzer,
                                   parameter_count)
 
 
 def _format_size(x: int, sig_figs: int = 3, hide_zero: bool = False) -> str:
     """Formats an integer for printing in a table or model representation.
 
@@ -671,37 +672,78 @@
         max_depth=max_depth,
         stat_columns=stat_columns,
     )
 
 
 def get_model_complexity_info(
     model: nn.Module,
-    input_shape: tuple,
-    inputs: Optional[torch.Tensor] = None,
+    input_shape: Union[Tuple[int, ...], Tuple[Tuple[int, ...], ...],
+                       None] = None,
+    inputs: Union[torch.Tensor, Tuple[torch.Tensor, ...], Tuple[Any, ...],
+                  None] = None,
     show_table: bool = True,
     show_arch: bool = True,
 ):
     """Interface to get the complexity of a model.
 
+    The parameter `inputs` are fed to the forward method of model.
+    If `inputs` is not specified, the `input_shape` is required and
+    it will be used to construct the dummy input fed to model.
+    If the forward of model requires two or more inputs, the `inputs`
+    should be a tuple of tensor or the `input_shape` should be a tuple
+    of tuple which each element will be constructed into a dumpy input.
+
+    Examples:
+        >>> # the forward of model accepts only one input
+        >>> input_shape = (3, 224, 224)
+        >>> get_model_complexity_info(model, input_shape=input_shape)
+        >>> # the forward of model accepts two or more inputs
+        >>> input_shape = ((3, 224, 224), (3, 10))
+        >>> get_model_complexity_info(model, input_shape=input_shape)
+
     Args:
         model (nn.Module): The model to analyze.
-        input_shape (tuple): The input shape of the model.
-        inputs (torch.Tensor, optional): The input tensor of the model.
-            If not given the input tensor will be generated automatically
-            with the given input_shape.
+        input_shape (Union[Tuple[int, ...], Tuple[Tuple[int, ...]], None]):
+            The input shape of the model.
+            If "inputs" is not specified, the "input_shape" should be set.
+            Defaults to None.
+        inputs (torch.Tensor, tuple[torch.Tensor, ...] or Tuple[Any, ...],\
+            optional]):
+            The input tensor(s) of the model. If not given the input tensor
+            will be generated automatically with the given input_shape.
+            Defaults to None.
         show_table (bool): Whether to show the complexity table.
             Defaults to True.
         show_arch (bool): Whether to show the complexity arch.
             Defaults to True.
 
     Returns:
         dict: The complexity information of the model.
     """
+    if input_shape is None and inputs is None:
+        raise ValueError('One of "input_shape" and "inputs" should be set.')
+    elif input_shape is not None and inputs is not None:
+        raise ValueError('"input_shape" and "inputs" cannot be both set.')
+
     if inputs is None:
-        inputs = (torch.randn(1, *input_shape), )
+        if is_tuple_of(input_shape, int):  # tuple of int, construct one tensor
+            inputs = (torch.randn(1, *input_shape), )
+        elif is_tuple_of(input_shape, tuple) and all([
+                is_tuple_of(one_input_shape, int)
+                for one_input_shape in input_shape  # type: ignore
+        ]):  # tuple of tuple of int, construct multiple tensors
+            inputs = tuple([
+                torch.randn(1, *one_input_shape)
+                for one_input_shape in input_shape  # type: ignore
+            ])
+        else:
+            raise ValueError(
+                '"input_shape" should be either a `tuple of int` (to construct'
+                'one input tensor) or a `tuple of tuple of int` (to construct'
+                'multiple input tensors).')
 
     flop_handler = FlopAnalyzer(model, inputs)
     activation_handler = ActivationAnalyzer(model, inputs)
 
     flops = flop_handler.total()
     activations = activation_handler.total()
     params = parameter_count(model)['']
```

### Comparing `mmengine-0.7.2/mmengine/config/config.py` & `mmengine-0.7.3/mmengine/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import ast
 import copy
 import os
 import os.path as osp
 import platform
 import shutil
+import sys
 import tempfile
 import types
 import uuid
 import warnings
 from argparse import Action, ArgumentParser, Namespace
 from collections import abc
 from pathlib import Path
@@ -176,15 +177,23 @@
         filename = str(filename) if isinstance(filename, Path) else filename
         cfg_dict, cfg_text, env_variables = Config._file2dict(
             filename, use_predefined_variables, use_environment_variables)
         if import_custom_modules and cfg_dict.get('custom_imports', None):
             try:
                 import_modules_from_strings(**cfg_dict['custom_imports'])
             except ImportError as e:
-                raise ImportError('Failed to custom import!') from e
+                err_msg = (
+                    'Failed to import custom modules from '
+                    f"{cfg_dict['custom_imports']}, the current sys.path is: ")
+                for p in sys.path:
+                    err_msg += f'\n    {p}'
+                err_msg += (
+                    '\nYou should set `PYTHONPATH` to make `sys.path` include '
+                    'the directory which contains your custom module')
+                raise ImportError(err_msg) from e
         return Config(
             cfg_dict,
             cfg_text=cfg_text,
             filename=filename,
             env_variables=env_variables)
 
     @staticmethod
```

### Comparing `mmengine-0.7.2/mmengine/config/utils.py` & `mmengine-0.7.3/mmengine/config/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     'mmrazor': 'mmrazor',
     'mmflow': 'mmflow',
     'mmhuman3d': 'mmhuman3d',
     'mmrotate': 'mmrotate',
     'mmselfsup': 'mmselfsup',
     'mmyolo': 'mmyolo',
     'mmpretrain': 'mmpretrain',
+    'mmagic': 'mmagic',
 }
 
 # PKG2PROJECT is not a proper name to represent the mapping between module name
 # (module import from) and package name (used by pip install). Therefore,
 # PKG2PROJECT will be deprecated and this alias will only be kept until
 # MMEngine v1.0.0
 PKG2PROJECT = MODULE2PACKAGE
```

### Comparing `mmengine-0.7.2/mmengine/dataset/__init__.py` & `mmengine-0.7.3/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/dataset/base_dataset.py` & `mmengine-0.7.3/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.7.3/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/dataset/sampler.py` & `mmengine-0.7.3/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/dataset/utils.py` & `mmengine-0.7.3/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/device/utils.py` & `mmengine-0.7.3/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/dist/__init__.py` & `mmengine-0.7.3/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/dist/dist.py` & `mmengine-0.7.3/mmengine/dist/dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,17 +410,21 @@
     # ``current_device`` is CUDA if backend is NCCL otherwise CPU device. In
     # the case it is not ``None`` we move the size and object tensors to be
     # broadcasted to this device.
     group_backend = get_backend(group)
     is_nccl_backend = group_backend == torch_dist.Backend.NCCL
     current_device = torch.device('cpu')
     is_hccl_backend = group_backend == 'hccl'
+    is_cncl_backend = group_backend == 'cncl'
     if is_hccl_backend:
         current_device = torch.npu.current_device()
         object_sizes_tensor = object_sizes_tensor.to(current_device)
+    elif is_cncl_backend:
+        current_device = torch.device('mlu', torch.mlu.current_device())
+        object_sizes_tensor = object_sizes_tensor.to(current_device)
     elif is_nccl_backend:
         # See note about using torch.cuda.current_device() here in
         # docstring. We cannot simply use my_rank since rank == device is
         # not necessarily true.
         current_device = torch.device('cuda', torch.cuda.current_device())
         object_sizes_tensor = object_sizes_tensor.to(current_device)
 
@@ -432,15 +436,15 @@
         object_tensor = torch.cat(tensor_list)
     else:
         object_tensor = torch.empty(
             torch.sum(object_sizes_tensor).int().item(),
             dtype=torch.uint8,
         )
 
-    if is_nccl_backend or is_hccl_backend:
+    if is_nccl_backend or is_hccl_backend or is_cncl_backend:
         object_tensor = object_tensor.to(current_device)
     torch_dist.broadcast(object_tensor, src=src, group=group)
     # Deserialize objects using their stored sizes.
     offset = 0
     if my_rank != src:
         for i, obj_size in enumerate(object_sizes_tensor):
             obj_view = object_tensor[offset:offset + obj_size]
@@ -992,14 +996,19 @@
     if rank != 0:
         return None
     else:
         # load results of all parts from tmp dir
         part_list = []
         for i in range(world_size):
             path = osp.join(tmpdir, f'part_{i}.pkl')  # type: ignore
+            if not osp.exists(path):
+                raise FileNotFoundError(
+                    f'{tmpdir} is not an shared directory for '
+                    f'rank {i}, please make sure {tmpdir} is a shared '
+                    'directory for all ranks!')
             with open(path, 'rb') as f:
                 part_list.append(pickle.load(f))
         # sort the results
         ordered_results = []
         for res in zip(*part_list):
             ordered_results.extend(list(res))
         # the dataloader may pad some samples
```

### Comparing `mmengine-0.7.2/mmengine/dist/utils.py` & `mmengine-0.7.3/mmengine/dist/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     """Initialize distributed environment with PyTorch launcher.
 
     Args:
         backend (str): Backend of torch.distributed. Supported backends are
             'nccl', 'gloo' and 'mpi'. Defaults to 'nccl'.
         **kwargs: keyword arguments are passed to ``init_process_group``.
     """
-    # TODO: use local_rank instead of rank % num_gpus
     rank = int(os.environ['RANK'])
     if is_mlu_available():
         import torch_mlu  # noqa: F401
         torch.mlu.set_device(rank)
         torch_dist.init_process_group(
             backend='cncl',
             rank=rank,
@@ -99,16 +98,17 @@
         torch.npu.set_device(rank)
         torch_dist.init_process_group(
             backend='hccl',
             rank=rank,
             world_size=int(os.environ['WORLD_SIZE']),
             **kwargs)
     else:
-        num_gpus = torch.cuda.device_count()
-        torch.cuda.set_device(rank % num_gpus)
+        # LOCAL_RANK is set by `torch.distributed.launch` since PyTorch 1.1
+        local_rank = int(os.environ['LOCAL_RANK'])
+        torch.cuda.set_device(local_rank)
         torch_dist.init_process_group(backend=backend, **kwargs)
 
 
 def _init_dist_mpi(backend, **kwargs) -> None:
     """Initialize distributed environment with MPI launcher.
 
     Args:
@@ -147,31 +147,37 @@
     Args:
         backend (str): Backend of torch.distributed.
         port (int, optional): Master port. Defaults to None.
     """
     proc_id = int(os.environ['SLURM_PROCID'])
     ntasks = int(os.environ['SLURM_NTASKS'])
     node_list = os.environ['SLURM_NODELIST']
-    num_gpus = torch.cuda.device_count()
-    torch.cuda.set_device(proc_id % num_gpus)
+    # Not sure when this environment variable could be None, so use a fallback
+    local_rank_env = os.environ.get('SLURM_LOCALID', None)
+    if local_rank_env is not None:
+        local_rank = int(local_rank_env)
+    else:
+        num_gpus = torch.cuda.device_count()
+        local_rank = proc_id % num_gpus
+    torch.cuda.set_device(local_rank)
     addr = subprocess.getoutput(
         f'scontrol show hostname {node_list} | head -n1')
     # specify master port
     if port is not None:
         os.environ['MASTER_PORT'] = str(port)
     elif 'MASTER_PORT' in os.environ:
         pass  # use MASTER_PORT in the environment variable
     else:
         # 29500 is torch.distributed default port
         os.environ['MASTER_PORT'] = '29500'
     # use MASTER_ADDR in the environment variable if it already exists
     if 'MASTER_ADDR' not in os.environ:
         os.environ['MASTER_ADDR'] = addr
     os.environ['WORLD_SIZE'] = str(ntasks)
-    os.environ['LOCAL_RANK'] = str(proc_id % num_gpus)
+    os.environ['LOCAL_RANK'] = str(local_rank)
     os.environ['RANK'] = str(proc_id)
     torch_dist.init_process_group(backend=backend)
 
 
 def init_local_group(node_rank: int, num_gpus_per_node: int):
     """Setup the local process group.
```

### Comparing `mmengine-0.7.2/mmengine/evaluator/evaluator.py` & `mmengine-0.7.3/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/evaluator/metric.py` & `mmengine-0.7.3/mmengine/evaluator/metric.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,25 +28,36 @@
         collect_device (str): Device name used for collecting results from
             different ranks during distributed training. Must be 'cpu' or
             'gpu'. Defaults to 'cpu'.
         prefix (str, optional): The prefix that will be added in the metric
             names to disambiguate homonymous metrics of different evaluators.
             If prefix is not provided in the argument, self.default_prefix
             will be used instead. Default: None
+        collect_dir: (str, optional): Synchronize directory for collecting data
+            from different ranks. This argument should only be configured when
+            ``collect_device`` is 'cpu'. Defaults to None.
+            `New in version 0.7.3.`
     """
 
     default_prefix: Optional[str] = None
 
     def __init__(self,
                  collect_device: str = 'cpu',
-                 prefix: Optional[str] = None) -> None:
+                 prefix: Optional[str] = None,
+                 collect_dir: Optional[str] = None) -> None:
+        if collect_dir is not None and collect_device != 'cpu':
+            raise ValueError('`collec_dir` could only be configured when '
+                             "`collect_device='cpu'`")
+
         self._dataset_meta: Union[None, dict] = None
         self.collect_device = collect_device
         self.results: List[Any] = []
         self.prefix = prefix or self.default_prefix
+        self.collect_dir = collect_dir
+
         if self.prefix is None:
             print_log(
                 'The prefix is not set in metric class '
                 f'{self.__class__.__name__}.',
                 logger='current',
                 level=logging.WARNING)
 
@@ -103,15 +114,22 @@
             print_log(
                 f'{self.__class__.__name__} got empty `self.results`. Please '
                 'ensure that the processed results are properly added into '
                 '`self.results` in `process` method.',
                 logger='current',
                 level=logging.WARNING)
 
-        results = collect_results(self.results, size, self.collect_device)
+        if self.collect_device == 'cpu':
+            results = collect_results(
+                self.results,
+                size,
+                self.collect_device,
+                tmpdir=self.collect_dir)
+        else:
+            collect_results(self.results, size, self.collect_device)
 
         if is_main_process():
             # cast all tensors in results list to cpu
             results = _to_cpu(results)
             _metrics = self.compute_metrics(results)  # type: ignore
             # Add prefix to metric names
             if self.prefix:
@@ -136,20 +154,26 @@
 
     Args:
         out_file_path (str): Path of the dumped file. Must end with '.pkl'
             or '.pickle'.
         collect_device (str): Device name used for collecting results from
             different ranks during distributed training. Must be 'cpu' or
             'gpu'. Defaults to 'cpu'.
+        collect_dir: (str, optional): Synchronize directory for collecting data
+            from different ranks. This argument should only be configured when
+            ``collect_device`` is 'cpu'. Defaults to None.
+            `New in version 0.7.3.`
     """
 
     def __init__(self,
                  out_file_path: str,
-                 collect_device: str = 'cpu') -> None:
-        super().__init__(collect_device=collect_device)
+                 collect_device: str = 'cpu',
+                 collect_dir: Optional[str] = None) -> None:
+        super().__init__(
+            collect_device=collect_device, collect_dir=collect_dir)
         if not out_file_path.endswith(('.pkl', '.pickle')):
             raise ValueError('The output file must be a pkl file.')
         self.out_file_path = out_file_path
 
     def process(self, data_batch: Any, predictions: Sequence[dict]) -> None:
         """transfer tensors in predictions to CPU."""
         self.results.extend(_to_cpu(predictions))
```

### Comparing `mmengine-0.7.2/mmengine/evaluator/utils.py` & `mmengine-0.7.3/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/__init__.py` & `mmengine-0.7.3/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/__init__.py` & `mmengine-0.7.3/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/base.py` & `mmengine-0.7.3/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/http_backend.py` & `mmengine-0.7.3/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.7.3/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/local_backend.py` & `mmengine-0.7.3/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.7.3/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.7.3/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.7.3/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/file_client.py` & `mmengine-0.7.3/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/handlers/base.py` & `mmengine-0.7.3/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.7.3/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.7.3/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.7.3/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.7.3/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/io.py` & `mmengine-0.7.3/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/fileio/parse.py` & `mmengine-0.7.3/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/__init__.py` & `mmengine-0.7.3/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.7.3/mmengine/hooks/checkpoint_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os.path as osp
 import pickle
 from math import inf
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Sequence, Union
 
-from mmengine.dist import is_main_process
+from mmengine.dist import is_main_process, master_only
 from mmengine.fileio import FileClient, get_file_backend
 from mmengine.logging import print_log
 from mmengine.registry import HOOKS
 from mmengine.utils import is_list_of, is_seq_of
 from .hook import Hook
 
 DATA_BATCH = Optional[Union[dict, tuple, list]]
@@ -343,14 +343,15 @@
 
         if getattr(self, 'best_ckpt_path', None) is not None:
             self._publish_model(runner, str(self.best_ckpt_path))
         if getattr(self, 'best_ckpt_path_dict', None) is not None:
             for key, best_ckpt in self.best_ckpt_path_dict.items():
                 self._publish_model(runner, best_ckpt)
 
+    @master_only
     def _publish_model(self, runner, ckpt_path: str) -> None:
         """Remove unnecessary keys from ckpt_path and save the new checkpoint.
 
         Args:
             runner (Runner): The runner of the training process.
             ckpt_path (str): The checkpoint path that ought to be published.
         """
@@ -474,32 +475,32 @@
                     key_score, best_score):
                 continue
 
             best_score = key_score
             runner.message_hub.update_info(best_score_key, best_score)
 
             if best_ckpt_path and \
-               self.file_client.isfile(best_ckpt_path) and \
+               self.file_backend.isfile(best_ckpt_path) and \
                is_main_process():
-                self.file_client.remove(best_ckpt_path)
+                self.file_backend.remove(best_ckpt_path)
                 runner.logger.info(
                     f'The previous best checkpoint {best_ckpt_path} '
                     'is removed')
 
             best_ckpt_name = f'best_{key_indicator}_{ckpt_filename}'
             # Replace illegal characters for filename with `_`
             best_ckpt_name = best_ckpt_name.replace('/', '_')
             if len(self.key_indicators) == 1:
-                self.best_ckpt_path = self.file_client.join_path(  # type: ignore # noqa: E501
+                self.best_ckpt_path = self.file_backend.join_path(  # type: ignore # noqa: E501
                     self.out_dir, best_ckpt_name)
                 runner.message_hub.update_info(runtime_best_ckpt_key,
                                                self.best_ckpt_path)
             else:
                 self.best_ckpt_path_dict[
-                    key_indicator] = self.file_client.join_path(  # type: ignore # noqa: E501
+                    key_indicator] = self.file_backend.join_path(  # type: ignore # noqa: E501
                         self.out_dir, best_ckpt_name)
                 runner.message_hub.update_info(
                     runtime_best_ckpt_key,
                     self.best_ckpt_path_dict[key_indicator])
             runner.save_checkpoint(
                 self.out_dir,
                 filename=best_ckpt_name,
```

### Comparing `mmengine-0.7.2/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.7.3/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/ema_hook.py` & `mmengine-0.7.3/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.7.3/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/hook.py` & `mmengine-0.7.3/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.7.3/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/logger_hook.py` & `mmengine-0.7.3/mmengine/hooks/logger_hook.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import torch
 
 from mmengine.fileio import FileClient, dump
 from mmengine.fileio.io import get_file_backend
 from mmengine.hooks import Hook
 from mmengine.logging import print_log
 from mmengine.registry import HOOKS
-from mmengine.utils import is_tuple_of, scandir
+from mmengine.utils import is_seq_of, scandir
 
 DATA_BATCH = Optional[Union[dict, tuple, list]]
 SUFFIX_TYPE = Union[Sequence[str], str]
 
 
 @HOOKS.register_module()
 class LoggerHook(Hook):
@@ -80,41 +80,59 @@
                  interval_exp_name: int = 1000,
                  out_dir: Optional[Union[str, Path]] = None,
                  out_suffix: SUFFIX_TYPE = ('.json', '.log', '.py', 'yaml'),
                  keep_local: bool = True,
                  file_client_args: Optional[dict] = None,
                  log_metric_by_epoch: bool = True,
                  backend_args: Optional[dict] = None):
-        self.interval = interval
-        self.ignore_last = ignore_last
-        self.interval_exp_name = interval_exp_name
+
+        if not isinstance(interval, int):
+            raise TypeError('interval must be an integer')
+        if interval <= 0:
+            raise ValueError('interval must be greater than 0')
+
+        if not isinstance(ignore_last, bool):
+            raise TypeError('ignore_last must be a boolean')
+
+        if not isinstance(interval_exp_name, int):
+            raise TypeError('interval_exp_name must be an integer')
+        if interval_exp_name <= 0:
+            raise ValueError('interval_exp_name must be greater than 0')
+
+        if out_dir is not None and not isinstance(out_dir, (str, Path)):
+            raise TypeError('out_dir must be a str or Path object')
+
+        if not isinstance(keep_local, bool):
+            raise TypeError('keep_local must be a boolean')
 
         if out_dir is None and file_client_args is not None:
             raise ValueError(
                 'file_client_args should be "None" when `out_dir` is not'
                 'specified.')
-        self.out_dir = out_dir
 
         if file_client_args is not None:
             print_log(
                 '"file_client_args" will be deprecated in future. '
                 'Please use "backend_args" instead',
                 logger='current',
                 level=logging.WARNING)
             if backend_args is not None:
                 raise ValueError(
                     '"file_client_args" and "backend_args" cannot be set '
                     'at the same time.')
 
-        if not (out_dir is None or isinstance(out_dir, str)
-                or is_tuple_of(out_dir, str)):
-            raise TypeError('out_dir should be None or string or tuple of '
-                            f'string, but got {type(out_dir)}')
-        self.out_suffix = out_suffix
+        if not (isinstance(out_suffix, str) or is_seq_of(out_suffix, str)):
+            raise TypeError('out_suffix should be a string or a sequence of '
+                            f'string, but got {type(out_suffix)}')
 
+        self.out_suffix = out_suffix
+        self.out_dir = out_dir
+        self.interval = interval
+        self.ignore_last = ignore_last
+        self.interval_exp_name = interval_exp_name
         self.keep_local = keep_local
         self.file_client_args = file_client_args
         self.json_log_path: Optional[str] = None
 
         if self.out_dir is not None:
             self.file_client = FileClient.infer_client(file_client_args,
                                                        self.out_dir)
@@ -163,15 +181,16 @@
                     runner.train_dataloader, batch_idx)):
             exp_info = f'Exp name: {runner.experiment_name}'
             runner.logger.info(exp_info)
         if self.every_n_inner_iters(batch_idx, self.interval):
             tag, log_str = runner.log_processor.get_log_after_iter(
                 runner, batch_idx, 'train')
         elif (self.end_of_epoch(runner.train_dataloader, batch_idx)
-              and not self.ignore_last):
+              and (not self.ignore_last
+                   or len(runner.train_dataloader) <= self.interval)):
             # `runner.max_iters` may not be divisible by `self.interval`. if
             # `self.ignore_last==True`, the log of remaining iterations will
             # be recorded (Epoch [4][1000/1007], the logs of 998-1007
             # iterations will be recorded).
             tag, log_str = runner.log_processor.get_log_after_iter(
                 runner, batch_idx, 'train')
         else:
@@ -230,19 +249,33 @@
                 metrics on validation dataset. The keys are the names of the
                 metrics, and the values are corresponding results.
         """
         tag, log_str = runner.log_processor.get_log_after_epoch(
             runner, len(runner.val_dataloader), 'val')
         runner.logger.info(log_str)
         if self.log_metric_by_epoch:
+            # Accessing the epoch attribute of the runner will trigger
+            # the construction of the train_loop. Therefore, to avoid
+            # triggering the construction of the train_loop during
+            # validation, check before accessing the epoch.
+            if (isinstance(runner._train_loop, dict)
+                    or runner._train_loop is None):
+                epoch = 0
+            else:
+                epoch = runner.epoch
             runner.visualizer.add_scalars(
-                tag, step=runner.epoch, file_path=self.json_log_path)
+                tag, step=epoch, file_path=self.json_log_path)
         else:
+            if (isinstance(runner._train_loop, dict)
+                    or runner._train_loop is None):
+                iter = 0
+            else:
+                iter = runner.iter
             runner.visualizer.add_scalars(
-                tag, step=runner.iter, file_path=self.json_log_path)
+                tag, step=iter, file_path=self.json_log_path)
 
     def after_test_epoch(self,
                          runner,
                          metrics: Optional[Dict[str, float]] = None) -> None:
         """All subclasses should override this method, if they need any
         operations after each test epoch.
 
@@ -284,25 +317,39 @@
     def after_run(self, runner) -> None:
         """Copy logs to ``self.out_dir`` if ``self.out_dir is not None``
 
         Args:
             runner (Runner): The runner of the training/testing/validation
                 process.
         """
+        # close the visualizer
+        runner.visualizer.close()
+
         # copy or upload logs to self.out_dir
         if self.out_dir is None:
             return
+
+        removed_files = []
         for filename in scandir(runner._log_dir, self.out_suffix, True):
             local_filepath = osp.join(runner._log_dir, filename)
+            removed_files.append(local_filepath)
             out_filepath = self.file_backend.join_path(self.out_dir, filename)
             with open(local_filepath) as f:
                 self.file_backend.put_text(f.read(), out_filepath)
 
             runner.logger.info(
                 f'The file {local_filepath} has been uploaded to '
                 f'{out_filepath}.')
 
             if not self.keep_local:
-                os.remove(local_filepath)
                 runner.logger.info(f'{local_filepath} was removed due to the '
                                    '`self.keep_local=False`. You can check '
                                    f'the running logs in {out_filepath}')
+
+        if not self.keep_local:
+            # Close file handler to avoid PermissionError on Windows.
+            for handler in runner.logger.handlers:
+                if isinstance(handler, logging.FileHandler):
+                    handler.close()
+
+            for file in removed_files:
+                os.remove(file)
```

### Comparing `mmengine-0.7.2/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.7.3/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.7.3/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/profiler_hook.py` & `mmengine-0.7.3/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.7.3/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.7.3/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.7.3/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hub/hub.py` & `mmengine-0.7.3/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hub/mmcls.json` & `mmengine-0.7.3/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hub/openmmlab.json` & `mmengine-0.7.3/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/hub/torchvision_0.12.json` & `mmengine-0.7.3/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/infer/infer.py` & `mmengine-0.7.3/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/logging/history_buffer.py` & `mmengine-0.7.3/mmengine/logging/history_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,7 +203,27 @@
         Returns:
             np.ndarray: Recently updated values in log histories.
         """
         if len(self._log_history) == 0:
             raise ValueError('HistoryBuffer._log_history is an empty array! '
                              'please call update first')
         return self._log_history[-1]
+
+    def __getstate__(self) -> dict:
+        """Make ``_statistics_methods`` can be resumed.
+
+        Returns:
+            dict: State dict including statistics_methods.
+        """
+        self.__dict__.update(statistics_methods=self._statistics_methods)
+        return self.__dict__
+
+    def __setstate__(self, state):
+        """Try to load ``_statistics_methods`` from state.
+
+        Args:
+            state (dict): State dict.
+        """
+        statistics_methods = state.pop('statistics_methods', {})
+        self._set_default_statistics()
+        self._statistics_methods.update(statistics_methods)
+        self.__dict__.update(state)
```

### Comparing `mmengine-0.7.2/mmengine/logging/logger.py` & `mmengine-0.7.3/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/logging/message_hub.py` & `mmengine-0.7.3/mmengine/logging/message_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,60 +23,53 @@
     during training phase, which will be stored as ``HistoryBuffer``. The
     runtime information refers to the iter times, meta information of
     runner etc., which will be overwritten by next update.
 
     Args:
         name (str): Name of message hub used to get corresponding instance
             globally.
-        log_scalars (OrderedDict, optional): Each key-value pair in the
+        log_scalars (dict, optional): Each key-value pair in the
             dictionary is the name of the log information such as "loss", "lr",
             "metric" and their corresponding values. The type of value must be
             HistoryBuffer. Defaults to None.
-        runtime_info (OrderedDict, optional): Each key-value pair in the
+        runtime_info (dict, optional): Each key-value pair in the
             dictionary is the name of the runtime information and their
             corresponding values. Defaults to None.
-        resumed_keys (OrderedDict, optional): Each key-value pair in the
+        resumed_keys (dict, optional): Each key-value pair in the
             dictionary decides whether the key in :attr:`_log_scalars` and
             :attr:`_runtime_info` will be serialized.
 
     Note:
         Key in :attr:`_resumed_keys` belongs to :attr:`_log_scalars` or
         :attr:`_runtime_info`. The corresponding value cannot be set
         repeatedly.
 
     Examples:
         >>> # create empty `MessageHub`.
-        >>> message_hub1 = MessageHub()
-        >>> log_scalars = OrderedDict(loss=HistoryBuffer())
-        >>> runtime_info = OrderedDict(task='task')
+        >>> message_hub1 = MessageHub('name')
+        >>> log_scalars = dict(loss=HistoryBuffer())
+        >>> runtime_info = dict(task='task')
         >>> resumed_keys = dict(loss=True)
         >>> # create `MessageHub` from data.
         >>> message_hub2 = MessageHub(
         >>>     name='name',
         >>>     log_scalars=log_scalars,
         >>>     runtime_info=runtime_info,
         >>>     resumed_keys=resumed_keys)
     """
 
     def __init__(self,
                  name: str,
-                 log_scalars: Optional[OrderedDict] = None,
-                 runtime_info: Optional[OrderedDict] = None,
-                 resumed_keys: Optional[OrderedDict] = None):
+                 log_scalars: Optional[dict] = None,
+                 runtime_info: Optional[dict] = None,
+                 resumed_keys: Optional[dict] = None):
         super().__init__(name)
-        self._log_scalars = log_scalars if log_scalars is not None else \
-            OrderedDict()
-        self._runtime_info = runtime_info if runtime_info is not None else \
-            OrderedDict()
-        self._resumed_keys = resumed_keys if resumed_keys is not None else \
-            OrderedDict()
-
-        assert isinstance(self._log_scalars, OrderedDict)
-        assert isinstance(self._runtime_info, OrderedDict)
-        assert isinstance(self._resumed_keys, OrderedDict)
+        self._log_scalars = self._parse_input('log_scalars', log_scalars)
+        self._runtime_info = self._parse_input('runtime_info', runtime_info)
+        self._resumed_keys = self._parse_input('resumed_keys', resumed_keys)
 
         for value in self._log_scalars.values():
             assert isinstance(value, HistoryBuffer), \
                 ("The type of log_scalars'value must be HistoryBuffer, but "
                  f'got {type(value)}')
 
         for key in self._resumed_keys.keys():
@@ -109,15 +102,15 @@
         Update ``HistoryBuffer`` in :attr:`_log_scalars`. If corresponding key
         ``HistoryBuffer`` has been created, ``value`` and ``count`` is the
         argument of ``HistoryBuffer.update``, Otherwise, ``update_scalar``
         will create an ``HistoryBuffer`` with value and count via the
         constructor of ``HistoryBuffer``.
 
         Examples:
-            >>> message_hub = MessageHub
+            >>> message_hub = MessageHub(name='name')
             >>> # create loss `HistoryBuffer` with value=1, count=1
             >>> message_hub.update_scalar('loss', 1)
             >>> # update loss `HistoryBuffer` with value
             >>> message_hub.update_scalar('loss', 3)
             >>> message_hub.update_scalar('loss', 3, resumed=False)
             AssertionError: loss used to be true, but got false now. resumed
             keys cannot be modified repeatedly'
@@ -193,15 +186,15 @@
         time calling ``update_info``.
 
         Note:
             The ``resumed`` argument needs to be consistent for the same
             ``key``.
 
         Examples:
-            >>> message_hub = MessageHub()
+            >>> message_hub = MessageHub(name='name')
             >>> message_hub.update_info('iter', 100)
 
         Args:
             key (str): Key of runtime information.
             value (Any): Value of runtime information.
             resumed (bool): Whether the corresponding ``HistoryBuffer``
                 could be resumed.
@@ -216,15 +209,15 @@
         time calling ``update_info``.
 
         Note:
             The ``resumed`` argument needs to be consistent for the same
             ``info_dict``.
 
         Examples:
-            >>> message_hub = MessageHub()
+            >>> message_hub = MessageHub(name='name')
             >>> message_hub.update_info({'iter': 100})
 
         Args:
             info_dict (str): Runtime information dictionary.
             resumed (bool): Whether the corresponding ``HistoryBuffer``
                 could be resumed.
         """
@@ -269,15 +262,14 @@
     @property
     def runtime_info(self) -> OrderedDict:
         """Get all runtime information.
 
         Returns:
             OrderedDict: A copy of all runtime information.
         """
-        # return copy.deepcopy(self._runtime_info)
         return self._runtime_info
 
     def get_scalar(self, key: str) -> HistoryBuffer:
         """Get ``HistoryBuffer`` instance by key.
 
         Note:
             Considering the large memory footprint of history buffers in the
@@ -292,30 +284,32 @@
             key exists.
         """
         if key not in self.log_scalars:
             raise KeyError(f'{key} is not found in Messagehub.log_buffers: '
                            f'instance name is: {MessageHub.instance_name}')
         return self.log_scalars[key]
 
-    def get_info(self, key: str) -> Any:
-        """Get runtime information by key.
+    def get_info(self, key: str, default: Optional[Any] = None) -> Any:
+        """Get runtime information by key. if the key does not exist, this
+        method will return default information.
 
         Args:
             key (str): Key of runtime information.
+            default (Any, optional): The default returned value for the
+                given key.
 
         Returns:
             Any: A copy of corresponding runtime information if the key exists.
         """
         if key not in self.runtime_info:
-            raise KeyError(f'{key} is not found in Messagehub.log_buffers: '
-                           f'instance name is: {MessageHub.instance_name}')
-
-        # TODO： There are restrictions on objects that can be saved
-        # return copy.deepcopy(self._runtime_info[key])
-        return self._runtime_info[key]
+            return default
+        else:
+            # TODO： There are restrictions on objects that can be saved
+            # return copy.deepcopy(self._runtime_info[key])
+            return self._runtime_info[key]
 
     def _get_valid_value(
         self,
         value: Union['torch.Tensor', np.ndarray, np.number, int, float],
     ) -> Union[int, float]:
         """Convert value to python built-in type.
 
@@ -438,7 +432,25 @@
         # Since some checkpoints saved serialized `message_hub` instance,
         # `load_state_dict` support loading `message_hub` instance for
         # compatibility
         else:
             self._log_scalars = copy.deepcopy(state_dict._log_scalars)
             self._runtime_info = copy.deepcopy(state_dict._runtime_info)
             self._resumed_keys = copy.deepcopy(state_dict._resumed_keys)
+
+    def _parse_input(self, name: str, value: Any) -> OrderedDict:
+        """Parse input value.
+
+        Args:
+            name (str): name of input value.
+            value (Any): Input value.
+
+        Returns:
+            dict: Parsed input value.
+        """
+        if value is None:
+            return OrderedDict()
+        elif isinstance(value, dict):
+            return OrderedDict(value)
+        else:
+            raise TypeError(f'{name} should be a dict or `None`, but '
+                            f'got {type(name)}')
```

### Comparing `mmengine-0.7.2/mmengine/model/__init__.py` & `mmengine-0.7.3/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/averaged_model.py` & `mmengine-0.7.3/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/base_model/base_model.py` & `mmengine-0.7.3/mmengine/model/base_model/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,28 @@
             nn.Module: The model itself.
         """
         if device is None or isinstance(device, int):
             device = torch.device('cuda', index=device)
         self._set_device(torch.device(device))
         return super().cuda(device)
 
+    def mlu(
+        self,
+        device: Union[int, str, torch.device, None] = None,
+    ) -> nn.Module:
+        """Overrides this method to call :meth:`BaseDataPreprocessor.mlu`
+        additionally.
+
+        Returns:
+            nn.Module: The model itself.
+        """
+        device = torch.device('mlu', torch.mlu.current_device())
+        self._set_device(device)
+        return super().mlu()
+
     def npu(
         self,
         device: Union[int, str, torch.device, None] = None,
     ) -> nn.Module:
         """Overrides this method to call :meth:`BaseDataPreprocessor.npu`
         additionally.
```

### Comparing `mmengine-0.7.2/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.7.3/mmengine/model/base_model/data_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,23 @@
 
         Returns:
             nn.Module: The model itself.
         """
         self._device = torch.device(torch.npu.current_device())
         return super().npu()
 
+    def mlu(self, *args, **kwargs) -> nn.Module:
+        """Overrides this method to set the :attr:`device`
+
+        Returns:
+            nn.Module: The model itself.
+        """
+        self._device = torch.device(torch.mlu.current_device())
+        return super().mlu()
+
     def cpu(self, *args, **kwargs) -> nn.Module:
         """Overrides this method to set the :attr:`device`
 
         Returns:
             nn.Module: The model itself.
         """
         self._device = torch.device('cpu')
```

### Comparing `mmengine-0.7.2/mmengine/model/base_module.py` & `mmengine-0.7.3/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/test_time_aug.py` & `mmengine-0.7.3/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/utils.py` & `mmengine-0.7.3/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/weight_init.py` & `mmengine-0.7.3/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/wrappers/__init__.py` & `mmengine-0.7.3/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/wrappers/distributed.py` & `mmengine-0.7.3/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.7.3/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.7.3/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/model/wrappers/utils.py` & `mmengine-0.7.3/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/__init__.py` & `mmengine-0.7.3/mmengine/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/__init__.py` & `mmengine-0.7.3/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.7.3/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from contextlib import contextmanager
 from typing import Union
 
 import torch
 import torch.nn as nn
 
-from mmengine.device import is_cuda_available, is_npu_available
+from mmengine.device import (is_cuda_available, is_mlu_available,
+                             is_npu_available)
 from mmengine.registry import OPTIM_WRAPPERS
 from mmengine.utils import digit_version
 from mmengine.utils.dl_utils import TORCH_VERSION
 from .optimizer_wrapper import OptimWrapper
 
 if is_npu_available():
     from torch.npu.amp import GradScaler
+elif is_mlu_available():
+    from torch.mlu.amp import GradScaler
 else:
     from torch.cuda.amp import GradScaler
 
 
 @OPTIM_WRAPPERS.register_module()
 class AmpOptimWrapper(OptimWrapper):
     """A subclass of :class:`OptimWrapper` that supports automatic mixed
@@ -61,16 +64,17 @@
 
     def __init__(self,
                  loss_scale: str = 'dynamic',
                  dtype: Union[str, torch.dtype] = None,
                  **kwargs):
         assert digit_version(TORCH_VERSION) >= digit_version('1.6.0'), (
             '`torch.cuda.amp` is only available when pytorch version >= 1.6')
-        assert is_cuda_available() or is_npu_available(), (
-            '``AmpOptimizerWrapper`` is only available training on gpu or npu')
+        assert is_cuda_available() or is_npu_available() or is_mlu_available(
+        ), ('``AmpOptimizerWrapper`` is only available training '
+            'on gpu, npu or mlu')
         super().__init__(**kwargs)
         self._scale_update_param = None
         if loss_scale == 'dynamic':
             #  If loss_scale is a string, it must be 'dynamic', then dynamic
             #  loss scaling will be used.
             self.loss_scaler = GradScaler()
         elif isinstance(loss_scale, float):
```

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.7.3/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/builder.py` & `mmengine-0.7.3/mmengine/optim/optimizer/builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,42 @@
             torch_optimizers.append(module_name)
     return torch_optimizers
 
 
 TORCH_OPTIMIZERS = register_torch_optimizers()
 
 
+def register_torch_npu_optimizers() -> List[str]:
+    """Register optimizers in ``torch npu`` to the ``OPTIMIZERS`` registry.
+
+    Returns:
+        List[str]: A list of registered optimizers' name.
+    """
+    if not is_npu_available():
+        return []
+
+    import torch_npu
+    if not hasattr(torch_npu, 'optim'):
+        return []
+
+    torch_npu_optimizers = []
+    for module_name in dir(torch_npu.optim):
+        if module_name.startswith('__') or module_name in OPTIMIZERS:
+            continue
+        _optim = getattr(torch_npu.optim, module_name)
+        if inspect.isclass(_optim) and issubclass(_optim,
+                                                  torch.optim.Optimizer):
+            OPTIMIZERS.register_module(module=_optim)
+            torch_npu_optimizers.append(module_name)
+    return torch_npu_optimizers
+
+
+NPU_OPTIMIZERS = register_torch_npu_optimizers()
+
+
 def register_dadaptation_optimizers() -> List[str]:
     """Register optimizers in ``dadaptation`` to the ``OPTIMIZERS`` registry.
 
     Returns:
         List[str]: A list of registered optimizers' name.
     """
     dadaptation_optimizers = []
```

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.7.3/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.7.3/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.7.3/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/scheduler/__init__.py` & `mmengine-0.7.3/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.7.3/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.7.3/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.7.3/mmengine/optim/scheduler/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/registry/__init__.py` & `mmengine-0.7.3/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/registry/build_functions.py` & `mmengine-0.7.3/mmengine/registry/build_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,16 @@
                 raise KeyError(
                     f'{obj_type} is not in the {registry.name} registry. '
                     f'Please check whether the value of `{obj_type}` is '
                     'correct or it was registered as expected. More details '
                     'can be found at '
                     'https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#import-the-custom-module'  # noqa: E501
                 )
-        elif inspect.isclass(obj_type) or inspect.isfunction(obj_type):
+        # this will include classes, functions, partial functions and more
+        elif callable(obj_type):
             obj_cls = obj_type
         else:
             raise TypeError(
                 f'type must be a str or valid type, but got {type(obj_type)}')
 
         try:
             # If `obj_cls` inherits from `ManagerMixin`, it should be
@@ -116,20 +117,28 @@
             # can be accessed globally.
             if inspect.isclass(obj_cls) and \
                     issubclass(obj_cls, ManagerMixin):  # type: ignore
                 obj = obj_cls.get_instance(**args)  # type: ignore
             else:
                 obj = obj_cls(**args)  # type: ignore
 
-            print_log(
-                f'An `{obj_cls.__name__}` instance is built from '  # type: ignore # noqa: E501
-                'registry, its implementation can be found in '
-                f'{obj_cls.__module__}',  # type: ignore
-                logger='current',
-                level=logging.DEBUG)
+            if (inspect.isclass(obj_cls) or inspect.isfunction(obj_cls)
+                    or inspect.ismethod(obj_cls)):
+                print_log(
+                    f'An `{obj_cls.__name__}` instance is built from '  # type: ignore # noqa: E501
+                    'registry, and its implementation can be found in '
+                    f'{obj_cls.__module__}',  # type: ignore
+                    logger='current',
+                    level=logging.DEBUG)
+            else:
+                print_log(
+                    'An instance is built from registry, and its constructor '
+                    f'is {obj_cls}',
+                    logger='current',
+                    level=logging.DEBUG)
             return obj
 
         except Exception as e:
             # Normal TypeError does not print class name.
             cls_location = '/'.join(
                 obj_cls.__module__.split('.'))  # type: ignore
             raise type(e)(
```

### Comparing `mmengine-0.7.2/mmengine/registry/default_scope.py` & `mmengine-0.7.3/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/registry/registry.py` & `mmengine-0.7.3/mmengine/registry/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,16 +483,19 @@
                     # If not skip directly, `root.get(key)` will recursively
                     # call itself until RecursionError is thrown.
                     pass
                 else:
                     obj_cls = root.get(key)
 
         if obj_cls is not None:
+            # For some rare cases (e.g. obj_cls is a partial function), obj_cls
+            # doesn't have `__name__`. Use default value to prevent error
+            cls_name = getattr(obj_cls, '__name__', str(obj_cls))
             print_log(
-                f'Get class `{obj_cls.__name__}` from "{registry_name}"'
+                f'Get class `{cls_name}` from "{registry_name}"'
                 f' registry in "{scope_name}"',
                 logger='current',
                 level=logging.DEBUG)
         return obj_cls
 
     def _search_child(self, scope: str) -> Optional['Registry']:
         """Depth-first search for the corresponding registry in its children.
@@ -561,24 +564,24 @@
     def _register_module(self,
                          module: Type,
                          module_name: Optional[Union[str, List[str]]] = None,
                          force: bool = False) -> None:
         """Register a module.
 
         Args:
-            module (type): Module class or function to be registered.
+            module (type): Module to be registered. Typically a class or a
+                function, but generally all ``Callable`` are acceptable.
             module_name (str or list of str, optional): The module name to be
                 registered. If not specified, the class name will be used.
                 Defaults to None.
             force (bool): Whether to override an existing class with the same
                 name. Defaults to False.
         """
-        if not inspect.isclass(module) and not inspect.isfunction(module):
-            raise TypeError('module must be a class or a function, '
-                            f'but got {type(module)}')
+        if not callable(module):
+            raise TypeError(f'module must be Callable, but got {type(module)}')
 
         if module_name is None:
             module_name = module.__name__
         if isinstance(module_name, str):
             module_name = [module_name]
         for name in module_name:
             if not force and name in self._module_dict:
```

### Comparing `mmengine-0.7.2/mmengine/registry/root.py` & `mmengine-0.7.3/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/registry/utils.py` & `mmengine-0.7.3/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/runner/__init__.py` & `mmengine-0.7.3/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/runner/amp.py` & `mmengine-0.7.3/mmengine/runner/amp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import logging
 from contextlib import contextmanager
 from typing import Optional
 
 import torch
 
-from mmengine.device import get_device, is_cuda_available, is_npu_available
+from mmengine.device import (get_device, is_cuda_available, is_mlu_available,
+                             is_npu_available)
 from mmengine.logging import print_log
 from mmengine.utils import digit_version
 from mmengine.utils.dl_utils import TORCH_VERSION
 
 
 @contextmanager
 def autocast(device_type: Optional[str] = None,
@@ -71,28 +72,33 @@
         'The minimum pytorch version requirements of mmengine is 1.5.0, but '
         f'got {TORCH_VERSION}')
 
     if (digit_version('1.5.0') <= digit_version(TORCH_VERSION) <
             digit_version('1.10.0')):
         # If pytorch version is between 1.5.0 and 1.10.0, the default value of
         # dtype for `torch.cuda.amp.autocast` is torch.float16.
-        assert device_type == 'cuda' or device_type is None, (
-            'Pytorch version under 1.10.0 only supports running automatic '
-            'mixed training with cuda')
+        assert (
+            device_type == 'cuda' or device_type == 'mlu'
+            or device_type is None), (
+                'Pytorch version under 1.10.0 only supports running automatic '
+                'mixed training with cuda or mlu')
         if dtype is not None or cache_enabled is not None:
             print_log(
                 f'{dtype} and {device_type} will not work for '
                 '`autocast` since your Pytorch version: '
                 f'{TORCH_VERSION} <= 1.10.0',
                 logger='current',
                 level=logging.WARNING)
 
         if is_npu_available():
             with torch.npu.amp.autocast(enabled=enabled):
                 yield
+        elif is_mlu_available():
+            with torch.mlu.amp.autocast(enabled=enabled):
+                yield
         elif is_cuda_available():
             with torch.cuda.amp.autocast(enabled=enabled):
                 yield
         else:
             if not enabled:
                 yield
             else:
```

### Comparing `mmengine-0.7.2/mmengine/runner/base_loop.py` & `mmengine-0.7.3/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/runner/checkpoint.py` & `mmengine-0.7.3/mmengine/runner/checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import io
 import logging
 import os
 import os.path as osp
 import pkgutil
 import re
-from collections import OrderedDict
+from collections import OrderedDict, namedtuple
 from importlib import import_module
 from tempfile import TemporaryDirectory
 from typing import Callable, Dict, Optional
 
 import torch
 
 import mmengine
 from mmengine.dist import get_dist_info
 from mmengine.fileio import FileClient, get_file_backend
 from mmengine.fileio import load as load_file
 from mmengine.logging import print_log
 from mmengine.model import BaseTTAModel, is_model_wrapper
-from mmengine.utils import deprecated_function, digit_version, mkdir_or_exist
+from mmengine.utils import (apply_to, deprecated_function, digit_version,
+                            mkdir_or_exist)
 from mmengine.utils.dl_utils import load_url
 
 # `MMENGINE_HOME` is the highest priority directory to save checkpoints
 # downloaded from Internet. If it is not set, as a workaround, using
 # `XDG_CACHE_HOME`` or `~/.cache` instead.
 # Note that `XDG_CACHE_HOME` defines the base directory relative to which
 # user-specific non-essential data files should be stored. If `XDG_CACHE_HOME`
 # is either not set or empty, a default equal to `~/.cache` should be used.
 ENV_MMENGINE_HOME = 'MMENGINE_HOME'
 ENV_XDG_CACHE_HOME = 'XDG_CACHE_HOME'
 DEFAULT_CACHE_DIR = '~/.cache'
 
 
+class _IncompatibleKeys(
+        namedtuple('IncompatibleKeys', ['missing_keys', 'unexpected_keys'])):
+
+    def __repr__(self):
+        if not self.missing_keys and not self.unexpected_keys:
+            return '<All keys matched successfully>'
+        return super().__repr__()
+
+    __str__ = __repr__
+
+
 def _get_mmengine_home():
     mmengine_home = os.path.expanduser(
         os.getenv(
             ENV_MMENGINE_HOME,
             os.path.join(
                 os.getenv(ENV_XDG_CACHE_HOME, DEFAULT_CACHE_DIR), 'mmengine')))
 
@@ -56,43 +68,61 @@
         strict (bool): whether to strictly enforce that the keys
             in :attr:`state_dict` match the keys returned by this module's
             :meth:`~torch.nn.Module.state_dict` function. Defaults to False.
         logger (:obj:`logging.Logger`, optional): Logger to log the error
             message. If not specified, print function will be used.
     """
     unexpected_keys = []
-    all_missing_keys = []
+    missing_keys = []
     err_msg = []
 
+    # copy state_dict so _load_from_state_dict can modify it
     metadata = getattr(state_dict, '_metadata', None)
     state_dict = state_dict.copy()
     if metadata is not None:
         state_dict._metadata = metadata
 
     # use _load_from_state_dict to enable checkpoint version control
-    def load(module, prefix=''):
+    def load(module, local_state_dict, prefix=''):
         # recursively check parallel module in case that the model has a
         # complicated structure, e.g., nn.Module(nn.Module(DDP))
         if is_model_wrapper(module) or isinstance(module, BaseTTAModel):
             module = module.module
         local_metadata = {} if metadata is None else metadata.get(
             prefix[:-1], {})
-        module._load_from_state_dict(state_dict, prefix, local_metadata, True,
-                                     all_missing_keys, unexpected_keys,
+        module._load_from_state_dict(local_state_dict, prefix, local_metadata,
+                                     True, missing_keys, unexpected_keys,
                                      err_msg)
         for name, child in module._modules.items():
             if child is not None:
-                load(child, prefix + name + '.')
+                child_prefix = prefix + name + '.'
+                child_state_dict = {
+                    k: v
+                    for k, v in local_state_dict.items()
+                    if k.startswith(child_prefix)
+                }
+                load(child, child_state_dict, child_prefix)
+
+        # Note that the hook can modify missing_keys and unexpected_keys.
+        incompatible_keys = _IncompatibleKeys(missing_keys, unexpected_keys)
+        if hasattr(module, '_load_state_dict_post_hooks'):
+            for hook in module._load_state_dict_post_hooks.values():
+                out = hook(module, incompatible_keys)
+                assert out is None, (
+                    'Hooks registered with '
+                    '``register_load_state_dict_post_hook`` are not expected '
+                    'to return new values, if incompatible_keys need to be '
+                    'modified, it should be done inplace.')
 
-    load(module)
+    load(module, state_dict)
     load = None  # break load->load reference cycle
 
     # ignore "num_batches_tracked" of BN layers
     missing_keys = [
-        key for key in all_missing_keys if 'num_batches_tracked' not in key
+        key for key in missing_keys if 'num_batches_tracked' not in key
     ]
 
     if unexpected_keys:
         err_msg.append('unexpected key in source '
                        f'state_dict: {", ".join(unexpected_keys)}\n')
     if missing_keys:
         err_msg.append(
@@ -618,20 +648,19 @@
 
     Args:
         state_dict (OrderedDict): Model weights on GPU.
 
     Returns:
         OrderedDict: Model weights on GPU.
     """
-    state_dict_cpu = OrderedDict()
-    for key, val in state_dict.items():
-        state_dict_cpu[key] = val.cpu()
+    state_dict = apply_to(state_dict, lambda x: hasattr(x, 'cpu'),
+                          lambda x: x.cpu())
     # Keep metadata in state_dict
-    state_dict_cpu._metadata = getattr(state_dict, '_metadata', OrderedDict())
-    return state_dict_cpu
+    state_dict._metadata = getattr(state_dict, '_metadata', OrderedDict())
+    return state_dict
 
 
 @deprecated_function(
     since='0.3.0',
     removed_in='0.5.0',
     instructions='`_save_to_state_dict` will be deprecated in the future, '
     'please use `nn.Module._save_to_state_dict` directly.')
```

### Comparing `mmengine-0.7.2/mmengine/runner/log_processor.py` & `mmengine-0.7.3/mmengine/runner/log_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 import datetime
+import re
 from collections import OrderedDict
 from itertools import chain
 from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 
@@ -55,14 +56,17 @@
         log_with_hierarchy (bool): Whether to log with hierarchy. If it is
             True, the information is written to visualizer backend such as
             :obj:`LocalVisBackend` and :obj:`TensorboardBackend`
             with hierarchy. For example, ``loss`` will be saved as
             ``train/loss``, and accuracy will be saved as ``val/accuracy``.
             Defaults to False.
             `New in version 0.7.0.`
+        mean_pattern (str): This is a regular expression used to match the log
+            that need to be included in the smoothing statistics.
+            `New in version 0.7.3.`
 
     Examples:
         >>> # `log_name` is defined, `loss_large_window` will be an additional
         >>> # record.
         >>> log_processor = dict(
         >>>     window_size=10,
         >>>     by_epoch=True,
@@ -102,20 +106,22 @@
     """
 
     def __init__(self,
                  window_size=10,
                  by_epoch=True,
                  custom_cfg: Optional[List[dict]] = None,
                  num_digits: int = 4,
-                 log_with_hierarchy: bool = False):
+                 log_with_hierarchy: bool = False,
+                 mean_pattern=r'.*(loss|time|data_time|grad_norm).*'):
         self.window_size = window_size
         self.by_epoch = by_epoch
         self.custom_cfg = custom_cfg if custom_cfg else []
         self.num_digits = num_digits
         self.log_with_hierarchy = log_with_hierarchy
+        self.mean_pattern = re.compile(mean_pattern)
         self._check_custom_cfg()
 
     def get_log_after_iter(self, runner, batch_idx: int,
                            mode: str) -> Tuple[dict, str]:
         """Format log string after training, validation or testing epoch.
 
         Args:
@@ -125,15 +131,14 @@
             mode (str): Current mode of runner, train, test or val.
 
         Return:
             Tuple(dict, str): Formatted log dict/string which will be
             recorded by :obj:`runner.message_hub` and :obj:`runner.visualizer`.
         """
         assert mode in ['train', 'test', 'val']
-        cur_iter = self._get_iter(runner, batch_idx=batch_idx)
         # Overwrite ``window_size`` defined in ``custom_cfg`` to int value.
         parsed_cfg = self._parse_windows_size(runner, batch_idx,
                                               self.custom_cfg)
         # log_tag is used to write log information to terminal
         # If `self.log_with_hierarchy` is False, the tag is the same as
         # log_tag. Otherwise, each key in tag starts with prefix `train`,
         # `test` or `val`
@@ -162,35 +167,40 @@
         #  val/test: Epoch [5/2000] ... (divided by length of dataloader)
         if self.by_epoch:
             # Align the iteration log:
             # Epoch(train)  [  9][010/270]
             # ...                 ||| |||
             # Epoch(train)  [ 10][100/270]
             dataloader_len = self._get_dataloader_size(runner, mode)
+            cur_iter = self._get_iter(runner, batch_idx)
             cur_iter_str = str(cur_iter).rjust(len(str(dataloader_len)))
-
             if mode in ['train', 'val']:
-                # Right Align the epoch log:
-                # Epoch(train)   [9][100/270]
-                # ...             ||
-                # Epoch(train) [100][100/270]
                 cur_epoch = self._get_epoch(runner, mode)
-                max_epochs = runner.max_epochs
-                # 3 means the three characters: "[", "]", and " " occupied in
-                # " [{max_epochs}]"
-                cur_epoch_str = f'[{cur_epoch}]'.rjust(
-                    len(str(max_epochs)) + 3, ' ')
+                if not (isinstance(runner._train_loop, dict)
+                        or runner._train_loop is None):
+                    # Right Align the epoch log:
+                    # Epoch(train)   [9][100/270]
+                    # ...             ||
+                    # Epoch(train) [100][100/270]
+                    max_epochs = runner.max_epochs
+                    # 3 means the three characters: "[", "]", and " " occupied
+                    # in " [{max_epochs}]"
+                    cur_epoch_str = f'[{cur_epoch}]'.rjust(
+                        len(str(max_epochs)) + 3, ' ')
+                else:
+                    cur_epoch_str = f'[{cur_epoch}]'
                 tag['epoch'] = cur_epoch
                 log_str = (f'Epoch({mode}){cur_epoch_str}'
                            f'[{cur_iter_str}/{dataloader_len}]  ')
             else:
                 log_str = (f'Epoch({mode}) '
                            f'[{cur_iter_str}/{dataloader_len}]  ')
         else:
             if mode == 'train':
+                cur_iter = self._get_iter(runner, batch_idx)
                 cur_iter_str = str(cur_iter).rjust(len(str(runner.max_iters)))
                 log_str = (f'Iter({mode}) '
                            f'[{cur_iter_str}/{runner.max_iters}]  ')
             else:
                 dataloader_len = self._get_dataloader_size(runner, mode)
                 cur_iter_str = str(batch_idx + 1).rjust(
                     len(str(dataloader_len)))
@@ -276,22 +286,19 @@
         custom_keys = [
             self._remove_prefix(cfg['data_src'], f'{mode}/')
             for cfg in custom_cfg_copy
         ]
         # Count the averaged time and data_time by epoch
         if 'time' not in custom_keys:
             custom_cfg_copy.append(
-                dict(
-                    data_src=f'{mode}/time',
-                    window_size='epoch',
-                    method_name='mean'))
+                dict(data_src='time', window_size='epoch', method_name='mean'))
         if 'data_time' not in custom_keys:
             custom_cfg_copy.append(
                 dict(
-                    data_src=f'{mode}/data_time',
+                    data_src='data_time',
                     window_size='epoch',
                     method_name='mean'))
         parsed_cfg = self._parse_windows_size(runner, batch_idx,
                                               custom_cfg_copy)
         # tag is used to write log information to different backends.
         ori_tag = self._collect_scalars(parsed_cfg, runner, mode,
                                         self.log_with_hierarchy)
@@ -337,14 +344,15 @@
                 process.
             mode (str): Current mode of runner.
             reserve_prefix (bool): Whether to reserve the prefix of the key.
 
         Returns:
             dict: Statistical values of logs.
         """
+        custom_cfg = copy.deepcopy(custom_cfg)
         tag = OrderedDict()
         # history_scalars of train/val/test phase.
         history_scalars = runner.message_hub.log_scalars
         # corresponding mode history_scalars
         mode_history_scalars = OrderedDict()
         # extract log scalars and remove prefix to `mode_history_scalars`
         # according to mode.
@@ -353,26 +361,27 @@
                 if not reserve_prefix:
                     key = self._remove_prefix(prefix_key, f'{mode}/')
                 else:
                     key = prefix_key
                 mode_history_scalars[key] = log_buffer
         for key in mode_history_scalars:
             # Update the latest learning rate and smoothed time logs.
-            if 'loss' in key or key in ('time', 'data_time', 'grad_norm'):
+            if re.search(self.mean_pattern, key) is not None:
                 tag[key] = mode_history_scalars[key].mean(self.window_size)
             else:
                 # Default statistic method is current.
                 tag[key] = mode_history_scalars[key].current()
         # Update custom keys.
         for log_cfg in custom_cfg:
-            data_src = log_cfg.pop('data_src')
-            if 'log_name' in log_cfg:
-                log_name = log_cfg.pop('log_name')
+            if not reserve_prefix:
+                data_src = log_cfg.pop('data_src')
+                log_name = f"{log_cfg.pop('log_name', data_src)}"
             else:
-                log_name = data_src
+                data_src = f"{mode}/{log_cfg.pop('data_src')}"
+                log_name = f"{mode}/{log_cfg.pop('log_name', data_src)}"
             # log item in custom_cfg could only exist in train or val
             # mode.
             if data_src in mode_history_scalars:
                 tag[log_name] = mode_history_scalars[data_src].statistics(
                     **log_cfg)
         return tag
 
@@ -483,27 +492,27 @@
             The maximum GPU memory occupied by tensors in megabytes for a given
             device.
         """
 
         device = getattr(runner.model, 'output_device', None)
         return get_max_cuda_memory(device)
 
-    def _get_iter(self, runner, batch_idx: int = None) -> int:
+    def _get_iter(self, runner, batch_idx: int) -> int:
         """Get current iteration index.
 
         Args:
             runner (Runner): The runner of the training/testing/validation
                 process.
-            batch_idx (int, optional): The iteration index of current
+            batch_idx (int): The iteration index of current
                 dataloader. Defaults to None.
 
         Returns:
             int: The current global iter or inner iter.
         """
-        if self.by_epoch and batch_idx is not None:
+        if self.by_epoch:
             current_iter = batch_idx + 1
         else:
             current_iter = runner.iter + 1
         return current_iter
 
     def _get_epoch(self, runner, mode: str) -> int:
         """Get current epoch according to mode.
@@ -515,17 +524,21 @@
 
         Returns:
             int: The current epoch.
         """
         if mode == 'train':
             epoch = runner.epoch + 1
         elif mode == 'val':
-            # normal val mode
-            # runner.epoch += 1 has been done before validation
-            epoch = runner.epoch
+            if (isinstance(runner._train_loop, dict)
+                    or runner._train_loop is None):
+                epoch = 0
+            else:
+                # normal val mode
+                # runner.epoch += 1 has been done before validation
+                epoch = runner.epoch
         else:
             raise ValueError(
                 f"runner mode should be 'train' or 'val', but got {mode}")
         return epoch
 
     def _get_cur_loop(self, runner, mode: str):
         """Get current loop according to mode.
```

### Comparing `mmengine-0.7.2/mmengine/runner/loops.py` & `mmengine-0.7.3/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/runner/priority.py` & `mmengine-0.7.3/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/runner/runner.py` & `mmengine-0.7.3/mmengine/runner/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import torch.nn as nn
 from torch.nn.parallel.distributed import DistributedDataParallel
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 
 import mmengine
 from mmengine.config import Config, ConfigDict
-from mmengine.dataset import worker_init_fn
+from mmengine.dataset import worker_init_fn as default_worker_init_fn
 from mmengine.device import get_device
 from mmengine.dist import (broadcast, get_dist_info, get_rank, init_dist,
                            is_distributed, master_only)
 from mmengine.evaluator import Evaluator
 from mmengine.fileio import FileClient, join_path
 from mmengine.hooks import Hook
 from mmengine.logging import MessageHub, MMLogger, print_log
@@ -31,22 +31,22 @@
                             is_model_wrapper, revert_sync_batchnorm)
 from mmengine.optim import (OptimWrapper, OptimWrapperDict, _ParamScheduler,
                             build_optim_wrapper)
 from mmengine.registry import (DATA_SAMPLERS, DATASETS, EVALUATOR, FUNCTIONS,
                                HOOKS, LOG_PROCESSORS, LOOPS, MODEL_WRAPPERS,
                                MODELS, OPTIM_WRAPPERS, PARAM_SCHEDULERS,
                                RUNNERS, VISUALIZERS, DefaultScope)
-from mmengine.utils import digit_version, get_git_hash, is_seq_of
+from mmengine.utils import apply_to, digit_version, get_git_hash, is_seq_of
 from mmengine.utils.dl_utils import (TORCH_VERSION, collect_env,
                                      set_multi_processing)
 from mmengine.visualization import Visualizer
 from .base_loop import BaseLoop
 from .checkpoint import (_load_checkpoint, _load_checkpoint_to_model,
-                         find_latest_checkpoint, get_state_dict,
-                         save_checkpoint, weights_to_cpu)
+                         find_latest_checkpoint, save_checkpoint,
+                         weights_to_cpu)
 from .log_processor import LogProcessor
 from .loops import EpochBasedTrainLoop, IterBasedTrainLoop, TestLoop, ValLoop
 from .priority import Priority, get_priority
 from .utils import set_random_seed
 
 ConfigType = Union[Dict, Config, ConfigDict]
 ParamSchedulerType = Union[List[_ParamScheduler], Dict[str,
@@ -815,15 +815,15 @@
         else:
             raise TypeError('model should be a nn.Module object or dict, '
                             f'but got {model}')
 
     def wrap_model(
             self, model_wrapper_cfg: Optional[Dict],
             model: nn.Module) -> Union[DistributedDataParallel, nn.Module]:
-        """Wrap the model to :obj:``MMDistributedDataParallel`` or other custom
+        """Wrap the model to :obj:`MMDistributedDataParallel` or other custom
         distributed data-parallel module wrappers.
 
         An example of ``model_wrapper_cfg``::
 
             model_wrapper_cfg = dict(
                 broadcast_buffers=False,
                 find_unused_parameters=False
@@ -1377,29 +1377,36 @@
             # fallback to raise error in dataloader
             # if `batch_sampler_cfg` is not a valid type
             batch_sampler = batch_sampler_cfg
 
         # build dataloader
         init_fn: Optional[partial]
 
-        if seed is not None:
-            disable_subprocess_warning = dataloader_cfg.pop(
-                'disable_subprocess_warning', False)
-            assert isinstance(
-                disable_subprocess_warning,
-                bool), ('disable_subprocess_warning should be a bool, but got '
-                        f'{type(disable_subprocess_warning)}')
-            init_fn = partial(
-                worker_init_fn,
-                num_workers=dataloader_cfg.get('num_workers'),
-                rank=get_rank(),
-                seed=seed,
-                disable_subprocess_warning=disable_subprocess_warning)
-        else:
-            init_fn = None
+        if 'worker_init_fn' in dataloader_cfg:
+            worker_init_fn_cfg = dataloader_cfg.pop('worker_init_fn')
+            worker_init_fn_type = worker_init_fn_cfg.pop('type')
+            worker_init_fn = FUNCTIONS.get(worker_init_fn_type)
+            assert callable(worker_init_fn)
+            init_fn = partial(worker_init_fn,
+                              **worker_init_fn_cfg)  # type: ignore
+        else:
+            if seed is not None:
+                disable_subprocess_warning = dataloader_cfg.pop(
+                    'disable_subprocess_warning', False)
+                assert isinstance(disable_subprocess_warning, bool), (
+                    'disable_subprocess_warning should be a bool, but got '
+                    f'{type(disable_subprocess_warning)}')
+                init_fn = partial(
+                    default_worker_init_fn,
+                    num_workers=dataloader_cfg.get('num_workers'),
+                    rank=get_rank(),
+                    seed=seed,
+                    disable_subprocess_warning=disable_subprocess_warning)
+            else:
+                init_fn = None
 
         # `persistent_workers` requires pytorch version >= 1.7
         if ('persistent_workers' in dataloader_cfg
                 and digit_version(TORCH_VERSION) < digit_version('1.7.0')):
             print_log(
                 '`persistent_workers` is only available when '
                 'pytorch version >= 1.7',
@@ -1410,17 +1417,25 @@
         # The default behavior of `collat_fn` in dataloader is to
         # merge a list of samples to form a mini-batch of Tensor(s).
         # However, in mmengine, if `collate_fn` is not defined in
         # dataloader_cfg, `pseudo_collate` will only convert the list of
         # samples into a dict without stacking the batch tensor.
         collate_fn_cfg = dataloader_cfg.pop('collate_fn',
                                             dict(type='pseudo_collate'))
-        collate_fn_type = collate_fn_cfg.pop('type')
-        collate_fn = FUNCTIONS.get(collate_fn_type)
-        collate_fn = partial(collate_fn, **collate_fn_cfg)  # type: ignore
+        if isinstance(collate_fn_cfg, dict):
+            collate_fn_type = collate_fn_cfg.pop('type')
+            collate_fn = FUNCTIONS.get(collate_fn_type)
+            collate_fn = partial(collate_fn, **collate_fn_cfg)  # type: ignore
+        elif callable(collate_fn_cfg):
+            collate_fn = collate_fn_cfg
+        else:
+            raise TypeError(
+                'collate_fn should be a dict or callable object, but got '
+                f'{collate_fn_cfg}')
+
         data_loader = DataLoader(
             dataset=dataset,
             sampler=sampler if batch_sampler is None else None,
             batch_sampler=batch_sampler,
             collate_fn=collate_fn,
             worker_init_fn=init_fn,
             **dataloader_cfg)
@@ -1448,15 +1463,15 @@
         Returns:
             :obj:`BaseLoop`: Training loop object build from ``loop``.
         """
         if isinstance(loop, BaseLoop):
             return loop
         elif not isinstance(loop, dict):
             raise TypeError(
-                f'loop should be a Loop object or dict, but got {loop}')
+                f'train_loop should be a Loop object or dict, but got {loop}')
 
         loop_cfg = copy.deepcopy(loop)
 
         if 'type' in loop_cfg and 'by_epoch' in loop_cfg:
             raise RuntimeError(
                 'Only one of `type` or `by_epoch` can exist in `loop_cfg`.')
 
@@ -1494,15 +1509,15 @@
         Returns:
             :obj:`BaseLoop`: Validation loop object build from ``loop``.
         """
         if isinstance(loop, BaseLoop):
             return loop
         elif not isinstance(loop, dict):
             raise TypeError(
-                f'train_loop should be a Loop object or dict, but got {loop}')
+                f'val_loop should be a Loop object or dict, but got {loop}')
 
         loop_cfg = copy.deepcopy(loop)
 
         if 'type' in loop_cfg:
             loop = LOOPS.build(
                 loop_cfg,
                 default_args=dict(
@@ -1536,15 +1551,15 @@
         Returns:
             :obj:`BaseLoop`: Test loop object build from ``loop_cfg``.
         """
         if isinstance(loop, BaseLoop):
             return loop
         elif not isinstance(loop, dict):
             raise TypeError(
-                f'train_loop should be a Loop object or dict, but got {loop}')
+                f'test_loop should be a Loop object or dict, but got {loop}')
 
         loop_cfg = copy.deepcopy(loop)  # type: ignore
 
         if 'type' in loop_cfg:
             loop = LOOPS.build(
                 loop_cfg,
                 default_args=dict(
@@ -2145,22 +2160,28 @@
 
         if is_model_wrapper(self.model):
             model = self.model.module
         else:
             model = self.model
 
         checkpoint = {
-            'meta': meta,
-            'state_dict': weights_to_cpu(get_state_dict(model)),
-            'message_hub': self.message_hub.state_dict()
+            'meta':
+            meta,
+            'state_dict':
+            weights_to_cpu(model.state_dict()),
+            'message_hub':
+            apply_to(self.message_hub.state_dict(),
+                     lambda x: hasattr(x, 'cpu'), lambda x: x.cpu()),
         }
         # save optimizer state dict to checkpoint
         if save_optimizer:
             if isinstance(self.optim_wrapper, OptimWrapper):
-                checkpoint['optimizer'] = self.optim_wrapper.state_dict()
+                checkpoint['optimizer'] = apply_to(
+                    self.optim_wrapper.state_dict(),
+                    lambda x: hasattr(x, 'cpu'), lambda x: x.cpu())
             else:
                 raise TypeError(
                     'self.optim_wrapper should be an `OptimWrapper` '
                     'or `OptimWrapperDict` instance, but got '
                     f'{self.optim_wrapper}')
 
         # save param scheduler state dict
@@ -2180,15 +2201,19 @@
             else:
                 checkpoint['param_schedulers'] = []
                 for scheduler in self.param_schedulers:  # type: ignore
                     state_dict = scheduler.state_dict()  # type: ignore
                     checkpoint['param_schedulers'].append(state_dict)
 
         self.call_hook('before_save_checkpoint', checkpoint=checkpoint)
-        save_checkpoint(checkpoint, filepath)
+        save_checkpoint(
+            checkpoint,
+            filepath,
+            file_client_args=file_client_args,
+            backend_args=backend_args)
 
     @master_only
     def dump_config(self) -> None:
         """Dump config to `work_dir`."""
         if self.cfg.filename is not None:
             filename = osp.basename(self.cfg.filename)
         else:
@@ -2234,15 +2259,14 @@
             >>> # dict of built list schedulers
             >>> scheduler = dict(linear1=[MultiStepLR(milestones=[1, 2], optimizer=optimizer)],
             >>>                  linear2=[MultiStepLR(milestones=[1, 2], optimizer=optimizer)])
 
         Args:
             param_scheduler (dict or list): The original parameter scheduler.
         """  # noqa: E501
-        param_schedulers: Union[dict, list, _ParamScheduler]
         if param_scheduler is None:
             return
         if isinstance(param_scheduler, _ParamScheduler):
             return
         if is_seq_of(param_scheduler, _ParamScheduler):
             return
```

### Comparing `mmengine-0.7.2/mmengine/runner/utils.py` & `mmengine-0.7.3/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/structures/base_data_element.py` & `mmengine-0.7.3/mmengine/structures/base_data_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,14 +517,24 @@
         for k, v in self.items():
             if isinstance(v, (torch.Tensor, BaseDataElement)):
                 v = v.npu()
                 data = {k: v}
                 new_data.set_data(data)
         return new_data
 
+    def mlu(self) -> 'BaseDataElement':
+        """Convert all tensors to MLU in data."""
+        new_data = self.new()
+        for k, v in self.items():
+            if isinstance(v, (torch.Tensor, BaseDataElement)):
+                v = v.mlu()
+                data = {k: v}
+                new_data.set_data(data)
+        return new_data
+
     # Tensor-like methods
     def detach(self) -> 'BaseDataElement':
         """Detach all tensors in data."""
         new_data = self.new()
         for k, v in self.items():
             if isinstance(v, (torch.Tensor, BaseDataElement)):
                 v = v.detach()
```

### Comparing `mmengine-0.7.2/mmengine/structures/instance_data.py` & `mmengine-0.7.3/mmengine/structures/instance_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import itertools
 from collections.abc import Sized
-from typing import List, Union
+from typing import Any, List, Union
 
 import numpy as np
 import torch
 
+from mmengine.device import get_device
 from .base_data_element import BaseDataElement
 
-IndexType = Union[str, slice, int, list, torch.LongTensor,
-                  torch.cuda.LongTensor, torch.BoolTensor,
-                  torch.cuda.BoolTensor, np.ndarray]
+BoolTypeTensor: Union[Any]
+LongTypeTensor: Union[Any]
+
+if get_device() == 'npu':
+    BoolTypeTensor = Union[torch.BoolTensor, torch.npu.BoolTensor]
+    LongTypeTensor = Union[torch.LongTensor, torch.npu.LongTensor]
+elif get_device() == 'mlu':
+    BoolTypeTensor = Union[torch.BoolTensor, torch.mlu.BoolTensor]
+    LongTypeTensor = Union[torch.LongTensor, torch.mlu.LongTensor]
+else:
+    BoolTypeTensor = Union[torch.BoolTensor, torch.cuda.BoolTensor]
+    LongTypeTensor = Union[torch.LongTensor, torch.cuda.LongTensor]
+
+IndexType: Union[Any] = Union[str, slice, int, list, LongTypeTensor,
+                              BoolTypeTensor, np.ndarray]
 
 
 # Modified from
 # https://github.com/open-mmlab/mmdetection/blob/master/mmdet/core/data_structures/instance_data.py # noqa
 class InstanceData(BaseDataElement):
     """Data structure for instance-level annotations or predictions.
 
@@ -152,26 +165,24 @@
             item (str, int, list, :obj:`slice`, :obj:`numpy.ndarray`,
                 :obj:`torch.LongTensor`, :obj:`torch.BoolTensor`):
                 Get the corresponding values according to item.
 
         Returns:
             :obj:`InstanceData`: Corresponding values.
         """
+        assert isinstance(item, IndexType.__args__)
         if isinstance(item, list):
             item = np.array(item)
         if isinstance(item, np.ndarray):
             # The default int type of numpy is platform dependent, int32 for
             # windows and int64 for linux. `torch.Tensor` requires the index
             # should be int64, therefore we simply convert it to int64 here.
             # More details in https://github.com/numpy/numpy/issues/9464
             item = item.astype(np.int64) if item.dtype == np.int32 else item
             item = torch.from_numpy(item)
-        assert isinstance(
-            item, (str, slice, int, torch.LongTensor, torch.cuda.LongTensor,
-                   torch.BoolTensor, torch.cuda.BoolTensor))
 
         if isinstance(item, str):
             return getattr(self, item)
 
         if isinstance(item, int):
             if item >= len(self) or item < -len(self):  # type:ignore
                 raise IndexError(f'Index {item} out of range!')
@@ -179,15 +190,15 @@
                 # keep the dimension
                 item = slice(item, None, len(self))
 
         new_data = self.__class__(metainfo=self.metainfo)
         if isinstance(item, torch.Tensor):
             assert item.dim() == 1, 'Only support to get the' \
                                     ' values along the first dimension.'
-            if isinstance(item, (torch.BoolTensor, torch.cuda.BoolTensor)):
+            if isinstance(item, BoolTypeTensor.__args__):
                 assert len(item) == len(self), 'The shape of the ' \
                                                'input(BoolTensor) ' \
                                                f'{len(item)} ' \
                                                'does not match the shape ' \
                                                'of the indexed tensor ' \
                                                'in results_field ' \
                                                f'{len(self)} at ' \
@@ -198,16 +209,15 @@
                     new_data[k] = v[item]
                 elif isinstance(v, np.ndarray):
                     new_data[k] = v[item.cpu().numpy()]
                 elif isinstance(
                         v, (str, list, tuple)) or (hasattr(v, '__getitem__')
                                                    and hasattr(v, 'cat')):
                     # convert to indexes from BoolTensor
-                    if isinstance(item,
-                                  (torch.BoolTensor, torch.cuda.BoolTensor)):
+                    if isinstance(item, BoolTypeTensor.__args__):
                         indexes = torch.nonzero(item).view(
                             -1).cpu().numpy().tolist()
                     else:
                         indexes = item.cpu().numpy().tolist()
                     slice_list = []
                     if indexes:
                         for index in indexes:
```

### Comparing `mmengine-0.7.2/mmengine/structures/label_data.py` & `mmengine-0.7.3/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/structures/pixel_data.py` & `mmengine-0.7.3/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/testing/__init__.py` & `mmengine-0.7.3/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/testing/_internal/distributed.py` & `mmengine-0.7.3/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/testing/compare.py` & `mmengine-0.7.3/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/testing/runner_test_case.py` & `mmengine-0.7.3/mmengine/testing/runner_test_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 import logging
 import os
+import shutil
 import tempfile
 import time
 from unittest import TestCase
 from uuid import uuid4
 
 import torch
 import torch.nn as nn
@@ -180,7 +181,16 @@
     def setup_dist_env(self):
         self.dist_cfg['MASTER_PORT'] += 1
         os.environ['MASTER_PORT'] = str(self.dist_cfg['MASTER_PORT'])
         os.environ['MASTER_ADDR'] = self.dist_cfg['MASTER_ADDR']
         os.environ['RANK'] = self.dist_cfg['RANK']
         os.environ['WORLD_SIZE'] = self.dist_cfg['WORLD_SIZE']
         os.environ['LOCAL_RANK'] = self.dist_cfg['LOCAL_RANK']
+
+    def clear_work_dir(self):
+        logging.shutdown()
+        for filename in os.listdir(self.temp_dir.name):
+            filepath = os.path.join(self.temp_dir.name, filename)
+            if os.path.isfile(filepath):
+                os.remove(filepath)
+            else:
+                shutil.rmtree(filepath)
```

### Comparing `mmengine-0.7.2/mmengine/utils/__init__.py` & `mmengine-0.7.3/mmengine/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .manager import ManagerMeta, ManagerMixin
-from .misc import (check_prerequisites, concat_list, deprecated_api_warning,
-                   deprecated_function, has_method,
+from .misc import (apply_to, check_prerequisites, concat_list,
+                   deprecated_api_warning, deprecated_function, has_method,
                    import_modules_from_strings, is_list_of,
                    is_method_overridden, is_seq_of, is_str, is_tuple_of,
                    iter_cast, list_cast, requires_executable, requires_package,
                    slice_list, to_1tuple, to_2tuple, to_3tuple, to_4tuple,
                    to_ntuple, tuple_cast)
 from .package_utils import (call_command, get_installed_path, install_package,
                             is_installed)
@@ -23,9 +23,10 @@
     'is_filepath', 'fopen', 'check_file_exist', 'mkdir_or_exist', 'symlink',
     'scandir', 'deprecated_api_warning', 'import_modules_from_strings',
     'to_1tuple', 'to_2tuple', 'to_3tuple', 'to_4tuple', 'to_ntuple',
     'is_installed', 'call_command', 'get_installed_path', 'install_package',
     'is_abs', 'is_method_overridden', 'has_method', 'digit_version',
     'get_git_hash', 'ManagerMeta', 'ManagerMixin', 'Timer', 'check_time',
     'TimerError', 'ProgressBar', 'track_iter_progress',
-    'track_parallel_progress', 'track_progress', 'deprecated_function'
+    'track_parallel_progress', 'track_progress', 'deprecated_function',
+    'apply_to'
 ]
```

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/hub.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/misc.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/trace.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.7.3/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/manager.py` & `mmengine-0.7.3/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/misc.py` & `mmengine-0.7.3/mmengine/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,14 +213,55 @@
 
     Returns:
         list: The concatenated flat list.
     """
     return list(itertools.chain(*in_list))
 
 
+def apply_to(data: Any, expr: Callable, apply_func: Callable):
+    """Apply function to each element in dict, list or tuple that matches with
+    the expression.
+
+    For examples, if you want to convert each element in a list of dict from
+    `np.ndarray` to `Tensor`. You can use the following code:
+
+    Examples:
+        >>> from mmengine.utils import apply_to
+        >>> import numpy as np
+        >>> import torch
+        >>> data = dict(array=[np.array(1)]) # {'array': [array(1)]}
+        >>> result = apply_to(data, lambda x: isinstance(x, np.ndarray), lambda x: torch.from_numpy(x))
+        >>> print(result) # {'array': [tensor(1)]}
+
+    Args:
+        data (Any): Data to be applied.
+        expr (Callable): Expression to tell which data should be applied with
+            the function. It should return a boolean.
+        apply_func (Callable): Function applied to data.
+
+    Returns:
+        Any: The data after applying.
+    """  # noqa: E501
+    if isinstance(data, dict):
+        # Keep the original dict type
+        res = type(data)()
+        for key, value in data.items():
+            res[key] = apply_to(value, expr, apply_func)
+        return res
+    elif isinstance(data, tuple) and hasattr(data, '_fields'):
+        # namedtuple
+        return type(data)(*(apply_to(sample, expr, apply_func) for sample in data))  # type: ignore  # noqa: E501  # yapf:disable
+    elif isinstance(data, (tuple, list)):
+        return type(data)(apply_to(sample, expr, apply_func) for sample in data)  # type: ignore  # noqa: E501  # yapf:disable
+    elif expr(data):
+        return apply_func(data)
+    else:
+        return data
+
+
 def check_prerequisites(
         prerequisites,
         checker,
         msg_tmpl='Prerequisites "{}" are required in method "{}" but not '
                  'found, please install them first.'):  # yapf: disable
     """A decorator factory to check if prerequisites are satisfied.
```

### Comparing `mmengine-0.7.2/mmengine/utils/package_utils.py` & `mmengine-0.7.3/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/path.py` & `mmengine-0.7.3/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/progressbar.py` & `mmengine-0.7.3/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/timer.py` & `mmengine-0.7.3/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/utils/version_utils.py` & `mmengine-0.7.3/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/mmengine/version.py` & `mmengine-0.7.3/mmengine/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.7.2'
+__version__ = '0.7.3'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.7.2/mmengine/visualization/utils.py` & `mmengine-0.7.3/mmengine/visualization/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,22 +166,22 @@
     heat_img = cv2.applyColorMap(norm_img, cv2.COLORMAP_JET)
     heat_img = cv2.cvtColor(heat_img, cv2.COLOR_BGR2RGB)
     if img is not None:
         heat_img = cv2.addWeighted(img, 1 - alpha, heat_img, alpha, 0)
     return heat_img
 
 
-def wait_continue(figure, timeout: int = 0, continue_key: str = ' ') -> int:
+def wait_continue(figure, timeout: float = 0, continue_key: str = ' ') -> int:
     """Show the image and wait for the user's input.
 
     This implementation refers to
     https://github.com/matplotlib/matplotlib/blob/v3.5.x/lib/matplotlib/_blocking_input.py
 
     Args:
-        timeout (int): If positive, continue after ``timeout`` seconds.
+        timeout (float): If positive, continue after ``timeout`` seconds.
             Defaults to 0.
         continue_key (str): The key for users to continue. Defaults to
             the space key.
 
     Returns:
         int: If zero, means time out or the user pressed ``continue_key``,
             and if one, means the user closed the show figure.
```

### Comparing `mmengine-0.7.2/mmengine/visualization/vis_backend.py` & `mmengine-0.7.3/mmengine/visualization/vis_backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 import copy
 import functools
 import logging
 import os
 import os.path as osp
 import warnings
 from abc import ABCMeta, abstractmethod
+from collections.abc import MutableMapping
 from typing import Any, Callable, Optional, Sequence, Union
 
 import cv2
 import numpy as np
 import torch
 
 from mmengine.config import Config
 from mmengine.fileio import dump
-from mmengine.logging import print_log
+from mmengine.hooks.logger_hook import SUFFIX_TYPE
+from mmengine.logging import MMLogger, print_log
 from mmengine.registry import VISBACKENDS
+from mmengine.utils import scandir
 from mmengine.utils.dl_utils import TORCH_VERSION
 
 
 def force_init_env(old_func: Callable) -> Any:
     """Those methods decorated by ``force_init_env`` will be forced to call
     ``_init_env`` if the instance has not been fully initiated. This function
     will decorated all the `add_xxx` method and `experiment` method, because
@@ -609,7 +612,207 @@
         for key, value in scalar_dict.items():
             self.add_scalar(key, value, step)
 
     def close(self):
         """close an opened tensorboard object."""
         if hasattr(self, '_tensorboard'):
             self._tensorboard.close()
+
+
+@VISBACKENDS.register_module()
+class MLflowVisBackend(BaseVisBackend):
+    """MLflow visualization backend class.
+
+    It can write images, config, scalars, etc. to a
+    mlflow file.
+
+    Examples:
+        >>> from mmengine.visualization import MLflowVisBackend
+        >>> from mmengine import Config
+        >>> import numpy as np
+        >>> vis_backend = MLflowVisBackend(save_dir='temp_dir')
+        >>> img = np.random.randint(0, 256, size=(10, 10, 3))
+        >>> vis_backend.add_image('img.png', img)
+        >>> vis_backend.add_scalar('mAP', 0.6)
+        >>> vis_backend.add_scalars({'loss': 0.1,'acc':0.8})
+        >>> cfg = Config(dict(a=1, b=dict(b1=[0, 1])))
+        >>> vis_backend.add_config(cfg)
+
+    Args:
+        save_dir (str): The root directory to save the files
+            produced by the backend.
+        exp_name (str, optional): The experiment name. Default to None.
+        run_name (str, optional): The run name. Default to None.
+        tags (dict, optional): The tags to be added to the experiment.
+            Default to None.
+        params (dict, optional): The params to be added to the experiment.
+            Default to None.
+        tracking_uri (str, optional): The tracking uri. Default to None.
+        artifact_suffix (Tuple[str] or str, optional): The artifact suffix.
+            Default to ('.json', '.log', '.py', 'yaml').
+    """
+
+    def __init__(self,
+                 save_dir: str,
+                 exp_name: Optional[str] = None,
+                 run_name: Optional[str] = None,
+                 tags: Optional[dict] = None,
+                 params: Optional[dict] = None,
+                 tracking_uri: Optional[str] = None,
+                 artifact_suffix: SUFFIX_TYPE = ('.json', '.log', '.py',
+                                                 'yaml')):
+        super().__init__(save_dir)
+        self._exp_name = exp_name
+        self._run_name = run_name
+        self._tags = tags
+        self._params = params
+        self._tracking_uri = tracking_uri
+        self._artifact_suffix = artifact_suffix
+
+    def _init_env(self):
+        """Setup env for MLflow."""
+        if not os.path.exists(self._save_dir):
+            os.makedirs(self._save_dir, exist_ok=True)  # type: ignore
+
+        try:
+            import mlflow
+        except ImportError:
+            raise ImportError(
+                'Please run "pip install mlflow" to install mlflow'
+            )  # type: ignore
+        self._mlflow = mlflow
+
+        # when mlflow is imported, a default logger is created.
+        # at this time, the default logger's stream is None
+        # so the stream is reopened only when the stream is None
+        # or the stream is closed
+        logger = MMLogger.get_current_instance()
+        for handler in logger.handlers:
+            if handler.stream is None or handler.stream.closed:
+                handler.stream = open(handler.baseFilename, 'a')
+
+        if self._tracking_uri is not None:
+            logger.warning(
+                'Please make sure that the mlflow server is running.')
+            self._mlflow.set_tracking_uri(self._tracking_uri)
+        else:
+            if os.name == 'nt':
+                file_url = f'file:\\{os.path.abspath(self._save_dir)}'
+            else:
+                file_url = f'file://{os.path.abspath(self._save_dir)}'
+            self._mlflow.set_tracking_uri(file_url)
+
+        self._exp_name = self._exp_name or 'Default'
+
+        if self._mlflow.get_experiment_by_name(self._exp_name) is None:
+            self._mlflow.create_experiment(self._exp_name)
+
+        self._mlflow.set_experiment(self._exp_name)
+
+        if self._run_name is not None:
+            self._mlflow.set_tag('mlflow.runName', self._run_name)
+        if self._tags is not None:
+            self._mlflow.set_tags(self._tags)
+        if self._params is not None:
+            self._mlflow.log_params(self._params)
+
+    @property  # type: ignore
+    @force_init_env
+    def experiment(self):
+        """Return MLflow object."""
+        return self._mlflow
+
+    @force_init_env
+    def add_config(self, config: Config, **kwargs) -> None:
+        """Record the config to mlflow.
+
+        Args:
+            config (Config): The Config object
+        """
+        self.cfg = config
+        self._mlflow.log_params(self._flatten(self.cfg))
+        self._mlflow.log_text(self.cfg.pretty_text, 'config.py')
+
+    @force_init_env
+    def add_image(self,
+                  name: str,
+                  image: np.ndarray,
+                  step: int = 0,
+                  **kwargs) -> None:
+        """Record the image to mlflow.
+
+        Args:
+            name (str): The image identifier.
+            image (np.ndarray): The image to be saved. The format
+                should be RGB.
+            step (int): Global step value to record. Default to 0.
+        """
+        self._mlflow.log_image(image, name)
+
+    @force_init_env
+    def add_scalar(self,
+                   name: str,
+                   value: Union[int, float, torch.Tensor, np.ndarray],
+                   step: int = 0,
+                   **kwargs) -> None:
+        """Record the scalar data to mlflow.
+
+        Args:
+            name (str): The scalar identifier.
+            value (int, float, torch.Tensor, np.ndarray): Value to save.
+            step (int): Global step value to record. Default to 0.
+        """
+        self._mlflow.log_metric(name, value, step)
+
+    @force_init_env
+    def add_scalars(self,
+                    scalar_dict: dict,
+                    step: int = 0,
+                    file_path: Optional[str] = None,
+                    **kwargs) -> None:
+        """Record the scalar's data to mlflow.
+
+        Args:
+            scalar_dict (dict): Key-value pair storing the tag and
+                corresponding values.
+            step (int): Global step value to record. Default to 0.
+            file_path (str, optional): Useless parameter. Just for
+                interface unification. Default to None.
+        """
+        assert isinstance(scalar_dict, dict)
+        assert 'step' not in scalar_dict, 'Please set it directly ' \
+                                          'through the step parameter'
+        self._mlflow.log_metrics(scalar_dict, step)
+
+    def close(self) -> None:
+        """Close the mlflow."""
+        file_paths = dict()
+        for filename in scandir(self.cfg.work_dir, self._artifact_suffix,
+                                True):
+            file_path = osp.join(self.cfg.work_dir, filename)
+            relative_path = os.path.relpath(file_path, self.cfg.work_dir)
+            dir_path = os.path.dirname(relative_path)
+            file_paths[file_path] = dir_path
+
+        for file_path, dir_path in file_paths.items():
+            self._mlflow.log_artifact(file_path, dir_path)
+
+        if hasattr(self, '_mlflow'):
+            self._mlflow.end_run()
+
+    def _flatten(self, d, parent_key='', sep='.') -> dict:
+        """Flatten the dict."""
+        items = dict()
+        for k, v in d.items():
+            new_key = parent_key + sep + k if parent_key else k
+            if isinstance(v, MutableMapping):
+                items.update(self._flatten(v, new_key, sep=sep))
+            elif isinstance(v, list):
+                if any(isinstance(x, dict) for x in v):
+                    for i, x in enumerate(v):
+                        items.update(
+                            self._flatten(x, new_key + sep + str(i), sep=sep))
+                else:
+                    items[new_key] = v
+            else:
+                items[new_key] = v
+        return items
```

### Comparing `mmengine-0.7.2/mmengine/visualization/visualizer.py` & `mmengine-0.7.3/mmengine/visualization/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,45 +224,61 @@
         """Set the dataset meta info to the Visualizer."""
         self._dataset_meta = dataset_meta
 
     @master_only
     def show(self,
              drawn_img: Optional[np.ndarray] = None,
              win_name: str = 'image',
-             wait_time: int = 0,
-             continue_key=' ') -> None:
+             wait_time: float = 0.,
+             continue_key: str = ' ',
+             backend: str = 'matplotlib') -> None:
         """Show the drawn image.
 
         Args:
             drawn_img (np.ndarray, optional): The image to show. If drawn_img
                 is None, it will show the image got by Visualizer. Defaults
                 to None.
             win_name (str):  The image title. Defaults to 'image'.
-            wait_time (int): Delay in milliseconds. 0 is the special
+            wait_time (float): Delay in seconds. 0 is the special
                 value that means "forever". Defaults to 0.
             continue_key (str): The key for users to continue. Defaults to
                 the space key.
+            backend (str): The backend to show the image. Defaults to
+                'matplotlib'. `New in version 0.7.3.`
         """
-        import matplotlib.pyplot as plt
-        is_inline = 'inline' in plt.get_backend()
-        img = self.get_image() if drawn_img is None else drawn_img
-        self._init_manager(win_name)
-        fig = self.manager.canvas.figure
-        # remove white edges by set subplot margin
-        fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
-        fig.clear()
-        ax = fig.add_subplot()
-        ax.axis(False)
-        ax.imshow(img)
-        self.manager.canvas.draw()
+        if backend == 'matplotlib':
+            import matplotlib.pyplot as plt
+            is_inline = 'inline' in plt.get_backend()
+            img = self.get_image() if drawn_img is None else drawn_img
+            self._init_manager(win_name)
+            fig = self.manager.canvas.figure
+            # remove white edges by set subplot margin
+            fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
+            fig.clear()
+            ax = fig.add_subplot()
+            ax.axis(False)
+            ax.imshow(img)
+            self.manager.canvas.draw()
 
-        # Find a better way for inline to show the image
-        if is_inline:
-            return fig
-        wait_continue(fig, timeout=wait_time, continue_key=continue_key)
+            # Find a better way for inline to show the image
+            if is_inline:
+                return fig
+            wait_continue(fig, timeout=wait_time, continue_key=continue_key)
+        elif backend == 'cv2':
+            # Keep images are shown in the same window, and the title of window
+            # will be updated with `win_name`.
+            cv2.namedWindow(winname=f'{id(self)}')
+            cv2.setWindowTitle(f'{id(self)}', win_name)
+            cv2.imshow(
+                str(id(self)),
+                self.get_image() if drawn_img is None else drawn_img)
+            cv2.waitKey(int(np.ceil(wait_time * 1000)))
+        else:
+            raise ValueError('backend should be "matplotlib" or "cv2", '
+                             f'but got {backend} instead')
 
     @master_only
     def set_image(self, image: np.ndarray) -> None:
         """Set the image to draw.
 
         Args:
             image (np.ndarray): The image to draw.
```

### Comparing `mmengine-0.7.2/mmengine.egg-info/PKG-INFO` & `mmengine-0.7.3/mmengine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.7.2
+Version: 0.7.3
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -84,17 +84,22 @@
         
            - Defines the training process just like playing with Legos.
            - Provides rich components and strategies.
            - Complete controls on the training process with different levels of APIs.
         
         ## What's New
         
-        v0.7.2 was released on 2023-04-06.
+        v0.7.3 was released on 2023-04-28.
         
-        Read [Changelog](./docs/en/notes/changelog.md#v071-04062023) for more details.
+        ### Highlights
+        
+        - Support using MLflow to record experiment data
+        - Support registering callable objects to the registry
+        
+        Read [Changelog](./docs/en/notes/changelog.md#v073-04282023) for more details.
         
         ## Installation
         
         Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
         
         Install MMEngine
         
@@ -333,32 +338,32 @@
         This project is released under the [Apache 2.0 license](LICENSE).
         
         ## Projects in OpenMMLab
         
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-        - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
+        - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+        - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
         - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
         - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
         - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
         - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
         - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
         - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
         - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
         - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
         - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
         - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
         - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+        - [Playground](https://github.com/open-mmlab/playground): A central hub for gathering and showcasing amazing projects built upon OpenMMLab.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mmengine-0.7.2/mmengine.egg-info/SOURCES.txt` & `mmengine-0.7.3/mmengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.2/setup.py` & `mmengine-0.7.3/setup.py`

 * *Files identical despite different names*

