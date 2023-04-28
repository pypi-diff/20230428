# Comparing `tmp/ddsp-3.5.1.tar.gz` & `tmp/ddsp-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddsp-3.5.1.tar", last modified: Wed Apr 26 18:27:36 2023, max compression
+gzip compressed data, was "dist/ddsp-3.6.0.tar", last modified: Fri Apr 28 01:27:41 2023, max compression
```

## Comparing `ddsp-3.5.1.tar` & `ddsp-3.6.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)       63 2023-04-26 18:27:36.000000 ddsp-3.5.1/setup.cfg
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13253 2023-04-26 18:27:33.000000 ddsp-3.5.1/README.md
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-26 18:27:36.000000 ddsp-3.5.1/PKG-INFO
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3269 2023-04-26 18:27:33.000000 ddsp-3.5.1/setup.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3873 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/effects_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11482 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/synths.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/colab/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/colab/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10035 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/colab/colab_utils.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1139 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/test_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      908 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3753 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/processors_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    63698 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/core.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19427 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/spectral_ops.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      794 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/version.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9610 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/processors.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11158 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/spectral_ops_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13484 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/effects.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3189 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/losses_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10127 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/heuristics.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/models/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11984 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/inverse_synthesis.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2482 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/autoencoder.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1594 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2834 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/autoencoder_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4715 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/model.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    23617 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/midi_autoencoder.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9529 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/metrics_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9122 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/eval_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9400 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/decoders.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8503 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/preprocessing.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    21779 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19583 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/inference.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8753 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/nn_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7919 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/plotting.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2292 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/preprocessing_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1182 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8700 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/ddsp_run.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19956 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/metrics.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     6810 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/trainers.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    15113 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/encoders.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    16563 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/summaries.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8307 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/evaluators.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/models/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/vst_32k.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/vst_48k.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2453 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/vst.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1854 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1049 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/solo_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/__init__.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/optimization/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      416 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/optimization/base.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/optimization/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      116 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/optimization/base_tpu.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/datasets/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      224 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/base.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      351 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/tfrecord.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      475 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/nsynth.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/eval/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      176 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/heuristic_power.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      170 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/heuristic.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      158 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/basic_f0_ld_twm.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      150 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/midi_ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      138 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/basic_f0_ld.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      119 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/basic.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/papers/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      217 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/tiny_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      221 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/nsynth_ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      267 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/solo_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/__init__.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1881 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_model.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      730 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/finetune_dataset.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      472 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/finetune_model.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      679 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    12720 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/ddsp_export.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2885 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/cloud.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13804 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/postprocessing.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11770 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/train_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4177 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/decoders_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    45858 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/nn.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3010 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/heuristics_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/docker/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3441 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/task_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      640 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9500 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/ddsp_ai_platform.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     5036 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/task.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/data_preparation/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4406 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10303 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      692 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3852 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10070 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/synthetic_data.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7832 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2970 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/cloud_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    36651 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/core_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    40636 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/losses.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3744 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/dags_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7416 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/dags.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3736 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/synths_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      445 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/requires.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3282 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/SOURCES.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/PKG-INFO
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      424 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/entry_points.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)        1 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/dependency_links.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)        5 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/top_level.txt
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)       63 2023-04-28 01:27:41.000000 ddsp-3.6.0/setup.cfg
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13253 2023-04-28 01:27:39.000000 ddsp-3.6.0/README.md
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-28 01:27:41.000000 ddsp-3.6.0/PKG-INFO
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3240 2023-04-28 01:27:39.000000 ddsp-3.6.0/setup.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3873 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/effects_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11482 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/synths.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/colab/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/colab/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10035 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/colab/colab_utils.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1139 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/test_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      908 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3753 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/processors_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    63698 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/core.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19427 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/spectral_ops.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      794 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/version.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9610 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/processors.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11158 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/spectral_ops_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13484 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/effects.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3189 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/losses_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10127 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/heuristics.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/models/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11984 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/inverse_synthesis.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2482 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/autoencoder.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1594 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2834 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/autoencoder_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4715 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/model.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    23617 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/models/midi_autoencoder.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9529 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/metrics_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9122 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/eval_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9400 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/decoders.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8503 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/preprocessing.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    21779 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19583 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/inference.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8753 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/nn_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7919 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/plotting.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2292 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/preprocessing_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1182 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8700 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/ddsp_run.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19956 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/metrics.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     6810 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/trainers.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    15113 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/encoders.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    16563 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/summaries.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8307 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/evaluators.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/models/
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/vst_32k.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/vst_48k.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2453 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/vst/vst.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1854 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1049 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/models/solo_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/optimization/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      416 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/optimization/base.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/optimization/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      116 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/optimization/base_tpu.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/datasets/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      224 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/base.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      351 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/tfrecord.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      475 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/datasets/nsynth.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/eval/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      176 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/heuristic_power.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      170 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/heuristic.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      158 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/basic_f0_ld_twm.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      150 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/midi_ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      138 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/basic_f0_ld.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      119 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/eval/basic.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/papers/
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      217 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/tiny_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      221 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/nsynth_ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      267 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/solo_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1881 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      730 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      472 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/finetune_model.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      679 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    12720 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/ddsp_export.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2885 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/cloud.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13804 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/postprocessing.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11770 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/train_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4177 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/decoders_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    49484 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/nn.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3010 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/heuristics_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/docker/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3441 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/task_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      640 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9500 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/ddsp_ai_platform.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     5036 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/docker/task.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp/training/data_preparation/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4406 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10303 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      692 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3852 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10070 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/synthetic_data.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7832 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2970 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/training/cloud_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    36651 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/core_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    40636 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/losses.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3744 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/dags_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7416 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/dags.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3736 2023-04-28 01:27:39.000000 ddsp-3.6.0/ddsp/synths_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      427 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/requires.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3282 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/SOURCES.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/PKG-INFO
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      424 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/entry_points.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)        1 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/dependency_links.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)        5 2023-04-28 01:27:41.000000 ddsp-3.6.0/ddsp.egg-info/top_level.txt
```

### Comparing `ddsp-3.5.1/README.md` & `ddsp-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/PKG-INFO` & `ddsp-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddsp
-Version: 3.5.1
+Version: 3.6.0
 Summary: Differentiable Digital Signal Processing 
 Home-page: http://github.com/magenta/ddsp
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
 Description: UNKNOWN
 Keywords: audio dsp signalprocessing machinelearning music
```

### Comparing `ddsp-3.5.1/setup.py` & `ddsp-3.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         'protobuf<=3.20',  # temporary fix for proto dependency bug
         'mir_eval',
         'note_seq<0.0.4',
         'numpy<1.24',
         'scipy',
         'six',
         'tensorflow',
-        'tensorflow-addons',
         'tensorflowjs<3.19',
         'tensorflow-probability',
         'tensorflow-datasets',
         'tflite_support'
     ],
     extras_require={
         'gcp': [
```

### Comparing `ddsp-3.5.1/ddsp/effects_test.py` & `ddsp-3.6.0/ddsp/effects_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/synths.py` & `ddsp-3.6.0/ddsp/synths.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/colab/__init__.py` & `ddsp-3.6.0/ddsp/colab/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/colab/colab_utils.py` & `ddsp-3.6.0/ddsp/colab/colab_utils.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/test_util.py` & `ddsp-3.6.0/ddsp/test_util.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/__init__.py` & `ddsp-3.6.0/ddsp/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/processors_test.py` & `ddsp-3.6.0/ddsp/processors_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/core.py` & `ddsp-3.6.0/ddsp/core.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/spectral_ops.py` & `ddsp-3.6.0/ddsp/spectral_ops.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/version.py` & `ddsp-3.6.0/ddsp/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 r"""Separate file for storing the current version of DDSP.
 
 Stored in a separate file so that setup.py can reference the version without
 pulling in all the dependencies in __init__.py.
 """
 
-__version__ = '3.5.1'
+__version__ = '3.6.0'
```

### Comparing `ddsp-3.5.1/ddsp/processors.py` & `ddsp-3.6.0/ddsp/processors.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/spectral_ops_test.py` & `ddsp-3.6.0/ddsp/spectral_ops_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/effects.py` & `ddsp-3.6.0/ddsp/effects.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/losses_test.py` & `ddsp-3.6.0/ddsp/losses_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/heuristics.py` & `ddsp-3.6.0/ddsp/training/heuristics.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/models/inverse_synthesis.py` & `ddsp-3.6.0/ddsp/training/models/inverse_synthesis.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/models/autoencoder.py` & `ddsp-3.6.0/ddsp/training/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/models/__init__.py` & `ddsp-3.6.0/ddsp/training/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/models/autoencoder_test.py` & `ddsp-3.6.0/ddsp/training/models/autoencoder_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/models/model.py` & `ddsp-3.6.0/ddsp/training/models/model.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/models/midi_autoencoder.py` & `ddsp-3.6.0/ddsp/training/models/midi_autoencoder.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/metrics_test.py` & `ddsp-3.6.0/ddsp/training/metrics_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/eval_util.py` & `ddsp-3.6.0/ddsp/training/eval_util.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/decoders.py` & `ddsp-3.6.0/ddsp/training/decoders.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/preprocessing.py` & `ddsp-3.6.0/ddsp/training/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data.py` & `ddsp-3.6.0/ddsp/training/data.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/inference.py` & `ddsp-3.6.0/ddsp/training/inference.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/nn_test.py` & `ddsp-3.6.0/ddsp/training/nn_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/plotting.py` & `ddsp-3.6.0/ddsp/training/plotting.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/preprocessing_test.py` & `ddsp-3.6.0/ddsp/training/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/__init__.py` & `ddsp-3.6.0/ddsp/training/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/ddsp_run.py` & `ddsp-3.6.0/ddsp/training/ddsp_run.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/metrics.py` & `ddsp-3.6.0/ddsp/training/metrics.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/trainers.py` & `ddsp-3.6.0/ddsp/training/trainers.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/encoders.py` & `ddsp-3.6.0/ddsp/training/encoders.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/summaries.py` & `ddsp-3.6.0/ddsp/training/summaries.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/evaluators.py` & `ddsp-3.6.0/ddsp/training/evaluators.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/vst/vst_32k.gin` & `ddsp-3.6.0/ddsp/training/gin/models/vst/vst_32k.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/vst/vst_48k.gin` & `ddsp-3.6.0/ddsp/training/gin/models/vst/vst_48k.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/vst/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/models/vst/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/vst/vst.gin` & `ddsp-3.6.0/ddsp/training/gin/models/vst/vst.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/ae.gin` & `ddsp-3.6.0/ddsp/training/gin/models/ae.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/models/solo_instrument.gin` & `ddsp-3.6.0/ddsp/training/gin/models/solo_instrument.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/optimization/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/datasets/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/eval/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/papers/iclr2020/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/papers/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/papers/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_model.gin` & `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/__init__.py` & `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/finetune_dataset.gin` & `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin` & `ddsp-3.6.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/ddsp_export.py` & `ddsp-3.6.0/ddsp/training/ddsp_export.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/cloud.py` & `ddsp-3.6.0/ddsp/training/cloud.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/postprocessing.py` & `ddsp-3.6.0/ddsp/training/postprocessing.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/train_util.py` & `ddsp-3.6.0/ddsp/training/train_util.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/decoders_test.py` & `ddsp-3.6.0/ddsp/training/decoders_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/nn.py` & `ddsp-3.6.0/ddsp/training/nn.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import inspect
 
 from ddsp import core
 from ddsp import losses
 import gin
 import tensorflow as tf
-from tensorflow_addons.layers import SpectralNormalization
 import tensorflow_probability as tfp
 
 tfk = tf.keras
 tfkl = tfk.layers
 
 
 # False positive lint error on tf.split().
@@ -942,14 +941,131 @@
 
   def call(self, x):
     return x
 
 gin.register(tfkl.Dense, module=__name__)
 
 
+class SpectralNormalization(tf.keras.layers.Wrapper):
+  """Performs spectral normalization on weights.
+
+  Copied from soon to be deprecated TF addons that broke training.
+  https://github.com/tensorflow/addons/issues/2807
+
+  This wrapper controls the Lipschitz constant of the layer by
+  constraining its spectral norm, which can stabilize the training of GANs.
+
+  See [Spectral Normalization for Generative Adversarial
+  Networks](https://arxiv.org/abs/1802.05957).
+
+  Wrap `tf.keras.layers.Conv2D`:
+
+  >>> x = np.random.rand(1, 10, 10, 1)
+  >>> conv2d = SpectralNormalization(tf.keras.layers.Conv2D(2, 2))
+  >>> y = conv2d(x)
+  >>> y.shape
+  TensorShape([1, 9, 9, 2])
+
+  Wrap `tf.keras.layers.Dense`:
+
+  >>> x = np.random.rand(1, 10, 10, 1)
+  >>> dense = SpectralNormalization(tf.keras.layers.Dense(10))
+  >>> y = dense(x)
+  >>> y.shape
+  TensorShape([1, 10, 10, 10])
+
+    Args:
+      layer: A `tf.keras.layers.Layer` instance that has either `kernel` or
+        `embeddings` attribute.
+      power_iterations: `int`, the number of iterations during normalization.
+
+    Raises:
+      AssertionError: If not initialized with a `Layer` instance.
+      ValueError: If initialized with negative `power_iterations`.
+      AttributeError: If `layer` does not has `kernel` or `embeddings`
+      attribute.
+  """
+
+  def __init__(self,
+               layer: tf.keras.layers,
+               power_iterations: int = 1,
+               **kwargs):
+    super().__init__(layer, **kwargs)
+    if power_iterations <= 0:
+      raise ValueError('`power_iterations` should be greater than zero, got '
+                       '`power_iterations={}`'.format(power_iterations))
+    self.power_iterations = power_iterations
+    self._initialized = False
+
+  def build(self, input_shape):
+    """Build `Layer`."""
+    super().build(input_shape)
+    input_shape = tf.TensorShape(input_shape)
+    self.input_spec = tf.keras.layers.InputSpec(shape=[None] + input_shape[1:])
+
+    if hasattr(self.layer, 'kernel'):
+      self.w = self.layer.kernel
+    elif hasattr(self.layer, 'embeddings'):
+      self.w = self.layer.embeddings
+    else:
+      raise AttributeError('{} object has no attribute "kernel" nor '
+                           '"embeddings"'.format(type(self.layer).__name__))
+
+    self.w_shape = self.w.shape.as_list()
+
+    self.u = self.add_weight(
+        shape=(1, self.w_shape[-1]),
+        initializer=tf.initializers.TruncatedNormal(stddev=0.02),
+        trainable=False,
+        name='sn_u',
+        dtype=self.w.dtype,
+    )
+
+  def call(self, inputs, training=None):
+    """Call `Layer`."""
+    if training is None:
+      training = tf.keras.backend.learning_phase()
+
+    if training:
+      self.normalize_weights()
+
+    output = self.layer(inputs)
+    return output
+
+  def compute_output_shape(self, input_shape):
+    return tf.TensorShape(
+        self.layer.compute_output_shape(input_shape).as_list())
+
+  @tf.function
+  def normalize_weights(self):
+    """Generate spectral normalized weights.
+
+    This method will update the value of `self.w` with the
+    spectral normalized value, so that the layer is ready for `call()`.
+    """
+
+    w = tf.reshape(self.w, [-1, self.w_shape[-1]])
+    u = self.u
+
+    with tf.name_scope('spectral_normalize'):
+      for _ in range(self.power_iterations):
+        v = tf.math.l2_normalize(tf.matmul(u, w, transpose_b=True))
+        u = tf.math.l2_normalize(tf.matmul(v, w))
+
+      sigma = tf.matmul(tf.matmul(v, w), u, transpose_b=True)
+
+      self.w.assign(self.w / sigma)
+      self.u.assign(u)
+
+  def get_config(self):
+    config = {'power_iterations': self.power_iterations}
+    base_config = super().get_config()
+    return {**base_config, **config}
+
+
 # ------------------ Embeddings ------------------------------------------------
 def get_embedding(vocab_size=1024, n_dims=256):
   """Get a real-valued embedding from an integer."""
   return tfkl.Embedding(
       input_dim=vocab_size,
       output_dim=n_dims,
       input_length=1)
```

### Comparing `ddsp-3.5.1/ddsp/training/heuristics_test.py` & `ddsp-3.6.0/ddsp/training/heuristics_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/docker/task_test.py` & `ddsp-3.6.0/ddsp/training/docker/task_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/docker/__init__.py` & `ddsp-3.6.0/ddsp/training/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/docker/ddsp_ai_platform.py` & `ddsp-3.6.0/ddsp/training/docker/ddsp_ai_platform.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/docker/task.py` & `ddsp-3.6.0/ddsp/training/docker/task.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py` & `ddsp-3.6.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib.py` & `ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data_preparation/__init__.py` & `ddsp-3.6.0/ddsp/training/data_preparation/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py` & `ddsp-3.6.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data_preparation/synthetic_data.py` & `ddsp-3.6.0/ddsp/training/data_preparation/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py` & `ddsp-3.6.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/training/cloud_test.py` & `ddsp-3.6.0/ddsp/training/cloud_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/core_test.py` & `ddsp-3.6.0/ddsp/core_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/losses.py` & `ddsp-3.6.0/ddsp/losses.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/dags_test.py` & `ddsp-3.6.0/ddsp/dags_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/dags.py` & `ddsp-3.6.0/ddsp/dags.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp/synths_test.py` & `ddsp-3.6.0/ddsp/synths_test.py`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp.egg-info/SOURCES.txt` & `ddsp-3.6.0/ddsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.1/ddsp.egg-info/PKG-INFO` & `ddsp-3.6.0/ddsp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddsp
-Version: 3.5.1
+Version: 3.6.0
 Summary: Differentiable Digital Signal Processing 
 Home-page: http://github.com/magenta/ddsp
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
 Description: UNKNOWN
 Keywords: audio dsp signalprocessing machinelearning music
```

