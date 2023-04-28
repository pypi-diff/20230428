# Comparing `tmp/returnn-1.20230428.123018.tar.gz` & `tmp/returnn-1.20230428.134452.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230428.123018.tar", last modified: Fri Apr 28 10:43:01 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230428.134452.tar", last modified: Fri Apr 28 11:58:15 2023, max compression
```

## Comparing `returnn-1.20230428.123018.tar` & `returnn-1.20230428.134452.tar`

### file list

```diff
@@ -1,436 +1,436 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 10:42:37.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-28 10:42:41.000000 returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98691 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157144 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36603 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69825 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   589058 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539812 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   293127 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55735 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144924 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:43:01.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-28 10:42:35.000000 returnn-1.20230428.123018/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 11:57:52.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-28 11:57:54.000000 returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99004 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157144 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36603 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69825 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   589058 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539812 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   293127 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55786 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144924 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:58:15.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-28 11:57:51.000000 returnn-1.20230428.134452/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230428.123018/.gitignore` & `returnn-1.20230428.134452/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/.gitmodules` & `returnn-1.20230428.134452/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/CHANGELOG.md` & `returnn-1.20230428.134452/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/CODEOWNERS` & `returnn-1.20230428.134452/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/CONTRIBUTING.md` & `returnn-1.20230428.134452/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/LICENSE` & `returnn-1.20230428.134452/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/MANIFEST.in` & `returnn-1.20230428.134452/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/PKG-INFO` & `returnn-1.20230428.134452/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230428.123018
+Version: 1.20230428.134452
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230428.123018/README.rst` & `returnn-1.20230428.134452/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/__init__.py` & `returnn-1.20230428.134452/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/12AX.cluster_map` & `returnn-1.20230428.134452/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-fwd.config` & `returnn-1.20230428.134452/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-horovod-mpi.py` & `returnn-1.20230428.134452/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230428.134452/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-hyper-param-tuning.config` & `returnn-1.20230428.134452/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-iter-dataset.py` & `returnn-1.20230428.134452/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-list-devices.py` & `returnn-1.20230428.134452/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-lua-torch-layer.config` & `returnn-1.20230428.134452/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230428.134452/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-returnn-as-framework.py` & `returnn-1.20230428.134452/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-rf.config` & `returnn-1.20230428.134452/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-rhn-enwik8.config` & `returnn-1.20230428.134452/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-sprint-interface.py` & `returnn-1.20230428.134452/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-att-copy.config` & `returnn-1.20230428.134452/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-attention.config` & `returnn-1.20230428.134452/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-enc-dec.config` & `returnn-1.20230428.134452/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230428.134452/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230428.134452/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230428.134452/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230428.134452/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230428.134452/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-rec-self-att.config` & `returnn-1.20230428.134452/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230428.134452/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230428.134452/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230428.134452/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-torch.config` & `returnn-1.20230428.134452/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230428.134452/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/demo.sh` & `returnn-1.20230428.134452/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230428.134452/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/README.txt` & `returnn-1.20230428.134452/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/config_demo` & `returnn-1.20230428.134452/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230428.134452/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/config_real` & `returnn-1.20230428.134452/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230428.134452/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/decode.py` & `returnn-1.20230428.134452/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230428.134452/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230428.134452/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230428.134452/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230428.134452/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230428.134452/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230428.134452/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230428.134452/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230428.134452/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/__init__.py` & `returnn-1.20230428.134452/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/__main__.py` & `returnn-1.20230428.134452/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/__old_mod_loader__.py` & `returnn-1.20230428.134452/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/__setup__.py` & `returnn-1.20230428.134452/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/config.py` & `returnn-1.20230428.134452/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/audio.py` & `returnn-1.20230428.134452/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/basic.py` & `returnn-1.20230428.134452/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/bundle_file.py` & `returnn-1.20230428.134452/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/cached.py` & `returnn-1.20230428.134452/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/cached2.py` & `returnn-1.20230428.134452/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/generating.py` & `returnn-1.20230428.134452/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/hdf.py` & `returnn-1.20230428.134452/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/lm.py` & `returnn-1.20230428.134452/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/map.py` & `returnn-1.20230428.134452/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/meta.py` & `returnn-1.20230428.134452/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/multi_proc.py` & `returnn-1.20230428.134452/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/normalization_data.py` & `returnn-1.20230428.134452/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/numpy_dump.py` & `returnn-1.20230428.134452/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/raw_wav.py` & `returnn-1.20230428.134452/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/sprint.py` & `returnn-1.20230428.134452/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/stereo.py` & `returnn-1.20230428.134452/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230428.134452/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/datasets/util/vocabulary.py` & `returnn-1.20230428.134452/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/engine/base.py` & `returnn-1.20230428.134452/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/engine/batch.py` & `returnn-1.20230428.134452/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230428.134452/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/edit.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/select.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/transform.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/extern/graph_editor/util.py` & `returnn-1.20230428.134452/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/__init__.py` & `returnn-1.20230428.134452/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/_backend.py` & `returnn-1.20230428.134452/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/_numpy_backend.py` & `returnn-1.20230428.134452/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/_utils.py` & `returnn-1.20230428.134452/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/array_.py` & `returnn-1.20230428.134452/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/attention.py` & `returnn-1.20230428.134452/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/cond.py` & `returnn-1.20230428.134452/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/const.py` & `returnn-1.20230428.134452/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/container.py` & `returnn-1.20230428.134452/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/conv.py` & `returnn-1.20230428.134452/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/device.py` & `returnn-1.20230428.134452/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/dims.py` & `returnn-1.20230428.134452/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/dropout.py` & `returnn-1.20230428.134452/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/dtype.py` & `returnn-1.20230428.134452/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/encoder/base.py` & `returnn-1.20230428.134452/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/encoder/conformer.py` & `returnn-1.20230428.134452/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/init.py` & `returnn-1.20230428.134452/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/linear.py` & `returnn-1.20230428.134452/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/loop.py` & `returnn-1.20230428.134452/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/loss.py` & `returnn-1.20230428.134452/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/math_.py` & `returnn-1.20230428.134452/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/matmul.py` & `returnn-1.20230428.134452/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/module.py` & `returnn-1.20230428.134452/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/normalization.py` & `returnn-1.20230428.134452/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/parameter.py` & `returnn-1.20230428.134452/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/rand.py` & `returnn-1.20230428.134452/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/rec.py` & `returnn-1.20230428.134452/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/reduce.py` & `returnn-1.20230428.134452/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/run_ctx.py` & `returnn-1.20230428.134452/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/signal.py` & `returnn-1.20230428.134452/returnn/frontend/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,26 @@
         If not given, infer this from in_dim, as (in_dim - 1) * 2.
     :param f_min:
     :param f_max:
     :return:
     """
     if not fft_length:
         fft_length = (in_dim.dimension - 1) * 2
+    f_min = f_min or 0
+    f_max = f_max or sampling_rate / 2.0
     # noinspection PyProtectedMember
     backend = x._raw_backend
-    cache_key = (f_min, f_max, sampling_rate, fft_length, out_dim.dimension, backend, x.device)
+    cache_key = (f_min, f_max, sampling_rate, fft_length, out_dim.dimension, backend, x.dtype, x.device)
     if cache_key in _mel_filter_bank_matrix_cache:
         filter_bank_matrix = _mel_filter_bank_matrix_cache[cache_key]
     else:
         filter_bank_matrix_np = _mel_filter_bank_matrix_np(
             f_min=f_min, f_max=f_max, sampling_rate=sampling_rate, fft_size=fft_length, nr_of_filters=out_dim.dimension
         )
+        filter_bank_matrix_np = filter_bank_matrix_np.astype(x.dtype)
         filter_bank_matrix = rf.convert_to_tensor(filter_bank_matrix_np, dims=(in_dim, out_dim), _backend=backend)
         filter_bank_matrix = rf.copy_to_device(filter_bank_matrix, x.device)
         if backend.executing_eagerly():
             if len(_mel_filter_bank_matrix_cache) > 100:
                 # Very simple cache management. No LRU logic or anything like that.
                 _mel_filter_bank_matrix_cache.clear()
             _mel_filter_bank_matrix_cache[cache_key] = filter_bank_matrix
```

### Comparing `returnn-1.20230428.123018/returnn/frontend/state.py` & `returnn-1.20230428.134452/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/frontend/types.py` & `returnn-1.20230428.134452/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/import_/common.py` & `returnn-1.20230428.134452/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/import_/git.py` & `returnn-1.20230428.134452/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/import_/import_.py` & `returnn-1.20230428.134452/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/learning_rate_control.py` & `returnn-1.20230428.134452/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/log.py` & `returnn-1.20230428.134452/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/native_op.cpp` & `returnn-1.20230428.134452/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/native_op.py` & `returnn-1.20230428.134452/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/pretrain.py` & `returnn-1.20230428.134452/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/sprint/cache.py` & `returnn-1.20230428.134452/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/sprint/control.py` & `returnn-1.20230428.134452/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/sprint/error_signals.py` & `returnn-1.20230428.134452/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/sprint/extern_interface.py` & `returnn-1.20230428.134452/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/sprint/interface.py` & `returnn-1.20230428.134452/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/_dim_extra.py` & `returnn-1.20230428.134452/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -2357,3813 +2357,3832 @@
 00009340: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
 00009350: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
 00009360: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
 00009370: 2020 2020 2020 6261 636b 656e 6420 3d20        backend = 
 00009380: 782e 6479 6e5f 7369 7a65 5f65 7874 2e5f  x.dyn_size_ext._
 00009390: 7261 775f 6261 636b 656e 640a 2020 2020  raw_backend.    
 000093a0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000093b0: 6b0a 0a20 2020 2020 2020 2069 6d70 6f72  k..        impor
-000093c0: 7420 6e75 6d70 790a 2020 2020 2020 2020  t numpy.        
-000093d0: 696d 706f 7274 2072 6574 7572 6e6e 2e66  import returnn.f
-000093e0: 726f 6e74 656e 6420 6173 2072 660a 2020  rontend as rf.  
-000093f0: 2020 2020 2020 6672 6f6d 2072 6574 7572        from retur
-00009400: 6e6e 2e74 656e 736f 7220 696d 706f 7274  nn.tensor import
-00009410: 2054 656e 736f 720a 0a20 2020 2020 2020   Tensor..       
-00009420: 2074 6620 3d20 7466 5f75 7469 6c20 3d20   tf = tf_util = 
-00009430: 7465 6e73 6f72 5f75 7469 6c20 3d20 4e6f  tensor_util = No
-00009440: 6e65 0a20 2020 2020 2020 2069 6620 6261  ne.        if ba
-00009450: 636b 656e 6420 616e 6420 6261 636b 656e  ckend and backen
-00009460: 642e 6973 5f74 656e 736f 7266 6c6f 773a  d.is_tensorflow:
-00009470: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-00009480: 6f72 7420 7465 6e73 6f72 666c 6f77 2061  ort tensorflow a
-00009490: 7320 7466 0a0a 2020 2020 2020 2020 2020  s tf..          
-000094a0: 2020 6966 2062 6163 6b65 6e64 2e52 6177    if backend.Raw
-000094b0: 5465 6e73 6f72 5479 7065 203d 3d20 7466  TensorType == tf
-000094c0: 2e54 656e 736f 723a 0a20 2020 2020 2020  .Tensor:.       
-000094d0: 2020 2020 2020 2020 2066 726f 6d20 7265           from re
-000094e0: 7475 726e 6e2e 7466 2e75 7469 6c20 696d  turnn.tf.util im
-000094f0: 706f 7274 2062 6173 6963 2061 7320 7466  port basic as tf
-00009500: 5f75 7469 6c0a 2020 2020 2020 2020 2020  _util.          
-00009510: 2020 2020 2020 6672 6f6d 2074 656e 736f        from tenso
-00009520: 7266 6c6f 772e 7079 7468 6f6e 2e66 7261  rflow.python.fra
-00009530: 6d65 776f 726b 2069 6d70 6f72 7420 7465  mework import te
-00009540: 6e73 6f72 5f75 7469 6c0a 2020 2020 2020  nsor_util.      
-00009550: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009560: 2020 2020 2020 2020 2020 2020 7466 203d              tf =
-00009570: 204e 6f6e 650a 0a20 2020 2020 2020 206b   None..        k
-00009580: 696e 6420 3d20 6f70 2e6b 696e 640a 2020  ind = op.kind.  
-00009590: 2020 2020 2020 6966 206b 696e 642e 656e        if kind.en
-000095a0: 6473 7769 7468 2822 5f72 6967 6874 2229  dswith("_right")
-000095b0: 3a0a 2020 2020 2020 2020 2020 2020 6b69  :.            ki
-000095c0: 6e64 203d 206b 696e 645b 3a20 2d6c 656e  nd = kind[: -len
-000095d0: 2822 5f72 6967 6874 2229 5d20 2023 206f  ("_right")]  # o
-000095e0: 7264 6572 2064 6f65 7320 6e6f 7420 6d61  rder does not ma
-000095f0: 7474 6572 2068 6572 650a 2020 2020 2020  tter here.      
-00009600: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-00009610: 7468 2822 5f6c 6566 7422 293a 0a20 2020  th("_left"):.   
-00009620: 2020 2020 2020 2020 206b 696e 6420 3d20           kind = 
-00009630: 6b69 6e64 5b3a 202d 6c65 6e28 225f 6c65  kind[: -len("_le
-00009640: 6674 2229 5d0a 0a20 2020 2020 2020 2064  ft")]..        d
-00009650: 6566 205f 6973 5f6e 6567 6174 6976 6528  ef _is_negative(
-00009660: 785f 5f29 3a0a 2020 2020 2020 2020 2020  x__):.          
-00009670: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00009680: 785f 5f2c 206e 756d 7079 2e6e 6461 7272  x__, numpy.ndarr
-00009690: 6179 293a 0a20 2020 2020 2020 2020 2020  ay):.           
-000096a0: 2020 2020 2072 6574 7572 6e20 2878 5f5f       return (x__
-000096b0: 203c 2030 292e 616e 7928 290a 2020 2020   < 0).any().    
-000096c0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000096d0: 7461 6e63 6528 785f 5f2c 2028 696e 742c  tance(x__, (int,
-000096e0: 2066 6c6f 6174 2c20 6e75 6d70 792e 6e75   float, numpy.nu
-000096f0: 6d62 6572 2929 3a0a 2020 2020 2020 2020  mber)):.        
-00009700: 2020 2020 2020 2020 7265 7475 726e 2078          return x
-00009710: 5f5f 203c 2030 0a20 2020 2020 2020 2020  __ < 0.         
-00009720: 2020 2069 6620 6e6f 7420 7466 3a0a 2020     if not tf:.  
-00009730: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009740: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00009750: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
-00009760: 696e 7374 616e 6365 2878 5f5f 2c20 7466  instance(x__, tf
-00009770: 2e54 656e 736f 7229 0a20 2020 2020 2020  .Tensor).       
-00009780: 2020 2020 2078 5f5f 203d 2074 656e 736f       x__ = tenso
-00009790: 725f 7574 696c 2e63 6f6e 7374 616e 745f  r_util.constant_
-000097a0: 7661 6c75 6528 785f 5f29 0a20 2020 2020  value(x__).     
-000097b0: 2020 2020 2020 2069 6620 785f 5f20 6973         if x__ is
-000097c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000097d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000097e0: 6e20 5f69 735f 6e65 6761 7469 7665 2878  n _is_negative(x
-000097f0: 5f5f 290a 2020 2020 2020 2020 2020 2020  __).            
-00009800: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-00009810: 2020 2020 2020 6465 6620 5f62 696e 5f6f        def _bin_o
-00009820: 705f 7466 2861 2c20 6229 3a0a 2020 2020  p_tf(a, b):.    
-00009830: 2020 2020 2020 2020 6966 2074 656d 706c          if templ
-00009840: 6174 655f 6f6e 6c79 3a0a 2020 2020 2020  ate_only:.      
-00009850: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009860: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00009870: 2020 6966 2061 2069 7320 4e6f 6e65 206f    if a is None o
-00009880: 7220 6220 6973 204e 6f6e 653a 0a20 2020  r b is None:.   
-00009890: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000098a0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-000098b0: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-000098c0: 7374 616e 6365 2861 2c20 7466 2e54 656e  stance(a, tf.Ten
-000098d0: 736f 7229 2061 6e64 2069 7369 6e73 7461  sor) and isinsta
-000098e0: 6e63 6528 622c 2028 696e 742c 2074 662e  nce(b, (int, tf.
-000098f0: 5465 6e73 6f72 2929 0a20 2020 2020 2020  Tensor)).       
-00009900: 2020 2020 2077 6974 6820 7466 5f75 7469       with tf_uti
-00009910: 6c2e 7361 6d65 5f63 6f6e 7472 6f6c 5f66  l.same_control_f
-00009920: 6c6f 775f 6374 7828 5b61 2c20 625d 293a  low_ctx([a, b]):
-00009930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009940: 2069 6620 6b69 6e64 203d 3d20 2261 6464   if kind == "add
-00009950: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00009960: 2020 2020 2020 2075 7365 5f72 656c 7520         use_relu 
-00009970: 3d20 5f69 735f 6e65 6761 7469 7665 2861  = _is_negative(a
-00009980: 2920 6f72 205f 6973 5f6e 6567 6174 6976  ) or _is_negativ
-00009990: 6528 6229 2020 2320 666f 7220 6479 6e61  e(b)  # for dyna
-000099a0: 6d69 6320 7465 6e73 6f72 732c 2061 7373  mic tensors, ass
-000099b0: 756d 6520 616c 6c20 706f 7369 7469 7665  ume all positive
-000099c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000099d0: 2020 2020 2069 6620 7573 655f 7265 6c75       if use_relu
-000099e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000099f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009a00: 2074 662e 636f 6e76 6572 745f 746f 5f74   tf.convert_to_t
-00009a10: 656e 736f 7228 7466 5f75 7469 6c2e 7369  ensor(tf_util.si
-00009a20: 6d70 6c69 6679 5f6e 6f6e 5f6e 6567 6174  mplify_non_negat
-00009a30: 6976 655f 7365 715f 6c65 6e67 7468 2861  ive_seq_length(a
-00009a40: 202b 2062 2929 0a20 2020 2020 2020 2020   + b)).         
-00009a50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009a60: 6e20 6120 2b20 620a 2020 2020 2020 2020  n a + b.        
-00009a70: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-00009a80: 6420 3d3d 2022 7375 6222 3a0a 2020 2020  d == "sub":.    
-00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009aa0: 7265 7475 726e 2074 662e 636f 6e76 6572  return tf.conver
-00009ab0: 745f 746f 5f74 656e 736f 7228 7466 5f75  t_to_tensor(tf_u
-00009ac0: 7469 6c2e 7369 6d70 6c69 6679 5f6e 6f6e  til.simplify_non
-00009ad0: 5f6e 6567 6174 6976 655f 7365 715f 6c65  _negative_seq_le
-00009ae0: 6e67 7468 2861 202d 2062 2929 0a20 2020  ngth(a - b)).   
-00009af0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00009b00: 6620 6b69 6e64 203d 3d20 226d 756c 223a  f kind == "mul":
-00009b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b20: 2020 2020 2072 6574 7572 6e20 6120 2a20       return a * 
-00009b30: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-00009b40: 2020 656c 6966 206b 696e 6420 696e 2028    elif kind in (
-00009b50: 2266 6c6f 6f72 6469 7622 2c20 2274 7275  "floordiv", "tru
-00009b60: 6564 6976 2229 3a20 2023 2074 7275 6564  ediv"):  # trued
-00009b70: 6976 2061 7373 756d 6573 2074 6865 7265  iv assumes there
-00009b80: 2069 7320 6e6f 2072 656d 6169 6e64 6572   is no remainder
-00009b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ba0: 2020 2020 2072 6574 7572 6e20 6120 2f2f       return a //
-00009bb0: 2062 0a20 2020 2020 2020 2020 2020 2020   b.             
-00009bc0: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
-00009bd0: 2263 6569 6c64 6976 223a 0a20 2020 2020  "ceildiv":.     
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009bf0: 6574 7572 6e20 2d28 2d61 202f 2f20 6229  eturn -(-a // b)
-00009c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009c20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00009c30: 2056 616c 7565 4572 726f 7228 2275 6e6b   ValueError("unk
-00009c40: 6e6f 776e 206f 7020 6b69 6e64 2025 7222  nown op kind %r"
-00009c50: 2025 206f 702e 6b69 6e64 290a 0a20 2020   % op.kind)..   
-00009c60: 2020 2020 2064 6566 205f 6269 6e5f 6f70       def _bin_op
-00009c70: 2861 2c20 6229 3a0a 2020 2020 2020 2020  (a, b):.        
-00009c80: 2020 2020 6966 2074 656d 706c 6174 655f      if template_
-00009c90: 6f6e 6c79 206f 7220 6e6f 7420 6261 636b  only or not back
-00009ca0: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
-00009cb0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00009cc0: 6365 2861 2c20 5f74 2e54 656e 736f 7229  ce(a, _t.Tensor)
-00009cd0: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
-00009ce0: 622c 205f 742e 5465 6e73 6f72 293a 0a20  b, _t.Tensor):. 
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d00: 2020 2072 6574 7572 6e20 5f74 2e54 656e     return _t.Ten
-00009d10: 736f 722e 6765 745f 636f 6d6d 6f6e 5f64  sor.get_common_d
-00009d20: 6174 6128 5b61 2c20 625d 2c20 616c 6c6f  ata([a, b], allo
-00009d30: 775f 6272 6f61 6463 6173 745f 616c 6c5f  w_broadcast_all_
-00009d40: 736f 7572 6365 733d 5472 7565 290a 2020  sources=True).  
-00009d50: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009d60: 2069 7369 6e73 7461 6e63 6528 612c 205f   isinstance(a, _
-00009d70: 742e 5465 6e73 6f72 293a 0a20 2020 2020  t.Tensor):.     
-00009d80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009d90: 6574 7572 6e20 610a 2020 2020 2020 2020  eturn a.        
-00009da0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00009db0: 7461 6e63 6528 622c 205f 742e 5465 6e73  tance(b, _t.Tens
-00009dc0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00009dd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009de0: 620a 2020 2020 2020 2020 2020 2020 6966  b.            if
-00009df0: 206b 696e 6420 3d3d 2022 6164 6422 3a0a   kind == "add":.
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 7265 7475 726e 2061 202b 2062 0a20 2020  return a + b.   
-00009e20: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
-00009e30: 6e64 203d 3d20 2273 7562 223a 0a20 2020  nd == "sub":.   
-00009e40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009e50: 7572 6e20 6120 2d20 620a 2020 2020 2020  urn a - b.      
-00009e60: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
-00009e70: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00009e80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009e90: 2061 202a 2062 0a20 2020 2020 2020 2020   a * b.         
-00009ea0: 2020 2065 6c69 6620 6b69 6e64 2069 6e20     elif kind in 
-00009eb0: 2822 666c 6f6f 7264 6976 222c 2022 7472  ("floordiv", "tr
-00009ec0: 7565 6469 7622 293a 2020 2320 7472 7565  uediv"):  # true
-00009ed0: 6469 7620 6173 7375 6d65 7320 7468 6572  div assumes ther
-00009ee0: 6520 6973 206e 6f20 7265 6d61 696e 6465  e is no remainde
-00009ef0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00009f00: 2020 7265 7475 726e 2061 202f 2f20 620a    return a // b.
-00009f10: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00009f20: 206b 696e 6420 3d3d 2022 6365 696c 6469   kind == "ceildi
-00009f30: 7622 3a0a 2020 2020 2020 2020 2020 2020  v":.            
-00009f40: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00009f50: 6528 612c 2054 656e 736f 7229 3a0a 2020  e(a, Tensor):.  
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 2020 7265 7475 726e 2072 662e 6365 696c    return rf.ceil
-00009f80: 5f64 6976 6964 6528 612c 2062 290a 2020  _divide(a, b).  
-00009f90: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009fa0: 7475 726e 202d 282d 6120 2f2f 2062 290a  turn -(-a // b).
-00009fb0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00009fc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009fd0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00009fe0: 6f72 2822 756e 6b6e 6f77 6e20 6f70 206b  or("unknown op k
-00009ff0: 696e 6420 2572 2220 2520 6f70 2e6b 696e  ind %r" % op.kin
-0000a000: 6429 0a0a 2020 2020 2020 2020 795f 6e61  d)..        y_na
-0000a010: 6d65 203d 2073 656c 662e 6465 7363 7269  me = self.descri
-0000a020: 7074 696f 6e20 2b20 223a 7365 712d 6c65  ption + ":seq-le
-0000a030: 6e67 7468 220a 2020 2020 2020 2020 793a  ngth".        y:
-0000a040: 204f 7074 696f 6e61 6c5b 5f74 2e54 656e   Optional[_t.Ten
-0000a050: 736f 725d 203d 204e 6f6e 6520 2023 2072  sor] = None  # r
-0000a060: 6573 756c 7469 6e67 2064 796e 2073 697a  esulting dyn siz
-0000a070: 650a 2020 2020 2020 2020 696e 7075 7473  e.        inputs
-0000a080: 203d 206c 6973 7428 6f70 2e69 6e70 7574   = list(op.input
-0000a090: 7329 0a20 2020 2020 2020 2061 7373 6572  s).        asser
-0000a0a0: 7420 696e 7075 7473 0a20 2020 2020 2020  t inputs.       
-0000a0b0: 2077 6869 6c65 2069 6e70 7574 733a 0a20   while inputs:. 
-0000a0c0: 2020 2020 2020 2020 2020 2078 203d 2069             x = i
-0000a0d0: 6e70 7574 732e 706f 7028 3029 0a20 2020  nputs.pop(0).   
-0000a0e0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000a0f0: 782e 6973 5f64 796e 616d 6963 2829 3a20  x.is_dynamic(): 
-0000a100: 2023 2073 7461 7469 630a 2020 2020 2020   # static.      
-0000a110: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000a120: 2078 2e64 696d 656e 7369 6f6e 2069 7320   x.dimension is 
-0000a130: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000a140: 2020 2020 2020 2020 2069 6620 7920 6973           if y is
-0000a150: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000a160: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000a170: 7420 7465 6d70 6c61 7465 5f6f 6e6c 7920  t template_only 
-0000a180: 616e 6420 6261 636b 656e 6420 616e 6420  and backend and 
-0000a190: 6e6f 7420 7466 3a0a 2020 2020 2020 2020  not tf:.        
-0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 7920 3d20 6261 636b 656e 642e 636f 6e76  y = backend.conv
-0000a1c0: 6572 745f 746f 5f74 656e 736f 7228 782e  ert_to_tensor(x.
-0000a1d0: 6469 6d65 6e73 696f 6e2c 2064 696d 733d  dimension, dims=
-0000a1e0: 5b5d 2c20 6474 7970 653d 5f74 2e54 656e  [], dtype=_t.Ten
-0000a1f0: 736f 722e 7369 7a65 5f64 7479 7065 2c20  sor.size_dtype, 
-0000a200: 6e61 6d65 3d79 5f6e 616d 6529 0a20 2020  name=y_name).   
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a220: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0000a240: 203d 205f 742e 5465 6e73 6f72 280a 2020   = _t.Tensor(.  
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2020 2020 2020 2020 2020 6e61 6d65 3d79            name=y
-0000a270: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2064 696d 5f74 6167 733d 5b5d 2c0a     dim_tags=[],.
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-0000a2c0: 653d 5f74 2e54 656e 736f 722e 7369 7a65  e=_t.Tensor.size
-0000a2d0: 5f64 7479 7065 2c0a 2020 2020 2020 2020  _dtype,.        
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a300: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000a310: 2074 656d 706c 6174 655f 6f6e 6c79 2061   template_only a
-0000a320: 6e64 2074 663a 0a20 2020 2020 2020 2020  nd tf:.         
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 2020 2077 6974 6820 7466 2e63 6f6e 7472     with tf.contr
-0000a350: 6f6c 5f64 6570 656e 6465 6e63 6965 7328  ol_dependencies(
-0000a360: 4e6f 6e65 293a 2020 2320 7468 6973 2077  None):  # this w
-0000a370: 696c 6c20 7265 7365 7420 7468 6520 636f  ill reset the co
-0000a380: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
-0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3a0: 2020 2020 2020 792e 7261 775f 7465 6e73        y.raw_tens
-0000a3b0: 6f72 203d 2074 662e 636f 6e73 7461 6e74  or = tf.constant
-0000a3c0: 2878 2e64 696d 656e 7369 6f6e 290a 2020  (x.dimension).  
-0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3e0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-0000a3f0: 2020 2020 2020 2020 2020 2069 6620 7466             if tf
-0000a400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a410: 2020 2020 2020 792e 706c 6163 6568 6f6c        y.placehol
-0000a420: 6465 7220 3d20 5f62 696e 5f6f 705f 7466  der = _bin_op_tf
-0000a430: 2879 2e70 6c61 6365 686f 6c64 6572 2c20  (y.placeholder, 
-0000a440: 782e 6469 6d65 6e73 696f 6e29 0a20 2020  x.dimension).   
-0000a450: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000a460: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000a470: 2020 2020 2020 2079 203d 205f 6269 6e5f         y = _bin_
-0000a480: 6f70 2879 2c20 782e 6469 6d65 6e73 696f  op(y, x.dimensio
-0000a490: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-0000a4a0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000a4b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a4c0: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
-0000a4d0: 2020 2020 2020 2078 203d 2078 2e67 6574         x = x.get
-0000a4e0: 5f66 6f72 5f62 6174 6368 5f63 7478 2873  _for_batch_ctx(s
-0000a4f0: 656c 662e 6261 7463 682c 2073 656c 662e  elf.batch, self.
-0000a500: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-0000a510: 290a 2020 2020 2020 2020 2020 2020 782e  ).            x.
-0000a520: 636f 6d70 6c65 7465 5f64 796e 5f73 697a  complete_dyn_siz
-0000a530: 6528 7465 6d70 6c61 7465 5f6f 6e6c 793d  e(template_only=
-0000a540: 7465 6d70 6c61 7465 5f6f 6e6c 7929 0a20  template_only). 
-0000a550: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000a560: 7420 782e 6479 6e5f 7369 7a65 5f65 7874  t x.dyn_size_ext
-0000a570: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a580: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000a590: 2020 2020 2078 203d 2078 2e64 796e 5f73       x = x.dyn_s
-0000a5a0: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
-0000a5b0: 2020 2020 6966 2079 2069 7320 4e6f 6e65      if y is None
-0000a5c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a5d0: 2020 7920 3d20 782e 636f 7079 286e 616d    y = x.copy(nam
-0000a5e0: 653d 795f 6e61 6d65 290a 2020 2020 2020  e=y_name).      
-0000a5f0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0000a600: 7565 0a20 2020 2020 2020 2020 2020 2069  ue.            i
-0000a610: 6620 782e 6469 6d5f 7461 6773 2021 3d20  f x.dim_tags != 
-0000a620: 792e 6469 6d5f 7461 6773 3a0a 2020 2020  y.dim_tags:.    
-0000a630: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-0000a640: 6f6e 203d 205f 742e 5465 6e73 6f72 2e67  on = _t.Tensor.g
-0000a650: 6574 5f63 6f6d 6d6f 6e5f 6461 7461 285b  et_common_data([
-0000a660: 782c 2079 5d2c 2061 6c6c 6f77 5f62 726f  x, y], allow_bro
-0000a670: 6164 6361 7374 5f61 6c6c 5f73 6f75 7263  adcast_all_sourc
-0000a680: 6573 3d54 7275 6529 0a20 2020 2020 2020  es=True).       
-0000a690: 2020 2020 2020 2020 2078 5f20 3d20 782e           x_ = x.
-0000a6a0: 636f 7079 5f63 6f6d 7061 7469 626c 655f  copy_compatible_
-0000a6b0: 746f 2863 6f6d 6d6f 6e29 2069 6620 782e  to(common) if x.
-0000a6c0: 6469 6d5f 7461 6773 2065 6c73 6520 780a  dim_tags else x.
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6e0: 795f 203d 2079 2e63 6f70 795f 636f 6d70  y_ = y.copy_comp
-0000a6f0: 6174 6962 6c65 5f74 6f28 636f 6d6d 6f6e  atible_to(common
-0000a700: 2920 6966 2079 2e64 696d 5f74 6167 7320  ) if y.dim_tags 
-0000a710: 656c 7365 2079 0a20 2020 2020 2020 2020  else y.         
-0000a720: 2020 2020 2020 2079 203d 2063 6f6d 6d6f         y = commo
-0000a730: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
-0000a740: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a750: 2020 2020 785f 2c20 795f 203d 2078 2c20      x_, y_ = x, 
-0000a760: 790a 2020 2020 2020 2020 2020 2020 6966  y.            if
-0000a770: 2074 663a 0a20 2020 2020 2020 2020 2020   tf:.           
-0000a780: 2020 2020 2079 2e70 6c61 6365 686f 6c64       y.placehold
-0000a790: 6572 203d 205f 6269 6e5f 6f70 5f74 6628  er = _bin_op_tf(
-0000a7a0: 795f 2e70 6c61 6365 686f 6c64 6572 2c20  y_.placeholder, 
-0000a7b0: 785f 2e70 6c61 6365 686f 6c64 6572 290a  x_.placeholder).
-0000a7c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000a7d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a7e0: 2020 7920 3d20 5f62 696e 5f6f 7028 795f    y = _bin_op(y_
-0000a7f0: 2c20 785f 290a 2020 2020 2020 2020 6173  , x_).        as
-0000a800: 7365 7274 2079 2c20 6622 6f70 207b 6f70  sert y, f"op {op
-0000a810: 7d3f 220a 2020 2020 2020 2020 6966 2073  }?".        if s
-0000a820: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-0000a830: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-0000a840: 7365 7274 2073 656c 662e 6479 6e5f 7369  sert self.dyn_si
-0000a850: 7a65 5f65 7874 2e64 696d 5f74 6167 7320  ze_ext.dim_tags 
-0000a860: 3d3d 2079 2e64 696d 5f74 6167 730a 2020  == y.dim_tags.  
-0000a870: 2020 2020 2020 6966 2079 2e62 6174 6368        if y.batch
-0000a880: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000a890: 2073 656c 662e 6261 7463 683a 0a20 2020   self.batch:.   
-0000a8a0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-0000a8b0: 6572 7420 7365 6c66 2e62 6174 6368 203d  ert self.batch =
-0000a8c0: 3d20 792e 6261 7463 680a 2020 2020 2020  = y.batch.      
-0000a8d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000a8e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a8f0: 2e62 6174 6368 203d 2079 2e62 6174 6368  .batch = y.batch
-0000a900: 0a20 2020 2020 2020 2073 656c 662e 6479  .        self.dy
-0000a910: 6e5f 7369 7a65 5f65 7874 203d 2079 0a20  n_size_ext = y. 
-0000a920: 2020 2020 2020 2069 6620 7466 2061 6e64         if tf and
-0000a930: 2079 2e70 6c61 6365 686f 6c64 6572 2069   y.placeholder i
-0000a940: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000a950: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a960: 5f74 6167 5f6f 6e5f 7369 7a65 5f74 656e  _tag_on_size_ten
-0000a970: 736f 7228 792e 706c 6163 6568 6f6c 6465  sor(y.placeholde
-0000a980: 7229 0a0a 2020 2020 6465 6620 6973 5f65  r)..    def is_e
-0000a990: 7175 616c 280a 2020 2020 2020 2020 7365  qual(.        se
-0000a9a0: 6c66 2c0a 2020 2020 2020 2020 6f74 6865  lf,.        othe
-0000a9b0: 722c 0a20 2020 2020 2020 2069 676e 6f72  r,.        ignor
-0000a9c0: 655f 6665 6174 7572 655f 6469 6d3d 4661  e_feature_dim=Fa
-0000a9d0: 6c73 652c 0a20 2020 2020 2020 2061 6c6c  lse,.        all
-0000a9e0: 6f77 5f73 616d 655f 6665 6174 7572 655f  ow_same_feature_
-0000a9f0: 6469 6d3d 4661 6c73 652c 0a20 2020 2020  dim=False,.     
-0000aa00: 2020 2061 6c6c 6f77 5f73 616d 655f 7370     allow_same_sp
-0000aa10: 6174 6961 6c5f 6469 6d3d 4e6f 6e65 2c0a  atial_dim=None,.
-0000aa20: 2020 2020 2020 2020 7472 6561 745f 6665          treat_fe
-0000aa30: 6174 7572 655f 6173 5f73 7061 7469 616c  ature_as_spatial
-0000aa40: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000aa50: 6272 6f61 6463 6173 745f 6d61 7463 6865  broadcast_matche
-0000aa60: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-0000aa70: 2075 6e6b 6e6f 776e 5f73 7061 7469 616c   unknown_spatial
-0000aa80: 5f6d 6174 6368 6573 3d46 616c 7365 2c0a  _matches=False,.
-0000aa90: 2020 2020 2020 2020 756e 6465 6669 6e65          undefine
-0000aaa0: 645f 6d61 7463 6865 733d 4661 6c73 652c  d_matches=False,
-0000aab0: 0a20 2020 2020 2020 2064 6572 6976 6564  .        derived
-0000aac0: 5f6d 6174 6368 6573 3d46 616c 7365 2c0a  _matches=False,.
-0000aad0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0000aae0: 2222 0a20 2020 2020 2020 2043 6f6d 7061  "".        Compa
-0000aaf0: 7265 7320 7365 6c66 2074 6f20 6f74 6865  res self to othe
-0000ab00: 7220 666f 7220 6571 7561 6c69 7479 2e0a  r for equality..
-0000ab10: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-0000ab20: 6174 2074 6865 2064 6566 6175 6c74 2062  at the default b
-0000ab30: 6568 6176 696f 7220 6973 2076 6572 7920  ehavior is very 
-0000ab40: 7265 7374 7269 6374 6976 652e 0a20 2020  restrictive..   
-0000ab50: 2020 2020 2055 7365 2066 756e 6374 696f       Use functio
-0000ab60: 6e73 2073 7563 6820 6173 203a 6675 6e63  ns such as :func
-0000ab70: 3a60 6765 745f 616c 6c5f 6469 6d65 6e73  :`get_all_dimens
-0000ab80: 696f 6e5f 7461 6773 6020 6f72 203a 6675  ion_tags` or :fu
-0000ab90: 6e63 3a60 6765 745f 6578 6973 7469 6e67  nc:`get_existing
-0000aba0: 5f74 6167 5f66 726f 6d5f 636f 6c6c 6563  _tag_from_collec
-0000abb0: 7469 6f6e 600a 2020 2020 2020 2020 746f  tion`.        to
-0000abc0: 2065 7870 6c69 6369 746c 7920 7370 6563   explicitly spec
-0000abd0: 6966 7920 7468 6520 6265 6861 7669 6f72  ify the behavior
-0000abe0: 2066 6f72 2074 6865 2063 6f6d 7061 7269   for the compari
-0000abf0: 736f 6e2e 0a0a 2020 2020 2020 2020 416c  son...        Al
-0000ac00: 736f 206e 6f74 6520 7468 6174 2074 6865  so note that the
-0000ac10: 2064 6566 696e 6974 696f 6e20 6973 2073   definition is s
-0000ac20: 6c69 6768 746c 7920 6164 2d68 6f63 2066  lightly ad-hoc f
-0000ac30: 6f72 2073 6f6d 6520 6361 7365 732c 0a20  or some cases,. 
-0000ac40: 2020 2020 2020 2061 6e64 206d 6967 6874         and might
-0000ac50: 2070 6f74 656e 7469 616c 6c79 2063 6861   potentially cha
-0000ac60: 6e67 6520 696e 2074 6865 2066 7574 7572  nge in the futur
-0000ac70: 652e 0a20 2020 2020 2020 2020 2068 7474  e..          htt
-0000ac80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000ac90: 7277 7468 2d69 362f 7265 7475 726e 6e2f  rwth-i6/returnn/
-0000aca0: 6973 7375 6573 2f36 3334 0a0a 2020 2020  issues/634..    
-0000acb0: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
-0000acc0: 7468 6572 3a0a 2020 2020 2020 2020 3a70  ther:.        :p
-0000acd0: 6172 616d 2062 6f6f 6c20 6967 6e6f 7265  aram bool ignore
-0000ace0: 5f66 6561 7475 7265 5f64 696d 3a0a 2020  _feature_dim:.  
-0000acf0: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
-0000ad00: 6c20 616c 6c6f 775f 7361 6d65 5f66 6561  l allow_same_fea
-0000ad10: 7475 7265 5f64 696d 3a0a 2020 2020 2020  ture_dim:.      
-0000ad20: 2020 3a70 6172 616d 2062 6f6f 6c7c 4e6f    :param bool|No
-0000ad30: 6e65 2061 6c6c 6f77 5f73 616d 655f 7370  ne allow_same_sp
-0000ad40: 6174 6961 6c5f 6469 6d3a 0a20 2020 2020  atial_dim:.     
-0000ad50: 2020 203a 7061 7261 6d20 626f 6f6c 2074     :param bool t
-0000ad60: 7265 6174 5f66 6561 7475 7265 5f61 735f  reat_feature_as_
-0000ad70: 7370 6174 6961 6c3a 0a20 2020 2020 2020  spatial:.       
-0000ad80: 203a 7061 7261 6d20 626f 6f6c 2062 726f   :param bool bro
-0000ad90: 6164 6361 7374 5f6d 6174 6368 6573 3a0a  adcast_matches:.
-0000ada0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-0000adb0: 6f6f 6c20 756e 6b6e 6f77 6e5f 7370 6174  ool unknown_spat
-0000adc0: 6961 6c5f 6d61 7463 6865 733a 0a20 2020  ial_matches:.   
-0000add0: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
-0000ade0: 2075 6e64 6566 696e 6564 5f6d 6174 6368   undefined_match
-0000adf0: 6573 3a0a 2020 2020 2020 2020 3a70 6172  es:.        :par
-0000ae00: 616d 2062 6f6f 6c20 6465 7269 7665 645f  am bool derived_
-0000ae10: 6d61 7463 6865 733a 0a20 2020 2020 2020  matches:.       
-0000ae20: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-0000ae30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ae40: 2020 6672 6f6d 2072 6574 7572 6e6e 2e75    from returnn.u
-0000ae50: 7469 6c20 696d 706f 7274 2042 6568 6176  til import Behav
-0000ae60: 696f 7256 6572 7369 6f6e 0a0a 2020 2020  iorVersion..    
-0000ae70: 2020 2020 6966 2073 656c 6620 6973 206f      if self is o
-0000ae80: 7468 6572 3a20 2023 2066 6972 7374 2073  ther:  # first s
-0000ae90: 6f6d 6520 6661 7374 2070 6174 6820 6368  ome fast path ch
-0000aea0: 6563 6b0a 2020 2020 2020 2020 2020 2020  eck.            
-0000aeb0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000aec0: 2020 2020 6966 2073 656c 662e 7370 6563      if self.spec
-0000aed0: 6961 6c20 6f72 206f 7468 6572 2e73 7065  ial or other.spe
-0000aee0: 6369 616c 3a0a 2020 2020 2020 2020 2020  cial:.          
-0000aef0: 2020 7265 7475 726e 2046 616c 7365 2020    return False  
-0000af00: 2320 6f6e 6c79 2074 7275 6520 6966 2073  # only true if s
-0000af10: 616d 6520 696e 7374 616e 6365 2c20 6368  ame instance, ch
-0000af20: 6563 6b20 6162 6f76 650a 2020 2020 2020  eck above.      
-0000af30: 2020 6966 2061 6c6c 6f77 5f73 616d 655f    if allow_same_
-0000af40: 7370 6174 6961 6c5f 6469 6d20 6973 204e  spatial_dim is N
-0000af50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000af60: 2061 6c6c 6f77 5f73 616d 655f 7370 6174   allow_same_spat
-0000af70: 6961 6c5f 6469 6d20 3d20 616c 6c6f 775f  ial_dim = allow_
-0000af80: 7361 6d65 5f66 6561 7475 7265 5f64 696d  same_feature_dim
-0000af90: 0a20 2020 2020 2020 2073 656c 665f 6261  .        self_ba
-0000afa0: 7365 203d 2073 656c 662e 6765 745f 7361  se = self.get_sa
-0000afb0: 6d65 5f64 6572 6976 6564 5f62 6173 6528  me_derived_base(
-0000afc0: 2920 6966 2064 6572 6976 6564 5f6d 6174  ) if derived_mat
-0000afd0: 6368 6573 2065 6c73 6520 7365 6c66 2e67  ches else self.g
-0000afe0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-0000aff0: 2020 2020 2020 206f 7468 6572 5f62 6173         other_bas
-0000b000: 6520 3d20 6f74 6865 722e 6765 745f 7361  e = other.get_sa
-0000b010: 6d65 5f64 6572 6976 6564 5f62 6173 6528  me_derived_base(
-0000b020: 2920 6966 2064 6572 6976 6564 5f6d 6174  ) if derived_mat
-0000b030: 6368 6573 2065 6c73 6520 6f74 6865 722e  ches else other.
-0000b040: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
-0000b050: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
-0000b060: 6261 7365 2069 7320 6f74 6865 725f 6261  base is other_ba
-0000b070: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000b080: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000b090: 2020 2020 6966 2073 656c 665f 6261 7365      if self_base
-0000b0a0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-0000b0b0: 2061 6e64 206f 7468 6572 5f62 6173 652e   and other_base.
-0000b0c0: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
-0000b0d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b0e0: 7365 6c66 5f62 6173 652e 6465 7269 7665  self_base.derive
-0000b0f0: 645f 6672 6f6d 5f6f 7020 3d3d 206f 7468  d_from_op == oth
-0000b100: 6572 5f62 6173 652e 6465 7269 7665 645f  er_base.derived_
-0000b110: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
-0000b120: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000b130: 5472 7565 0a20 2020 2020 2020 2073 656c  True.        sel
-0000b140: 665f 6b69 6e64 203d 2073 656c 662e 6b69  f_kind = self.ki
-0000b150: 6e64 0a20 2020 2020 2020 206f 7468 6572  nd.        other
-0000b160: 5f6b 696e 6420 3d20 6f74 6865 722e 6b69  _kind = other.ki
-0000b170: 6e64 0a20 2020 2020 2020 2069 6620 7365  nd.        if se
-0000b180: 6c66 5f6b 696e 6420 3d3d 206f 7468 6572  lf_kind == other
-0000b190: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
-0000b1a0: 732e 4665 6174 7572 6520 616e 6420 6967  s.Feature and ig
-0000b1b0: 6e6f 7265 5f66 6561 7475 7265 5f64 696d  nore_feature_dim
-0000b1c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000b1d0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-0000b1e0: 2020 6966 2074 7265 6174 5f66 6561 7475    if treat_featu
-0000b1f0: 7265 5f61 735f 7370 6174 6961 6c3a 0a20  re_as_spatial:. 
-0000b200: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000b210: 6c66 5f6b 696e 6420 3d3d 2044 696d 5479  lf_kind == DimTy
-0000b220: 7065 732e 4665 6174 7572 653a 0a20 2020  pes.Feature:.   
-0000b230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b240: 665f 6b69 6e64 203d 2044 696d 5479 7065  f_kind = DimType
-0000b250: 732e 5370 6174 6961 6c0a 2020 2020 2020  s.Spatial.      
-0000b260: 2020 2020 2020 6966 206f 7468 6572 5f6b        if other_k
-0000b270: 696e 6420 3d3d 2044 696d 5479 7065 732e  ind == DimTypes.
-0000b280: 4665 6174 7572 653a 0a20 2020 2020 2020  Feature:.       
-0000b290: 2020 2020 2020 2020 206f 7468 6572 5f6b           other_k
-0000b2a0: 696e 6420 3d20 4469 6d54 7970 6573 2e53  ind = DimTypes.S
-0000b2b0: 7061 7469 616c 0a20 2020 2020 2020 2069  patial.        i
-0000b2c0: 6620 7365 6c66 2e64 696d 656e 7369 6f6e  f self.dimension
-0000b2d0: 2021 3d20 6f74 6865 722e 6469 6d65 6e73   != other.dimens
-0000b2e0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-0000b2f0: 2069 6620 6272 6f61 6463 6173 745f 6d61   if broadcast_ma
-0000b300: 7463 6865 7320 616e 6420 2873 656c 662e  tches and (self.
-0000b310: 6469 6d65 6e73 696f 6e20 3d3d 2031 206f  dimension == 1 o
-0000b320: 7220 6f74 6865 722e 6469 6d65 6e73 696f  r other.dimensio
-0000b330: 6e20 3d3d 2031 293a 0a20 2020 2020 2020  n == 1):.       
-0000b340: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
-0000b350: 2070 6173 7320 6f6e 0a20 2020 2020 2020   pass on.       
-0000b360: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b370: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b380: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-0000b390: 6966 2073 656c 665f 6b69 6e64 2021 3d20  if self_kind != 
-0000b3a0: 6f74 6865 725f 6b69 6e64 3a0a 2020 2020  other_kind:.    
-0000b3b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0000b3c0: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-0000b3d0: 7365 6c66 5f6b 696e 6420 3d3d 206f 7468  self_kind == oth
-0000b3e0: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
-0000b3f0: 7065 732e 4261 7463 683a 0a20 2020 2020  pes.Batch:.     
-0000b400: 2020 2020 2020 2023 204e 6f74 653a 2054         # Note: T
-0000b410: 6869 7320 6d69 6768 7420 6265 2069 6e63  his might be inc
-0000b420: 6f72 7265 6374 2069 6e20 736f 6d65 2063  orrect in some c
-0000b430: 6173 6573 2c0a 2020 2020 2020 2020 2020  ases,.          
-0000b440: 2020 2320 652e 672e 2066 6f72 2062 6561    # e.g. for bea
-0000b450: 6d20 7365 6172 6368 2077 6865 6e20 7765  m search when we
-0000b460: 2068 6176 6520 7468 6520 6265 616d 2068   have the beam h
-0000b470: 6964 6465 6e20 696e 2074 6865 2062 6174  idden in the bat
-0000b480: 6368 2064 696d 2c0a 2020 2020 2020 2020  ch dim,.        
-0000b490: 2020 2020 2320 6f72 2077 6865 6e20 7765      # or when we
-0000b4a0: 2075 7365 6420 4d65 7267 6544 696d 734c   used MergeDimsL
-0000b4b0: 6179 6572 206f 6e20 7468 6520 6261 7463  ayer on the batc
-0000b4c0: 6820 6178 6973 2c20 6f72 2073 6f2e 0a20  h axis, or so.. 
-0000b4d0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-0000b4e0: 6d69 6768 7420 6e65 6564 2074 6f20 6578  might need to ex
-0000b4f0: 7465 6e64 2074 6865 206c 6f67 6963 2068  tend the logic h
-0000b500: 6572 6520 6c61 7465 722e 0a20 2020 2020  ere later..     
-0000b510: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b520: 7565 0a20 2020 2020 2020 2069 6620 4265  ue.        if Be
-0000b530: 6861 7669 6f72 5665 7273 696f 6e2e 6765  haviorVersion.ge
-0000b540: 7428 2920 3e3d 2031 363a 0a20 2020 2020  t() >= 16:.     
-0000b550: 2020 2020 2020 2023 2045 6974 6865 7220         # Either 
-0000b560: 7365 6c66 206f 7220 6f74 6865 7220 6973  self or other is
-0000b570: 2073 6f6d 6520 6469 6d20 7461 6720 6578   some dim tag ex
-0000b580: 706c 6963 6974 6c79 2063 7265 6174 6564  plicitly created
-0000b590: 2062 7920 7468 6520 7573 6572 2c0a 2020   by the user,.  
-0000b5a0: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
-0000b5b0: 7468 6579 2061 7265 206e 6f74 2074 6865  they are not the
-0000b5c0: 2073 616d 652c 2073 6f20 7765 206e 6576   same, so we nev
-0000b5d0: 6572 2074 7265 6174 2074 6865 6d20 6173  er treat them as
-0000b5e0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
-0000b5f0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0000b600: 6175 746f 5f67 656e 6572 6174 6564 206f  auto_generated o
-0000b610: 7220 6e6f 7420 6f74 6865 722e 6175 746f  r not other.auto
-0000b620: 5f67 656e 6572 6174 6564 3a0a 2020 2020  _generated:.    
-0000b630: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000b640: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000b650: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
-0000b660: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
-0000b670: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
-0000b680: 616e 6420 7365 6c66 2e61 7574 6f5f 6765  and self.auto_ge
-0000b690: 6e65 7261 7465 6429 206f 7220 286f 7468  nerated) or (oth
-0000b6a0: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-0000b6b0: 3120 616e 6420 6f74 6865 722e 6175 746f  1 and other.auto
-0000b6c0: 5f67 656e 6572 6174 6564 290a 2020 2020  _generated).    
-0000b6d0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 2070 6173 7320 2023 2065 7863 6570     pass  # excep
-0000b700: 7469 6f6e 2c20 616c 6c6f 7720 6272 6f61  tion, allow broa
-0000b710: 6463 6173 7420 6c6f 6769 630a 2020 2020  dcast logic.    
-0000b720: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b740: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000b750: 7365 0a20 2020 2020 2020 2069 6620 7365  se.        if se
-0000b760: 6c66 5f6b 696e 6420 3d3d 206f 7468 6572  lf_kind == other
-0000b770: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
-0000b780: 732e 4665 6174 7572 653a 0a20 2020 2020  s.Feature:.     
-0000b790: 2020 2020 2020 2069 6620 616c 6c6f 775f         if allow_
-0000b7a0: 7361 6d65 5f66 6561 7475 7265 5f64 696d  same_feature_dim
-0000b7b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b7c0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000b7d0: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
-0000b7e0: 6e64 203d 3d20 6f74 6865 725f 6b69 6e64  nd == other_kind
-0000b7f0: 203d 3d20 4469 6d54 7970 6573 2e53 7061   == DimTypes.Spa
-0000b800: 7469 616c 3a0a 2020 2020 2020 2020 2020  tial:.          
-0000b810: 2020 6966 2061 6c6c 6f77 5f73 616d 655f    if allow_same_
-0000b820: 7370 6174 6961 6c5f 6469 6d3a 0a20 2020  spatial_dim:.   
-0000b830: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000b840: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-0000b850: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000b880: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000b890: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000b8a0: 2061 6e64 2028 7365 6c66 2e64 696d 656e   and (self.dimen
-0000b8b0: 7369 6f6e 203d 3d20 3120 6f72 206f 7468  sion == 1 or oth
-0000b8c0: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-0000b8d0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-0000b8e0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000b8f0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000b900: 6966 2075 6e6b 6e6f 776e 5f73 7061 7469  if unknown_spati
-0000b910: 616c 5f6d 6174 6368 6573 2061 6e64 2028  al_matches and (
-0000b920: 2873 656c 662e 6479 6e5f 7369 7a65 2069  (self.dyn_size i
-0000b930: 7320 4e6f 6e65 2920 6f72 2028 6f74 6865  s None) or (othe
-0000b940: 722e 6479 6e5f 7369 7a65 2069 7320 4e6f  r.dyn_size is No
-0000b950: 6e65 2929 3a0a 2020 2020 2020 2020 2020  ne)):.          
-0000b960: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000b970: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-0000b980: 2075 6e64 6566 696e 6564 5f6d 6174 6368   undefined_match
-0000b990: 6573 2061 6e64 2028 7365 6c66 2e75 6e64  es and (self.und
-0000b9a0: 6566 696e 6564 206f 7220 6f74 6865 722e  efined or other.
-0000b9b0: 756e 6465 6669 6e65 6429 3a0a 2020 2020  undefined):.    
-0000b9c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b9d0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000b9e0: 2320 496e 2070 7269 6e63 6970 6c65 2c20  # In principle, 
-0000b9f0: 7765 2077 6f75 6c64 2077 616e 7420 746f  we would want to
-0000ba00: 2063 6865 636b 2066 6f72 2069 6465 6e74   check for ident
-0000ba10: 6974 7920 2873 656c 6620 6973 206f 7468  ity (self is oth
-0000ba20: 6572 292e 0a20 2020 2020 2020 2023 2057  er)..        # W
-0000ba30: 6520 6375 7272 656e 746c 7920 7573 6520  e currently use 
-0000ba40: 7468 6520 6465 7363 7269 7074 696f 6e20  the description 
-0000ba50: 6265 6361 7573 6520 7468 6520 6964 656e  because the iden
-0000ba60: 7469 7479 2077 6f75 6c64 206e 6f74 2062  tity would not b
-0000ba70: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
-0000ba80: 2020 2023 2069 6e20 6361 7365 206f 6620     # in case of 
-0000ba90: 7465 6d70 6c61 7465 2063 6f6e 7374 7275  template constru
-0000baa0: 6374 696f 6e20 7768 6572 6520 6120 6469  ction where a di
-0000bab0: 6d20 7461 6720 6973 206f 6e63 6520 6372  m tag is once cr
-0000bac0: 6561 7465 6420 666f 7220 6120 7465 6d70  eated for a temp
-0000bad0: 6c61 7465 206c 6179 6572 2c0a 2020 2020  late layer,.    
-0000bae0: 2020 2020 2320 616e 6420 7468 656e 206c      # and then l
-0000baf0: 6174 6572 2061 6761 696e 2066 6f72 2074  ater again for t
-0000bb00: 6865 2072 6561 6c20 6c61 7965 722e 0a20  he real layer.. 
-0000bb10: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0000bb20: 7574 6f5f 6765 6e65 7261 7465 6420 616e  uto_generated an
-0000bb30: 6420 6f74 6865 722e 6175 746f 5f67 656e  d other.auto_gen
-0000bb40: 6572 6174 6564 2061 6e64 2073 656c 662e  erated and self.
-0000bb50: 6465 7363 7269 7074 696f 6e20 3d3d 206f  description == o
-0000bb60: 7468 6572 2e64 6573 6372 6970 7469 6f6e  ther.description
-0000bb70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000bb80: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-0000bb90: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-0000bba0: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-0000bbb0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-0000bbc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bbd0: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
-0000bbe0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-0000bbf0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-0000bc00: 3a72 6574 7572 6e3a 203a 6675 6e63 3a60  :return: :func:`
-0000bc10: 6973 5f65 7175 616c 6020 7769 7468 2064  is_equal` with d
-0000bc20: 6566 6175 6c74 206f 7074 696f 6e73 0a20  efault options. 
-0000bc30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000bc40: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-0000bc50: 616e 6365 286f 7468 6572 2c20 5f64 2e44  ance(other, _d.D
-0000bc60: 696d 293a 0a20 2020 2020 2020 2020 2020  im):.           
-0000bc70: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0000bc80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000bc90: 662e 6973 5f65 7175 616c 286f 7468 6572  f.is_equal(other
-0000bca0: 290a 0a20 2020 2064 6566 205f 5f6e 655f  )..    def __ne_
-0000bcb0: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
-0000bcc0: 6572 3a20 4469 6d29 3a0a 2020 2020 2020  er: Dim):.      
-0000bcd0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-0000bce0: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
-0000bcf0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-0000bd00: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
-0000bd10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000bd20: 6e6f 7420 2873 656c 6620 3d3d 206f 7468  not (self == oth
-0000bd30: 6572 290a 0a20 2020 2064 6566 205f 5f68  er)..    def __h
-0000bd40: 6173 685f 5f28 7365 6c66 293a 0a20 2020  ash__(self):.   
-0000bd50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bd60: 203a 7274 7970 653a 2069 6e74 0a20 2020   :rtype: int.   
-0000bd70: 2020 2020 203a 7265 7475 726e 3a20 6861       :return: ha
-0000bd80: 7368 2c20 6d61 7463 6869 6e67 2074 6f20  sh, matching to 
-0000bd90: 3a66 756e 633a 605f 5f65 715f 5f60 0a20  :func:`__eq__`. 
-0000bda0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000bdb0: 2020 2023 2054 6869 7320 6d75 7374 206d     # This must m
-0000bdc0: 6174 6368 2074 6865 2062 6568 6176 696f  atch the behavio
-0000bdd0: 7220 696e 205f 5f65 715f 5f2c 2077 6869  r in __eq__, whi
-0000bde0: 6368 2069 7320 6973 5f65 7175 616c 2077  ch is is_equal w
-0000bdf0: 6974 6820 6465 6661 756c 7420 6f70 7469  ith default opti
-0000be00: 6f6e 732e 0a20 2020 2020 2020 2023 2049  ons..        # I
-0000be10: 2e65 2e20 6469 6666 6572 656e 7420 6861  .e. different ha
-0000be20: 7368 2069 6d70 6c69 6573 206e 6f74 2065  sh implies not e
-0000be30: 7175 616c 2028 6275 7420 7361 6d65 2068  qual (but same h
-0000be40: 6173 6820 6e6f 7420 6e65 6365 7373 6172  ash not necessar
-0000be50: 696c 7920 6571 7561 6c29 2e0a 2020 2020  ily equal)..    
-0000be60: 2020 2020 6966 2073 656c 662e 7370 6563      if self.spec
-0000be70: 6961 6c3a 0a20 2020 2020 2020 2020 2020  ial:.           
-0000be80: 2072 6574 7572 6e20 6861 7368 2869 6428   return hash(id(
-0000be90: 7365 6c66 2929 0a20 2020 2020 2020 2069  self)).        i
-0000bea0: 6620 7365 6c66 2e69 735f 6261 7463 685f  f self.is_batch_
-0000beb0: 6469 6d28 293a 0a20 2020 2020 2020 2020  dim():.         
-0000bec0: 2020 2072 6574 7572 6e20 6861 7368 2828     return hash((
-0000bed0: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-0000bee0: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
-0000bef0: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
-0000bf00: 2e44 696d 2e5f 5f68 6173 685f 5f2c 2073  .Dim.__hash__, s
-0000bf10: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-0000bf20: 2020 6261 7365 203d 2073 656c 662e 6765    base = self.ge
-0000bf30: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000bf40: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000bf50: 6520 6973 206e 6f74 2073 656c 663a 0a20  e is not self:. 
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bf70: 6574 7572 6e20 6861 7368 2862 6173 6529  eturn hash(base)
-0000bf80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000bf90: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
-0000bfa0: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000bfb0: 2020 2020 2020 7265 7475 726e 2068 6173        return has
-0000bfc0: 6828 7365 6c66 2e64 6572 6976 6564 5f66  h(self.derived_f
-0000bfd0: 726f 6d5f 6f70 290a 2020 2020 2020 2020  rom_op).        
-0000bfe0: 2020 2020 6966 2073 656c 662e 6175 746f      if self.auto
-0000bff0: 5f67 656e 6572 6174 6564 3a0a 2020 2020  _generated:.    
-0000c000: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c010: 726e 2068 6173 6828 2862 6173 652e 6b69  rn hash((base.ki
-0000c020: 6e64 2c20 6261 7365 2e64 696d 656e 7369  nd, base.dimensi
-0000c030: 6f6e 2c20 6261 7365 2e64 6573 6372 6970  on, base.descrip
-0000c040: 7469 6f6e 2929 0a20 2020 2020 2020 2020  tion)).         
-0000c050: 2020 2072 6574 7572 6e20 6861 7368 2869     return hash(i
-0000c060: 6428 6261 7365 2929 0a0a 2020 2020 6465  d(base))..    de
-0000c070: 6620 5f5f 6c74 5f5f 2873 656c 663a 2044  f __lt__(self: D
-0000c080: 696d 2c20 6f74 6865 723a 2044 696d 293a  im, other: Dim):
-0000c090: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c0a0: 2020 2020 2044 6566 696e 6520 736f 6d65       Define some
-0000c0b0: 206f 7264 6572 2e20 5468 6973 2069 7320   order. This is 
-0000c0c0: 6a75 7374 2073 7563 6820 7468 6174 2060  just such that `
-0000c0d0: 736f 7274 6564 6020 776f 726b 732c 206f  sorted` works, o
-0000c0e0: 7220 736f 6d65 2064 6966 6620 7265 706f  r some diff repo
-0000c0f0: 7274 696e 672c 206f 7220 736f 2e0a 2020  rting, or so..  
-0000c100: 2020 2020 2020 4974 2069 7320 6f6e 2073        It is on s
-0000c110: 796d 626f 6c69 6320 6c65 7665 6c2c 2069  ymbolic level, i
-0000c120: 2e65 2e20 6974 2064 6f65 7320 6e6f 7420  .e. it does not 
-0000c130: 636f 6e73 6964 6572 2074 6865 2061 6374  consider the act
-0000c140: 7561 6c20 6469 6d65 6e73 696f 6e20 7661  ual dimension va
-0000c150: 6c75 652e 0a20 2020 2020 2020 2054 6865  lue..        The
-0000c160: 2064 6566 696e 6564 206f 7264 6572 2073   defined order s
-0000c170: 6f6d 6577 6861 7420 6172 6269 7472 6172  omewhat arbitrar
-0000c180: 792c 2073 6f20 646f 206e 6f74 2072 656c  y, so do not rel
-0000c190: 7920 6f6e 2074 6865 2065 7861 6374 2062  y on the exact b
-0000c1a0: 6568 6176 696f 722c 0a20 2020 2020 2020  ehavior,.       
-0000c1b0: 2061 7320 7468 6973 206d 6967 6874 2063   as this might c
-0000c1c0: 6861 6e67 6520 6174 2073 6f6d 6520 6c61  hange at some la
-0000c1d0: 7465 7220 706f 696e 742e 0a20 2020 2020  ter point..     
-0000c1e0: 2020 2043 7572 7265 6e74 6c79 2c20 6974     Currently, it
-0000c1f0: 2064 6570 656e 6473 206f 6e20 7468 6520   depends on the 
-0000c200: 6372 6561 7469 6f6e 2069 6e64 6578 2e0a  creation index..
-0000c210: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c220: 4469 6d20 6f74 6865 723a 0a20 2020 2020  Dim other:.     
-0000c230: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-0000c240: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c250: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000c260: 7461 6e63 6528 6f74 6865 722c 2028 5f64  tance(other, (_d
-0000c270: 2e44 696d 2c20 5f6d 2e4d 6172 6b65 6444  .Dim, _m.MarkedD
-0000c280: 696d 2929 3a0a 2020 2020 2020 2020 2020  im)):.          
-0000c290: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0000c2a0: 7228 2263 616e 6e6f 7420 636f 6d70 6172  r("cannot compar
-0000c2b0: 6520 2572 2077 6974 6820 2572 2220 2520  e %r with %r" % 
-0000c2c0: 2873 656c 662c 206f 7468 6572 2929 0a20  (self, other)). 
-0000c2d0: 2020 2020 2020 2069 6620 7365 6c66 203d         if self =
-0000c2e0: 3d20 6f74 6865 723a 0a20 2020 2020 2020  = other:.       
-0000c2f0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0000c300: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000c310: 2064 696d 5f63 6d70 5f76 616c 7565 2873   dim_cmp_value(s
-0000c320: 656c 6629 203c 2064 696d 5f63 6d70 5f76  elf) < dim_cmp_v
-0000c330: 616c 7565 286f 7468 6572 290a 0a20 2020  alue(other)..   
-0000c340: 2064 6566 205f 5f67 745f 5f28 7365 6c66   def __gt__(self
-0000c350: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-0000c360: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000c370: 6520 3a66 756e 633a 605f 5f6c 745f 5f60  e :func:`__lt__`
-0000c380: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-0000c390: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
-0000c3a0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-0000c3b0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-0000c3c0: 2020 2020 2020 7265 7475 726e 206f 7468        return oth
-0000c3d0: 6572 203c 2073 656c 660a 0a20 2020 2064  er < self..    d
-0000c3e0: 6566 205f 5f67 655f 5f28 7365 6c66 2c20  ef __ge__(self, 
-0000c3f0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-0000c400: 7265 7475 726e 206e 6f74 2073 656c 6620  return not self 
-0000c410: 3c20 6f74 6865 720a 0a20 2020 2064 6566  < other..    def
-0000c420: 205f 5f6c 655f 5f28 7365 6c66 2c20 6f74   __le__(self, ot
-0000c430: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-0000c440: 7475 726e 206e 6f74 2073 656c 6620 3e20  turn not self > 
-0000c450: 6f74 6865 720a 0a20 2020 2064 6566 2067  other..    def g
-0000c460: 6574 5f73 616d 655f 6261 7365 2873 656c  et_same_base(sel
-0000c470: 663a 205f 642e 4469 6d29 202d 3e20 5f64  f: _d.Dim) -> _d
-0000c480: 2e44 696d 3a0a 2020 2020 2020 2020 2222  .Dim:.        ""
-0000c490: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
-0000c4a0: 6e3a 2073 616d 6520 6261 7365 0a20 2020  n: same base.   
-0000c4b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c4c0: 2069 6620 6e6f 7420 7365 6c66 2e5f 6578   if not self._ex
-0000c4d0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
-0000c4e0: 2072 6574 7572 6e20 7365 6c66 0a20 2020   return self.   
-0000c4f0: 2020 2020 2062 6173 6520 3d20 7365 6c66       base = self
-0000c500: 0a20 2020 2020 2020 2077 6869 6c65 2062  .        while b
-0000c510: 6173 652e 7361 6d65 5f61 733a 0a20 2020  ase.same_as:.   
-0000c520: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000c530: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
-0000c540: 2020 2020 2072 6574 7572 6e20 6261 7365       return base
-0000c550: 0a0a 2020 2020 6465 6620 6765 745f 7361  ..    def get_sa
-0000c560: 6d65 5f64 6572 6976 6564 5f62 6173 6528  me_derived_base(
-0000c570: 7365 6c66 3a20 5f64 2e44 696d 2920 2d3e  self: _d.Dim) ->
-0000c580: 205f 642e 4469 6d3a 0a20 2020 2020 2020   _d.Dim:.       
-0000c590: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
-0000c5a0: 7475 726e 3a20 7361 6d65 2062 6173 652c  turn: same base,
-0000c5b0: 2062 7574 2061 6c73 6f20 636f 6e73 6964   but also consid
-0000c5c0: 6572 2064 6572 6976 6564 5f66 726f 6d5f  er derived_from_
-0000c5d0: 2e2e 2e0a 2020 2020 2020 2020 2222 220a  ....        """.
-0000c5e0: 2020 2020 2020 2020 6261 7365 203d 2073          base = s
-0000c5f0: 656c 660a 2020 2020 2020 2020 7669 7369  elf.        visi
-0000c600: 7465 6420 3d20 7b7d 0a20 2020 2020 2020  ted = {}.       
-0000c610: 2077 6869 6c65 2062 6173 652e 7361 6d65   while base.same
-0000c620: 5f61 7320 6f72 2062 6173 652e 6465 7269  _as or base.deri
-0000c630: 7665 645f 6672 6f6d 5f74 6167 3a0a 2020  ved_from_tag:.  
-0000c640: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000c650: 2069 6428 6261 7365 2920 6e6f 7420 696e   id(base) not in
-0000c660: 2076 6973 6974 6564 2020 2320 7368 6f75   visited  # shou
-0000c670: 6c64 206e 6f74 2068 6176 6520 6379 636c  ld not have cycl
-0000c680: 6573 2e20 6e6f 726d 616c 6c79 2074 6869  es. normally thi
-0000c690: 7320 7368 6f75 6c64 206e 6576 6572 2062  s should never b
-0000c6a0: 6520 7472 6967 6765 7265 640a 2020 2020  e triggered.    
-0000c6b0: 2020 2020 2020 2020 7669 7369 7465 645b          visited[
-0000c6c0: 6964 2862 6173 6529 5d20 3d20 6261 7365  id(base)] = base
-0000c6d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c6e0: 6261 7365 2e73 616d 655f 6173 3a0a 2020  base.same_as:.  
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-0000c700: 7365 203d 2062 6173 652e 7361 6d65 5f61  se = base.same_a
-0000c710: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000c720: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-0000c730: 2020 2020 2020 2062 6173 6520 3d20 6261         base = ba
-0000c740: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000c750: 7461 670a 2020 2020 2020 2020 2020 2020  tag.            
-0000c760: 6173 7365 7274 2062 6173 650a 2020 2020  assert base.    
-0000c770: 2020 2020 7265 7475 726e 2062 6173 650a      return base.
-0000c780: 0a20 2020 2064 6566 2067 6574 5f64 6572  .    def get_der
-0000c790: 6976 6564 5f62 6173 6573 5f73 6574 2873  ived_bases_set(s
-0000c7a0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000c7b0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
-0000c7c0: 3a20 7365 745b 4469 6d5d 0a20 2020 2020  : set[Dim].     
-0000c7d0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000c7e0: 6573 203d 2073 6574 2829 0a20 2020 2020  es = set().     
-0000c7f0: 2020 2071 7565 7565 203d 205b 7365 6c66     queue = [self
-0000c800: 5d0a 2020 2020 2020 2020 7669 7369 7465  ].        visite
-0000c810: 6420 3d20 7b7d 2020 2320 7479 7065 3a20  d = {}  # type: 
-0000c820: 4469 6374 5b69 6e74 2c5f 642e 4469 6d5d  Dict[int,_d.Dim]
-0000c830: 2020 2320 6279 2069 640a 2020 2020 2020    # by id.      
-0000c840: 2020 7768 696c 6520 7175 6575 653a 0a20    while queue:. 
-0000c850: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0000c860: 3d20 7175 6575 652e 706f 7028 2d31 290a  = queue.pop(-1).
-0000c870: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000c880: 6173 652e 7361 6d65 5f61 733a 0a20 2020  ase.same_as:.   
-0000c890: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-0000c8a0: 6520 3d20 6261 7365 2e73 616d 655f 6173  e = base.same_as
-0000c8b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c8c0: 6964 2862 6173 6529 2069 6e20 7669 7369  id(base) in visi
-0000c8d0: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
-0000c8e0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-0000c8f0: 2020 2020 2020 2020 2020 7669 7369 7465            visite
-0000c900: 645b 6964 2862 6173 6529 5d20 3d20 6261  d[id(base)] = ba
-0000c910: 7365 0a20 2020 2020 2020 2020 2020 2072  se.            r
-0000c920: 6573 2e61 6464 2862 6173 6529 0a20 2020  es.add(base).   
-0000c930: 2020 2020 2020 2020 2069 6620 6261 7365           if base
-0000c940: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-0000c950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c960: 2020 7175 6575 652e 6578 7465 6e64 2862    queue.extend(b
-0000c970: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-0000c980: 5f6f 702e 696e 7075 7473 290a 2020 2020  _op.inputs).    
-0000c990: 2020 2020 2020 2020 656c 6966 2062 6173          elif bas
-0000c9a0: 652e 6465 7269 7665 645f 6672 6f6d 5f74  e.derived_from_t
-0000c9b0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
-0000c9c0: 2020 2020 7175 6575 652e 6170 7065 6e64      queue.append
-0000c9d0: 2862 6173 652e 6465 7269 7665 645f 6672  (base.derived_fr
-0000c9e0: 6f6d 5f74 6167 290a 2020 2020 2020 2020  om_tag).        
-0000c9f0: 7265 7475 726e 2072 6573 0a0a 2020 2020  return res..    
-0000ca00: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000ca10: 6620 756e 6465 6669 6e65 6428 7365 6c66  f undefined(self
-0000ca20: 3a20 5f64 2e44 696d 2920 2d3e 2062 6f6f  : _d.Dim) -> boo
-0000ca30: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-0000ca40: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-0000ca50: 7768 6574 6865 7220 7468 6520 756e 6465  whether the unde
-0000ca60: 6669 6e65 6420 666c 6167 2069 7320 7365  fined flag is se
-0000ca70: 742c 2069 6e20 7365 6c66 2c20 6261 7365  t, in self, base
-0000ca80: 732c 206f 7220 616e 7920 6465 7269 7665  s, or any derive
-0000ca90: 6420 6261 7365 732e 2061 6c73 6f20 7365  d bases. also se
-0000caa0: 6520 3a66 756e 633a 6069 735f 6469 6d5f  e :func:`is_dim_
-0000cab0: 6b6e 6f77 6e60 0a20 2020 2020 2020 2022  known`.        "
-0000cac0: 2222 0a20 2020 2020 2020 2062 6173 6520  "".        base 
-0000cad0: 3d20 7365 6c66 0a20 2020 2020 2020 2076  = self.        v
-0000cae0: 6973 6974 6564 203d 207b 7d0a 2020 2020  isited = {}.    
-0000caf0: 2020 2020 7768 696c 6520 6261 7365 2e73      while base.s
-0000cb00: 616d 655f 6173 206f 7220 6261 7365 2e64  ame_as or base.d
-0000cb10: 6572 6976 6564 5f66 726f 6d5f 7461 673a  erived_from_tag:
-0000cb20: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000cb30: 6572 7420 6964 2862 6173 6529 206e 6f74  ert id(base) not
-0000cb40: 2069 6e20 7669 7369 7465 6420 2023 2073   in visited  # s
-0000cb50: 686f 756c 6420 6e6f 7420 6861 7665 2063  hould not have c
-0000cb60: 7963 6c65 732e 206e 6f72 6d61 6c6c 7920  ycles. normally 
-0000cb70: 7468 6973 2073 686f 756c 6420 6e65 7665  this should neve
-0000cb80: 7220 6265 2074 7269 6767 6572 6564 0a20  r be triggered. 
-0000cb90: 2020 2020 2020 2020 2020 2076 6973 6974             visit
-0000cba0: 6564 5b69 6428 6261 7365 295d 203d 2062  ed[id(base)] = b
-0000cbb0: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
-0000cbc0: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-0000cbd0: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-0000cbe0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000cbf0: 6261 7365 2e5f 6578 7472 6120 616e 6420  base._extra and 
-0000cc00: 6261 7365 2e5f 6578 7472 612e 756e 6465  base._extra.unde
-0000cc10: 6669 6e65 643a 0a20 2020 2020 2020 2020  fined:.         
-0000cc20: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000cc30: 7565 0a20 2020 2020 2020 2020 2020 2069  ue.            i
-0000cc40: 6620 6261 7365 2e73 616d 655f 6173 3a0a  f base.same_as:.
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc60: 6261 7365 203d 2062 6173 652e 7361 6d65  base = base.same
-0000cc70: 5f61 730a 2020 2020 2020 2020 2020 2020  _as.            
-0000cc80: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-0000cc90: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000cca0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
-0000ccb0: 6d5f 7461 670a 2020 2020 2020 2020 2020  m_tag.          
-0000ccc0: 2020 6173 7365 7274 2062 6173 650a 2020    assert base.  
-0000ccd0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000cce0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000ccf0: 4d65 6d62 6572 0a20 2020 2020 2020 2072  Member.        r
-0000cd00: 6574 7572 6e20 6261 7365 2e5f 6578 7472  eturn base._extr
-0000cd10: 6120 616e 6420 6261 7365 2e5f 6578 7472  a and base._extr
-0000cd20: 612e 756e 6465 6669 6e65 640a 0a20 2020  a.undefined..   
-0000cd30: 2064 6566 2064 6563 6c61 7265 5f73 616d   def declare_sam
-0000cd40: 655f 6173 2873 656c 663a 205f 642e 4469  e_as(self: _d.Di
-0000cd50: 6d2c 206f 7468 6572 3a20 5f64 2e44 696d  m, other: _d.Dim
-0000cd60: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000cd70: 2020 2020 2020 203a 7061 7261 6d20 6f74         :param ot
-0000cd80: 6865 723a 0a20 2020 2020 2020 2022 2222  her:.        """
-0000cd90: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000cda0: 7365 6c66 2e63 616e 5f62 655f 7573 6564  self.can_be_used
-0000cdb0: 5f61 735f 6469 6d28 2920 616e 6420 6f74  _as_dim() and ot
-0000cdc0: 6865 722e 6361 6e5f 6265 5f75 7365 645f  her.can_be_used_
-0000cdd0: 6173 5f64 696d 2829 2020 2320 6465 636c  as_dim()  # decl
-0000cde0: 6172 655f 7361 6d65 5f61 7320 646f 6573  are_same_as does
-0000cdf0: 206e 6f74 206d 616b 6520 7365 6e73 6520   not make sense 
-0000ce00: 6f74 6865 7277 6973 650a 2020 2020 2020  otherwise.      
-0000ce10: 2020 2320 4e6f 7465 3a20 4368 6563 6b20    # Note: Check 
-0000ce20: 6069 7360 2c20 6e6f 7420 603d 3d60 2e20  `is`, not `==`. 
-0000ce30: 603d 3d60 2063 616e 2062 6520 7472 7565  `==` can be true
-0000ce40: 2065 7665 6e20 7468 6f75 6768 2073 616d   even though sam
-0000ce50: 655f 6173 2061 7265 206e 6f74 2074 6865  e_as are not the
-0000ce60: 2073 616d 6520 696e 7374 616e 6365 2c0a   same instance,.
-0000ce70: 2020 2020 2020 2020 2320 652e 672e 2076          # e.g. v
-0000ce80: 6961 2061 7574 6f5f 6765 6e65 7261 7465  ia auto_generate
-0000ce90: 642e 0a20 2020 2020 2020 2069 6620 7365  d..        if se
-0000cea0: 6c66 2069 7320 6f74 6865 723a 0a20 2020  lf is other:.   
-0000ceb0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000cec0: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
-0000ced0: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
-0000cee0: 2020 2020 2073 656c 662e 5f76 616c 6964       self._valid
-0000cef0: 6174 655f 696e 5f63 7572 7265 6e74 5f67  ate_in_current_g
-0000cf00: 7261 7068 2829 0a20 2020 2020 2020 206f  raph().        o
-0000cf10: 7468 6572 2e5f 7661 6c69 6461 7465 5f69  ther._validate_i
-0000cf20: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
-0000cf30: 290a 2020 2020 2020 2020 6f74 6865 725f  ).        other_
-0000cf40: 7361 6d65 5f62 6173 6520 3d20 6f74 6865  same_base = othe
-0000cf50: 722e 6765 745f 7361 6d65 5f62 6173 6528  r.get_same_base(
-0000cf60: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000cf70: 6620 6973 206f 7468 6572 5f73 616d 655f  f is other_same_
-0000cf80: 6261 7365 206f 7220 7365 6c66 2e73 616d  base or self.sam
-0000cf90: 655f 6173 2069 7320 6f74 6865 725f 7361  e_as is other_sa
-0000cfa0: 6d65 5f62 6173 653a 0a20 2020 2020 2020  me_base:.       
-0000cfb0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000cfc0: 2020 2020 7365 6c66 5f73 616d 655f 6173      self_same_as
-0000cfd0: 203d 2073 656c 662e 6765 745f 7361 6d65   = self.get_same
-0000cfe0: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
-0000cff0: 6966 2073 656c 665f 7361 6d65 5f61 7320  if self_same_as 
-0000d000: 6973 206f 7468 6572 5f73 616d 655f 6261  is other_same_ba
-0000d010: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d020: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000d030: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
-0000d040: 652e 6765 745f 7361 6d65 5f64 6572 6976  e.get_same_deriv
-0000d050: 6564 5f62 6173 6528 2920 6973 2073 656c  ed_base() is sel
-0000d060: 665f 7361 6d65 5f61 733a 0a20 2020 2020  f_same_as:.     
-0000d070: 2020 2020 2020 2023 2057 6520 6163 7475         # We actu
-0000d080: 616c 6c79 2077 616e 7420 6974 2074 6f20  ally want it to 
-0000d090: 6265 2074 6865 206f 7468 6572 2077 6179  be the other way
-0000d0a0: 2061 726f 756e 642e 0a20 2020 2020 2020   around..       
-0000d0b0: 2020 2020 2077 6974 6820 7574 696c 2e67       with util.g
-0000d0c0: 7561 7264 5f69 6e66 696e 6974 655f 7265  uard_infinite_re
-0000d0d0: 6375 7273 696f 6e28 5f64 2e44 696d 2e64  cursion(_d.Dim.d
-0000d0e0: 6563 6c61 7265 5f73 616d 655f 6173 2c20  eclare_same_as, 
-0000d0f0: 6f74 6865 722c 2073 656c 6629 3a0a 2020  other, self):.  
-0000d100: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000d110: 7475 726e 206f 7468 6572 2e64 6563 6c61  turn other.decla
-0000d120: 7265 5f73 616d 655f 6173 2873 656c 6629  re_same_as(self)
-0000d130: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000d140: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
-0000d150: 2020 2020 2320 4966 2073 656c 6620 6973      # If self is
-0000d160: 2064 6566 696e 6564 2028 7365 6c66 2e69   defined (self.i
-0000d170: 735f 6469 6d5f 6b6e 6f77 6e29 2c20 6265  s_dim_known), be
-0000d180: 2066 6169 7220 746f 206f 7468 6572 2c20   fair to other, 
-0000d190: 616e 6420 6164 6170 7420 6974 2074 6f20  and adapt it to 
-0000d1a0: 7468 6520 7269 6768 7420 6261 7463 682c  the right batch,
-0000d1b0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-0000d1c0: 7563 6820 7468 6174 206f 7468 6572 2e69  uch that other.i
-0000d1d0: 735f 6469 6d5f 6b6e 6f77 6e20 6973 2063  s_dim_known is c
-0000d1e0: 6f72 7265 6374 2c20 6279 2070 6f74 656e  orrect, by poten
-0000d1f0: 7469 616c 6c79 2063 6f6d 706c 6574 696e  tially completin
-0000d200: 6720 6974 2e0a 2020 2020 2020 2020 2020  g it..          
-0000d210: 2020 6f74 6865 725f 203d 206f 7468 6572    other_ = other
-0000d220: 2e67 6574 5f66 6f72 5f62 6174 6368 5f63  .get_for_batch_c
-0000d230: 7478 2873 656c 662e 6261 7463 682c 2063  tx(self.batch, c
-0000d240: 7478 3d73 656c 662e 636f 6e74 726f 6c5f  tx=self.control_
-0000d250: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
-0000d260: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000d270: 2020 2020 6f74 6865 725f 203d 206f 7468      other_ = oth
-0000d280: 6572 0a20 2020 2020 2020 2069 6620 280a  er.        if (.
-0000d290: 2020 2020 2020 2020 2020 2020 2873 656c              (sel
-0000d2a0: 662e 6973 5f64 696d 5f6b 6e6f 776e 2829  f.is_dim_known()
-0000d2b0: 2061 6e64 206e 6f74 206f 7468 6572 5f2e   and not other_.
-0000d2c0: 6973 5f64 696d 5f6b 6e6f 776e 2829 290a  is_dim_known()).
-0000d2d0: 2020 2020 2020 2020 2020 2020 6f72 0a20              or. 
-0000d2e0: 2020 2020 2020 2020 2020 2023 204c 696b             # Lik
-0000d2f0: 6520 6973 5f64 696d 5f6b 6e6f 776e 2062  e is_dim_known b
-0000d300: 7574 2066 6f72 2073 7461 7469 6320 6469  ut for static di
-0000d310: 6d73 2c20 7765 206d 6967 6874 206b 6e6f  ms, we might kno
-0000d320: 7720 626f 7468 2c0a 2020 2020 2020 2020  w both,.        
-0000d330: 2020 2020 2320 6275 7420 7468 6520 6465      # but the de
-0000d340: 7269 7665 645f 6672 6f6d 5f6f 7020 7374  rived_from_op st
-0000d350: 696c 6c20 776f 756c 6420 7072 6f76 6964  ill would provid
-0000d360: 6520 6d6f 7265 2069 6e66 6f72 6d61 7469  e more informati
-0000d370: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000d380: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d390: 2020 7365 6c66 5f73 616d 655f 6173 2e64    self_same_as.d
-0000d3a0: 6572 6976 6564 5f66 726f 6d5f 6f70 0a20  erived_from_op. 
-0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000d3c0: 6e64 206e 6f74 206f 7468 6572 5f73 616d  nd not other_sam
-0000d3d0: 655f 6261 7365 2e64 6572 6976 6564 5f66  e_base.derived_f
-0000d3e0: 726f 6d5f 6f70 0a20 2020 2020 2020 2020  rom_op.         
-0000d3f0: 2020 2020 2020 2061 6e64 206f 7468 6572         and other
-0000d400: 206e 6f74 2069 6e20 7365 6c66 2e67 6574   not in self.get
-0000d410: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
-0000d420: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
-0000d430: 2029 0a20 2020 2020 2020 2020 2020 206f   ).            o
-0000d440: 7220 286e 6f74 2073 656c 662e 756e 6465  r (not self.unde
-0000d450: 6669 6e65 6420 616e 6420 6f74 6865 725f  fined and other_
-0000d460: 2e75 6e64 6566 696e 6564 290a 2020 2020  .undefined).    
-0000d470: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-0000d480: 2020 2077 6974 6820 7574 696c 2e67 7561     with util.gua
-0000d490: 7264 5f69 6e66 696e 6974 655f 7265 6375  rd_infinite_recu
-0000d4a0: 7273 696f 6e28 5f64 2e44 696d 2e64 6563  rsion(_d.Dim.dec
-0000d4b0: 6c61 7265 5f73 616d 655f 6173 2c20 6f74  lare_same_as, ot
-0000d4c0: 6865 722c 2073 656c 6629 3a0a 2020 2020  her, self):.    
-0000d4d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d4e0: 726e 206f 7468 6572 2e64 6563 6c61 7265  rn other.declare
-0000d4f0: 5f73 616d 655f 6173 2873 656c 6629 0a20  _same_as(self). 
-0000d500: 2020 2020 2020 206f 7468 6572 5f64 6572         other_der
-0000d510: 6976 6564 5f62 6173 6573 203d 206f 7468  ived_bases = oth
-0000d520: 6572 2e67 6574 5f64 6572 6976 6564 5f62  er.get_derived_b
-0000d530: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
-0000d540: 2020 2073 656c 665f 6465 7269 7665 645f     self_derived_
-0000d550: 6261 7365 7320 3d20 7365 6c66 2e67 6574  bases = self.get
-0000d560: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
-0000d570: 6574 2829 0a20 2020 2020 2020 2069 6620  et().        if 
-0000d580: 6f74 6865 725f 6465 7269 7665 645f 6261  other_derived_ba
-0000d590: 7365 7320 213d 2073 656c 665f 6465 7269  ses != self_deri
-0000d5a0: 7665 645f 6261 7365 7320 616e 6420 7365  ved_bases and se
-0000d5b0: 6c66 5f64 6572 6976 6564 5f62 6173 6573  lf_derived_bases
-0000d5c0: 2e69 7373 7562 7365 7428 6f74 6865 725f  .issubset(other_
-0000d5d0: 6465 7269 7665 645f 6261 7365 7329 3a0a  derived_bases):.
-0000d5e0: 2020 2020 2020 2020 2020 2020 2320 4176              # Av
-0000d5f0: 6f69 6420 6379 636c 6573 206f 6e20 6465  oid cycles on de
-0000d600: 7269 7665 645f 6672 6f6d 5f74 6167 2e20  rived_from_tag. 
-0000d610: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000d620: 6f6d 2f72 7774 682d 6936 2f72 6574 7572  om/rwth-i6/retur
-0000d630: 6e6e 2f69 7373 7565 732f 3130 3534 0a20  nn/issues/1054. 
-0000d640: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000d650: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
-0000d660: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
-0000d670: 2e44 696d 2e64 6563 6c61 7265 5f73 616d  .Dim.declare_sam
-0000d680: 655f 6173 2c20 6f74 6865 722c 2073 656c  e_as, other, sel
-0000d690: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-0000d6a0: 2020 2020 7265 7475 726e 206f 7468 6572      return other
-0000d6b0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
-0000d6c0: 2873 656c 6629 0a20 2020 2020 2020 2069  (self).        i
-0000d6d0: 6620 7365 6c66 2e5f 6578 7472 613a 0a20  f self._extra:. 
-0000d6e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d6f0: 5f65 7874 7261 2e64 6572 6976 6564 5f66  _extra.derived_f
-0000d700: 726f 6d5f 6f70 203d 204e 6f6e 650a 2020  rom_op = None.  
-0000d710: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000d720: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
-0000d730: 6f6d 5f74 6167 203d 204e 6f6e 650a 2020  om_tag = None.  
-0000d740: 2020 2020 2020 6966 2073 656c 665f 7361        if self_sa
-0000d750: 6d65 5f61 7320 6973 206e 6f74 2073 656c  me_as is not sel
-0000d760: 663a 0a20 2020 2020 2020 2020 2020 2061  f:.            a
-0000d770: 7373 6572 7420 6e6f 7420 7365 6c66 5f73  ssert not self_s
-0000d780: 616d 655f 6173 2e73 616d 655f 6173 0a20  ame_as.same_as. 
-0000d790: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000d7a0: 6c66 5f73 616d 655f 6173 2069 7320 6f74  lf_same_as is ot
-0000d7b0: 6865 725f 7361 6d65 5f62 6173 653a 0a20  her_same_base:. 
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d7d0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000d7e0: 2020 7769 7468 2075 7469 6c2e 6775 6172    with util.guar
-0000d7f0: 645f 696e 6669 6e69 7465 5f72 6563 7572  d_infinite_recur
-0000d800: 7369 6f6e 285f 642e 4469 6d2e 6465 636c  sion(_d.Dim.decl
-0000d810: 6172 655f 7361 6d65 5f61 732c 2073 656c  are_same_as, sel
-0000d820: 665f 7361 6d65 5f61 732c 206f 7468 6572  f_same_as, other
-0000d830: 5f73 616d 655f 6261 7365 293a 0a20 2020  _same_base):.   
-0000d840: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d850: 665f 7361 6d65 5f61 732e 6465 636c 6172  f_same_as.declar
-0000d860: 655f 7361 6d65 5f61 7328 6f74 6865 725f  e_same_as(other_
-0000d870: 7361 6d65 5f62 6173 6529 0a20 2020 2020  same_base).     
-0000d880: 2020 2020 2020 2069 6620 2873 656c 662e         if (self.
-0000d890: 6479 6e5f 7369 7a65 5f65 7874 2069 7320  dyn_size_ext is 
-0000d8a0: 4e6f 6e65 206f 7220 6e6f 7420 7365 6c66  None or not self
-0000d8b0: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
-0000d8c0: 7272 656e 745f 6772 6170 6828 2929 2061  rrent_graph()) a
-0000d8d0: 6e64 2073 656c 665f 7361 6d65 5f61 732e  nd self_same_as.
-0000d8e0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-0000d8f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d900: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
-0000d910: 3d20 7365 6c66 5f73 616d 655f 6173 2e67  = self_same_as.g
-0000d920: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
-0000d930: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
-0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d950: 2020 2073 656c 662e 6261 7463 682c 2073     self.batch, s
-0000d960: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000d970: 5f63 7478 2c20 7465 6d70 6c61 7465 5f6f  _ctx, template_o
-0000d980: 6e6c 793d 5472 7565 0a20 2020 2020 2020  nly=True.       
-0000d990: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000d9a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000d9b0: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
-0000d9c0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
-0000d9d0: 2020 2020 2066 6f72 2064 696d 5f20 696e       for dim_ in
-0000d9e0: 2073 656c 662e 5f65 7874 7261 2e73 616d   self._extra.sam
-0000d9f0: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
-0000da00: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
-0000da10: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000da20: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-0000da30: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2069 6620 6469 6d5f 2e5f 6578 7472     if dim_._extr
-0000da60: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-0000da70: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
-0000da80: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-0000da90: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dab0: 2020 2020 6469 6d5f 2e5f 6578 7472 612e      dim_._extra.
-0000dac0: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000dad0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000daf0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-0000db00: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db20: 2020 2020 2020 2020 6469 6d5f 2e5f 6578          dim_._ex
-0000db30: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
-0000db40: 5f74 6167 203d 204e 6f6e 650a 2020 2020  _tag = None.    
-0000db50: 2020 2020 2320 4e6f 7720 6d65 7267 6520      # Now merge 
-0000db60: 6578 6973 7469 6e67 2076 6172 6961 6e74  existing variant
-0000db70: 732e 2042 7574 206f 6e6c 7920 6966 206e  s. But only if n
-0000db80: 6f74 2064 6572 6976 6564 2076 6961 206f  ot derived via o
-0000db90: 702c 2062 6563 6175 7365 2069 6e20 7468  p, because in th
-0000dba0: 6174 2063 6173 652c 2077 6520 6361 6e20  at case, we can 
-0000dbb0: 2861 6e64 2073 686f 756c 6421 290a 2020  (and should!).  
-0000dbc0: 2020 2020 2020 2320 6175 746f 6d61 7469        # automati
-0000dbd0: 6361 6c6c 7920 696e 6665 7220 6974 2e20  cally infer it. 
-0000dbe0: 4e6f 7465 2074 6861 7420 7765 206f 6e6c  Note that we onl
-0000dbf0: 7920 676f 7420 6865 7265 2077 6865 6e20  y got here when 
-0000dc00: 7468 6520 6f74 6865 7220 6973 206e 6f74  the other is not
-0000dc10: 2074 6865 2073 616d 6520 6469 6d2c 2073   the same dim, s
-0000dc20: 6f20 6974 206d 6561 6e73 2074 6861 740a  o it means that.
-0000dc30: 2020 2020 2020 2020 2320 7468 6520 6f74          # the ot
-0000dc40: 6865 7220 6973 2072 6561 6c6c 7920 6469  her is really di
-0000dc50: 6666 6572 656e 742c 2074 6865 2073 697a  fferent, the siz
-0000dc60: 6573 2061 7265 2070 6f74 656e 7469 616c  es are potential
-0000dc70: 6c79 2064 6966 6665 7265 6e74 2c20 6275  ly different, bu
-0000dc80: 7420 7765 2077 616e 7420 746f 206f 7665  t we want to ove
-0000dc90: 7274 616b 6520 7468 6520 6f74 6865 722e  rtake the other.
-0000dca0: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-0000dcb0: 725f 7361 6d65 5f62 6173 652e 6465 7269  r_same_base.deri
-0000dcc0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
-0000dcd0: 2020 2020 2020 2020 2023 2043 6c65 616e           # Clean
-0000dce0: 7570 2065 7665 7279 7468 696e 672c 2065  up everything, e
-0000dcf0: 7370 2070 6f74 656e 7469 616c 2061 6c72  sp potential alr
-0000dd00: 6561 6479 2063 6f6d 7075 7465 6420 7369  eady computed si
-0000dd10: 7a65 732c 2061 7320 7468 6573 6520 6d69  zes, as these mi
-0000dd20: 6768 7420 6265 2069 6e76 616c 6964 2e0a  ght be invalid..
-0000dd30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000dd40: 6469 6d5f 2069 6e20 5b73 656c 665f 7361  dim_ in [self_sa
-0000dd50: 6d65 5f61 732c 2073 656c 665d 202b 2028  me_as, self] + (
-0000dd60: 6c69 7374 2873 656c 662e 5f65 7874 7261  list(self._extra
-0000dd70: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-0000dd80: 6374 782e 7661 6c75 6573 2829 2920 6966  ctx.values()) if
-0000dd90: 2073 656c 662e 5f65 7874 7261 2065 6c73   self._extra els
-0000dda0: 6520 5b5d 293a 0a20 2020 2020 2020 2020  e []):.         
-0000ddb0: 2020 2020 2020 2069 6620 6469 6d5f 2e64         if dim_.d
-0000ddc0: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
-0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dde0: 2064 696d 5f2e 6479 6e5f 7369 7a65 5f65   dim_.dyn_size_e
-0000ddf0: 7874 2e70 6c61 6365 686f 6c64 6572 203d  xt.placeholder =
-0000de00: 204e 6f6e 650a 2020 2020 2020 2020 6f74   None.        ot
-0000de10: 6865 725f 7361 6d65 5f62 6173 652e 5f6d  her_same_base._m
-0000de20: 6572 6765 5f73 616d 655f 666f 725f 6261  erge_same_for_ba
-0000de30: 7463 685f 6374 785f 6469 6374 2873 656c  tch_ctx_dict(sel
-0000de40: 6629 0a20 2020 2020 2020 206f 7468 6572  f).        other
-0000de50: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
-0000de60: 0a20 2020 2020 2020 2073 656c 662e 7361  .        self.sa
-0000de70: 6d65 5f61 7320 3d20 6f74 6865 725f 7361  me_as = other_sa
-0000de80: 6d65 5f62 6173 650a 2020 2020 2020 2020  me_base.        
-0000de90: 7365 6c66 2e5f 6d61 7962 655f 7570 6461  self._maybe_upda
-0000dea0: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
-0000deb0: 7365 6c66 2e64 796e 5f73 697a 6520 6973  self.dyn_size is
-0000dec0: 206e 6f74 204e 6f6e 6520 616e 6420 6f74   not None and ot
-0000ded0: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
-0000dee0: 6e5f 7369 7a65 2069 7320 6e6f 7420 4e6f  n_size is not No
-0000def0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000df00: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-0000df10: 2069 7320 6e6f 7420 6f74 6865 725f 7361   is not other_sa
-0000df20: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
-0000df30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000df40: 2020 6966 2073 656c 662e 6261 7463 6820    if self.batch 
-0000df50: 3d3d 206f 7468 6572 5f73 616d 655f 6261  == other_same_ba
-0000df60: 7365 2e62 6174 6368 2061 6e64 2073 656c  se.batch and sel
-0000df70: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-0000df80: 7478 203d 3d20 6f74 6865 725f 7361 6d65  tx == other_same
-0000df90: 5f62 6173 652e 636f 6e74 726f 6c5f 666c  _base.control_fl
-0000dfa0: 6f77 5f63 7478 3a0a 2020 2020 2020 2020  ow_ctx:.        
-0000dfb0: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
-0000dfc0: 7465 3a20 496e 7374 6561 6420 6f66 206d  te: Instead of m
-0000dfd0: 616b 696e 6720 7468 6973 2061 2077 6172  aking this a war
-0000dfe0: 6e69 6e67 2c20 7765 2063 6f75 6c64 2061  ning, we could a
-0000dff0: 6c73 6f20 656e 666f 7263 6520 7468 6973  lso enforce this
-0000e000: 2061 7420 736f 6d65 2070 6f69 6e74 2e0a   at some point..
-0000e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e020: 2020 2020 2320 2020 5468 6520 7573 6572      #   The user
-0000e030: 2073 686f 756c 6420 6265 2061 626c 6520   should be able 
-0000e040: 746f 2066 6978 2060 6578 7465 726e 5f64  to fix `extern_d
-0000e050: 6174 6160 2069 6e20 7468 6520 636f 6e66  ata` in the conf
-0000e060: 6967 0a20 2020 2020 2020 2020 2020 2020  ig.             
-0000e070: 2020 2020 2020 2023 2020 2073 7563 6820         #   such 
-0000e080: 7468 6174 2074 6869 7320 6973 2063 6f72  that this is cor
-0000e090: 7265 6374 2069 6e20 7468 6520 6669 7273  rect in the firs
-0000e0a0: 7420 706c 6163 652e 0a20 2020 2020 2020  t place..       
-0000e0b0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-0000e0c0: 2041 6c73 6f2c 2069 6e20 6164 6469 7469   Also, in additi
-0000e0d0: 6f6e 2074 6f20 7468 6973 2077 6172 6e69  on to this warni
-0000e0e0: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-0000e0f0: 2020 2020 2020 2020 2320 2020 7765 206d          #   we m
-0000e100: 6967 6874 2077 616e 7420 746f 2061 6464  ight want to add
-0000e110: 2073 6f6d 6520 7275 6e74 696d 6520 6368   some runtime ch
-0000e120: 6563 6b20 6f6e 2074 6865 2065 7120 6f66  eck on the eq of
-0000e130: 2074 6865 2064 796e 2073 697a 6573 2e0a   the dyn sizes..
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 2020 2022 5761 726e 696e 673a 2061 7373     "Warning: ass
-0000e180: 756d 696e 6720 6469 6d20 7461 6773 2061  uming dim tags a
-0000e190: 7265 2073 616d 6520 7769 7468 2064 6966  re same with dif
-0000e1a0: 6665 7265 6e74 2073 697a 6520 706c 6163  ferent size plac
-0000e1b0: 6568 6f6c 6465 7273 3a20 2572 2076 7320  eholders: %r vs 
-0000e1c0: 2572 220a 2020 2020 2020 2020 2020 2020  %r".            
-0000e1d0: 2020 2020 2020 2020 2020 2020 2520 2873              % (s
-0000e1e0: 656c 662e 6479 6e5f 7369 7a65 2c20 6f74  elf.dyn_size, ot
-0000e1f0: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
-0000e200: 6e5f 7369 7a65 290a 2020 2020 2020 2020  n_size).        
-0000e210: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000e220: 2020 2020 2020 2320 4966 2077 6520 6861        # If we ha
-0000e230: 7665 2061 2064 6566 696e 6564 2073 6f75  ve a defined sou
-0000e240: 7263 652c 2061 6e64 2074 6869 7320 6973  rce, and this is
-0000e250: 2061 2064 796e 616d 6963 2073 7061 7469   a dynamic spati
-0000e260: 616c 2061 7869 732c 2061 6e64 2069 7420  al axis, and it 
-0000e270: 7761 7320 756e 6465 6669 6e65 6420 6265  was undefined be
-0000e280: 666f 7265 2c0a 2020 2020 2020 2020 2320  fore,.        # 
-0000e290: 6d61 7962 6520 7765 2063 616e 206f 7665  maybe we can ove
-0000e2a0: 7274 616b 6520 7468 6520 7369 7a65 5f70  rtake the size_p
-0000e2b0: 6c61 6365 686f 6c64 6572 206e 6f77 2e0a  laceholder now..
-0000e2c0: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-0000e2d0: 5f73 616d 655f 6261 7365 2e64 796e 5f73  _same_base.dyn_s
-0000e2e0: 697a 6520 6973 206e 6f74 204e 6f6e 6520  ize is not None 
-0000e2f0: 616e 6420 7365 6c66 2e5f 6578 7472 6120  and self._extra 
-0000e300: 616e 6420 7365 6c66 2e5f 6578 7472 612e  and self._extra.
-0000e310: 7372 635f 6461 7461 3a0a 2020 2020 2020  src_data:.      
-0000e320: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-0000e330: 6e73 7461 6e63 6528 7365 6c66 2e5f 6578  nstance(self._ex
-0000e340: 7472 612e 7372 635f 6178 6973 2c20 696e  tra.src_axis, in
-0000e350: 7429 0a20 2020 2020 2020 2020 2020 2023  t).            #
-0000e360: 204d 6179 6265 2069 7420 6368 616e 6765   Maybe it change
-0000e370: 6420 696e 2074 6865 206d 6561 6e77 6869  d in the meanwhi
-0000e380: 6c65 2c20 736f 2063 6865 636b 2e0a 2020  le, so check..  
-0000e390: 2020 2020 2020 2020 2020 7461 6720 3d20            tag = 
-0000e3a0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
-0000e3b0: 6461 7461 2e67 6574 5f64 696d 5f74 6167  data.get_dim_tag
-0000e3c0: 2873 656c 662e 5f65 7874 7261 2e73 7263  (self._extra.src
-0000e3d0: 5f61 7869 7329 0a20 2020 2020 2020 2020  _axis).         
-0000e3e0: 2020 2069 6620 7461 672e 6465 7363 7269     if tag.descri
-0000e3f0: 7074 696f 6e20 3d3d 2073 656c 662e 6465  ption == self.de
-0000e400: 7363 7269 7074 696f 6e20 616e 6420 286e  scription and (n
-0000e410: 6f74 2074 6167 2e64 796e 5f73 697a 655f  ot tag.dyn_size_
-0000e420: 6578 7420 6f72 206e 6f74 2074 6167 2e5f  ext or not tag._
-0000e430: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000e440: 656e 745f 6772 6170 6828 2929 3a0a 2020  ent_graph()):.  
-0000e450: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000e460: 672e 6479 6e5f 7369 7a65 5f65 7874 203d  g.dyn_size_ext =
-0000e470: 2073 656c 662e 6765 745f 6479 6e5f 7369   self.get_dyn_si
-0000e480: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000e490: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000e4a0: 2020 2020 2020 2020 2020 7461 672e 6261            tag.ba
-0000e4b0: 7463 682c 2074 6167 2e63 6f6e 7472 6f6c  tch, tag.control
-0000e4c0: 5f66 6c6f 775f 6374 782c 2074 656d 706c  _flow_ctx, templ
-0000e4d0: 6174 655f 6f6e 6c79 3d54 7275 650a 2020  ate_only=True.  
-0000e4e0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e500: 7461 672e 5f6d 6179 6265 5f75 7064 6174  tag._maybe_updat
-0000e510: 6528 290a 2020 2020 2020 2020 2320 4966  e().        # If
-0000e520: 206f 7468 6572 7320 6479 6e5f 7369 7a65   others dyn_size
-0000e530: 2069 7320 4e6f 6e65 2062 7574 2077 6520   is None but we 
-0000e540: 6861 7665 2061 2064 796e 5f73 697a 652c  have a dyn_size,
-0000e550: 206d 6179 6265 2075 7064 6174 6520 6f74   maybe update ot
-0000e560: 6865 7273 2064 796e 5f73 697a 652e 0a20  hers dyn_size.. 
-0000e570: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0000e580: 796e 5f73 697a 6520 6973 206e 6f74 204e  yn_size is not N
-0000e590: 6f6e 6520 616e 6420 6f74 6865 725f 7361  one and other_sa
-0000e5a0: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
-0000e5b0: 2069 7320 6e6f 7420 7365 6c66 2e64 796e   is not self.dyn
-0000e5c0: 5f73 697a 653a 0a20 2020 2020 2020 2020  _size:.         
-0000e5d0: 2020 2023 2043 6f75 6c64 2062 6520 756e     # Could be un
-0000e5e0: 7365 7420 6966 2069 7420 636f 6d65 7320  set if it comes 
-0000e5f0: 6672 6f6d 2074 6865 2063 6f6e 6669 672c  from the config,
-0000e600: 206f 7220 6672 6f6d 2070 7265 7620 6772   or from prev gr
-0000e610: 6170 6820 6372 6561 7469 6f6e 2e0a 2020  aph creation..  
-0000e620: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-0000e630: 2069 7320 696d 706f 7274 616e 7420 7375   is important su
-0000e640: 6368 2074 6861 7420 7365 6c66 2e63 616e  ch that self.can
-0000e650: 5f63 6f6d 7061 7265 2829 2069 7320 7361  _compare() is sa
-0000e660: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
-0000e670: 6966 206f 7468 6572 5f73 616d 655f 6261  if other_same_ba
-0000e680: 7365 2e64 796e 5f73 697a 6520 6973 204e  se.dyn_size is N
-0000e690: 6f6e 6520 6f72 206e 6f74 206f 7468 6572  one or not other
-0000e6a0: 5f73 616d 655f 6261 7365 2e5f 7661 6c69  _same_base._vali
-0000e6b0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000e6c0: 6772 6170 6828 293a 0a20 2020 2020 2020  graph():.       
-0000e6d0: 2020 2020 2020 2020 206f 7468 6572 5f73           other_s
-0000e6e0: 616d 655f 6261 7365 2e64 796e 5f73 697a  ame_base.dyn_siz
-0000e6f0: 655f 6578 7420 3d20 7365 6c66 2e67 6574  e_ext = self.get
-0000e700: 5f64 796e 5f73 697a 655f 6578 745f 666f  _dyn_size_ext_fo
-0000e710: 725f 6261 7463 685f 6374 7828 0a20 2020  r_batch_ctx(.   
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e730: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000e740: 2e62 6174 6368 2c20 6f74 6865 725f 7361  .batch, other_sa
-0000e750: 6d65 5f62 6173 652e 636f 6e74 726f 6c5f  me_base.control_
-0000e760: 666c 6f77 5f63 7478 2c20 7465 6d70 6c61  flow_ctx, templa
-0000e770: 7465 5f6f 6e6c 793d 5472 7565 0a20 2020  te_only=True.   
-0000e780: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000e790: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000e7a0: 7468 6572 5f73 616d 655f 6261 7365 2e5f  ther_same_base._
-0000e7b0: 6d61 7962 655f 7570 6461 7465 2829 0a20  maybe_update(). 
-0000e7c0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000e7d0: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
-0000e7e0: 6f72 206e 6f74 2073 656c 662e 5f76 616c  or not self._val
-0000e7f0: 6964 6174 655f 696e 5f63 7572 7265 6e74  idate_in_current
-0000e800: 5f67 7261 7068 2829 3a0a 2020 2020 2020  _graph():.      
-0000e810: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-0000e820: 697a 655f 6578 7420 3d20 6f74 6865 725f  ize_ext = other_
-0000e830: 7361 6d65 5f62 6173 652e 6765 745f 6479  same_base.get_dy
-0000e840: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
-0000e850: 6174 6368 5f63 7478 280a 2020 2020 2020  atch_ctx(.      
-0000e860: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0000e870: 6174 6368 2c20 7365 6c66 2e63 6f6e 7472  atch, self.contr
-0000e880: 6f6c 5f66 6c6f 775f 6374 782c 2074 656d  ol_flow_ctx, tem
-0000e890: 706c 6174 655f 6f6e 6c79 3d54 7275 650a  plate_only=True.
-0000e8a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000e8b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e8c0: 6d61 7962 655f 7570 6461 7465 2829 0a20  maybe_update(). 
-0000e8d0: 2020 2020 2020 2065 6c69 6620 6f74 6865         elif othe
-0000e8e0: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
-0000e8f0: 7369 7a65 5f65 7874 2069 7320 4e6f 6e65  size_ext is None
-0000e900: 206f 7220 6e6f 7420 6f74 6865 725f 7361   or not other_sa
-0000e910: 6d65 5f62 6173 652e 5f76 616c 6964 6174  me_base._validat
-0000e920: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000e930: 7068 2829 3a0a 2020 2020 2020 2020 2020  ph():.          
-0000e940: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000e950: 652e 6479 6e5f 7369 7a65 5f65 7874 203d  e.dyn_size_ext =
-0000e960: 2073 656c 662e 6765 745f 6479 6e5f 7369   self.get_dyn_si
-0000e970: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000e980: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000e990: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000e9a0: 5f62 6173 652e 6261 7463 682c 206f 7468  _base.batch, oth
-0000e9b0: 6572 5f73 616d 655f 6261 7365 2e63 6f6e  er_same_base.con
-0000e9c0: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
-0000e9d0: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
-0000e9e0: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
-0000e9f0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-0000ea00: 725f 7361 6d65 5f62 6173 652e 5f6d 6179  r_same_base._may
-0000ea10: 6265 5f75 7064 6174 6528 290a 2020 2020  be_update().    
-0000ea20: 2020 2020 6966 2073 656c 662e 6973 5f64      if self.is_d
-0000ea30: 696d 5f6b 6e6f 776e 2829 2061 6e64 206f  im_known() and o
-0000ea40: 7468 6572 2e69 735f 6469 6d5f 6b6e 6f77  ther.is_dim_know
-0000ea50: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-0000ea60: 2061 7373 6572 7420 7365 6c66 2e64 696d   assert self.dim
-0000ea70: 656e 7369 6f6e 203d 3d20 6f74 6865 722e  ension == other.
-0000ea80: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
-0000ea90: 2020 656c 6966 2073 656c 662e 6973 5f64    elif self.is_d
-0000eaa0: 696d 5f6b 6e6f 776e 2829 2061 6e64 206e  im_known() and n
-0000eab0: 6f74 206f 7468 6572 2e69 735f 6469 6d5f  ot other.is_dim_
-0000eac0: 6b6e 6f77 6e28 293a 0a20 2020 2020 2020  known():.       
-0000ead0: 2020 2020 206f 7468 6572 2e63 6170 6163       other.capac
-0000eae0: 6974 7920 3d20 7365 6c66 2e63 6170 6163  ity = self.capac
-0000eaf0: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
-0000eb00: 6f74 6865 722e 7369 7a65 203d 2073 656c  other.size = sel
-0000eb10: 662e 7369 7a65 0a20 2020 2020 2020 2065  f.size.        e
-0000eb20: 6c69 6620 6e6f 7420 7365 6c66 2e69 735f  lif not self.is_
-0000eb30: 6469 6d5f 6b6e 6f77 6e28 2920 616e 6420  dim_known() and 
-0000eb40: 6f74 6865 722e 6973 5f64 696d 5f6b 6e6f  other.is_dim_kno
-0000eb50: 776e 2829 3a0a 2020 2020 2020 2020 2020  wn():.          
-0000eb60: 2020 7365 6c66 2e63 6170 6163 6974 7920    self.capacity 
-0000eb70: 3d20 6f74 6865 722e 6361 7061 6369 7479  = other.capacity
-0000eb80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000eb90: 662e 7369 7a65 203d 206f 7468 6572 2e73  f.size = other.s
-0000eba0: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
-0000ebb0: 656c 662e 766f 6361 6220 616e 6420 6e6f  elf.vocab and no
-0000ebc0: 7420 6f74 6865 725f 7361 6d65 5f62 6173  t other_same_bas
-0000ebd0: 652e 766f 6361 623a 0a20 2020 2020 2020  e.vocab:.       
-0000ebe0: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
-0000ebf0: 6261 7365 2e76 6f63 6162 203d 2073 656c  base.vocab = sel
-0000ec00: 662e 766f 6361 620a 2020 2020 2020 2020  f.vocab.        
-0000ec10: 656c 6966 206f 7468 6572 5f73 616d 655f  elif other_same_
-0000ec20: 6261 7365 2e76 6f63 6162 2061 6e64 206e  base.vocab and n
-0000ec30: 6f74 2073 656c 662e 766f 6361 623a 0a20  ot self.vocab:. 
-0000ec40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ec50: 766f 6361 6220 3d20 6f74 6865 725f 7361  vocab = other_sa
-0000ec60: 6d65 5f62 6173 652e 766f 6361 620a 2020  me_base.vocab.  
-0000ec70: 2020 2020 2020 7365 6c66 2e5f 6d61 6b65        self._make
-0000ec80: 5f65 7874 7261 2829 0a20 2020 2020 2020  _extra().       
-0000ec90: 2073 656c 665f 7361 6d65 5f61 732e 5f6d   self_same_as._m
-0000eca0: 616b 655f 6578 7472 6128 290a 2020 2020  ake_extra().    
-0000ecb0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-0000ecc0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-0000ecd0: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
-0000ece0: 662e 5f65 7874 7261 2e61 7574 6f5f 6765  f._extra.auto_ge
-0000ecf0: 6e65 7261 7465 6420 3d20 7365 6c66 5f73  nerated = self_s
-0000ed00: 616d 655f 6173 2e5f 6578 7472 612e 6175  ame_as._extra.au
-0000ed10: 746f 5f67 656e 6572 6174 6564 203d 206f  to_generated = o
-0000ed20: 7468 6572 5f73 616d 655f 6261 7365 2e61  ther_same_base.a
-0000ed30: 7574 6f5f 6765 6e65 7261 7465 640a 2020  uto_generated.  
-0000ed40: 2020 2020 2020 2320 5461 6b65 206f 7665        # Take ove
-0000ed50: 7220 6465 7269 7665 645f 6672 6f6d 5f6f  r derived_from_o
-0000ed60: 702e 2048 6f77 6576 6572 2c20 6f6e 6c79  p. However, only
-0000ed70: 2069 6620 7468 6973 2077 6f75 6c64 206e   if this would n
-0000ed80: 6f74 2069 6e74 726f 6475 6365 2063 7963  ot introduce cyc
-0000ed90: 6c65 7321 0a20 2020 2020 2020 2069 6620  les!.        if 
-0000eda0: 6e6f 7420 7365 6c66 5f64 6572 6976 6564  not self_derived
-0000edb0: 5f62 6173 6573 2e69 7373 7570 6572 7365  _bases.issuperse
-0000edc0: 7428 6f74 6865 725f 6465 7269 7665 645f  t(other_derived_
-0000edd0: 6261 7365 7329 3a0a 2020 2020 2020 2020  bases):.        
-0000ede0: 2020 2020 6966 2073 656c 662e 6465 7269      if self.deri
-0000edf0: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-0000ee00: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000ee10: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-0000ee20: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
-0000ee30: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
-0000ee40: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
-0000ee50: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
-0000ee60: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000ee70: 5f62 6173 652e 5f6d 616b 655f 6578 7472  _base._make_extr
-0000ee80: 6128 292e 6465 7269 7665 645f 6672 6f6d  a().derived_from
-0000ee90: 5f6f 7020 3d20 7365 6c66 2e64 6572 6976  _op = self.deriv
-0000eea0: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000eeb0: 2020 2020 2020 2065 6c69 6620 6f74 6865         elif othe
-0000eec0: 725f 7361 6d65 5f62 6173 652e 6465 7269  r_same_base.deri
-0000eed0: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-0000eee0: 6e6f 7420 7365 6c66 2e64 6572 6976 6564  not self.derived
-0000eef0: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-0000ef00: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000ef10: 6d61 6b65 5f65 7874 7261 2829 2e64 6572  make_extra().der
-0000ef20: 6976 6564 5f66 726f 6d5f 6f70 203d 206f  ived_from_op = o
-0000ef30: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
-0000ef40: 6572 6976 6564 5f66 726f 6d5f 6f70 0a20  erived_from_op. 
-0000ef50: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000ef60: 6578 7472 6120 616e 6420 6e6f 7420 6f74  extra and not ot
-0000ef70: 6865 725f 7361 6d65 5f62 6173 652e 6973  her_same_base.is
-0000ef80: 5f64 796e 616d 6963 2829 3a0a 2020 2020  _dynamic():.    
-0000ef90: 2020 2020 2020 2020 2320 5468 6f73 6520          # Those 
-0000efa0: 6d69 6768 7420 6265 2073 6574 2076 6961  might be set via
-0000efb0: 2067 6574 5f62 6174 6368 5f66 6f72 5f63   get_batch_for_c
-0000efc0: 7478 2066 6f72 2061 6e20 756e 6465 6669  tx for an undefi
-0000efd0: 6e65 6420 6469 6d2c 0a20 2020 2020 2020  ned dim,.       
-0000efe0: 2020 2020 2023 2077 6869 6368 206e 6f77       # which now
-0000eff0: 2062 6563 6f6d 6573 2073 7461 7469 6320   becomes static 
-0000f000: 6475 6520 746f 2060 6f74 6865 7260 2e0a  due to `other`..
-0000f010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f020: 2e5f 6578 7472 612e 6261 7463 6820 3d20  ._extra.batch = 
-0000f030: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000f040: 2073 656c 662e 5f65 7874 7261 2e63 6f6e   self._extra.con
-0000f050: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d20  trol_flow_ctx = 
-0000f060: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000f070: 2066 6f72 206b 6579 2c20 6469 6d5f 2069   for key, dim_ i
-0000f080: 6e20 7365 6c66 2e5f 6578 7472 612e 7361  n self._extra.sa
-0000f090: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
-0000f0a0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-0000f0b0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-0000f0c0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-0000f0d0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-0000f0e0: 2020 2020 2020 2020 2020 2064 696d 5f65             dim_e
-0000f0f0: 7874 7261 203d 2064 696d 5f2e 5f65 7874  xtra = dim_._ext
-0000f100: 7261 0a20 2020 2020 2020 2020 2020 2020  ra.             
-0000f110: 2020 2069 6620 6469 6d5f 6578 7472 613a     if dim_extra:
-0000f120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f130: 2020 2020 2064 696d 5f65 7874 7261 2e62       dim_extra.b
-0000f140: 6174 6368 203d 204e 6f6e 650a 2020 2020  atch = None.    
-0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f160: 6469 6d5f 6578 7472 612e 636f 6e74 726f  dim_extra.contro
-0000f170: 6c5f 666c 6f77 5f63 7478 203d 204e 6f6e  l_flow_ctx = Non
-0000f180: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000f190: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
-0000f1a0: 2020 2020 2073 656c 665f 203d 2073 656c       self_ = sel
-0000f1b0: 662e 6765 745f 666f 725f 6261 7463 685f  f.get_for_batch_
-0000f1c0: 6374 7828 6261 7463 683d 7365 6c66 2e62  ctx(batch=self.b
-0000f1d0: 6174 6368 2c20 6374 783d 7365 6c66 2e63  atch, ctx=self.c
-0000f1e0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7829  ontrol_flow_ctx)
-0000f1f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f200: 7365 6c66 5f20 6973 206e 6f74 2073 656c  self_ is not sel
-0000f210: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-0000f220: 2020 2073 656c 662e 636f 6e74 726f 6c5f     self.control_
-0000f230: 666c 6f77 5f63 7478 203d 2073 656c 665f  flow_ctx = self_
-0000f240: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000f250: 7820 2023 206d 6967 6874 2062 6520 6469  x  # might be di
-0000f260: 6666 6572 656e 740a 2020 2020 2020 2020  fferent.        
-0000f270: 2020 2020 2020 2020 7365 6c66 2e64 796e          self.dyn
-0000f280: 5f73 697a 655f 6578 7420 3d20 7365 6c66  _size_ext = self
-0000f290: 5f2e 6479 6e5f 7369 7a65 5f65 7874 2020  _.dyn_size_ext  
-0000f2a0: 2320 6d69 6768 7420 6265 2075 6e73 6574  # might be unset
-0000f2b0: 0a0a 2020 2020 6465 6620 5f6d 6572 6765  ..    def _merge
-0000f2c0: 5f73 616d 655f 666f 725f 6261 7463 685f  _same_for_batch_
-0000f2d0: 6374 785f 6469 6374 2873 656c 663a 205f  ctx_dict(self: _
-0000f2e0: 642e 4469 6d2c 206f 7468 6572 3a20 5f64  d.Dim, other: _d
-0000f2f0: 2e44 696d 293a 0a20 2020 2020 2020 2022  .Dim):.        "
-0000f300: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0000f310: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-0000f320: 2022 2222 0a20 2020 2020 2020 2023 206e   """.        # n
-0000f330: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
-0000f340: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
-0000f350: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000f360: 662e 5f65 7874 7261 2061 6e64 206e 6f74  f._extra and not
-0000f370: 206f 7468 6572 2e5f 6578 7472 613a 0a20   other._extra:. 
-0000f380: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000f390: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
-0000f3a0: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000f3b0: 656e 745f 6772 6170 6828 290a 2020 2020  ent_graph().    
-0000f3c0: 2020 2020 6966 2073 656c 662e 5f65 7874      if self._ext
-0000f3d0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
-0000f3e0: 666f 7220 5f2c 2064 696d 2069 6e20 6c69  for _, dim in li
-0000f3f0: 7374 2873 656c 662e 5f65 7874 7261 2e73  st(self._extra.s
-0000f400: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
-0000f410: 782e 6974 656d 7328 2929 3a0a 2020 2020  x.items()):.    
-0000f420: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000f430: 7274 2069 7369 6e73 7461 6e63 6528 6469  rt isinstance(di
-0000f440: 6d2c 205f 642e 4469 6d29 0a20 2020 2020  m, _d.Dim).     
-0000f450: 2020 2020 2020 2020 2020 2064 696d 2e5f             dim._
-0000f460: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000f470: 656e 745f 6772 6170 6828 290a 2020 2020  ent_graph().    
-0000f480: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-0000f490: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-0000f4a0: 6d62 6572 0a20 2020 2020 2020 2069 6620  mber.        if 
-0000f4b0: 6f74 6865 722e 5f65 7874 7261 3a0a 2020  other._extra:.  
-0000f4c0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-0000f4d0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-0000f4e0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-0000f4f0: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
-0000f500: 6469 6d20 696e 206f 7468 6572 2e5f 6578  dim in other._ex
-0000f510: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
-0000f520: 6368 5f63 7478 2e69 7465 6d73 2829 3a0a  ch_ctx.items():.
-0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f540: 6966 206e 6f74 2064 696d 2e5f 7661 6c69  if not dim._vali
-0000f550: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000f560: 6772 6170 6828 293a 0a20 2020 2020 2020  graph():.       
-0000f570: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000f580: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-0000f590: 2020 2020 2020 7365 6c66 5f64 696d 203d        self_dim =
-0000f5a0: 2073 656c 662e 5f6d 616b 655f 6578 7472   self._make_extr
-0000f5b0: 6128 292e 7361 6d65 5f66 6f72 5f62 6174  a().same_for_bat
-0000f5c0: 6368 5f63 7478 2e67 6574 286b 6579 2c20  ch_ctx.get(key, 
-0000f5d0: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
-0000f5e0: 2020 2020 2020 6966 2073 656c 665f 6469        if self_di
-0000f5f0: 6d20 616e 6420 2873 656c 665f 6469 6d2e  m and (self_dim.
-0000f600: 6479 6e5f 7369 7a65 5f65 7874 206f 7220  dyn_size_ext or 
-0000f610: 6e6f 7420 6469 6d2e 6479 6e5f 7369 7a65  not dim.dyn_size
-0000f620: 5f65 7874 293a 0a20 2020 2020 2020 2020  _ext):.         
-0000f630: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000f640: 6e75 6520 2023 206b 6565 7020 6f75 7273  nue  # keep ours
-0000f650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f660: 2069 6620 6e6f 7420 6469 6d2e 6479 6e5f   if not dim.dyn_
-0000f670: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-0000f680: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f690: 6e74 696e 7565 2020 2320 756e 6465 6669  ntinue  # undefi
-0000f6a0: 6e65 642c 2064 6f20 6e6f 7420 6f76 6572  ned, do not over
-0000f6b0: 7461 6b65 0a20 2020 2020 2020 2020 2020  take.           
-0000f6c0: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
-0000f6d0: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-0000f6e0: 6374 785b 6b65 795d 203d 2064 696d 0a20  ctx[key] = dim. 
-0000f6f0: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
-0000f700: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-0000f710: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-0000f720: 2020 2020 2020 2020 6f74 6865 722e 5f65          other._e
-0000f730: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
-0000f740: 7463 685f 6374 782e 636c 6561 7228 2920  tch_ctx.clear() 
-0000f750: 2023 2077 6520 6f6e 6c79 2077 616e 7420   # we only want 
-0000f760: 746f 2068 6176 6520 6974 206f 6e63 650a  to have it once.
-0000f770: 0a20 2020 2023 206e 6f69 6e73 7065 6374  .    # noinspect
-0000f780: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
-0000f790: 656d 6265 720a 2020 2020 6465 6620 6465  ember.    def de
-0000f7a0: 7269 7665 5f66 726f 6d28 7365 6c66 3a20  rive_from(self: 
-0000f7b0: 5f64 2e44 696d 2c20 6261 7365 3a20 5f64  _d.Dim, base: _d
-0000f7c0: 2e44 696d 2c20 7365 745f 6465 7269 7665  .Dim, set_derive
-0000f7d0: 645f 6672 6f6d 5f66 6c61 673a 2062 6f6f  d_from_flag: boo
-0000f7e0: 6c20 3d20 5472 7565 293a 0a20 2020 2020  l = True):.     
-0000f7f0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-0000f800: 7061 7261 6d20 6261 7365 3a20 6469 6d0a  param base: dim.
-0000f810: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0000f820: 6574 5f64 6572 6976 6564 5f66 726f 6d5f  et_derived_from_
-0000f830: 666c 6167 3a0a 2020 2020 2020 2020 2222  flag:.        ""
-0000f840: 220a 2020 2020 2020 2020 7365 6c66 5f62  ".        self_b
-0000f850: 6173 6520 3d20 7365 6c66 2e67 6574 5f73  ase = self.get_s
-0000f860: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
-0000f870: 2020 2073 656c 665f 6261 7365 5f65 7874     self_base_ext
-0000f880: 7261 203d 2073 656c 665f 6261 7365 2e5f  ra = self_base._
-0000f890: 6d61 6b65 5f65 7874 7261 2829 0a20 2020  make_extra().   
-0000f8a0: 2020 2020 2069 6620 7365 745f 6465 7269       if set_deri
-0000f8b0: 7665 645f 6672 6f6d 5f66 6c61 673a 0a20  ved_from_flag:. 
-0000f8c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f8d0: 6c66 5f62 6173 655f 6578 7472 612e 6465  lf_base_extra.de
-0000f8e0: 7269 7665 645f 6672 6f6d 5f74 6167 3a0a  rived_from_tag:.
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f900: 6173 7365 7274 2073 656c 665f 6261 7365  assert self_base
-0000f910: 5f65 7874 7261 2e64 6572 6976 6564 5f66  _extra.derived_f
-0000f920: 726f 6d5f 7461 6720 3d3d 2062 6173 650a  rom_tag == base.
-0000f930: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000f940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f950: 2020 7365 6c66 5f62 6173 655f 6578 7472    self_base_extr
-0000f960: 612e 6465 7269 7665 645f 6672 6f6d 5f74  a.derived_from_t
-0000f970: 6167 203d 2062 6173 650a 2020 2020 2020  ag = base.      
-0000f980: 2020 6966 206e 6f74 2073 656c 662e 6261    if not self.ba
-0000f990: 7463 6820 616e 6420 6261 7365 2e62 6174  tch and base.bat
-0000f9a0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-0000f9b0: 7365 6c66 2e62 6174 6368 203d 2062 6173  self.batch = bas
-0000f9c0: 652e 6261 7463 680a 2020 2020 2020 2020  e.batch.        
-0000f9d0: 2020 2020 7365 6c66 2e63 6f6e 7472 6f6c      self.control
-0000f9e0: 5f66 6c6f 775f 6374 7820 3d20 6261 7365  _flow_ctx = base
-0000f9f0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000fa00: 780a 2020 2020 2020 2020 2020 2020 6b65  x.            ke
-0000fa10: 7920 3d20 6261 7365 2e62 6174 6368 2c20  y = base.batch, 
-0000fa20: 6261 7365 2e63 6f6e 7472 6f6c 5f66 6c6f  base.control_flo
-0000fa30: 775f 6374 780a 2020 2020 2020 2020 2020  w_ctx.          
-0000fa40: 2020 6173 7365 7274 206b 6579 206e 6f74    assert key not
-0000fa50: 2069 6e20 7365 6c66 5f62 6173 655f 6578   in self_base_ex
-0000fa60: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
-0000fa70: 6368 5f63 7478 0a20 2020 2020 2020 2020  ch_ctx.         
-0000fa80: 2020 2073 656c 665f 6261 7365 5f65 7874     self_base_ext
-0000fa90: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
-0000faa0: 685f 6374 785b 6b65 795d 203d 2073 656c  h_ctx[key] = sel
-0000fab0: 660a 2020 2020 2020 2020 6966 2073 656c  f.        if sel
-0000fac0: 662e 6973 5f64 796e 616d 6963 2829 206f  f.is_dynamic() o
-0000fad0: 7220 6e6f 7420 7365 6c66 2e69 735f 6469  r not self.is_di
-0000fae0: 6d5f 6b6e 6f77 6e28 293a 0a20 2020 2020  m_known():.     
-0000faf0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000fb00: 6c66 2e64 796e 5f73 697a 655f 6578 743a  lf.dyn_size_ext:
-0000fb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fb20: 2069 6620 6261 7365 2e64 796e 5f73 697a   if base.dyn_siz
-0000fb30: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
-0000fb40: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
-0000fb50: 7365 2e62 6174 6368 2061 6e64 2062 6173  se.batch and bas
-0000fb60: 652e 6261 7463 6820 3d3d 2073 656c 662e  e.batch == self.
-0000fb70: 6261 7463 6820 616e 6420 6261 7365 2e63  batch and base.c
-0000fb80: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7820  ontrol_flow_ctx 
-0000fb90: 3d3d 2073 656c 662e 636f 6e74 726f 6c5f  == self.control_
-0000fba0: 666c 6f77 5f63 7478 3a0a 2020 2020 2020  flow_ctx:.      
-0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbc0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-0000fbd0: 6578 7420 3d20 6261 7365 2e64 796e 5f73  ext = base.dyn_s
-0000fbe0: 697a 655f 6578 742e 636f 7079 5f74 656d  ize_ext.copy_tem
-0000fbf0: 706c 6174 6528 6e61 6d65 3d22 2573 3a73  plate(name="%s:s
-0000fc00: 697a 6522 2025 2073 656c 665f 6261 7365  ize" % self_base
-0000fc10: 2e64 6573 6372 6970 7469 6f6e 290a 2020  .description).  
-0000fc20: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000fc30: 6966 2062 6173 652e 6973 5f62 6174 6368  if base.is_batch
-0000fc40: 5f64 696d 2829 3a0a 2020 2020 2020 2020  _dim():.        
-0000fc50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fc60: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
-0000fc70: 5f74 2e54 656e 736f 7228 0a20 2020 2020  _t.Tensor(.     
-0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc90: 2020 206e 616d 653d 2225 733a 6261 7463     name="%s:batc
-0000fca0: 6822 2025 2073 656c 665f 6261 7365 2e64  h" % self_base.d
-0000fcb0: 6573 6372 6970 7469 6f6e 2c20 7368 6170  escription, shap
-0000fcc0: 653d 2829 2c20 6474 7970 653d 2269 6e74  e=(), dtype="int
-0000fcd0: 3332 222c 2062 6174 6368 5f64 696d 5f61  32", batch_dim_a
-0000fce0: 7869 733d 4e6f 6e65 0a20 2020 2020 2020  xis=None.       
-0000fcf0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000fd00: 2020 2020 6465 6620 636f 7079 5f66 726f      def copy_fro
-0000fd10: 6d28 7365 6c66 3a20 4469 6d2c 206f 7468  m(self: Dim, oth
-0000fd20: 6572 3a20 4469 6d29 3a0a 2020 2020 2020  er: Dim):.      
-0000fd30: 2020 2222 2264 6566 696e 6522 2222 0a20    """define""". 
-0000fd40: 2020 2020 2020 2073 656c 662e 7369 7a65         self.size
-0000fd50: 203d 206f 7468 6572 2e73 697a 650a 2020   = other.size.  
-0000fd60: 2020 2020 2020 7365 6c66 2e63 6170 6163        self.capac
-0000fd70: 6974 7920 3d20 6f74 6865 722e 6361 7061  ity = other.capa
-0000fd80: 6369 7479 0a20 2020 2020 2020 2073 656c  city.        sel
-0000fd90: 662e 6479 6e5f 7369 7a65 5f65 7874 203d  f.dyn_size_ext =
-0000fda0: 206f 7468 6572 2e64 796e 5f73 697a 655f   other.dyn_size_
-0000fdb0: 6578 740a 2020 2020 2020 2020 7365 6c66  ext.        self
-0000fdc0: 2e64 6572 6976 655f 6672 6f6d 286f 7468  .derive_from(oth
-0000fdd0: 6572 290a 0a20 2020 2040 636c 6173 736d  er)..    @classm
-0000fde0: 6574 686f 640a 2020 2020 6465 6620 6765  ethod.    def ge
-0000fdf0: 745f 6578 6973 7469 6e67 5f74 6167 5f66  t_existing_tag_f
-0000fe00: 726f 6d5f 636f 6c6c 6563 7469 6f6e 2863  rom_collection(c
-0000fe10: 6c73 2c20 6f74 6865 722c 2074 6167 732c  ls, other, tags,
-0000fe20: 2069 735f 6571 7561 6c5f 6f70 7473 3d4e   is_equal_opts=N
-0000fe30: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-0000fe40: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-0000fe50: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
-0000fe60: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
-0000fe70: 4469 6d5d 7c74 7570 6c65 5b44 696d 5d7c  Dim]|tuple[Dim]|
-0000fe80: 7365 745b 4469 6d5d 2074 6167 733a 0a20  set[Dim] tags:. 
-0000fe90: 2020 2020 2020 203a 7061 7261 6d20 6469         :param di
-0000fea0: 6374 5b73 7472 5d7c 4e6f 6e65 2069 735f  ct[str]|None is_
-0000feb0: 6571 7561 6c5f 6f70 7473 3a20 7061 7373  equal_opts: pass
-0000fec0: 6564 2074 6f20 4469 6d2e 6973 5f65 7175  ed to Dim.is_equ
-0000fed0: 616c 0a20 2020 2020 2020 203a 7274 7970  al.        :rtyp
-0000fee0: 653a 2044 696d 7c4e 6f6e 650a 2020 2020  e: Dim|None.    
-0000fef0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ff00: 6966 2069 735f 6571 7561 6c5f 6f70 7473  if is_equal_opts
-0000ff10: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000ff20: 2020 2020 2020 6973 5f65 7175 616c 5f6f        is_equal_o
-0000ff30: 7074 7320 3d20 7b7d 0a20 2020 2020 2020  pts = {}.       
-0000ff40: 2023 2057 6520 646f 2070 6f74 656e 7469   # We do potenti
-0000ff50: 616c 206d 756c 7469 706c 6520 726f 756e  al multiple roun
-0000ff60: 6473 2c20 7375 6368 2074 6861 7420 7765  ds, such that we
-0000ff70: 2070 7265 6665 7220 226d 6f72 6520 6571   prefer "more eq
-0000ff80: 7561 6c22 2028 7573 696e 6720 6c65 7373  ual" (using less
-0000ff90: 2069 735f 6571 7561 6c5f 6f70 7473 292e   is_equal_opts).
-0000ffa0: 0a20 2020 2020 2020 2072 6f75 6e64 7320  .        rounds 
-0000ffb0: 3d20 5b7b 7d5d 0a20 2020 2020 2020 2069  = [{}].        i
-0000ffc0: 6620 6973 5f65 7175 616c 5f6f 7074 733a  f is_equal_opts:
-0000ffd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ffe0: 2262 726f 6164 6361 7374 5f6d 6174 6368  "broadcast_match
-0000fff0: 6573 2220 696e 2069 735f 6571 7561 6c5f  es" in is_equal_
-00010000: 6f70 7473 3a0a 2020 2020 2020 2020 2020  opts:.          
-00010010: 2020 2020 2020 726f 756e 6473 2e61 7070        rounds.app
-00010020: 656e 6428 7b6b 3a20 7620 666f 7220 286b  end({k: v for (k
-00010030: 2c20 7629 2069 6e20 6973 5f65 7175 616c  , v) in is_equal
-00010040: 5f6f 7074 732e 6974 656d 7328 2920 6966  _opts.items() if
-00010050: 206b 2021 3d20 2262 726f 6164 6361 7374   k != "broadcast
-00010060: 5f6d 6174 6368 6573 227d 290a 2020 2020  _matches"}).    
-00010070: 2020 2020 2020 2020 726f 756e 6473 2e61          rounds.a
-00010080: 7070 656e 6428 6973 5f65 7175 616c 5f6f  ppend(is_equal_o
-00010090: 7074 7329 0a20 2020 2020 2020 2066 6f72  pts).        for
-000100a0: 205f 6973 5f65 7175 616c 5f6f 7074 7320   _is_equal_opts 
-000100b0: 696e 2072 6f75 6e64 733a 0a20 2020 2020  in rounds:.     
-000100c0: 2020 2020 2020 2066 6f72 205f 7461 6720         for _tag 
-000100d0: 696e 2074 6167 733a 0a20 2020 2020 2020  in tags:.       
-000100e0: 2020 2020 2020 2020 2069 6620 5f74 6167           if _tag
-000100f0: 2e69 735f 6571 7561 6c28 6f74 6865 722c  .is_equal(other,
-00010100: 202a 2a5f 6973 5f65 7175 616c 5f6f 7074   **_is_equal_opt
-00010110: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00010120: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00010130: 7461 670a 2020 2020 2020 2020 7265 7475  tag.        retu
-00010140: 726e 204e 6f6e 650a 0a20 2020 2040 636c  rn None..    @cl
-00010150: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00010160: 6620 6765 745f 616c 6c5f 6469 6d65 6e73  f get_all_dimens
-00010170: 696f 6e5f 7461 6773 2863 6c73 2c20 6461  ion_tags(cls, da
-00010180: 7461 5f6c 6973 742c 2069 735f 6571 7561  ta_list, is_equa
-00010190: 6c5f 6f70 7473 3d4e 6f6e 652c 2075 6e69  l_opts=None, uni
-000101a0: 7175 655f 7365 7061 7261 7465 5f61 7865  que_separate_axe
-000101b0: 733d 5472 7565 293a 0a20 2020 2020 2020  s=True):.       
-000101c0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-000101d0: 7261 6d20 6c69 7374 5b5f 742e 5465 6e73  ram list[_t.Tens
-000101e0: 6f72 5d20 6461 7461 5f6c 6973 743a 0a20  or] data_list:. 
-000101f0: 2020 2020 2020 203a 7061 7261 6d20 6469         :param di
-00010200: 6374 5b73 7472 5d7c 4e6f 6e65 2069 735f  ct[str]|None is_
-00010210: 6571 7561 6c5f 6f70 7473 3a20 7061 7373  equal_opts: pass
-00010220: 6564 2074 6f20 4469 6d2e 6973 5f65 7175  ed to Dim.is_equ
-00010230: 616c 0a20 2020 2020 2020 203a 7061 7261  al.        :para
-00010240: 6d20 626f 6f6c 2075 6e69 7175 655f 7365  m bool unique_se
-00010250: 7061 7261 7465 5f61 7865 733a 2065 2e67  parate_axes: e.g
-00010260: 2e20 6461 7461 5f6c 6973 743d 5b44 6174  . data_list=[Dat
-00010270: 6120 7769 7468 2073 6861 7065 2028 422c  a with shape (B,
-00010280: 352c 352c 3130 295d 2072 6573 756c 7473  5,5,10)] results
-00010290: 2069 6e20 3420 6469 6d20 7461 6773 2c20   in 4 dim tags, 
-000102a0: 6e6f 7420 332e 0a20 2020 2020 2020 203a  not 3..        :
-000102b0: 7265 7475 726e 3a20 6c69 7374 206f 6620  return: list of 
-000102c0: 6469 6d65 6e73 696f 6e20 7461 6773 2c20  dimension tags, 
-000102d0: 6469 6374 2066 6f72 2064 6174 6120 2d3e  dict for data ->
-000102e0: 206c 6973 7420 6f66 2064 696d 656e 7369   list of dimensi
-000102f0: 6f6e 2074 6167 7320 2866 6f72 2065 6163  on tags (for eac
-00010300: 6820 6178 6973 290a 2020 2020 2020 2020  h axis).        
-00010310: 3a72 7479 7065 3a20 286c 6973 745b 4469  :rtype: (list[Di
-00010320: 6d5d 2c20 7574 696c 2e44 6963 7452 6566  m], util.DictRef
-00010330: 4b65 7973 5b5f 742e 5465 6e73 6f72 2c20  Keys[_t.Tensor, 
-00010340: 6c69 7374 5b44 696d 5d5d 290a 2020 2020  list[Dim]]).    
-00010350: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010360: 7461 6773 203d 205b 5d0a 2020 2020 2020  tags = [].      
-00010370: 2020 6461 7461 5f61 7865 735f 6469 6374    data_axes_dict
-00010380: 203d 2075 7469 6c2e 4469 6374 5265 664b   = util.DictRefK
-00010390: 6579 7328 2920 2023 2074 7970 653a 2075  eys()  # type: u
-000103a0: 7469 6c2e 4469 6374 5265 664b 6579 735b  til.DictRefKeys[
-000103b0: 5f74 2e54 656e 736f 722c 204c 6973 745b  _t.Tensor, List[
-000103c0: 4469 6d5d 5d0a 2020 2020 2020 2020 666f  Dim]].        fo
-000103d0: 7220 6461 7461 2069 6e20 6461 7461 5f6c  r data in data_l
-000103e0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-000103f0: 2064 6174 615f 6178 6573 5f64 6963 745b   data_axes_dict[
-00010400: 6461 7461 5d20 3d20 5b5d 0a20 2020 2020  data] = [].     
-00010410: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
-00010420: 7461 675f 636f 6c6c 6563 7469 6f6e 5f66  tag_collection_f
-00010430: 6f72 5f64 6174 6120 3d20 6c69 7374 2874  or_data = list(t
-00010440: 6167 7329 2069 6620 756e 6971 7565 5f73  ags) if unique_s
-00010450: 6570 6172 6174 655f 6178 6573 2065 6c73  eparate_axes els
-00010460: 6520 7461 6773 0a20 2020 2020 2020 2020  e tags.         
-00010470: 2020 2066 6f72 2061 7869 7320 696e 2072     for axis in r
-00010480: 616e 6765 2864 6174 612e 6261 7463 685f  ange(data.batch_
-00010490: 6e64 696d 293a 0a20 2020 2020 2020 2020  ndim):.         
-000104a0: 2020 2020 2020 2074 6167 203d 2064 6174         tag = dat
-000104b0: 612e 6765 745f 6469 6d5f 7461 6728 6178  a.get_dim_tag(ax
-000104c0: 6973 290a 2020 2020 2020 2020 2020 2020  is).            
-000104d0: 2020 2020 6578 6973 7469 6e67 5f74 6167      existing_tag
-000104e0: 203d 2063 6c73 2e67 6574 5f65 7869 7374   = cls.get_exist
-000104f0: 696e 675f 7461 675f 6672 6f6d 5f63 6f6c  ing_tag_from_col
-00010500: 6c65 6374 696f 6e28 0a20 2020 2020 2020  lection(.       
-00010510: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-00010520: 2c20 7461 6773 3d65 7869 7374 696e 675f  , tags=existing_
-00010530: 7461 675f 636f 6c6c 6563 7469 6f6e 5f66  tag_collection_f
-00010540: 6f72 5f64 6174 612c 2069 735f 6571 7561  or_data, is_equa
-00010550: 6c5f 6f70 7473 3d69 735f 6571 7561 6c5f  l_opts=is_equal_
-00010560: 6f70 7473 0a20 2020 2020 2020 2020 2020  opts.           
-00010570: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00010580: 2020 2020 2020 2069 6620 6578 6973 7469         if existi
-00010590: 6e67 5f74 6167 3a0a 2020 2020 2020 2020  ng_tag:.        
-000105a0: 2020 2020 2020 2020 2020 2020 6966 2075              if u
-000105b0: 6e69 7175 655f 7365 7061 7261 7465 5f61  nique_separate_a
-000105c0: 7865 733a 0a20 2020 2020 2020 2020 2020  xes:.           
-000105d0: 2020 2020 2020 2020 2020 2020 2065 7869               exi
-000105e0: 7374 696e 675f 7461 675f 636f 6c6c 6563  sting_tag_collec
-000105f0: 7469 6f6e 5f66 6f72 5f64 6174 612e 7265  tion_for_data.re
-00010600: 6d6f 7665 2865 7869 7374 696e 675f 7461  move(existing_ta
-00010610: 6729 2020 2320 646f 6e27 7420 7461 6b65  g)  # don't take
-00010620: 2069 7420 6167 6169 6e20 666f 7220 7468   it again for th
-00010630: 6973 2064 6174 610a 2020 2020 2020 2020  is data.        
-00010640: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00010650: 6163 655f 6578 6973 7469 6e67 203d 2028  ace_existing = (
-00010660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010670: 2020 2020 2020 2020 2065 7869 7374 696e           existin
-00010680: 675f 7461 672e 756e 6465 6669 6e65 6420  g_tag.undefined 
-00010690: 616e 6420 6e6f 7420 7461 672e 756e 6465  and not tag.unde
-000106a0: 6669 6e65 6420 616e 6420 7461 672e 6469  fined and tag.di
-000106b0: 6d65 6e73 696f 6e20 3d3d 2065 7869 7374  mension == exist
-000106c0: 696e 675f 7461 672e 6469 6d65 6e73 696f  ing_tag.dimensio
-000106d0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-000106e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000106f0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00010700: 6570 6c61 6365 5f65 7869 7374 696e 673a  eplace_existing:
-00010710: 2020 2320 5265 706c 6163 6520 7468 6520    # Replace the 
-00010720: 6578 6973 7469 6e67 2062 7920 7468 6520  existing by the 
-00010730: 6e65 7720 7461 672e 0a20 2020 2020 2020  new tag..       
-00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010750: 2074 6167 735b 7461 6773 2e69 6e64 6578   tags[tags.index
-00010760: 2865 7869 7374 696e 675f 7461 6729 5d20  (existing_tag)] 
-00010770: 3d20 7461 670a 2020 2020 2020 2020 2020  = tag.          
-00010780: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00010790: 7220 5f2c 2064 696d 735f 2069 6e20 6461  r _, dims_ in da
-000107a0: 7461 5f61 7865 735f 6469 6374 2e69 7465  ta_axes_dict.ite
-000107b0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107d0: 2020 6469 6d73 5f5b 3a5d 203d 205b 7461    dims_[:] = [ta
-000107e0: 6720 6966 2064 203d 3d20 6578 6973 7469  g if d == existi
-000107f0: 6e67 5f74 6167 2065 6c73 6520 6420 666f  ng_tag else d fo
-00010800: 7220 6420 696e 2064 696d 735f 5d0a 2020  r d in dims_].  
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 2020 6578 6973 7469 6e67 5f74        existing_t
-00010830: 6167 203d 2074 6167 0a20 2020 2020 2020  ag = tag.       
-00010840: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
-00010850: 2320 6e6f 2065 7869 7374 696e 6720 7461  # no existing ta
-00010860: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00010870: 2020 2020 2020 7461 6773 2e61 7070 656e        tags.appen
-00010880: 6428 7461 6729 0a20 2020 2020 2020 2020  d(tag).         
-00010890: 2020 2020 2020 2064 6174 615f 6178 6573         data_axes
-000108a0: 5f64 6963 745b 6461 7461 5d2e 6170 7065  _dict[data].appe
-000108b0: 6e64 2865 7869 7374 696e 675f 7461 6720  nd(existing_tag 
-000108c0: 6f72 2074 6167 290a 2020 2020 2020 2020  or tag).        
-000108d0: 7265 7475 726e 2074 6167 732c 2064 6174  return tags, dat
-000108e0: 615f 6178 6573 5f64 6963 740a 0a20 2020  a_axes_dict..   
-000108f0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00010900: 2020 6465 6620 6765 745f 756e 6971 5f63    def get_uniq_c
-00010910: 6f6c 6c65 6374 696f 6e28 636c 732c 2074  ollection(cls, t
-00010920: 6167 732c 2069 735f 6571 7561 6c5f 6f70  ags, is_equal_op
-00010930: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
-00010940: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00010950: 6172 616d 206c 6973 745b 4469 6d5d 7c74  aram list[Dim]|t
-00010960: 7570 6c65 5b44 696d 5d7c 7365 745b 4469  uple[Dim]|set[Di
-00010970: 6d5d 2074 6167 733a 0a20 2020 2020 2020  m] tags:.       
-00010980: 203a 7061 7261 6d20 6469 6374 5b73 7472   :param dict[str
-00010990: 5d7c 4e6f 6e65 2069 735f 6571 7561 6c5f  ]|None is_equal_
-000109a0: 6f70 7473 3a20 7061 7373 6564 2074 6f20  opts: passed to 
-000109b0: 4469 6d2e 6973 5f65 7175 616c 0a20 2020  Dim.is_equal.   
-000109c0: 2020 2020 203a 7274 7970 653a 206c 6973       :rtype: lis
-000109d0: 745b 4469 6d5d 0a20 2020 2020 2020 2022  t[Dim].        "
-000109e0: 2222 0a20 2020 2020 2020 2072 6573 203d  "".        res =
-000109f0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-00010a00: 7461 6720 696e 2074 6167 733a 0a20 2020  tag in tags:.   
-00010a10: 2020 2020 2020 2020 2065 7820 3d20 636c           ex = cl
-00010a20: 732e 6765 745f 6578 6973 7469 6e67 5f74  s.get_existing_t
-00010a30: 6167 5f66 726f 6d5f 636f 6c6c 6563 7469  ag_from_collecti
-00010a40: 6f6e 2874 6167 2c20 7265 732c 2069 735f  on(tag, res, is_
-00010a50: 6571 7561 6c5f 6f70 7473 3d69 735f 6571  equal_opts=is_eq
-00010a60: 7561 6c5f 6f70 7473 290a 2020 2020 2020  ual_opts).      
-00010a70: 2020 2020 2020 6966 206e 6f74 2065 783a        if not ex:
-00010a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010a90: 2072 6573 2e61 7070 656e 6428 7461 6729   res.append(tag)
-00010aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010ab0: 7265 730a 0a20 2020 2064 6566 2067 6574  res..    def get
-00010ac0: 5f73 697a 655f 7465 6e73 6f72 2873 656c  _size_tensor(sel
-00010ad0: 6629 202d 3e20 5f74 2e54 656e 736f 723a  f) -> _t.Tensor:
-00010ae0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010af0: 2020 2020 203a 7265 7475 726e 3a20 7369       :return: si
-00010b00: 7a65 2074 656e 736f 722c 206f 7220 6479  ze tensor, or dy
-00010b10: 6e5f 7369 7a65 5f65 7874 2069 6620 6465  n_size_ext if de
-00010b20: 6669 6e65 640a 2020 2020 2020 2020 3a72  fined.        :r
-00010b30: 7479 7065 3a20 5f74 2e54 656e 736f 720a  type: _t.Tensor.
-00010b40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010b50: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
-00010b60: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-00010b70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00010b80: 662e 6479 6e5f 7369 7a65 5f65 7874 0a0a  f.dyn_size_ext..
-00010b90: 2020 2020 2020 2020 696d 706f 7274 2072          import r
-00010ba0: 6574 7572 6e6e 2e66 726f 6e74 656e 6420  eturnn.frontend 
-00010bb0: 6173 2072 660a 0a20 2020 2020 2020 2061  as rf..        a
-00010bc0: 7373 6572 7420 7365 6c66 2e73 697a 6520  ssert self.size 
-00010bd0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00010be0: 2020 2020 7265 7475 726e 2072 662e 636f      return rf.co
-00010bf0: 6e76 6572 745f 746f 5f74 656e 736f 7228  nvert_to_tensor(
-00010c00: 7365 6c66 2e73 697a 652c 206e 616d 653d  self.size, name=
-00010c10: 2225 733a 7369 7a65 2220 2520 7365 6c66  "%s:size" % self
-00010c20: 2e64 6573 6372 6970 7469 6f6e 290a 0a20  .description).. 
-00010c30: 2020 2064 6566 2067 6574 5f64 696d 5f76     def get_dim_v
-00010c40: 616c 7565 2873 656c 6629 202d 3e20 556e  alue(self) -> Un
-00010c50: 696f 6e5b 696e 742c 205f 742e 5261 7754  ion[int, _t.RawT
-00010c60: 656e 736f 7254 7970 655d 3a0a 2020 2020  ensorType]:.    
-00010c70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010c80: 496e 6665 7273 2074 6865 2064 696d 2074  Infers the dim t
-00010c90: 6869 7320 6178 6973 2073 686f 756c 6420  his axis should 
-00010ca0: 6861 7665 2069 6620 756e 6272 6f61 6463  have if unbroadc
-00010cb0: 6173 7465 642e 0a20 2020 2020 2020 2049  asted..        I
-00010cc0: 6620 6073 656c 662e 7372 635f 6461 7461  f `self.src_data
-00010cd0: 6020 6861 7320 6120 706c 6163 6568 6f6c  ` has a placehol
-00010ce0: 6465 722c 2077 696c 6c20 7573 6520 7468  der, will use th
-00010cf0: 6520 7368 6170 6520 6672 6f6d 2074 6865  e shape from the
-00010d00: 7265 2e0a 2020 2020 2020 2020 4f74 6865  re..        Othe
-00010d10: 7277 6973 652c 2075 7365 7320 6073 656c  rwise, uses `sel
-00010d20: 662e 6469 6d65 6e73 696f 6e60 2028 6966  f.dimension` (if
-00010d30: 2073 7461 7469 6329 206f 7220 6073 656c   static) or `sel
-00010d40: 662e 6479 6e5f 7369 7a65 6020 2869 6620  f.dyn_size` (if 
-00010d50: 6479 6e61 6d69 6329 2e0a 0a20 2020 2020  dynamic)...     
-00010d60: 2020 203a 7265 7475 726e 3a20 6d61 7828     :return: max(
-00010d70: 7369 7a65 206f 7220 6479 6e5f 7369 7a65  size or dyn_size
-00010d80: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00010d90: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-00010da0: 2e67 6574 5f64 696d 5f76 616c 7565 5f74  .get_dim_value_t
-00010db0: 656e 736f 7228 290a 2020 2020 2020 2020  ensor().        
-00010dc0: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
-00010dd0: 732c 205f 742e 5465 6e73 6f72 293a 0a20  s, _t.Tensor):. 
-00010de0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00010df0: 7420 7265 732e 6469 6d73 203d 3d20 2829  t res.dims == ()
-00010e00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00010e10: 7572 6e20 7265 732e 7261 775f 7465 6e73  urn res.raw_tens
-00010e20: 6f72 0a20 2020 2020 2020 2061 7373 6572  or.        asser
-00010e30: 7420 6973 696e 7374 616e 6365 2872 6573  t isinstance(res
-00010e40: 2c20 696e 7429 0a20 2020 2020 2020 2072  , int).        r
-00010e50: 6574 7572 6e20 7265 730a 0a20 2020 2064  eturn res..    d
-00010e60: 6566 2067 6574 5f64 696d 5f76 616c 7565  ef get_dim_value
-00010e70: 5f74 656e 736f 7228 7365 6c66 2920 2d3e  _tensor(self) ->
-00010e80: 2055 6e69 6f6e 5b69 6e74 2c20 5f74 2e54   Union[int, _t.T
-00010e90: 656e 736f 725d 3a0a 2020 2020 2020 2020  ensor]:.        
-00010ea0: 2222 220a 2020 2020 2020 2020 496e 6665  """.        Infe
-00010eb0: 7273 2074 6865 2064 696d 2074 6869 7320  rs the dim this 
-00010ec0: 6178 6973 2073 686f 756c 6420 6861 7665  axis should have
-00010ed0: 2069 6620 756e 6272 6f61 6463 6173 7465   if unbroadcaste
-00010ee0: 642e 0a20 2020 2020 2020 2049 6620 6073  d..        If `s
-00010ef0: 656c 662e 7372 635f 6461 7461 6020 6861  elf.src_data` ha
-00010f00: 7320 6120 706c 6163 6568 6f6c 6465 722c  s a placeholder,
-00010f10: 2077 696c 6c20 7573 6520 7468 6520 7368   will use the sh
-00010f20: 6170 6520 6672 6f6d 2074 6865 7265 2e0a  ape from there..
-00010f30: 2020 2020 2020 2020 4f74 6865 7277 6973          Otherwis
-00010f40: 652c 2075 7365 7320 6073 656c 662e 6469  e, uses `self.di
-00010f50: 6d65 6e73 696f 6e60 2028 6966 2073 7461  mension` (if sta
-00010f60: 7469 6329 206f 7220 6073 656c 662e 6479  tic) or `self.dy
-00010f70: 6e5f 7369 7a65 6020 2869 6620 6479 6e61  n_size` (if dyna
-00010f80: 6d69 6329 2e0a 0a20 2020 2020 2020 203a  mic)...        :
-00010f90: 7265 7475 726e 3a20 6d61 7828 7369 7a65  return: max(size
-00010fa0: 206f 7220 6479 6e5f 7369 7a65 290a 2020   or dyn_size).  
-00010fb0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010fc0: 2020 696d 706f 7274 2072 6574 7572 6e6e    import returnn
-00010fd0: 2e66 726f 6e74 656e 6420 6173 2072 660a  .frontend as rf.
-00010fe0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00010ff0: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
-00011000: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00011010: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011020: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
-00011030: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
-00011040: 7a65 5f65 7874 2061 6e64 2073 656c 662e  ze_ext and self.
-00011050: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-00011060: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-00011070: 4e6f 6e65 3a20 2023 2066 6173 7420 7061  None:  # fast pa
-00011080: 7468 0a20 2020 2020 2020 2020 2020 2069  th.            i
-00011090: 6620 7365 6c66 2e64 796e 5f73 697a 655f  f self.dyn_size_
-000110a0: 6578 742e 6261 7463 685f 6e64 696d 203e  ext.batch_ndim >
-000110b0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-000110c0: 2020 2020 7265 7475 726e 2072 662e 7265      return rf.re
-000110d0: 6475 6365 5f6d 6178 280a 2020 2020 2020  duce_max(.      
-000110e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000110f0: 6c66 2e64 796e 5f73 697a 655f 6578 742c  lf.dyn_size_ext,
-00011100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011110: 2020 2020 2061 7869 733d 7365 6c66 2e64       axis=self.d
-00011120: 796e 5f73 697a 655f 6578 742e 6469 6d5f  yn_size_ext.dim_
-00011130: 7461 6773 2c0a 2020 2020 2020 2020 2020  tags,.          
-00011140: 2020 2020 2020 2020 2020 2320 4d61 736b            # Mask
-00011150: 696e 6720 6973 206e 6f74 2061 6c77 6179  ing is not alway
-00011160: 7320 706f 7373 6962 6c65 2068 6572 652c  s possible here,
-00011170: 2065 2e67 2e0a 2020 2020 2020 2020 2020   e.g..          
-00011180: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00011190: 203d 2044 696d 7b27 7365 6c66 2d61 7474   = Dim{'self-att
-000111a0: 2d6b 6579 7327 5b27 7469 6d65 3a76 6172  -keys'['time:var
-000111b0: 3a65 7874 6572 6e5f 6461 7461 3a63 6c61  :extern_data:cla
-000111c0: 7373 6573 275b 425d 5d7d 2e0a 2020 2020  sses'[B]]}..    
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 7573 655f 6d61 736b 3d46 616c 7365 2c0a  use_mask=False,.
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00011210: 7475 726e 2073 656c 662e 6479 6e5f 7369  turn self.dyn_si
-00011220: 7a65 5f65 7874 0a20 2020 2020 2020 2069  ze_ext.        i
-00011230: 6620 7365 6c66 2e69 735f 6261 7463 685f  f self.is_batch_
-00011240: 6469 6d28 293a 0a20 2020 2020 2020 2020  dim():.         
-00011250: 2020 2072 6573 203d 204e 6f6e 650a 2020     res = None.  
-00011260: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00011270: 662e 5f65 7874 7261 2061 6e64 2073 656c  f._extra and sel
-00011280: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
-00011290: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-000112a0: 2020 2072 6573 203d 2073 656c 662e 5f65     res = self._e
-000112b0: 7874 7261 2e73 7263 5f64 6174 612e 6765  xtra.src_data.ge
-000112c0: 745f 6261 7463 685f 6469 6d28 290a 2020  t_batch_dim().  
-000112d0: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-000112e0: 656c 662e 6261 7463 683a 0a20 2020 2020  elf.batch:.     
-000112f0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00011300: 2073 656c 662e 6261 7463 682e 6469 6d0a   self.batch.dim.
-00011310: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00011320: 7369 6e73 7461 6e63 6528 7265 732c 2069  sinstance(res, i
-00011330: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00011340: 2020 2020 2072 6574 7572 6e20 7265 730a       return res.
-00011350: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00011360: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011380: 7265 7475 726e 205f 742e 5465 6e73 6f72  return _t.Tensor
-00011390: 2822 6261 7463 6822 2c20 6469 6d73 3d28  ("batch", dims=(
-000113a0: 292c 2064 7479 7065 3d72 662e 6765 745f  ), dtype=rf.get_
-000113b0: 6465 6661 756c 745f 6172 7261 795f 696e  default_array_in
-000113c0: 6465 785f 6474 7970 6528 292c 2072 6177  dex_dtype(), raw
-000113d0: 5f74 656e 736f 723d 7265 7329 0a20 2020  _tensor=res).   
-000113e0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-000113f0: 2020 2020 2020 7365 6c66 2e5f 6578 7472        self._extr
-00011400: 610a 2020 2020 2020 2020 2020 2020 616e  a.            an
-00011410: 6420 7365 6c66 2e5f 6578 7472 612e 7372  d self._extra.sr
-00011420: 635f 6461 7461 2069 7320 6e6f 7420 4e6f  c_data is not No
-00011430: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
-00011440: 6e64 2073 656c 662e 5f65 7874 7261 2e73  nd self._extra.s
-00011450: 7263 5f61 7869 7320 6973 206e 6f74 204e  rc_axis is not N
-00011460: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00011470: 616e 6420 7365 6c66 2e5f 6578 7472 612e  and self._extra.
-00011480: 7372 635f 6461 7461 2e70 6c61 6365 686f  src_data.placeho
-00011490: 6c64 6572 2069 7320 6e6f 7420 4e6f 6e65  lder is not None
-000114a0: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-000114b0: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-000114c0: 6c66 2e5f 6578 7472 612e 7372 635f 6461  lf._extra.src_da
-000114d0: 7461 2e67 6574 5f64 696d 2873 656c 662e  ta.get_dim(self.
-000114e0: 5f65 7874 7261 2e73 7263 5f61 7869 7329  _extra.src_axis)
-000114f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011500: 6973 696e 7374 616e 6365 2872 6573 2c20  isinstance(res, 
-00011510: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00011520: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00011530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00011540: 7572 6e20 5f74 2e54 656e 736f 7228 2262  urn _t.Tensor("b
-00011550: 6174 6368 222c 2064 696d 733d 2829 2c20  atch", dims=(), 
-00011560: 6474 7970 653d 7266 2e67 6574 5f64 6566  dtype=rf.get_def
-00011570: 6175 6c74 5f61 7272 6179 5f69 6e64 6578  ault_array_index
-00011580: 5f64 7479 7065 2829 2c20 7261 775f 7465  _dtype(), raw_te
-00011590: 6e73 6f72 3d72 6573 290a 2020 2020 2020  nsor=res).      
-000115a0: 2020 7365 6c66 2e63 6f6d 706c 6574 655f    self.complete_
-000115b0: 6479 6e5f 7369 7a65 2829 0a20 2020 2020  dyn_size().     
-000115c0: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-000115d0: 697a 655f 6578 7420 616e 6420 7365 6c66  ize_ext and self
-000115e0: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
-000115f0: 6163 6568 6f6c 6465 7220 6973 206e 6f74  aceholder is not
-00011600: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00011610: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-00011620: 697a 655f 6578 742e 6261 7463 685f 6e64  ize_ext.batch_nd
-00011630: 696d 203e 2030 3a0a 2020 2020 2020 2020  im > 0:.        
-00011640: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00011650: 662e 7265 6475 6365 5f6d 6178 2873 656c  f.reduce_max(sel
-00011660: 662e 6479 6e5f 7369 7a65 5f65 7874 2c20  f.dyn_size_ext, 
-00011670: 6178 6973 3d73 656c 662e 6479 6e5f 7369  axis=self.dyn_si
-00011680: 7a65 5f65 7874 2e64 696d 5f74 6167 7329  ze_ext.dim_tags)
-00011690: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000116a0: 7572 6e20 7365 6c66 2e64 796e 5f73 697a  urn self.dyn_siz
-000116b0: 655f 6578 740a 2020 2020 2020 2020 7261  e_ext.        ra
-000116c0: 6973 6520 4578 6365 7074 696f 6e28 2225  ise Exception("%
-000116d0: 733a 206e 6565 6420 706c 6163 6568 6f6c  s: need placehol
-000116e0: 6465 722c 2073 656c 662e 6469 6d65 6e73  der, self.dimens
-000116f0: 696f 6e20 6f72 2073 656c 662e 6479 6e5f  ion or self.dyn_
-00011700: 7369 7a65 2066 6f72 2064 696d 2076 616c  size for dim val
-00011710: 7565 2220 2520 7365 6c66 290a 0a20 2020  ue" % self)..   
-00011720: 2064 6566 2061 7869 735f 7370 6c69 745f   def axis_split_
-00011730: 696e 666f 2873 656c 6629 3a0a 2020 2020  info(self):.    
-00011740: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011750: 3a72 6574 7572 6e3a 2061 7869 7320 7370  :return: axis sp
-00011760: 6c69 7420 696e 666f 2e20 7365 6520 3a66  lit info. see :f
-00011770: 756e 633a 6067 6574 5f70 6172 616d 5f61  unc:`get_param_a
-00011780: 7865 735f 7370 6c69 745f 696e 666f 6020  xes_split_info` 
-00011790: 616e 6420 7573 6167 6520 2865 2e67 2e20  and usage (e.g. 
-000117a0: 7072 6574 7261 696e 696e 6729 0a20 2020  pretraining).   
-000117b0: 2020 2020 203a 7274 7970 653a 206c 6973       :rtype: lis
-000117c0: 745b 696e 747c 4e6f 6e65 5d0a 2020 2020  t[int|None].    
-000117d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000117e0: 7361 6d65 5f62 6173 6520 3d20 7365 6c66  same_base = self
-000117f0: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
-00011800: 0a20 2020 2020 2020 206f 7020 3d20 7365  .        op = se
-00011810: 6c66 2e64 6572 6976 6564 5f66 726f 6d5f  lf.derived_from_
-00011820: 6f70 206f 7220 7361 6d65 5f62 6173 652e  op or same_base.
-00011830: 6465 7269 7665 645f 6672 6f6d 5f6f 700a  derived_from_op.
-00011840: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
-00011850: 703a 0a20 2020 2020 2020 2020 2020 2072  p:.            r
-00011860: 6574 7572 6e20 5b73 656c 662e 6469 6d65  eturn [self.dime
-00011870: 6e73 696f 6e5d 0a20 2020 2020 2020 2069  nsion].        i
-00011880: 6620 6f70 2e6b 696e 6420 3d3d 2022 6164  f op.kind == "ad
-00011890: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
-000118a0: 7265 7475 726e 2073 756d 285b 782e 6178  return sum([x.ax
-000118b0: 6973 5f73 706c 6974 5f69 6e66 6f28 2920  is_split_info() 
-000118c0: 666f 7220 7820 696e 206f 702e 696e 7075  for x in op.inpu
-000118d0: 7473 5d2c 205b 5d29 2020 2320 666c 6174  ts], [])  # flat
-000118e0: 7465 6e0a 2020 2020 2020 2020 6966 206f  ten.        if o
-000118f0: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
-00011900: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00011910: 203d 205b 315d 0a20 2020 2020 2020 2020   = [1].         
-00011920: 2020 2066 6f72 2078 2069 6e20 6f70 2e69     for x in op.i
-00011930: 6e70 7574 733a 0a20 2020 2020 2020 2020  nputs:.         
-00011940: 2020 2020 2020 2072 6573 203d 2073 756d         res = sum
-00011950: 285b 6e20 2a20 782e 6178 6973 5f73 706c  ([n * x.axis_spl
-00011960: 6974 5f69 6e66 6f28 2920 6966 206e 2069  it_info() if n i
-00011970: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00011980: 4e6f 6e65 2066 6f72 206e 2069 6e20 7265  None for n in re
-00011990: 735d 2c20 5b5d 2920 2023 2066 6c61 7474  s], [])  # flatt
-000119a0: 656e 0a20 2020 2020 2020 2020 2020 2072  en.            r
-000119b0: 6574 7572 6e20 7265 730a 2020 2020 2020  eturn res.      
-000119c0: 2020 7265 7475 726e 205b 7365 6c66 2e64    return [self.d
-000119d0: 696d 656e 7369 6f6e 5d0a 0a20 2020 2064  imension]..    d
-000119e0: 6566 205f 6765 745f 7361 6d65 5f62 6173  ef _get_same_bas
-000119f0: 655f 6578 7472 6128 7365 6c66 2920 2d3e  e_extra(self) ->
-00011a00: 204f 7074 696f 6e61 6c5b 5f44 696d 4578   Optional[_DimEx
-00011a10: 7472 615d 3a0a 2020 2020 2020 2020 6966  tra]:.        if
-00011a20: 206e 6f74 2073 656c 662e 5f65 7874 7261   not self._extra
-00011a30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00011a40: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00011a50: 2020 6261 7365 203d 2073 656c 662e 6765    base = self.ge
-00011a60: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-00011a70: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-00011a80: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-00011a90: 4d65 6d62 6572 0a20 2020 2020 2020 2072  Member.        r
-00011aa0: 6574 7572 6e20 6261 7365 2e5f 6578 7472  eturn base._extr
-00011ab0: 610a 0a20 2020 2064 6566 205f 6d61 6b65  a..    def _make
-00011ac0: 5f65 7874 7261 2873 656c 663a 205f 642e  _extra(self: _d.
-00011ad0: 4469 6d29 202d 3e20 5f44 696d 4578 7472  Dim) -> _DimExtr
-00011ae0: 613a 0a20 2020 2020 2020 2069 6620 6e6f  a:.        if no
-00011af0: 7420 7365 6c66 2e5f 6578 7472 613a 0a20  t self._extra:. 
-00011b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011b10: 5f65 7874 7261 203d 205f 4469 6d45 7874  _extra = _DimExt
-00011b20: 7261 2864 696d 3d73 656c 6629 0a20 2020  ra(dim=self).   
-00011b30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00011b40: 2e5f 6578 7472 610a 0a20 2020 2040 7072  ._extra..    @pr
-00011b50: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
-00011b60: 6f63 6162 2873 656c 6629 3a0a 2020 2020  ocab(self):.    
-00011b70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011b80: 3a72 7479 7065 3a20 7265 7475 726e 6e2e  :rtype: returnn.
-00011b90: 6461 7461 7365 7473 2e75 7469 6c2e 766f  datasets.util.vo
-00011ba0: 6361 6275 6c61 7279 2e56 6f63 6162 756c  cabulary.Vocabul
-00011bb0: 6172 797c 4e6f 6e65 0a20 2020 2020 2020  ary|None.       
-00011bc0: 2022 2222 0a20 2020 2020 2020 2065 7874   """.        ext
-00011bd0: 7261 203d 2073 656c 662e 5f67 6574 5f73  ra = self._get_s
-00011be0: 616d 655f 6261 7365 5f65 7874 7261 2829  ame_base_extra()
-00011bf0: 0a20 2020 2020 2020 2069 6620 6578 7472  .        if extr
-00011c00: 613a 0a20 2020 2020 2020 2020 2020 2072  a:.            r
-00011c10: 6574 7572 6e20 6578 7472 612e 766f 6361  eturn extra.voca
-00011c20: 620a 2020 2020 2020 2020 7265 7475 726e  b.        return
-00011c30: 204e 6f6e 650a 0a20 2020 2040 766f 6361   None..    @voca
-00011c40: 622e 7365 7474 6572 0a20 2020 2064 6566  b.setter.    def
-00011c50: 2076 6f63 6162 2873 656c 662c 2076 6f63   vocab(self, voc
-00011c60: 6162 293a 0a20 2020 2020 2020 2022 2222  ab):.        """
-00011c70: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00011c80: 7265 7475 726e 6e2e 6461 7461 7365 7473  returnn.datasets
-00011c90: 2e75 7469 6c2e 766f 6361 6275 6c61 7279  .util.vocabulary
-00011ca0: 2e56 6f63 6162 756c 6172 797c 4e6f 6e65  .Vocabulary|None
-00011cb0: 2076 6f63 6162 3a0a 2020 2020 2020 2020   vocab:.        
-00011cc0: 2222 220a 2020 2020 2020 2020 6966 2076  """.        if v
-00011cd0: 6f63 6162 2069 7320 7365 6c66 2e76 6f63  ocab is self.voc
-00011ce0: 6162 3a0a 2020 2020 2020 2020 2020 2020  ab:.            
-00011cf0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00011d00: 6620 7365 6c66 2e73 616d 655f 6173 3a0a  f self.same_as:.
-00011d10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011d20: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
-00011d30: 2e76 6f63 6162 203d 2076 6f63 6162 0a20  .vocab = vocab. 
-00011d40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00011d50: 6e0a 2020 2020 2020 2020 6578 7472 6120  n.        extra 
-00011d60: 3d20 7365 6c66 2e5f 6765 745f 7361 6d65  = self._get_same
-00011d70: 5f62 6173 655f 6578 7472 6128 290a 2020  _base_extra().  
-00011d80: 2020 2020 2020 6966 2065 7874 7261 3a0a        if extra:.
-00011d90: 2020 2020 2020 2020 2020 2020 6578 7472              extr
-00011da0: 612e 766f 6361 6220 3d20 766f 6361 620a  a.vocab = vocab.
-00011db0: 0a20 2020 2023 2054 6865 206b 696e 6420  .    # The kind 
-00011dc0: 6f66 206f 7065 7261 7469 6f6e 7320 7765  of operations we
-00011dd0: 2068 6176 653a 0a20 2020 2023 2061 202b   have:.    # a +
-00011de0: 2062 3a20 7061 6464 696e 672c 2063 6f6e   b: padding, con
-00011df0: 6361 740a 2020 2020 2320 6120 2d20 623a  cat.    # a - b:
-00011e00: 2077 696e 646f 7720 7769 7468 2076 616c   window with val
-00011e10: 6964 2066 7261 6d65 7320 6f6e 6c79 0a20  id frames only. 
-00011e20: 2020 2023 2061 202a 2062 3a20 6d65 7267     # a * b: merg
-00011e30: 6520 6469 6d73 2c20 7570 7361 6d70 6c65  e dims, upsample
-00011e40: 2c20 7472 616e 7370 6f73 6564 2063 6f6e  , transposed con
-00011e50: 7620 7769 7468 2073 7472 6964 696e 670a  v with striding.
-00011e60: 2020 2020 2320 6120 2f20 6220 2877 6865      # a / b (whe
-00011e70: 6e20 6120 2520 6220 3d3d 2030 293a 2073  n a % b == 0): s
-00011e80: 706c 6974 2064 696d 732c 2064 6f77 6e73  plit dims, downs
-00011e90: 616d 706c 652c 2063 6f6e 7620 7769 7468  ample, conv with
-00011ea0: 2073 7472 6964 696e 670a 2020 2020 2320   striding.    # 
-00011eb0: 6365 696c 6469 7628 612c 2062 293a 2063  ceildiv(a, b): c
-00011ec0: 6f6e 7620 7769 7468 2073 7472 6964 696e  onv with stridin
-00011ed0: 670a 2020 2020 2320 6375 7374 6f6d 3a20  g.    # custom: 
-00011ee0: 7265 7065 6174 2c20 7265 6d6f 7665 2c20  repeat, remove, 
-00011ef0: 6d61 736b 2c20 6c6f 6f70 2077 6974 6820  mask, loop with 
-00011f00: 6479 6e20 656e 640a 2020 2020 2320 4e6f  dyn end.    # No
-00011f10: 7465 2074 6861 7420 7765 2064 6966 6665  te that we diffe
-00011f20: 7265 6e74 6961 7465 2062 6574 7765 656e  rentiate between
-00011f30: 2074 6865 206f 7264 6572 2c20 692e 652e   the order, i.e.
-00011f40: 2061 202b 2062 2021 3d20 6220 2b20 612e   a + b != b + a.
-00011f50: 0a20 2020 2023 204e 6f74 6520 7468 6174  .    # Note that
-00011f60: 2077 6520 616c 7761 7973 2068 6176 6520   we always have 
-00011f70: 7468 6520 6173 7375 6d70 7469 6f6e 2074  the assumption t
-00011f80: 6861 7420 6120 6469 6d65 6e73 696f 6e20  hat a dimension 
-00011f90: 6973 206e 6f6e 2d6e 6567 6174 6976 652e  is non-negative.
-00011fa0: 0a20 2020 2023 2054 6869 7320 6173 7375  .    # This assu
-00011fb0: 6d70 7469 6f6e 2069 7320 6e65 6365 7373  mption is necess
-00011fc0: 6172 7920 666f 7220 736f 6d65 2073 696d  ary for some sim
-00011fd0: 706c 6966 6963 6174 696f 6e73 2e0a 2020  plifications..  
-00011fe0: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
-00011ff0: 7562 2e63 6f6d 2f72 7774 682d 6936 2f72  ub.com/rwth-i6/r
-00012000: 6574 7572 6e6e 2f70 756c 6c2f 3835 330a  eturnn/pull/853.
-00012010: 0a20 2020 2064 6566 205f 5f61 6464 5f5f  .    def __add__
-00012020: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
-00012030: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
-00012040: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00012050: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
-00012060: 2020 2020 2020 3a72 6574 7572 6e3a 2073        :return: s
-00012070: 656c 6620 2b20 6f74 6865 722e 206e 6f74  elf + other. not
-00012080: 6520 7468 6174 2074 6869 7320 6973 206e  e that this is n
-00012090: 6f74 2063 6f6d 6d75 7461 7469 7665 2c20  ot commutative, 
-000120a0: 692e 652e 2064 6966 6665 7265 6e74 2066  i.e. different f
-000120b0: 726f 6d20 6f74 6865 7220 2b20 7365 6c66  rom other + self
-000120c0: 2e0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-000120d0: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
-000120e0: 220a 2020 2020 2020 2020 7465 726d 203d  ".        term =
-000120f0: 205f 4f70 4c69 6e65 6172 5465 726d 2e66   _OpLinearTerm.f
-00012100: 726f 6d5f 6469 6d28 7365 6c66 290a 2020  rom_dim(self).  
-00012110: 2020 2020 2020 7465 726d 2e65 7874 656e        term.exten
-00012120: 645f 6164 645f 7375 625f 286f 7468 6572  d_add_sub_(other
-00012130: 2c20 6b69 6e64 3d22 6164 6422 2c20 7269  , kind="add", ri
-00012140: 6768 743d 5472 7565 290a 2020 2020 2020  ght=True).      
-00012150: 2020 7265 7475 726e 2074 6572 6d2e 6173    return term.as
-00012160: 5f64 696d 2829 0a0a 2020 2020 6465 6620  _dim()..    def 
-00012170: 5f5f 7261 6464 5f5f 2873 656c 663a 2044  __radd__(self: D
-00012180: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
-00012190: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000121a0: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
-000121b0: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
-000121c0: 6574 7572 6e3a 206f 7468 6572 202b 2073  eturn: other + s
-000121d0: 656c 660a 2020 2020 2020 2020 3a72 7479  elf.        :rty
-000121e0: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
-000121f0: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
-00012200: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
-00012210: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
-00012220: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
-00012230: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
-00012240: 6572 2c20 6b69 6e64 3d22 6164 6422 2c20  er, kind="add", 
-00012250: 7269 6768 743d 4661 6c73 6529 0a20 2020  right=False).   
-00012260: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012270: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012280: 6566 205f 5f73 7562 5f5f 2873 656c 662c  ef __sub__(self,
-00012290: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-000122a0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-000122b0: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-000122c0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-000122d0: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-000122e0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-000122f0: 6e20 7365 6c66 2e73 7562 5f72 6967 6874  n self.sub_right
-00012300: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
-00012310: 2073 7562 5f72 6967 6874 2873 656c 663a   sub_right(self:
-00012320: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
-00012330: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012340: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
-00012350: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-00012360: 3a72 6574 7572 6e3a 2073 656c 6620 2d20  :return: self - 
-00012370: 6f74 6865 720a 2020 2020 2020 2020 3a72  other.        :r
-00012380: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
-00012390: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
-000123a0: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
-000123b0: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
-000123c0: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
-000123d0: 7874 656e 645f 6164 645f 7375 625f 286f  xtend_add_sub_(o
-000123e0: 7468 6572 2c20 6b69 6e64 3d22 7375 6222  ther, kind="sub"
-000123f0: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
-00012400: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00012410: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-00012420: 6465 6620 7375 625f 6c65 6674 2873 656c  def sub_left(sel
-00012430: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
-00012440: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012450: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
-00012460: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
-00012470: 2020 3a72 6574 7572 6e3a 2028 2d6f 7468    :return: (-oth
-00012480: 6572 2920 2b20 7365 6c66 0a20 2020 2020  er) + self.     
-00012490: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-000124a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000124b0: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-000124c0: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-000124d0: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-000124e0: 6572 6d2e 6578 7465 6e64 5f61 6464 5f73  erm.extend_add_s
-000124f0: 7562 5f28 6f74 6865 722c 206b 696e 643d  ub_(other, kind=
-00012500: 2273 7562 222c 2072 6967 6874 3d46 616c  "sub", right=Fal
-00012510: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
-00012520: 726e 2074 6572 6d2e 6173 5f64 696d 2829  rn term.as_dim()
-00012530: 0a0a 2020 2020 6465 6620 5f5f 6d75 6c5f  ..    def __mul_
-00012540: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
-00012550: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
-00012560: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00012570: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-00012580: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00012590: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-000125a0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-000125b0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-000125c0: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-000125d0: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
-000125e0: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
-000125f0: 696e 643d 226d 756c 222c 2072 6967 6874  ind="mul", right
-00012600: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
-00012610: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
-00012620: 6d28 290a 0a20 2020 2064 6566 205f 5f72  m()..    def __r
-00012630: 6d75 6c5f 5f28 7365 6c66 3a20 4469 6d2c  mul__(self: Dim,
-00012640: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00012650: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012660: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00012670: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-00012680: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00012690: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
-000126a0: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
-000126b0: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
-000126c0: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
-000126d0: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
-000126e0: 722c 206b 696e 643d 226d 756c 222c 2072  r, kind="mul", r
-000126f0: 6967 6874 3d46 616c 7365 290a 2020 2020  ight=False).    
-00012700: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
-00012710: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
-00012720: 6620 5f5f 666c 6f6f 7264 6976 5f5f 2873  f __floordiv__(s
-00012730: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
-00012740: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012750: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00012760: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-00012770: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00012780: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012790: 2020 2020 7465 726d 203d 205f 4f70 4c69      term = _OpLi
-000127a0: 6e65 6172 5465 726d 2e66 726f 6d5f 6469  nearTerm.from_di
-000127b0: 6d28 7365 6c66 290a 2020 2020 2020 2020  m(self).        
-000127c0: 7465 726d 2e65 7874 656e 645f 6d75 6c5f  term.extend_mul_
-000127d0: 6469 765f 286f 7468 6572 2c20 6b69 6e64  div_(other, kind
-000127e0: 3d22 666c 6f6f 7264 6976 222c 2072 6967  ="floordiv", rig
-000127f0: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
-00012800: 2072 6574 7572 6e20 7465 726d 2e61 735f   return term.as_
-00012810: 6469 6d28 290a 0a20 2020 2064 6566 205f  dim()..    def _
-00012820: 5f74 7275 6564 6976 5f5f 2873 656c 662c  _truediv__(self,
-00012830: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00012840: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012850: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00012860: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-00012870: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00012880: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00012890: 6e20 7365 6c66 2e64 6976 5f72 6967 6874  n self.div_right
-000128a0: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
-000128b0: 2064 6976 5f6c 6566 7428 7365 6c66 3a20   div_left(self: 
-000128c0: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
-000128d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000128e0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-000128f0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012900: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012910: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00012920: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
-00012930: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
-00012940: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
-00012950: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
-00012960: 6f74 6865 722c 206b 696e 643d 2274 7275  other, kind="tru
-00012970: 6564 6976 222c 2072 6967 6874 3d46 616c  ediv", right=Fal
-00012980: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
-00012990: 726e 2074 6572 6d2e 6173 5f64 696d 2829  rn term.as_dim()
-000129a0: 0a0a 2020 2020 6465 6620 6469 765f 7269  ..    def div_ri
-000129b0: 6768 7428 7365 6c66 3a20 4469 6d2c 206f  ght(self: Dim, o
-000129c0: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
-000129d0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-000129e0: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
-000129f0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00012a00: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-00012a10: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
-00012a20: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
-00012a30: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
-00012a40: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
-00012a50: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
-00012a60: 206b 696e 643d 2274 7275 6564 6976 222c   kind="truediv",
-00012a70: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
-00012a80: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012a90: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012aa0: 6566 2063 6569 6c64 6976 5f6c 6566 7428  ef ceildiv_left(
-00012ab0: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
-00012ac0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00012ad0: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
-00012ae0: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
-00012af0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00012b00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012b10: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
-00012b20: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
-00012b30: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
-00012b40: 2074 6572 6d2e 6578 7465 6e64 5f6d 756c   term.extend_mul
-00012b50: 5f64 6976 5f28 6f74 6865 722c 206b 696e  _div_(other, kin
-00012b60: 643d 2263 6569 6c64 6976 222c 2072 6967  d="ceildiv", rig
-00012b70: 6874 3d46 616c 7365 290a 2020 2020 2020  ht=False).      
-00012b80: 2020 7265 7475 726e 2074 6572 6d2e 6173    return term.as
-00012b90: 5f64 696d 2829 0a0a 2020 2020 6465 6620  _dim()..    def 
-00012ba0: 6365 696c 6469 765f 7269 6768 7428 7365  ceildiv_right(se
-00012bb0: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
-00012bc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012bd0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00012be0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00012bf0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00012c00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012c10: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-00012c20: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-00012c30: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-00012c40: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
-00012c50: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
-00012c60: 2263 6569 6c64 6976 222c 2072 6967 6874  "ceildiv", right
-00012c70: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
-00012c80: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
-00012c90: 6d28 290a 0a20 2020 2064 6566 205f 5f6e  m()..    def __n
-00012ca0: 6567 5f5f 2873 656c 6629 3a0a 2020 2020  eg__(self):.    
-00012cb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012cc0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-00012cd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012ce0: 7265 7475 726e 202d 3120 2a20 7365 6c66  return -1 * self
-00012cf0: 0a0a 2020 2020 6465 6620 6973 5f63 6f6e  ..    def is_con
-00012d00: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-00012d10: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00012d20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012d30: 2020 2020 3a72 6574 7572 6e3a 2064 6572      :return: der
-00012d40: 6976 6564 206f 7020 6f66 2074 7970 6520  ived op of type 
-00012d50: 636f 6e73 7461 6e74 0a20 2020 2020 2020  constant.       
-00012d60: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00012d70: 7572 6e20 7365 6c66 2e64 6572 6976 6564  urn self.derived
-00012d80: 5f66 726f 6d5f 6f70 2061 6e64 2073 656c  _from_op and sel
-00012d90: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
-00012da0: 702e 6b69 6e64 203d 3d20 2263 6f6e 7374  p.kind == "const
-00012db0: 616e 7422 0a0a 0a64 6566 205f 6d61 6b65  ant"...def _make
-00012dc0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00012dd0: 5f64 696d 2876 616c 7565 2c20 6b69 6e64  _dim(value, kind
-00012de0: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
-00012df0: 2020 2020 3a70 6172 616d 2069 6e74 2076      :param int v
-00012e00: 616c 7565 3a0a 2020 2020 3a70 6172 616d  alue:.    :param
-00012e10: 2045 6e74 6974 797c 4e6f 6e65 206b 696e   Entity|None kin
-00012e20: 643a 0a20 2020 203a 7274 7970 653a 2044  d:.    :rtype: D
-00012e30: 696d 0a20 2020 2022 2222 0a20 2020 2072  im.    """.    r
-00012e40: 6574 7572 6e20 5f64 2e44 696d 280a 2020  eturn _d.Dim(.  
-00012e50: 2020 2020 2020 6469 6d65 6e73 696f 6e3d        dimension=
-00012e60: 7661 6c75 652c 0a20 2020 2020 2020 206b  value,.        k
-00012e70: 696e 643d 6b69 6e64 206f 7220 4469 6d54  ind=kind or DimT
-00012e80: 7970 6573 2e55 6e73 7065 6369 6669 6564  ypes.Unspecified
-00012e90: 2c0a 2020 2020 2020 2020 6465 7363 7269  ,.        descri
-00012ea0: 7074 696f 6e3d 2275 6e6e 616d 6564 5f25  ption="unnamed_%
-00012eb0: 7364 696d 5f25 6922 2025 2028 6b69 6e64  sdim_%i" % (kind
-00012ec0: 2e6e 616d 6520 2b20 225f 2220 6966 206b  .name + "_" if k
-00012ed0: 696e 6420 656c 7365 2022 222c 2076 616c  ind else "", val
-00012ee0: 7565 292c 0a20 2020 2020 2020 2064 6572  ue),.        der
-00012ef0: 6976 6564 5f66 726f 6d5f 6f70 3d4f 7028  ived_from_op=Op(
-00012f00: 6b69 6e64 3d22 636f 6e73 7461 6e74 222c  kind="constant",
-00012f10: 2069 6e70 7574 733d 5b5d 2c20 6174 7472   inputs=[], attr
-00012f20: 6962 733d 7b22 7661 6c75 6522 3a20 7661  ibs={"value": va
-00012f30: 6c75 657d 292c 0a20 2020 2020 2020 2061  lue}),.        a
-00012f40: 7574 6f5f 6765 6e65 7261 7465 643d 5472  uto_generated=Tr
-00012f50: 7565 2c0a 2020 2020 290a 0a0a 636c 6173  ue,.    )...clas
-00012f60: 7320 4f70 3a0a 2020 2020 2222 220a 2020  s Op:.    """.  
-00012f70: 2020 4f70 206f 6e20 3a63 6c61 7373 3a60    Op on :class:`
-00012f80: 4469 6d60 2077 6869 6368 2072 6573 756c  Dim` which resul
-00012f90: 7473 2069 6e20 6120 6465 7269 7665 6420  ts in a derived 
-00012fa0: 3a63 6c61 7373 3a60 4469 6d60 2e0a 2020  :class:`Dim`..  
-00012fb0: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-00012fc0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6b69  _init__(self, ki
-00012fd0: 6e64 2c20 696e 7075 7473 2c20 6174 7472  nd, inputs, attr
-00012fe0: 6962 733d 4e6f 6e65 293a 0a20 2020 2020  ibs=None):.     
-00012ff0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00013000: 7061 7261 6d20 7374 7220 6b69 6e64 3a20  param str kind: 
-00013010: 2261 6464 222c 2022 7375 6222 2c20 226d  "add", "sub", "m
-00013020: 756c 222c 2022 6365 696c 6469 7622 0a20  ul", "ceildiv". 
-00013030: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
-00013040: 7374 5b44 696d 5d20 696e 7075 7473 3a0a  st[Dim] inputs:.
-00013050: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00013060: 6963 745b 7374 725d 7c4e 6f6e 6520 6174  ict[str]|None at
-00013070: 7472 6962 733a 0a20 2020 2020 2020 2022  tribs:.        "
-00013080: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00013090: 6b69 6e64 203d 206b 696e 640a 2020 2020  kind = kind.    
-000130a0: 2020 2020 7365 6c66 2e69 6e70 7574 7320      self.inputs 
-000130b0: 3d20 696e 7075 7473 0a20 2020 2020 2020  = inputs.       
-000130c0: 2073 656c 662e 6f75 7470 7574 203d 204e   self.output = N
-000130d0: 6f6e 6520 2023 2074 7970 653a 204f 7074  one  # type: Opt
-000130e0: 696f 6e61 6c5b 5f64 2e44 696d 5d0a 2020  ional[_d.Dim].  
-000130f0: 2020 2020 2020 7365 6c66 2e61 7474 7269        self.attri
-00013100: 6273 203d 2061 7474 7269 6273 0a0a 2020  bs = attribs..  
-00013110: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-00013120: 656c 6629 3a0a 2020 2020 2020 2020 6174  elf):.        at
-00013130: 7472 6962 7320 3d20 2822 2025 7222 2025  tribs = (" %r" %
-00013140: 2073 656c 662e 6174 7472 6962 7329 2069   self.attribs) i
-00013150: 6620 7365 6c66 2e61 7474 7269 6273 2065  f self.attribs e
-00013160: 6c73 6520 2222 0a20 2020 2020 2020 2072  lse "".        r
-00013170: 6574 7572 6e20 223c 4469 6d2e 4f70 2025  eturn "<Dim.Op %
-00013180: 7220 2573 2573 3e22 2025 2028 7365 6c66  r %s%s>" % (self
-00013190: 2e6b 696e 642c 2073 656c 662e 696e 7075  .kind, self.inpu
-000131a0: 7473 2c20 6174 7472 6962 7329 0a0a 2020  ts, attribs)..  
-000131b0: 2020 6465 6620 5f76 616c 7565 2873 656c    def _value(sel
-000131c0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-000131d0: 726e 2073 656c 662e 6b69 6e64 2c20 7475  rn self.kind, tu
-000131e0: 706c 6528 7365 6c66 2e69 6e70 7574 7329  ple(self.inputs)
-000131f0: 2c20 6672 6f7a 656e 7365 7428 7365 6c66  , frozenset(self
-00013200: 2e61 7474 7269 6273 2e69 7465 6d73 2829  .attribs.items()
-00013210: 2920 6966 2073 656c 662e 6174 7472 6962  ) if self.attrib
-00013220: 7320 656c 7365 204e 6f6e 650a 0a20 2020  s else None..   
-00013230: 2064 6566 205f 5f68 6173 685f 5f28 7365   def __hash__(se
-00013240: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00013250: 7572 6e20 6861 7368 2873 656c 662e 5f76  urn hash(self._v
-00013260: 616c 7565 2829 290a 0a20 2020 2064 6566  alue())..    def
-00013270: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
-00013280: 6865 7229 3a0a 2020 2020 2020 2020 6966  her):.        if
-00013290: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-000132a0: 722c 204f 7029 3a0a 2020 2020 2020 2020  r, Op):.        
-000132b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000132c0: 5f76 616c 7565 2829 203d 3d20 6f74 6865  _value() == othe
-000132d0: 722e 5f76 616c 7565 2829 0a20 2020 2020  r._value().     
-000132e0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000132f0: 0a20 2020 2064 6566 205f 5f6e 655f 5f28  .    def __ne__(
-00013300: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-00013310: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
-00013320: 2073 656c 662e 5f5f 6571 5f5f 286f 7468   self.__eq__(oth
-00013330: 6572 290a 0a0a 6465 6620 5f67 6574 5f64  er)...def _get_d
-00013340: 6573 6372 6970 7469 6f6e 2864 696d 2c20  escription(dim, 
-00013350: 6272 6163 6b65 7473 3d54 7275 6529 3a0a  brackets=True):.
-00013360: 2020 2020 2222 220a 2020 2020 3a70 6172      """.    :par
-00013370: 616d 2044 696d 2064 696d 3a0a 2020 2020  am Dim dim:.    
-00013380: 3a70 6172 616d 2062 6f6f 6c20 6272 6163  :param bool brac
-00013390: 6b65 7473 3a20 6164 6420 6272 6163 6b65  kets: add bracke
-000133a0: 7473 2077 6865 6e20 6e65 6365 7373 6172  ts when necessar
-000133b0: 790a 2020 2020 3a72 7479 7065 3a20 7374  y.    :rtype: st
-000133c0: 720a 2020 2020 2222 220a 2020 2020 6966  r.    """.    if
-000133d0: 2064 696d 2e64 6573 6372 6970 7469 6f6e   dim.description
-000133e0: 2061 6e64 2064 696d 2e64 6573 6372 6970   and dim.descrip
-000133f0: 7469 6f6e 2e73 7461 7274 7377 6974 6828  tion.startswith(
-00013400: 2275 6e6e 616d 6564 5f22 2920 616e 6420  "unnamed_") and 
-00013410: 6469 6d2e 6469 6d65 6e73 696f 6e20 6973  dim.dimension is
-00013420: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00013430: 2020 2072 6574 7572 6e20 7374 7228 6469     return str(di
-00013440: 6d2e 6469 6d65 6e73 696f 6e29 0a20 2020  m.dimension).   
-00013450: 2069 6620 6469 6d2e 6465 7363 7269 7074   if dim.descript
-00013460: 696f 6e3a 0a20 2020 2020 2020 2069 6620  ion:.        if 
-00013470: 6272 6163 6b65 7473 3a0a 2020 2020 2020  brackets:.      
-00013480: 2020 2020 2020 696d 706f 7274 2072 650a        import re.
-00013490: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000134a0: 7265 2e73 6561 7263 6828 225b 2b5c 5c2d  re.search("[+\\-
-000134b0: 2f20 5d22 2c20 6469 6d2e 6465 7363 7269  / ]", dim.descri
-000134c0: 7074 696f 6e29 3a0a 2020 2020 2020 2020  ption):.        
-000134d0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-000134e0: 2825 7329 2220 2520 6469 6d2e 6465 7363  (%s)" % dim.desc
-000134f0: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-00013500: 7265 7475 726e 2064 696d 2e64 6573 6372  return dim.descr
-00013510: 6970 7469 6f6e 0a20 2020 2072 6574 7572  iption.    retur
-00013520: 6e20 2275 6e6e 616d 6564 5f25 735f 6469  n "unnamed_%s_di
-00013530: 6d25 7322 2025 2028 6469 6d2e 6b69 6e64  m%s" % (dim.kind
-00013540: 2c20 6469 6d2e 6469 6d65 6e73 696f 6e20  , dim.dimension 
-00013550: 6966 2064 696d 2e64 696d 656e 7369 6f6e  if dim.dimension
-00013560: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00013570: 6520 223f 2229 0a0a 0a63 6c61 7373 205f  e "?")...class _
-00013580: 4f70 4d75 6c74 5465 726d 3a0a 2020 2020  OpMultTerm:.    
-00013590: 2222 220a 2020 2020 7265 7072 6573 656e  """.    represen
-000135a0: 7473 2073 7468 206c 696b 6520 6120 2a20  ts sth like a * 
-000135b0: 6220 2a20 630a 2020 2020 2222 220a 0a20  b * c.    """.. 
-000135c0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-000135d0: 2020 2020 6465 6620 6672 6f6d 5f64 696d      def from_dim
-000135e0: 2863 6c73 2c20 6469 6d3a 205f 642e 4469  (cls, dim: _d.Di
-000135f0: 6d29 202d 3e20 5f4f 704d 756c 7454 6572  m) -> _OpMultTer
-00013600: 6d3a 0a20 2020 2020 2020 2022 2222 0a20  m:.        """. 
-00013610: 2020 2020 2020 203a 7061 7261 6d20 6469         :param di
-00013620: 6d3a 0a20 2020 2020 2020 203a 7265 7475  m:.        :retu
-00013630: 726e 3a20 6f70 206d 756c 7420 7465 726d  rn: op mult term
-00013640: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013650: 2020 2020 2064 696d 203d 2064 696d 2e67       dim = dim.g
-00013660: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-00013670: 2020 2020 2020 2069 6620 6469 6d2e 6469         if dim.di
-00013680: 6d65 6e73 696f 6e20 3d3d 2031 2061 6e64  mension == 1 and
-00013690: 2064 696d 2e69 735f 636f 6e73 7461 6e74   dim.is_constant
-000136a0: 5f73 7461 7469 635f 6469 6d28 293a 0a20  _static_dim():. 
-000136b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000136c0: 6e20 636c 732e 6f6e 6528 290a 2020 2020  n cls.one().    
-000136d0: 2020 2020 6966 2064 696d 2e64 6572 6976      if dim.deriv
-000136e0: 6564 5f66 726f 6d5f 6f70 2061 6e64 2064  ed_from_op and d
-000136f0: 696d 2e64 6572 6976 6564 5f66 726f 6d5f  im.derived_from_
-00013700: 6f70 2e6b 696e 6420 3d3d 2022 6d75 6c22  op.kind == "mul"
-00013710: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00013720: 7475 726e 2063 6c73 286c 6973 7428 6469  turn cls(list(di
-00013730: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
-00013740: 702e 696e 7075 7473 2929 0a20 2020 2020  p.inputs)).     
-00013750: 2020 2072 6574 7572 6e20 636c 7328 5b64     return cls([d
-00013760: 696d 5d29 0a0a 2020 2020 4063 6c61 7373  im])..    @class
-00013770: 6d65 7468 6f64 0a20 2020 2064 6566 2066  method.    def f
-00013780: 726f 6d5f 6469 6d5f 6661 6374 6f72 7328  rom_dim_factors(
-00013790: 636c 732c 2064 696d 7329 3a0a 2020 2020  cls, dims):.    
-000137a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000137b0: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
-000137c0: 2064 696d 733a 0a20 2020 2020 2020 203a   dims:.        :
-000137d0: 7274 7970 653a 2044 696d 2e5f 4f70 4d75  rtype: Dim._OpMu
-000137e0: 6c74 5465 726d 0a20 2020 2020 2020 2022  ltTerm.        "
-000137f0: 2222 0a20 2020 2020 2020 2072 6573 203d  "".        res =
-00013800: 2063 6c73 2e6f 6e65 2829 0a20 2020 2020   cls.one().     
-00013810: 2020 2066 6f72 2064 2069 6e20 6469 6d73     for d in dims
-00013820: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00013830: 732e 6578 7465 6e64 5f6d 756c 5f64 6976  s.extend_mul_div
-00013840: 5f28 642c 206b 696e 643d 226d 756c 222c  _(d, kind="mul",
-00013850: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
-00013860: 2020 2020 2072 6574 7572 6e20 7265 730a       return res.
-00013870: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00013880: 640a 2020 2020 6465 6620 6f6e 6528 636c  d.    def one(cl
-00013890: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
-000138a0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000138b0: 4469 6d2e 5f4f 704d 756c 7454 6572 6d0a  Dim._OpMultTerm.
-000138c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000138d0: 2020 2020 7265 7475 726e 2063 6c73 285b      return cls([
-000138e0: 5d29 0a0a 2020 2020 6465 6620 5f5f 696e  ])..    def __in
-000138f0: 6974 5f5f 2873 656c 662c 2074 6572 6d73  it__(self, terms
-00013900: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00013910: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
-00013920: 7374 5b44 696d 5d20 7465 726d 733a 0a20  st[Dim] terms:. 
-00013930: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013940: 2020 2073 656c 662e 7465 726d 7320 3d20     self.terms = 
-00013950: 7465 726d 730a 0a20 2020 2064 6566 205f  terms..    def _
-00013960: 5f68 6173 685f 5f28 7365 6c66 293a 0a20  _hash__(self):. 
-00013970: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
-00013980: 7368 2874 7570 6c65 2873 656c 662e 7465  sh(tuple(self.te
-00013990: 726d 7329 290a 0a20 2020 2064 6566 205f  rms))..    def _
-000139a0: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
-000139b0: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
-000139c0: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-000139d0: 696d 7c44 696d 2e5f 4f70 4d75 6c74 5465  im|Dim._OpMultTe
-000139e0: 726d 206f 7468 6572 3a0a 2020 2020 2020  rm other:.      
-000139f0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00013a00: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-00013a10: 722c 205f 4f70 4d75 6c74 5465 726d 293a  r, _OpMultTerm):
-00013a20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00013a30: 7572 6e20 7365 6c66 2e74 6572 6d73 203d  urn self.terms =
-00013a40: 3d20 6f74 6865 722e 7465 726d 730a 2020  = other.terms.  
-00013a50: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00013a60: 7365 0a0a 2020 2020 6465 6620 5f5f 6e65  se..    def __ne
-00013a70: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-00013a80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013a90: 6e6f 7420 7365 6c66 2e5f 5f65 715f 5f28  not self.__eq__(
-00013aa0: 6f74 6865 7229 0a0a 2020 2020 6465 6620  other)..    def 
-00013ab0: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
-00013ac0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00013ad0: 4469 6d2e 5f4f 704d 756c 7454 6572 6d28  Dim._OpMultTerm(
-00013ae0: 2572 2922 2025 2028 7365 6c66 2e74 6572  %r)" % (self.ter
-00013af0: 6d73 2c29 0a0a 2020 2020 4070 726f 7065  ms,)..    @prope
-00013b00: 7274 790a 2020 2020 6465 6620 6469 6d65  rty.    def dime
-00013b10: 6e73 696f 6e28 7365 6c66 293a 0a20 2020  nsion(self):.   
-00013b20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013b30: 203a 7274 7970 653a 2069 6e74 7c4e 6f6e   :rtype: int|Non
-00013b40: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00013b50: 2020 2020 2020 6469 6d20 3d20 310a 2020        dim = 1.  
-00013b60: 2020 2020 2020 666f 7220 7061 7274 2069        for part i
-00013b70: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
-00013b80: 2020 2020 2020 2020 2020 6966 2070 6172            if par
-00013b90: 742e 6469 6d65 6e73 696f 6e20 6973 204e  t.dimension is N
-00013ba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00013bb0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00013bc0: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
-00013bd0: 202a 3d20 7061 7274 2e64 696d 656e 7369   *= part.dimensi
-00013be0: 6f6e 0a20 2020 2020 2020 2072 6574 7572  on.        retur
-00013bf0: 6e20 6469 6d0a 0a20 2020 2064 6566 2062  n dim..    def b
-00013c00: 6173 655f 7465 726d 2873 656c 6629 3a0a  ase_term(self):.
-00013c10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013c20: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00013c30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013c40: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00013c50: 7465 726d 730a 2020 2020 2020 2020 7265  terms.        re
-00013c60: 7475 726e 2073 656c 662e 7465 726d 735b  turn self.terms[
-00013c70: 2d31 5d0a 0a20 2020 2064 6566 2069 735f  -1]..    def is_
-00013c80: 6f6e 6528 7365 6c66 293a 0a20 2020 2020  one(self):.     
-00013c90: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00013ca0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-00013cb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013cc0: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
-00013cd0: 7465 726d 730a 0a20 2020 2064 6566 2069  terms..    def i
-00013ce0: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
-00013cf0: 635f 6469 6d28 7365 6c66 293a 0a20 2020  c_dim(self):.   
-00013d00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013d10: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00013d20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013d30: 2020 6966 206e 6f74 2073 656c 662e 7465    if not self.te
-00013d40: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
-00013d50: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00013d60: 2020 2020 2072 6574 7572 6e20 616c 6c28       return all(
-00013d70: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
-00013d80: 5f73 7461 7469 635f 6469 6d28 2920 666f  _static_dim() fo
-00013d90: 7220 7465 726d 2069 6e20 7365 6c66 2e74  r term in self.t
-00013da0: 6572 6d73 290a 0a20 2020 2064 6566 2063  erms)..    def c
-00013db0: 6f70 7928 7365 6c66 293a 0a20 2020 2020  opy(self):.     
-00013dc0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00013dd0: 7274 7970 653a 2044 696d 2e5f 4f70 4d75  rtype: Dim._OpMu
-00013de0: 6c74 5465 726d 0a20 2020 2020 2020 2022  ltTerm.        "
-00013df0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00013e00: 6e20 5f4f 704d 756c 7454 6572 6d28 6c69  n _OpMultTerm(li
-00013e10: 7374 2873 656c 662e 7465 726d 7329 290a  st(self.terms)).
-00013e20: 0a20 2020 2064 6566 206e 6567 6174 6976  .    def negativ
-00013e30: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00013e40: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
-00013e50: 7970 653a 2044 696d 2e5f 4f70 4d75 6c74  ype: Dim._OpMult
-00013e60: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
-00013e70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00013e80: 2e74 6572 6d73 2061 6e64 2073 656c 662e  .terms and self.
-00013e90: 7465 726d 735b 305d 2e69 735f 636f 6e73  terms[0].is_cons
-00013ea0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00013eb0: 2920 616e 6420 7365 6c66 2e74 6572 6d73  ) and self.terms
-00013ec0: 5b30 5d2e 6469 6d65 6e73 696f 6e20 3d3d  [0].dimension ==
-00013ed0: 202d 313a 0a20 2020 2020 2020 2020 2020   -1:.           
-00013ee0: 2072 6574 7572 6e20 5f4f 704d 756c 7454   return _OpMultT
-00013ef0: 6572 6d28 7365 6c66 2e74 6572 6d73 5b31  erm(self.terms[1
-00013f00: 3a5d 290a 2020 2020 2020 2020 7265 7320  :]).        res 
-00013f10: 3d20 7365 6c66 2e63 6f70 7928 290a 2020  = self.copy().  
-00013f20: 2020 2020 2020 7265 732e 6578 7465 6e64        res.extend
-00013f30: 5f6d 756c 5f64 6976 5f28 5f6d 616b 655f  _mul_div_(_make_
-00013f40: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-00013f50: 6469 6d28 2d31 292c 206b 696e 643d 226d  dim(-1), kind="m
-00013f60: 756c 222c 2072 6967 6874 3d46 616c 7365  ul", right=False
-00013f70: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00013f80: 2072 6573 0a0a 2020 2020 6465 6620 6469   res..    def di
-00013f90: 7669 7369 626c 6528 7365 6c66 2c20 6f74  visible(self, ot
-00013fa0: 6865 722c 2072 6967 6874 293a 0a20 2020  her, right):.   
-00013fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013fc0: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
-00013fd0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00013fe0: 6d20 626f 6f6c 2072 6967 6874 3a0a 2020  m bool right:.  
-00013ff0: 2020 2020 2020 3a72 6574 7572 6e3a 2077        :return: w
-00014000: 6865 7468 6572 2077 6520 6361 6e20 6469  hether we can di
-00014010: 7669 6465 206f 7468 6572 2c20 7769 7468  vide other, with
-00014020: 6f75 7420 7265 6d61 696e 6465 720a 2020  out remainder.  
-00014030: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
-00014040: 6f6c 0a20 2020 2020 2020 2022 2222 0a20  ol.        """. 
-00014050: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00014060: 6c66 2e74 6572 6d73 3a0a 2020 2020 2020  lf.terms:.      
-00014070: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00014080: 7365 0a20 2020 2020 2020 2069 6620 6f74  se.        if ot
-00014090: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
-000140a0: 5f6f 7020 616e 6420 6f74 6865 722e 6465  _op and other.de
-000140b0: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-000140c0: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
-000140d0: 2020 2020 2020 2020 2074 6d70 203d 2073           tmp = s
-000140e0: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
-000140f0: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
-00014100: 696e 206f 7468 6572 2e64 6572 6976 6564  in other.derived
-00014110: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7320  _from_op.inputs 
-00014120: 6966 2072 6967 6874 2065 6c73 6520 7265  if right else re
-00014130: 7665 7273 6564 286f 7468 6572 2e64 6572  versed(other.der
-00014140: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00014150: 7574 7329 3a0a 2020 2020 2020 2020 2020  uts):.          
-00014160: 2020 2020 2020 6966 206e 6f74 2074 6d70        if not tmp
-00014170: 2e64 6976 6973 6962 6c65 2874 6572 6d2c  .divisible(term,
-00014180: 2072 6967 6874 3d72 6967 6874 293a 0a20   right=right):. 
-00014190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141a0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141c0: 746d 702e 6578 7465 6e64 5f6d 756c 5f64  tmp.extend_mul_d
-000141d0: 6976 5f28 7465 726d 2c20 6b69 6e64 3d22  iv_(term, kind="
-000141e0: 7472 7565 6469 7622 2c20 7269 6768 743d  truediv", right=
-000141f0: 7269 6768 7429 0a20 2020 2020 2020 2020  right).         
-00014200: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00014210: 2020 2020 2020 206d 6f73 745f 7265 6365         most_rece
-00014220: 6e74 5f74 6572 6d20 3d20 7365 6c66 2e74  nt_term = self.t
-00014230: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-00014240: 2065 6c73 6520 305d 0a20 2020 2020 2020   else 0].       
-00014250: 2069 6620 6f74 6865 7220 3d3d 206d 6f73   if other == mos
-00014260: 745f 7265 6365 6e74 5f74 6572 6d3a 0a20  t_recent_term:. 
-00014270: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014280: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
-00014290: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
-000142a0: 726d 2e64 696d 656e 7369 6f6e 2069 7320  rm.dimension is 
-000142b0: 6e6f 7420 4e6f 6e65 2061 6e64 206f 7468  not None and oth
-000142c0: 6572 2e64 696d 656e 7369 6f6e 2069 7320  er.dimension is 
-000142d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000142e0: 2020 2020 2020 6966 206d 6f73 745f 7265        if most_re
-000142f0: 6365 6e74 5f74 6572 6d2e 6469 6d65 6e73  cent_term.dimens
-00014300: 696f 6e20 2520 6f74 6865 722e 6469 6d65  ion % other.dime
-00014310: 6e73 696f 6e20 3d3d 2030 3a0a 2020 2020  nsion == 0:.    
-00014320: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014330: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00014340: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-00014350: 2020 6465 6620 6361 6e5f 7369 6d70 6c69    def can_simpli
-00014360: 6679 2873 656c 662c 206f 7468 6572 2c20  fy(self, other, 
-00014370: 6b69 6e64 2c20 7269 6768 7429 3a0a 2020  kind, right):.  
-00014380: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014390: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
-000143a0: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
-000143b0: 616d 2073 7472 206b 696e 643a 0a20 2020  am str kind:.   
-000143c0: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
-000143d0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-000143e0: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
-000143f0: 2077 6520 6361 6e20 7369 6d70 6c69 6679   we can simplify
-00014400: 2077 6865 6e20 6170 706c 7969 6e67 2074   when applying t
-00014410: 6869 7320 6f70 6572 6174 696f 6e0a 2020  his operation.  
-00014420: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
-00014430: 6f6c 0a20 2020 2020 2020 2022 2222 0a20  ol.        """. 
-00014440: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
-00014450: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-00014460: 616e 6420 6f74 6865 722e 6465 7269 7665  and other.derive
-00014470: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
-00014480: 3d20 226d 756c 223a 0a20 2020 2020 2020  = "mul":.       
-00014490: 2020 2020 2074 6d70 203d 2073 656c 662e       tmp = self.
-000144a0: 636f 7079 2829 0a20 2020 2020 2020 2020  copy().         
-000144b0: 2020 2066 6f72 2074 6572 6d20 696e 206f     for term in o
-000144c0: 7468 6572 2e64 6572 6976 6564 5f66 726f  ther.derived_fro
-000144d0: 6d5f 6f70 2e69 6e70 7574 7320 6966 2072  m_op.inputs if r
-000144e0: 6967 6874 2065 6c73 6520 7265 7665 7273  ight else revers
-000144f0: 6564 286f 7468 6572 2e64 6572 6976 6564  ed(other.derived
-00014500: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7329  _from_op.inputs)
-00014510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014520: 2020 6966 206e 6f74 2074 6d70 2e63 616e    if not tmp.can
-00014530: 5f73 696d 706c 6966 7928 7465 726d 2c20  _simplify(term, 
-00014540: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00014550: 3d72 6967 6874 293a 0a20 2020 2020 2020  =right):.       
-00014560: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00014570: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00014580: 2020 2020 2020 2020 2020 746d 702e 6578            tmp.ex
-00014590: 7465 6e64 5f6d 756c 5f64 6976 5f28 7465  tend_mul_div_(te
-000145a0: 726d 2c20 6b69 6e64 3d6b 696e 642c 2072  rm, kind=kind, r
-000145b0: 6967 6874 3d72 6967 6874 290a 2020 2020  ight=right).    
-000145c0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-000145d0: 7275 650a 2020 2020 2020 2020 6964 7820  rue.        idx 
-000145e0: 3d20 7365 6c66 2e5f 7369 6d70 6c69 6679  = self._simplify
-000145f0: 5f74 6572 6d5f 6964 7828 6f74 6865 722c  _term_idx(other,
-00014600: 206b 696e 643d 6b69 6e64 2c20 7269 6768   kind=kind, righ
-00014610: 743d 7269 6768 7429 0a20 2020 2020 2020  t=right).       
-00014620: 2072 6574 7572 6e20 6964 7820 6973 206e   return idx is n
-00014630: 6f74 204e 6f6e 650a 0a20 2020 2064 6566  ot None..    def
-00014640: 205f 7369 6d70 6c69 6679 5f74 6572 6d5f   _simplify_term_
-00014650: 6964 7828 7365 6c66 2c20 6f74 6865 722c  idx(self, other,
-00014660: 206b 696e 642c 2072 6967 6874 293a 0a20   kind, right):. 
-00014670: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014680: 2020 203a 7061 7261 6d20 4469 6d20 6f74     :param Dim ot
-00014690: 6865 723a 0a20 2020 2020 2020 203a 7061  her:.        :pa
-000146a0: 7261 6d20 7374 7220 6b69 6e64 3a0a 2020  ram str kind:.  
-000146b0: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
-000146c0: 6c20 7269 6768 743a 0a20 2020 2020 2020  l right:.       
-000146d0: 203a 7265 7475 726e 3a20 696e 6465 7820   :return: index 
-000146e0: 6f66 2074 6572 6d20 746f 2073 696d 706c  of term to simpl
-000146f0: 6966 790a 2020 2020 2020 2020 3a72 7479  ify.        :rty
-00014700: 7065 3a20 696e 747c 4e6f 6e65 0a20 2020  pe: int|None.   
-00014710: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014720: 2069 6620 6e6f 7420 7365 6c66 2e74 6572   if not self.ter
-00014730: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00014740: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00014750: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
-00014760: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
-00014770: 2020 2320 5765 2077 616e 7420 2862 202a    # We want (b *
-00014780: 2061 2920 2f2f 2062 2021 3d20 612e 0a20   a) // b != a.. 
-00014790: 2020 2020 2020 2020 2020 2023 2048 6f77             # How
-000147a0: 6576 6572 2c20 7765 2077 616e 7420 6820  ever, we want h 
-000147b0: 2a20 2832 202a 2061 202f 2f20 6829 203d  * (2 * a // h) =
-000147c0: 3d20 3220 2a20 612e 0a20 2020 2020 2020  = 2 * a..       
-000147d0: 2020 2020 2023 2053 6f2c 2066 6f72 2060       # So, for `
-000147e0: 6d75 6c60 2c20 616e 6420 6f6e 6c79 2066  mul`, and only f
-000147f0: 6f72 2060 6d75 6c60 2c20 6368 6563 6b20  or `mul`, check 
-00014800: 616c 6c20 7465 726d 732c 2077 6865 7468  all terms, wheth
-00014810: 6572 2077 6520 6361 6e20 7369 6d70 6c69  er we can simpli
-00014820: 6679 2073 6f6d 6520 6469 7669 7369 6f6e  fy some division
-00014830: 2d74 6572 6d2e 0a20 2020 2020 2020 2020  -term..         
-00014840: 2020 2066 6f72 2069 2c20 7465 726d 2069     for i, term i
-00014850: 6e20 7265 7665 7273 6564 286c 6973 7428  n reversed(list(
-00014860: 656e 756d 6572 6174 6528 7365 6c66 2e74  enumerate(self.t
-00014870: 6572 6d73 2929 2920 6966 2072 6967 6874  erms))) if right
-00014880: 2065 6c73 6520 656e 756d 6572 6174 6528   else enumerate(
-00014890: 7365 6c66 2e74 6572 6d73 293a 0a20 2020  self.terms):.   
-000148a0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-000148b0: 6572 7420 6973 696e 7374 616e 6365 2874  ert isinstance(t
-000148c0: 6572 6d2c 205f 642e 4469 6d29 0a20 2020  erm, _d.Dim).   
-000148d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000148e0: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
-000148f0: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-00014900: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
-00014910: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
-00014920: 702e 6b69 6e64 203d 3d20 2274 7275 6564  p.kind == "trued
-00014930: 6976 5f22 202b 2028 2272 6967 6874 2220  iv_" + ("right" 
-00014940: 6966 2072 6967 6874 2065 6c73 6520 226c  if right else "l
-00014950: 6566 7422 293a 0a20 2020 2020 2020 2020  eft"):.         
-00014960: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014970: 6620 7465 726d 2e64 6572 6976 6564 5f66  f term.derived_f
-00014980: 726f 6d5f 6f70 2e69 6e70 7574 735b 2d31  rom_op.inputs[-1
-00014990: 5d20 3d3d 206f 7468 6572 3a0a 2020 2020  ] == other:.    
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149b0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-000149c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000149d0: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
-000149e0: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
-000149f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014a00: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-00014a10: 6672 6f6d 5f6f 702e 6b69 6e64 203d 3d20  from_op.kind == 
-00014a20: 2274 7275 6564 6976 5f22 202b 2028 2272  "truediv_" + ("r
-00014a30: 6967 6874 2220 6966 206e 6f74 2072 6967  ight" if not rig
-00014a40: 6874 2065 6c73 6520 226c 6566 7422 293a  ht else "left"):
-00014a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014a60: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
-00014a70: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014a80: 702e 696e 7075 7473 5b2d 315d 203d 3d20  p.inputs[-1] == 
-00014a90: 7465 726d 3a0a 2020 2020 2020 2020 2020  term:.          
-00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ab0: 2020 7265 7475 726e 2069 0a20 2020 2020    return i.     
-00014ac0: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00014ad0: 726d 2e69 735f 636f 6e73 7461 6e74 5f73  rm.is_constant_s
-00014ae0: 7461 7469 635f 6469 6d28 2920 616e 6420  tatic_dim() and 
-00014af0: 6f74 6865 722e 6973 5f63 6f6e 7374 616e  other.is_constan
-00014b00: 745f 7374 6174 6963 5f64 696d 2829 3a0a  t_static_dim():.
-00014b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b20: 2020 2020 7265 7475 726e 2069 0a20 2020      return i.   
-00014b30: 2020 2020 2023 2046 6f72 2074 6865 206c       # For the l
-00014b40: 6173 742f 6669 7273 7420 7465 726d 2c20  ast/first term, 
-00014b50: 6578 7472 6120 6368 6563 6b73 2e0a 2020  extra checks..  
-00014b60: 2020 2020 2020 6920 3d20 6c65 6e28 7365        i = len(se
-00014b70: 6c66 2e74 6572 6d73 2920 2d20 3120 6966  lf.terms) - 1 if
-00014b80: 2072 6967 6874 2065 6c73 6520 300a 2020   right else 0.  
-00014b90: 2020 2020 2020 7465 726d 203d 2073 656c        term = sel
-00014ba0: 662e 7465 726d 735b 695d 0a20 2020 2020  f.terms[i].     
-00014bb0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
-00014bc0: 6974 6828 2264 6976 2229 2061 6e64 206f  ith("div") and o
-00014bd0: 7468 6572 203d 3d20 7465 726d 3a0a 2020  ther == term:.  
-00014be0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014bf0: 2069 0a20 2020 2020 2020 206f 705f 6b69   i.        op_ki
-00014c00: 6e64 203d 206b 696e 6420 2b20 225f 2220  nd = kind + "_" 
-00014c10: 2b20 2822 7269 6768 7422 2069 6620 7269  + ("right" if ri
-00014c20: 6768 7420 656c 7365 2022 6c65 6674 2229  ght else "left")
-00014c30: 0a20 2020 2020 2020 2069 6620 7465 726d  .        if term
-00014c40: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00014c50: 2061 6e64 2074 6572 6d2e 6465 7269 7665   and term.derive
-00014c60: 645f 6672 6f6d 5f6f 702e 6b69 6e64 203d  d_from_op.kind =
-00014c70: 3d20 6f70 5f6b 696e 643a 0a20 2020 2020  = op_kind:.     
-00014c80: 2020 2020 2020 2072 6574 7572 6e20 690a         return i.
-00014c90: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00014ca0: 6f6e 650a 0a20 2020 2064 6566 2065 7874  one..    def ext
-00014cb0: 656e 645f 6d75 6c5f 6469 765f 2873 656c  end_mul_div_(sel
-00014cc0: 662c 206f 7468 6572 2c20 6b69 6e64 2c20  f, other, kind, 
-00014cd0: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
-00014ce0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00014cf0: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
-00014d00: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-00014d10: 206b 696e 643a 0a20 2020 2020 2020 203a   kind:.        :
-00014d20: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
-00014d30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00014d40: 2020 2020 2020 6173 7365 7274 206b 696e        assert kin
-00014d50: 6420 696e 207b 226d 756c 222c 2022 666c  d in {"mul", "fl
-00014d60: 6f6f 7264 6976 222c 2022 7472 7565 6469  oordiv", "truedi
-00014d70: 7622 2c20 2263 6569 6c64 6976 227d 0a20  v", "ceildiv"}. 
-00014d80: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
-00014d90: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
-00014da0: 6963 5f64 696d 2829 2061 6e64 206f 7468  ic_dim() and oth
-00014db0: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-00014dc0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
-00014dd0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00014de0: 206e 6f74 2073 656c 662e 7465 726d 733a   not self.terms:
-00014df0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014e00: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
-00014e10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014e20: 656c 662e 7465 726d 732e 6170 7065 6e64  elf.terms.append
-00014e30: 286f 7468 6572 290a 2020 2020 2020 2020  (other).        
-00014e40: 2020 2020 656c 6966 206b 696e 642e 656e      elif kind.en
-00014e50: 6473 7769 7468 2822 6469 7622 293a 0a20  dswith("div"):. 
-00014e60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014e70: 656c 662e 7465 726d 7320 3d20 5b5f 4f70  elf.terms = [_Op
-00014e80: 4d75 6c74 5465 726d 2e6e 6577 5f64 6976  MultTerm.new_div
-00014e90: 5f64 696d 2873 656c 662e 6173 5f64 696d  _dim(self.as_dim
-00014ea0: 2829 2c20 6f74 6865 722c 206b 696e 643d  (), other, kind=
-00014eb0: 6b69 6e64 2c20 7269 6768 743d 7269 6768  kind, right=righ
-00014ec0: 7429 5d0a 2020 2020 2020 2020 2020 2020  t)].            
-00014ed0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00014ee0: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-00014ef0: 6672 6f6d 5f6f 7020 616e 6420 6f74 6865  from_op and othe
-00014f00: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014f10: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
-00014f20: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00014f30: 2074 6572 6d20 696e 206f 7468 6572 2e64   term in other.d
-00014f40: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
-00014f50: 6e70 7574 7320 6966 2072 6967 6874 2065  nputs if right e
-00014f60: 6c73 6520 7265 7665 7273 6564 286f 7468  lse reversed(oth
-00014f70: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-00014f80: 6f70 2e69 6e70 7574 7329 3a0a 2020 2020  op.inputs):.    
-00014f90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014fa0: 2e65 7874 656e 645f 6d75 6c5f 6469 765f  .extend_mul_div_
-00014fb0: 2874 6572 6d2c 206b 696e 643d 6b69 6e64  (term, kind=kind
-00014fc0: 2c20 7269 6768 743d 7269 6768 7429 0a20  , right=right). 
-00014fd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014fe0: 6e0a 2020 2020 2020 2020 6964 7820 3d20  n.        idx = 
-00014ff0: 7365 6c66 2e5f 7369 6d70 6c69 6679 5f74  self._simplify_t
-00015000: 6572 6d5f 6964 7828 6f74 6865 722c 206b  erm_idx(other, k
-00015010: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-00015020: 7269 6768 7429 0a20 2020 2020 2020 2069  right).        i
-00015030: 6620 6964 7820 6973 206e 6f74 204e 6f6e  f idx is not Non
-00015040: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00015050: 6572 6d20 3d20 7365 6c66 2e74 6572 6d73  erm = self.terms
-00015060: 5b69 6478 5d0a 2020 2020 2020 2020 2020  [idx].          
-00015070: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00015080: 6e63 6528 7465 726d 2c20 5f64 2e44 696d  nce(term, _d.Dim
-00015090: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000150a0: 206b 696e 642e 656e 6473 7769 7468 2822   kind.endswith("
-000150b0: 6469 7622 2920 616e 6420 6f74 6865 7220  div") and other 
-000150c0: 3d3d 2074 6572 6d3a 0a20 2020 2020 2020  == term:.       
-000150d0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-000150e0: 726d 732e 706f 7028 6964 7829 0a20 2020  rms.pop(idx).   
-000150f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00015100: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00015110: 6966 206b 696e 6420 3d3d 2022 6d75 6c22  if kind == "mul"
-00015120: 2061 6e64 2074 6572 6d2e 6465 7269 7665   and term.derive
-00015130: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
-00015140: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00015150: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
-00015160: 6f70 2e6b 696e 6420 3d3d 2022 7472 7565  op.kind == "true
-00015170: 6469 765f 2220 2b20 2822 7269 6768 7422  div_" + ("right"
-00015180: 2069 6620 7269 6768 7420 656c 7365 2022   if right else "
-00015190: 6c65 6674 2229 3a0a 2020 2020 2020 2020  left"):.        
-000151a0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000151b0: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
-000151c0: 5f6f 702e 696e 7075 7473 5b2d 315d 203d  _op.inputs[-1] =
-000151d0: 3d20 6f74 6865 723a 0a20 2020 2020 2020  = other:.       
-000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151f0: 2073 656c 662e 7465 726d 735b 6964 785d   self.terms[idx]
-00015200: 203d 2074 6572 6d2e 6465 7269 7665 645f   = term.derived_
-00015210: 6672 6f6d 5f6f 702e 696e 7075 7473 5b30  from_op.inputs[0
-00015220: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00015230: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00015240: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015250: 6b69 6e64 203d 3d20 226d 756c 2220 616e  kind == "mul" an
-00015260: 6420 6f74 6865 722e 6465 7269 7665 645f  d other.derived_
-00015270: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
-00015280: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
-00015290: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-000152a0: 702e 6b69 6e64 203d 3d20 2274 7275 6564  p.kind == "trued
-000152b0: 6976 5f22 202b 2028 2272 6967 6874 2220  iv_" + ("right" 
-000152c0: 6966 206e 6f74 2072 6967 6874 2065 6c73  if not right els
-000152d0: 6520 226c 6566 7422 293a 0a20 2020 2020  e "left"):.     
-000152e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000152f0: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-00015300: 6672 6f6d 5f6f 702e 696e 7075 7473 5b2d  from_op.inputs[-
-00015310: 315d 203d 3d20 7465 726d 3a0a 2020 2020  1] == term:.    
-00015320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015330: 2020 2020 7365 6c66 2e74 6572 6d73 5b69      self.terms[i
-00015340: 6478 5d20 3d20 6f74 6865 722e 6465 7269  dx] = other.deri
-00015350: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015360: 7473 5b30 5d0a 2020 2020 2020 2020 2020  ts[0].          
-00015370: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015380: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00015390: 2069 6620 7465 726d 2e69 735f 636f 6e73   if term.is_cons
-000153a0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-000153b0: 2920 616e 6420 6f74 6865 722e 6973 5f63  ) and other.is_c
-000153c0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
-000153d0: 696d 2829 3a0a 2020 2020 2020 2020 2020  im():.          
-000153e0: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
-000153f0: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
-00015400: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00015410: 6572 6d2e 6469 6d65 6e73 696f 6e20 2a20  erm.dimension * 
-00015420: 6f74 6865 722e 6469 6d65 6e73 696f 6e20  other.dimension 
-00015430: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00015440: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015450: 6c66 2e74 6572 6d73 2e70 6f70 2869 6478  lf.terms.pop(idx
-00015460: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015470: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00015480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015490: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
-000154a0: 6964 785d 203d 205f 6d61 6b65 5f63 6f6e  idx] = _make_con
-000154b0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-000154c0: 2874 6572 6d2e 6469 6d65 6e73 696f 6e20  (term.dimension 
-000154d0: 2a20 6f74 6865 722e 6469 6d65 6e73 696f  * other.dimensio
-000154e0: 6e2c 206b 696e 643d 7465 726d 2e6b 696e  n, kind=term.kin
-000154f0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00015500: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00015510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00015520: 206b 696e 642e 656e 6473 7769 7468 2822   kind.endswith("
-00015530: 6469 7622 2920 616e 6420 7465 726d 2e64  div") and term.d
-00015540: 696d 656e 7369 6f6e 2025 206f 7468 6572  imension % other
-00015550: 2e64 696d 656e 7369 6f6e 203d 3d20 303a  .dimension == 0:
-00015560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015570: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
-00015580: 6964 785d 203d 205f 6d61 6b65 5f63 6f6e  idx] = _make_con
-00015590: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-000155a0: 2874 6572 6d2e 6469 6d65 6e73 696f 6e20  (term.dimension 
-000155b0: 2f2f 206f 7468 6572 2e64 696d 656e 7369  // other.dimensi
-000155c0: 6f6e 2c20 6b69 6e64 3d74 6572 6d2e 6b69  on, kind=term.ki
-000155d0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-000155e0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-000155f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00015600: 2046 616c 6c62 6163 6b20 7769 7468 2067   Fallback with g
-00015610: 656e 6572 6963 2068 616e 646c 696e 672e  eneric handling.
-00015620: 0a20 2020 2020 2020 2020 2020 206f 705f  .            op_
-00015630: 6b69 6e64 203d 206b 696e 6420 2b20 225f  kind = kind + "_
-00015640: 2220 2b20 2822 7269 6768 7422 2069 6620  " + ("right" if 
-00015650: 7269 6768 7420 656c 7365 2022 6c65 6674  right else "left
-00015660: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00015670: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
-00015680: 2264 6976 2229 2061 6e64 2074 6572 6d2e  "div") and term.
-00015690: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-000156a0: 616e 6420 7465 726d 2e64 6572 6976 6564  and term.derived
-000156b0: 5f66 726f 6d5f 6f70 2e6b 696e 6420 3d3d  _from_op.kind ==
-000156c0: 206f 705f 6b69 6e64 3a0a 2020 2020 2020   op_kind:.      
-000156d0: 2020 2020 2020 2020 2020 6e75 6d65 7261            numera
-000156e0: 746f 7220 3d20 7465 726d 2e64 6572 6976  tor = term.deriv
-000156f0: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00015700: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
-00015710: 2020 2020 2064 656e 6f6d 696e 6174 6f72       denominator
-00015720: 203d 2074 6572 6d2e 6465 7269 7665 645f   = term.derived_
-00015730: 6672 6f6d 5f6f 702e 696e 7075 7473 5b31  from_op.inputs[1
-00015740: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00015750: 2020 7365 6c66 2e74 6572 6d73 5b69 6478    self.terms[idx
-00015760: 5d20 3d20 5f4f 704d 756c 7454 6572 6d2e  ] = _OpMultTerm.
-00015770: 6e65 775f 6469 765f 6469 6d28 6e75 6d65  new_div_dim(nume
-00015780: 7261 746f 722c 2064 656e 6f6d 696e 6174  rator, denominat
-00015790: 6f72 202a 206f 7468 6572 2c20 6b69 6e64  or * other, kind
-000157a0: 3d6b 696e 642c 2072 6967 6874 3d72 6967  =kind, right=rig
-000157b0: 6874 290a 2020 2020 2020 2020 2020 2020  ht).            
-000157c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000157d0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
-000157e0: 6974 6828 2264 6976 2229 3a0a 2020 2020  ith("div"):.    
-000157f0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00015800: 6d73 203d 205b 5f4f 704d 756c 7454 6572  ms = [_OpMultTer
-00015810: 6d2e 6e65 775f 6469 765f 6469 6d28 7365  m.new_div_dim(se
-00015820: 6c66 2e61 735f 6469 6d28 292c 206f 7468  lf.as_dim(), oth
-00015830: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
-00015840: 6967 6874 3d72 6967 6874 295d 0a20 2020  ight=right)].   
-00015850: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00015860: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
-00015870: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00015880: 2020 2020 2020 6966 2072 6967 6874 3a0a        if right:.
-00015890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158a0: 7365 6c66 2e74 6572 6d73 2e61 7070 656e  self.terms.appen
-000158b0: 6428 6f74 6865 7229 0a20 2020 2020 2020  d(other).       
-000158c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000158d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000158e0: 7465 726d 732e 696e 7365 7274 2830 2c20  terms.insert(0, 
-000158f0: 6f74 6865 7229 0a20 2020 2020 2020 2020  other).         
-00015900: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00015910: 2020 6173 7365 7274 2046 616c 7365 0a0a    assert False..
-00015920: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00015930: 0a20 2020 2064 6566 206e 6577 5f64 6976  .    def new_div
-00015940: 5f64 696d 2863 6c73 2c20 6e75 6d65 7261  _dim(cls, numera
-00015950: 746f 722c 2064 656e 6f6d 696e 6174 6f72  tor, denominator
-00015960: 2c20 6b69 6e64 2c20 7269 6768 7429 3a0a  , kind, right):.
-00015970: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015980: 2020 2020 3a70 6172 616d 2044 696d 206e      :param Dim n
-00015990: 756d 6572 6174 6f72 3a0a 2020 2020 2020  umerator:.      
-000159a0: 2020 3a70 6172 616d 2044 696d 2064 656e    :param Dim den
-000159b0: 6f6d 696e 6174 6f72 3a0a 2020 2020 2020  ominator:.      
-000159c0: 2020 3a70 6172 616d 2073 7472 206b 696e    :param str kin
-000159d0: 643a 2022 666c 6f6f 7264 6976 2220 6f72  d: "floordiv" or
-000159e0: 2022 6365 696c 6469 7622 206f 7220 2274   "ceildiv" or "t
-000159f0: 7275 6564 6976 220a 2020 2020 2020 2020  ruediv".        
-00015a00: 3a70 6172 616d 2062 6f6f 6c20 7269 6768  :param bool righ
-00015a10: 743a 0a20 2020 2020 2020 203a 7274 7970  t:.        :rtyp
-00015a20: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00015a30: 2222 0a20 2020 2020 2020 2064 696d 5f76  "".        dim_v
-00015a40: 616c 7565 203d 204e 6f6e 650a 2020 2020  alue = None.    
-00015a50: 2020 2020 6120 3d20 6e75 6d65 7261 746f      a = numerato
-00015a60: 722e 6469 6d65 6e73 696f 6e0a 2020 2020  r.dimension.    
-00015a70: 2020 2020 6220 3d20 6465 6e6f 6d69 6e61      b = denomina
-00015a80: 746f 722e 6469 6d65 6e73 696f 6e0a 2020  tor.dimension.  
-00015a90: 2020 2020 2020 6966 2061 2069 7320 6e6f        if a is no
-00015aa0: 7420 4e6f 6e65 2061 6e64 2062 2069 7320  t None and b is 
-00015ab0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00015ac0: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
-00015ad0: 2022 666c 6f6f 7264 6976 223a 0a20 2020   "floordiv":.   
-00015ae0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00015af0: 5f76 616c 7565 203d 2061 202f 2f20 620a  _value = a // b.
-00015b00: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00015b10: 206b 696e 6420 3d3d 2022 6365 696c 6469   kind == "ceildi
-00015b20: 7622 3a0a 2020 2020 2020 2020 2020 2020  v":.            
-00015b30: 2020 2020 6469 6d5f 7661 6c75 6520 3d20      dim_value = 
-00015b40: 2d28 2d61 202f 2f20 6229 0a20 2020 2020  -(-a // b).     
-00015b50: 2020 2020 2020 2020 2020 2069 6620 6120             if a 
-00015b60: 2520 6220 3d3d 2030 2061 6e64 2072 6967  % b == 0 and rig
-00015b70: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-00015b80: 2020 2020 2020 2020 6b69 6e64 203d 2022          kind = "
-00015b90: 666c 6f6f 7264 6976 2220 2023 2066 6f72  floordiv"  # for
-00015ba0: 206e 6963 6572 2064 6573 6372 6970 7469   nicer descripti
-00015bb0: 6f6e 2c20 616e 6420 646f 6573 206e 6f74  on, and does not
-00015bc0: 206d 6174 7465 720a 2020 2020 2020 2020   matter.        
-00015bd0: 2020 2020 656c 6966 206b 696e 6420 3d3d      elif kind ==
-00015be0: 2022 7472 7565 6469 7622 3a0a 2020 2020   "truediv":.    
-00015bf0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00015c00: 2025 2062 2021 3d20 303a 0a20 2020 2020   % b != 0:.     
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00015c20: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00015c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c40: 2020 2020 2020 2020 2022 2573 2074 7275           "%s tru
-00015c50: 6564 6976 2025 7320 6f6e 6c79 2061 6c6c  ediv %s only all
-00015c60: 6f77 6564 2069 6620 7468 6520 7265 7375  owed if the resu
-00015c70: 6c74 2069 7320 616e 2069 6e74 6567 6572  lt is an integer
-00015c80: 2220 2520 286e 756d 6572 6174 6f72 2c20  " % (numerator, 
-00015c90: 6465 6e6f 6d69 6e61 746f 7229 0a20 2020  denominator).   
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00015cc0: 2020 2064 696d 5f76 616c 7565 203d 2061     dim_value = a
-00015cd0: 202f 2f20 620a 2020 2020 2020 2020 2020   // b.          
-00015ce0: 2020 2020 2020 6966 2072 6967 6874 3a0a        if right:.
-00015cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d00: 2020 2020 6b69 6e64 203d 2022 666c 6f6f      kind = "floo
-00015d10: 7264 6976 2220 2023 2066 6f72 206e 6963  rdiv"  # for nic
-00015d20: 6572 2064 6573 6372 6970 7469 6f6e 2c20  er description, 
-00015d30: 616e 6420 646f 6573 206e 6f74 206d 6174  and does not mat
-00015d40: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
-00015d50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015d60: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00015d70: 6545 7272 6f72 2822 696e 7661 6c69 6420  eError("invalid 
-00015d80: 6b69 6e64 2025 7222 2025 2028 6b69 6e64  kind %r" % (kind
-00015d90: 2c29 290a 2020 2020 2020 2020 6966 206b  ,)).        if k
-00015da0: 696e 6420 3d3d 2022 666c 6f6f 7264 6976  ind == "floordiv
-00015db0: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
-00015dc0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00015dd0: 7469 6f6e 203d 2022 2573 2f2f 2573 2220  tion = "%s//%s" 
-00015de0: 2520 285f 6765 745f 6465 7363 7269 7074  % (_get_descript
-00015df0: 696f 6e28 6e75 6d65 7261 746f 7229 2c20  ion(numerator), 
-00015e00: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
-00015e10: 2864 656e 6f6d 696e 6174 6f72 2929 0a20  (denominator)). 
-00015e20: 2020 2020 2020 2065 6c69 6620 6b69 6e64         elif kind
-00015e30: 203d 3d20 2263 6569 6c64 6976 2220 616e   == "ceildiv" an
-00015e40: 6420 7269 6768 743a 0a20 2020 2020 2020  d right:.       
-00015e50: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00015e60: 203d 2022 e28c 8825 732f 2573 e28c 8922   = "...%s/%s..."
-00015e70: 2025 2028 5f67 6574 5f64 6573 6372 6970   % (_get_descrip
-00015e80: 7469 6f6e 286e 756d 6572 6174 6f72 292c  tion(numerator),
-00015e90: 205f 6765 745f 6465 7363 7269 7074 696f   _get_descriptio
-00015ea0: 6e28 6465 6e6f 6d69 6e61 746f 7229 290a  n(denominator)).
-00015eb0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00015ec0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00015ed0: 7074 696f 6e20 3d20 2225 735f 2573 2825  ption = "%s_%s(%
-00015ee0: 732c 2025 7329 2220 2520 280a 2020 2020  s, %s)" % (.    
-00015ef0: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-00015f00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015f10: 2020 2272 6967 6874 2220 6966 2072 6967    "right" if rig
-00015f20: 6874 2065 6c73 6520 226c 6566 7422 2c0a  ht else "left",.
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
-00015f50: 286e 756d 6572 6174 6f72 2c20 6272 6163  (numerator, brac
-00015f60: 6b65 7473 3d46 616c 7365 292c 0a20 2020  kets=False),.   
-00015f70: 2020 2020 2020 2020 2020 2020 205f 6765               _ge
-00015f80: 745f 6465 7363 7269 7074 696f 6e28 6465  t_description(de
-00015f90: 6e6f 6d69 6e61 746f 722c 2062 7261 636b  nominator, brack
-00015fa0: 6574 733d 4661 6c73 6529 2c0a 2020 2020  ets=False),.    
-00015fb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00015fc0: 2020 6f70 5f6b 696e 6420 3d20 6b69 6e64    op_kind = kind
-00015fd0: 0a20 2020 2020 2020 2069 6620 6120 6973  .        if a is
-00015fe0: 206e 6f74 204e 6f6e 6520 616e 6420 6220   not None and b 
-00015ff0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00016000: 6120 2520 6220 3d3d 2030 3a0a 2020 2020  a % b == 0:.    
-00016010: 2020 2020 2020 2020 6f70 5f6b 696e 6420          op_kind 
-00016020: 3d20 2274 7275 6564 6976 2220 2023 206d  = "truediv"  # m
-00016030: 616b 6573 2073 6f6d 6520 6f74 6865 7220  akes some other 
-00016040: 6368 6563 6b73 2073 696d 706c 6572 0a20  checks simpler. 
-00016050: 2020 2020 2020 206f 705f 6b69 6e64 202b         op_kind +
-00016060: 3d20 225f 2220 2b20 2822 7269 6768 7422  = "_" + ("right"
-00016070: 2069 6620 7269 6768 7420 656c 7365 2022   if right else "
-00016080: 6c65 6674 2229 0a20 2020 2020 2020 2072  left").        r
-00016090: 6574 7572 6e20 5f64 2e44 696d 280a 2020  eturn _d.Dim(.  
-000160a0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-000160b0: 7074 696f 6e3d 6465 7363 7269 7074 696f  ption=descriptio
-000160c0: 6e2c 0a20 2020 2020 2020 2020 2020 206b  n,.            k
-000160d0: 696e 643d 6e75 6d65 7261 746f 722e 6b69  ind=numerator.ki
-000160e0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-000160f0: 6469 6d65 6e73 696f 6e3d 6469 6d5f 7661  dimension=dim_va
-00016100: 6c75 652c 0a20 2020 2020 2020 2020 2020  lue,.           
-00016110: 2064 6572 6976 6564 5f66 726f 6d5f 6f70   derived_from_op
-00016120: 3d4f 7028 6b69 6e64 3d6f 705f 6b69 6e64  =Op(kind=op_kind
-00016130: 2c20 696e 7075 7473 3d5b 6e75 6d65 7261  , inputs=[numera
-00016140: 746f 722c 2064 656e 6f6d 696e 6174 6f72  tor, denominator
-00016150: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00016160: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-00016170: 3d6e 756d 6572 6174 6f72 2c0a 2020 2020  =numerator,.    
-00016180: 2020 2020 290a 0a20 2020 2064 6566 2061      )..    def a
-00016190: 735f 6469 6d28 7365 6c66 293a 0a20 2020  s_dim(self):.   
-000161a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000161b0: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
-000161c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000161d0: 2069 6620 7365 6c66 2e69 735f 6f6e 6528   if self.is_one(
-000161e0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-000161f0: 6574 7572 6e20 5f6d 616b 655f 636f 6e73  eturn _make_cons
-00016200: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00016210: 3129 0a20 2020 2020 2020 2069 6620 6c65  1).        if le
-00016220: 6e28 7365 6c66 2e74 6572 6d73 2920 3d3d  n(self.terms) ==
-00016230: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00016240: 7265 7475 726e 2073 656c 662e 7465 726d  return self.term
-00016250: 735b 305d 0a20 2020 2020 2020 2064 696d  s[0].        dim
-00016260: 5f6b 696e 6420 3d20 5f67 6574 5f6d 6572  _kind = _get_mer
-00016270: 6765 645f 6469 6d5f 6b69 6e64 2873 656c  ged_dim_kind(sel
-00016280: 662e 7465 726d 7329 0a20 2020 2020 2020  f.terms).       
-00016290: 2072 6574 7572 6e20 5f64 2e44 696d 280a   return _d.Dim(.
-000162a0: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-000162b0: 3d64 696d 5f6b 696e 642c 0a20 2020 2020  =dim_kind,.     
-000162c0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000162d0: 6f6e 3d22 2a22 2e6a 6f69 6e28 6d61 7028  on="*".join(map(
-000162e0: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
-000162f0: 2c20 7365 6c66 2e74 6572 6d73 2929 2c0a  , self.terms)),.
-00016300: 2020 2020 2020 2020 2020 2020 6469 6d65              dime
-00016310: 6e73 696f 6e3d 7365 6c66 2e64 696d 656e  nsion=self.dimen
-00016320: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
-00016330: 2020 6465 7269 7665 645f 6672 6f6d 5f6f    derived_from_o
-00016340: 703d 4f70 286b 696e 643d 226d 756c 222c  p=Op(kind="mul",
-00016350: 2069 6e70 7574 733d 6c69 7374 2873 656c   inputs=list(sel
-00016360: 662e 7465 726d 7329 292c 0a20 2020 2020  f.terms)),.     
-00016370: 2020 2020 2020 2064 6572 6976 6564 5f66         derived_f
-00016380: 726f 6d5f 7461 673d 7365 6c66 2e72 6570  rom_tag=self.rep
-00016390: 7265 7365 6e74 6174 6976 655f 7461 6728  resentative_tag(
-000163a0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
-000163b0: 2020 6465 6620 7265 7072 6573 656e 7461    def representa
-000163c0: 7469 7665 5f74 6167 2873 656c 6629 3a0a  tive_tag(self):.
-000163d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000163e0: 2020 2020 3a72 7479 7065 3a20 4469 6d7c      :rtype: Dim|
-000163f0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00016400: 0a20 2020 2020 2020 2023 2041 6c73 6f20  .        # Also 
-00016410: 7365 6520 4469 6d2e 5f4f 704c 696e 6561  see Dim._OpLinea
-00016420: 7254 6572 6d2e 7265 7072 6573 656e 7461  rTerm.representa
-00016430: 7469 7665 5f74 6167 2829 2e0a 2020 2020  tive_tag()..    
-00016440: 2020 2020 2320 4669 7273 7420 6669 6e64      # First find
-00016450: 2061 6e79 2064 796e 616d 6963 2e0a 2020   any dynamic..  
-00016460: 2020 2020 2020 666f 7220 7465 726d 5f20        for term_ 
-00016470: 696e 2073 656c 662e 7465 726d 733a 0a20  in self.terms:. 
-00016480: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00016490: 726d 5f2e 6973 5f64 796e 616d 6963 2829  rm_.is_dynamic()
-000164a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000164b0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
-000164c0: 2020 2020 2020 2023 204e 6f77 2066 696e         # Now fin
-000164d0: 6420 6e6f 6e2d 756e 7370 6563 6966 6965  d non-unspecifie
-000164e0: 642e 0a20 2020 2020 2020 2066 6f72 2074  d..        for t
-000164f0: 6572 6d5f 2069 6e20 7365 6c66 2e74 6572  erm_ in self.ter
-00016500: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00016510: 6966 2074 6572 6d5f 2e6b 696e 6420 213d  if term_.kind !=
-00016520: 2044 696d 5479 7065 732e 556e 7370 6563   DimTypes.Unspec
-00016530: 6966 6965 643a 0a20 2020 2020 2020 2020  ified:.         
-00016540: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-00016550: 726d 5f0a 2020 2020 2020 2020 2320 4e6f  rm_.        # No
-00016560: 7720 6669 6e64 2061 6e79 2e0a 2020 2020  w find any..    
-00016570: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
-00016580: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
-00016590: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000165a0: 7465 726d 5f0a 2020 2020 2020 2020 7265  term_.        re
-000165b0: 7475 726e 204e 6f6e 650a 0a0a 636c 6173  turn None...clas
-000165c0: 7320 5f4f 704c 696e 6561 7254 6572 6d3a  s _OpLinearTerm:
-000165d0: 0a20 2020 2022 2222 0a20 2020 2072 6570  .    """.    rep
-000165e0: 7265 7365 6e74 7320 7374 6820 6c69 6b65  resents sth like
-000165f0: 2061 202a 2062 202b 2063 0a20 2020 2022   a * b + c.    "
-00016600: 2222 0a0a 2020 2020 4063 6c61 7373 6d65  ""..    @classme
-00016610: 7468 6f64 0a20 2020 2064 6566 2066 726f  thod.    def fro
-00016620: 6d5f 6469 6d28 636c 732c 2064 696d 293a  m_dim(cls, dim):
-00016630: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016640: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-00016650: 6469 6d3a 0a20 2020 2020 2020 203a 7274  dim:.        :rt
-00016660: 7970 653a 2044 696d 2e5f 4f70 4c69 6e65  ype: Dim._OpLine
-00016670: 6172 5465 726d 0a20 2020 2020 2020 2022  arTerm.        "
-00016680: 2222 0a20 2020 2020 2020 2072 6573 203d  "".        res =
-00016690: 2063 6c73 2e7a 6572 6f28 290a 2020 2020   cls.zero().    
-000166a0: 2020 2020 7265 732e 6578 7465 6e64 5f61      res.extend_a
-000166b0: 6464 5f73 7562 5f28 6469 6d2c 206b 696e  dd_sub_(dim, kin
-000166c0: 643d 2261 6464 222c 2072 6967 6874 3d54  d="add", right=T
-000166d0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-000166e0: 7572 6e20 7265 730a 0a20 2020 2040 636c  urn res..    @cl
-000166f0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00016700: 6620 7a65 726f 2863 6c73 293a 0a20 2020  f zero(cls):.   
-00016710: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00016720: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-00016730: 4c69 6e65 6172 5465 726d 0a20 2020 2020  LinearTerm.     
-00016740: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00016750: 6574 7572 6e20 5f4f 704c 696e 6561 7254  eturn _OpLinearT
-00016760: 6572 6d28 5b5d 290a 0a20 2020 2064 6566  erm([])..    def
-00016770: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00016780: 7465 726d 7329 3a0a 2020 2020 2020 2020  terms):.        
-00016790: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-000167a0: 616d 206c 6973 745b 4469 6d2e 5f4f 704d  am list[Dim._OpM
-000167b0: 756c 7454 6572 6d5d 2074 6572 6d73 3a0a  ultTerm] terms:.
-000167c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000167d0: 2020 2020 7365 6c66 2e74 6572 6d73 203d      self.terms =
-000167e0: 2074 6572 6d73 0a0a 2020 2020 6465 6620   terms..    def 
-000167f0: 5f5f 6861 7368 5f5f 2873 656c 6629 3a0a  __hash__(self):.
-00016800: 2020 2020 2020 2020 7265 7475 726e 2068          return h
-00016810: 6173 6828 7475 706c 6528 7365 6c66 2e74  ash(tuple(self.t
-00016820: 6572 6d73 2929 0a0a 2020 2020 6465 6620  erms))..    def 
-00016830: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
-00016840: 6572 293a 0a20 2020 2020 2020 2069 6620  er):.        if 
-00016850: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-00016860: 2c20 5f4f 704c 696e 6561 7254 6572 6d29  , _OpLinearTerm)
-00016870: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00016880: 7475 726e 2073 656c 662e 7465 726d 7320  turn self.terms 
-00016890: 3d3d 206f 7468 6572 2e74 6572 6d73 0a20  == other.terms. 
-000168a0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000168b0: 6c73 650a 0a20 2020 2064 6566 205f 5f6e  lse..    def __n
-000168c0: 655f 5f28 7365 6c66 2c20 6f74 6865 7229  e__(self, other)
-000168d0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000168e0: 206e 6f74 2073 656c 662e 5f5f 6571 5f5f   not self.__eq__
-000168f0: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
-00016900: 2061 735f 6469 6d28 7365 6c66 293a 0a20   as_dim(self):. 
-00016910: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016920: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00016930: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016940: 2020 2069 6620 7365 6c66 2e69 735f 7a65     if self.is_ze
-00016950: 726f 2829 3a0a 2020 2020 2020 2020 2020  ro():.          
-00016960: 2020 7265 7475 726e 205f 6d61 6b65 5f63    return _make_c
-00016970: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
-00016980: 696d 2830 290a 2020 2020 2020 2020 6966  im(0).        if
-00016990: 206c 656e 2873 656c 662e 7465 726d 7329   len(self.terms)
-000169a0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-000169b0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
-000169c0: 6572 6d73 5b30 5d2e 6173 5f64 696d 2829  erms[0].as_dim()
-000169d0: 0a20 2020 2020 2020 2061 6464 5f70 6172  .        add_par
-000169e0: 7473 203d 205b 5d0a 2020 2020 2020 2020  ts = [].        
-000169f0: 6465 7363 5f70 6172 7473 203d 205b 5d0a  desc_parts = [].
-00016a00: 2020 2020 2020 2020 6469 6d20 3d20 300a          dim = 0.
-00016a10: 2020 2020 2020 2020 666f 7220 7465 726d          for term
-00016a20: 2069 6e20 7365 6c66 2e74 6572 6d73 3a0a   in self.terms:.
-00016a30: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
-00016a40: 7465 726d 2e61 735f 6469 6d28 290a 2020  term.as_dim().  
-00016a50: 2020 2020 2020 2020 2020 6164 645f 7061            add_pa
-00016a60: 7274 732e 6170 7065 6e64 2873 290a 2020  rts.append(s).  
-00016a70: 2020 2020 2020 2020 2020 6465 7363 5f70            desc_p
-00016a80: 6172 7473 2e61 7070 656e 6428 5f67 6574  arts.append(_get
-00016a90: 5f64 6573 6372 6970 7469 6f6e 2873 2929  _description(s))
-00016aa0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00016ab0: 6469 6d20 6973 206e 6f74 204e 6f6e 6520  dim is not None 
-00016ac0: 616e 6420 732e 6469 6d65 6e73 696f 6e20  and s.dimension 
-00016ad0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00016ae0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00016af0: 202b 3d20 732e 6469 6d65 6e73 696f 6e0a   += s.dimension.
-00016b00: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00016b10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016b20: 2020 6469 6d20 3d20 4e6f 6e65 0a20 2020    dim = None.   
-00016b30: 2020 2020 2069 6620 6c65 6e28 6164 645f       if len(add_
-00016b40: 7061 7274 7329 203d 3d20 313a 0a20 2020  parts) == 1:.   
-00016b50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00016b60: 6164 645f 7061 7274 735b 305d 0a20 2020  add_parts[0].   
-00016b70: 2020 2020 2072 6574 7572 6e20 5f64 2e44       return _d.D
-00016b80: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-00016b90: 6b69 6e64 3d5f 6765 745f 6d65 7267 6564  kind=_get_merged
-00016ba0: 5f64 696d 5f6b 696e 6428 6164 645f 7061  _dim_kind(add_pa
-00016bb0: 7274 7329 2c0a 2020 2020 2020 2020 2020  rts),.          
-00016bc0: 2020 6465 7363 7269 7074 696f 6e3d 222b    description="+
-00016bd0: 222e 6a6f 696e 2864 6573 635f 7061 7274  ".join(desc_part
-00016be0: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
-00016bf0: 6469 6d65 6e73 696f 6e3d 6469 6d2c 0a20  dimension=dim,. 
-00016c00: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-00016c10: 6564 5f66 726f 6d5f 6f70 3d4f 7028 6b69  ed_from_op=Op(ki
-00016c20: 6e64 3d22 6164 6422 2c20 696e 7075 7473  nd="add", inputs
-00016c30: 3d61 6464 5f70 6172 7473 292c 0a20 2020  =add_parts),.   
-00016c40: 2020 2020 2020 2020 2064 6572 6976 6564           derived
-00016c50: 5f66 726f 6d5f 7461 673d 7365 6c66 2e72  _from_tag=self.r
-00016c60: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
-00016c70: 6728 292c 0a20 2020 2020 2020 2029 0a0a  g(),.        )..
-00016c80: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00016c90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00016ca0: 7265 7475 726e 2022 4469 6d2e 5f4f 704c  return "Dim._OpL
-00016cb0: 696e 6561 7254 6572 6d28 2572 2922 2025  inearTerm(%r)" %
-00016cc0: 2028 7365 6c66 2e74 6572 6d73 2c29 0a0a   (self.terms,)..
-00016cd0: 2020 2020 6465 6620 6973 5f7a 6572 6f28      def is_zero(
-00016ce0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00016cf0: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
-00016d00: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-00016d10: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00016d20: 726e 206e 6f74 2073 656c 662e 7465 726d  rn not self.term
-00016d30: 730a 0a20 2020 2064 6566 2065 7874 656e  s..    def exten
-00016d40: 645f 6164 645f 7375 625f 2873 656c 662c  d_add_sub_(self,
-00016d50: 206f 7468 6572 2c20 6b69 6e64 2c20 7269   other, kind, ri
-00016d60: 6768 7429 3a0a 2020 2020 2020 2020 2222  ght):.        ""
-00016d70: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00016d80: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
-00016d90: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00016da0: 7472 206b 696e 643a 2022 6164 6422 206f  tr kind: "add" o
-00016db0: 7220 2273 7562 220a 2020 2020 2020 2020  r "sub".        
-00016dc0: 3a70 6172 616d 2062 6f6f 6c20 7269 6768  :param bool righ
-00016dd0: 743a 206f 7220 6c65 6674 2e20 7269 6768  t: or left. righ
-00016de0: 7420 6d65 616e 7320 7365 6c66 202b 206f  t means self + o
-00016df0: 7468 6572 2c20 6c65 6674 206d 6561 6e73  ther, left means
-00016e00: 206f 7468 6572 202b 2073 656c 660a 2020   other + self.  
-00016e10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016e20: 2020 6173 7365 7274 206b 696e 6420 696e    assert kind in
-00016e30: 207b 2261 6464 222c 2022 7375 6222 7d0a   {"add", "sub"}.
-00016e40: 2020 2020 2020 2020 6f74 6865 7220 3d20          other = 
-00016e50: 7365 6c66 2e5f 6d61 6b65 5f64 696d 286f  self._make_dim(o
-00016e60: 7468 6572 2c20 6b69 6e64 3d6b 696e 6429  ther, kind=kind)
-00016e70: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-00016e80: 722e 6973 5f63 6f6e 7374 616e 745f 7374  r.is_constant_st
-00016e90: 6174 6963 5f64 696d 2829 2061 6e64 206f  atic_dim() and o
-00016ea0: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
-00016eb0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00016ec0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00016ed0: 6966 206f 7468 6572 2e64 6572 6976 6564  if other.derived
-00016ee0: 5f66 726f 6d5f 6f70 2061 6e64 206f 7468  _from_op and oth
-00016ef0: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-00016f00: 6f70 2e6b 696e 6420 3d3d 2022 6164 6422  op.kind == "add"
-00016f10: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00016f20: 7220 6f74 6865 725f 2069 6e20 6f74 6865  r other_ in othe
-00016f30: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00016f40: 702e 696e 7075 7473 2069 6620 7269 6768  p.inputs if righ
-00016f50: 7420 656c 7365 2072 6576 6572 7365 6428  t else reversed(
-00016f60: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00016f70: 6f6d 5f6f 702e 696e 7075 7473 293a 0a20  om_op.inputs):. 
-00016f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016f90: 656c 662e 6578 7465 6e64 5f61 6464 5f73  elf.extend_add_s
-00016fa0: 7562 5f28 6f74 6865 725f 2c20 6b69 6e64  ub_(other_, kind
-00016fb0: 3d6b 696e 642c 2072 6967 6874 3d72 6967  =kind, right=rig
-00016fc0: 6874 290a 2020 2020 2020 2020 2020 2020  ht).            
-00016fd0: 7265 7475 726e 0a20 2020 2020 2020 2074  return.        t
-00016fe0: 6572 6d20 3d20 5f4f 704d 756c 7454 6572  erm = _OpMultTer
-00016ff0: 6d2e 6672 6f6d 5f64 696d 286f 7468 6572  m.from_dim(other
-00017000: 290a 2020 2020 2020 2020 6e65 675f 7465  ).        neg_te
-00017010: 726d 203d 2074 6572 6d2e 6e65 6761 7469  rm = term.negati
-00017020: 7665 2829 0a20 2020 2020 2020 2069 6620  ve().        if 
-00017030: 6b69 6e64 203d 3d20 2273 7562 223a 0a20  kind == "sub":. 
-00017040: 2020 2020 2020 2020 2020 2074 6572 6d2c             term,
-00017050: 206e 6567 5f74 6572 6d20 3d20 6e65 675f   neg_term = neg_
-00017060: 7465 726d 2c20 7465 726d 0a20 2020 2020  term, term.     
-00017070: 2020 206d 6f73 745f 7265 6365 6e74 5f74     most_recent_t
-00017080: 6572 6d20 3d20 7365 6c66 2e74 6572 6d73  erm = self.terms
-00017090: 5b2d 3120 6966 2072 6967 6874 2065 6c73  [-1 if right els
-000170a0: 6520 305d 2069 6620 7365 6c66 2e74 6572  e 0] if self.ter
-000170b0: 6d73 2065 6c73 6520 4e6f 6e65 0a20 2020  ms else None.   
-000170c0: 2020 2020 2069 6620 6d6f 7374 5f72 6563       if most_rec
-000170d0: 656e 745f 7465 726d 3a0a 2020 2020 2020  ent_term:.      
-000170e0: 2020 2020 2020 6966 206d 6f73 745f 7265        if most_re
-000170f0: 6365 6e74 5f74 6572 6d20 3d3d 206e 6567  cent_term == neg
-00017100: 5f74 6572 6d3a 0a20 2020 2020 2020 2020  _term:.         
-00017110: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00017120: 732e 706f 7028 2d31 2069 6620 7269 6768  s.pop(-1 if righ
-00017130: 7420 656c 7365 2030 290a 2020 2020 2020  t else 0).      
-00017140: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017150: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00017160: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
-00017170: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
-00017180: 7469 635f 6469 6d28 2920 616e 6420 7465  tic_dim() and te
-00017190: 726d 2e69 735f 636f 6e73 7461 6e74 5f73  rm.is_constant_s
-000171a0: 7461 7469 635f 6469 6d28 293a 0a20 2020  tatic_dim():.   
-000171b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000171c0: 662e 7465 726d 735b 2d31 2069 6620 7269  f.terms[-1 if ri
-000171d0: 6768 7420 656c 7365 2030 5d20 3d20 5f4f  ght else 0] = _O
-000171e0: 704d 756c 7454 6572 6d2e 6672 6f6d 5f64  pMultTerm.from_d
-000171f0: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-00017200: 2020 2020 2020 2020 5f6d 616b 655f 636f          _make_co
-00017210: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
-00017220: 6d28 6d6f 7374 5f72 6563 656e 745f 7465  m(most_recent_te
-00017230: 726d 2e64 696d 656e 7369 6f6e 202b 2074  rm.dimension + t
-00017240: 6572 6d2e 6469 6d65 6e73 696f 6e2c 206b  erm.dimension, k
-00017250: 696e 643d 6f74 6865 722e 6b69 6e64 290a  ind=other.kind).
-00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017270: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017280: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00017290: 2020 2020 2069 6620 6d6f 7374 5f72 6563       if most_rec
-000172a0: 656e 745f 7465 726d 2e74 6572 6d73 2061  ent_term.terms a
-000172b0: 6e64 2074 6572 6d2e 7465 726d 7320 616e  nd term.terms an
-000172c0: 6420 6d6f 7374 5f72 6563 656e 745f 7465  d most_recent_te
-000172d0: 726d 2e74 6572 6d73 5b2d 315d 203d 3d20  rm.terms[-1] == 
-000172e0: 7465 726d 2e74 6572 6d73 5b2d 315d 3a0a  term.terms[-1]:.
-000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017300: 2320 4d65 7267 6520 7465 726d 730a 2020  # Merge terms.  
-00017310: 2020 2020 2020 2020 2020 2020 2020 6120                a 
-00017320: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
-00017330: 6f6d 5f64 696d 5f66 6163 746f 7273 286d  om_dim_factors(m
-00017340: 6f73 745f 7265 6365 6e74 5f74 6572 6d2e  ost_recent_term.
-00017350: 7465 726d 735b 3a2d 315d 292e 6173 5f64  terms[:-1]).as_d
-00017360: 696d 2829 0a20 2020 2020 2020 2020 2020  im().           
-00017370: 2020 2020 2062 203d 205f 4f70 4d75 6c74       b = _OpMult
-00017380: 5465 726d 2e66 726f 6d5f 6469 6d5f 6661  Term.from_dim_fa
-00017390: 6374 6f72 7328 7465 726d 2e74 6572 6d73  ctors(term.terms
-000173a0: 5b3a 2d31 5d29 2e61 735f 6469 6d28 290a  [:-1]).as_dim().
-000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173c0: 7265 7320 3d20 5f4f 704d 756c 7454 6572  res = _OpMultTer
-000173d0: 6d2e 6672 6f6d 5f64 696d 2828 6120 2b20  m.from_dim((a + 
-000173e0: 6229 2069 6620 7269 6768 7420 656c 7365  b) if right else
-000173f0: 2028 6220 2b20 6129 290a 2020 2020 2020   (b + a)).      
-00017400: 2020 2020 2020 2020 2020 7265 732e 6578            res.ex
-00017410: 7465 6e64 5f6d 756c 5f64 6976 5f28 7465  tend_mul_div_(te
-00017420: 726d 2e74 6572 6d73 5b2d 315d 2c20 6b69  rm.terms[-1], ki
-00017430: 6e64 3d22 6d75 6c22 2c20 7269 6768 743d  nd="mul", right=
-00017440: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00017450: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017460: 5b2d 3120 6966 2072 6967 6874 2065 6c73  [-1 if right els
-00017470: 6520 305d 203d 2072 6573 0a20 2020 2020  e 0] = res.     
-00017480: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017490: 6e0a 2020 2020 2020 2020 6966 2072 6967  n.        if rig
-000174a0: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-000174b0: 7365 6c66 2e74 6572 6d73 2e61 7070 656e  self.terms.appen
-000174c0: 6428 7465 726d 290a 2020 2020 2020 2020  d(term).        
-000174d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000174e0: 2020 7365 6c66 2e74 6572 6d73 2e69 6e73    self.terms.ins
-000174f0: 6572 7428 302c 2074 6572 6d29 0a0a 2020  ert(0, term)..  
-00017500: 2020 6465 6620 6578 7465 6e64 5f6d 756c    def extend_mul
-00017510: 5f64 6976 5f28 7365 6c66 2c20 6f74 6865  _div_(self, othe
-00017520: 722c 206b 696e 642c 2072 6967 6874 293a  r, kind, right):
-00017530: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00017540: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00017550: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00017560: 2020 203a 7061 7261 6d20 7374 7220 6b69     :param str ki
-00017570: 6e64 3a20 226d 756c 2220 6f72 2022 6365  nd: "mul" or "ce
-00017580: 696c 6469 7622 0a20 2020 2020 2020 203a  ildiv".        :
-00017590: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
-000175a0: 3a20 6f72 206c 6566 742e 2072 6967 6874  : or left. right
-000175b0: 206d 6561 6e73 2073 656c 6620 2a20 6f74   means self * ot
-000175c0: 6865 722c 206c 6566 7420 6d65 616e 7320  her, left means 
-000175d0: 6f74 6865 7220 2a20 7365 6c66 0a20 2020  other * self.   
-000175e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000175f0: 2061 7373 6572 7420 6b69 6e64 2069 6e20   assert kind in 
-00017600: 7b22 6d75 6c22 2c20 2266 6c6f 6f72 6469  {"mul", "floordi
-00017610: 7622 2c20 2274 7275 6564 6976 222c 2022  v", "truediv", "
-00017620: 6365 696c 6469 7622 7d0a 2020 2020 2020  ceildiv"}.      
-00017630: 2020 6f74 6865 7220 3d20 7365 6c66 2e5f    other = self._
-00017640: 6d61 6b65 5f64 696d 286f 7468 6572 2c20  make_dim(other, 
-00017650: 6b69 6e64 3d6b 696e 6429 0a20 2020 2020  kind=kind).     
-00017660: 2020 2069 6620 6b69 6e64 203d 3d20 226d     if kind == "m
-00017670: 756c 2220 616e 6420 7269 6768 743a 0a20  ul" and right:. 
-00017680: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00017690: 7420 616c 6c28 7465 726d 2e63 616e 5f73  t all(term.can_s
-000176a0: 696d 706c 6966 7928 6f74 6865 722c 206b  implify(other, k
-000176b0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-000176c0: 7269 6768 7429 2066 6f72 2074 6572 6d20  right) for term 
-000176d0: 696e 2073 656c 662e 7465 726d 7329 3a0a  in self.terms):.
-000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2320 446f 2069 7420 7468 6520 6f74 6865  # Do it the othe
-00017700: 7220 7761 7920 6172 6f75 6e64 0a20 2020  r way around.   
-00017710: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017720: 662e 7465 726d 732c 206f 7468 6572 203d  f.terms, other =
-00017730: 205f 4f70 4c69 6e65 6172 5465 726d 2e66   _OpLinearTerm.f
-00017740: 726f 6d5f 6469 6d28 6f74 6865 7229 2e74  rom_dim(other).t
-00017750: 6572 6d73 2c20 7365 6c66 2e61 735f 6469  erms, self.as_di
-00017760: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
-00017770: 2020 2020 7269 6768 7420 3d20 4661 6c73      right = Fals
-00017780: 650a 2020 2020 2020 2020 6966 206f 7468  e.        if oth
-00017790: 6572 2e69 735f 636f 6e73 7461 6e74 5f73  er.is_constant_s
-000177a0: 7461 7469 635f 6469 6d28 2920 616e 6420  tatic_dim() and 
-000177b0: 6f74 6865 722e 6469 6d65 6e73 696f 6e20  other.dimension 
-000177c0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-000177d0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-000177e0: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
-000177f0: 6828 2264 6976 2229 2061 6e64 206c 656e  h("div") and len
-00017800: 2873 656c 662e 7465 726d 7329 203e 3d20  (self.terms) >= 
-00017810: 323a 0a20 2020 2020 2020 2020 2020 2069  2:.            i
-00017820: 6620 616e 7928 6e6f 7420 7465 726d 2e64  f any(not term.d
-00017830: 6976 6973 6962 6c65 286f 7468 6572 2c20  ivisible(other, 
-00017840: 7269 6768 743d 7269 6768 7429 2066 6f72  right=right) for
-00017850: 2074 6572 6d20 696e 2073 656c 662e 7465   term in self.te
-00017860: 726d 7329 3a0a 2020 2020 2020 2020 2020  rms):.          
-00017870: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017880: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00017890: 2020 2020 2020 2020 205f 4f70 4d75 6c74           _OpMult
-000178a0: 5465 726d 2e66 726f 6d5f 6469 6d28 5f4f  Term.from_dim(_O
-000178b0: 704d 756c 7454 6572 6d2e 6e65 775f 6469  pMultTerm.new_di
-000178c0: 765f 6469 6d28 7365 6c66 2e61 735f 6469  v_dim(self.as_di
-000178d0: 6d28 292c 206f 7468 6572 2c20 6b69 6e64  m(), other, kind
-000178e0: 3d6b 696e 642c 2072 6967 6874 3d72 6967  =kind, right=rig
-000178f0: 6874 2929 0a20 2020 2020 2020 2020 2020  ht)).           
-00017900: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-00017910: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00017920: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
-00017930: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
-00017940: 2020 2020 2020 2020 2020 7465 726d 2e65            term.e
-00017950: 7874 656e 645f 6d75 6c5f 6469 765f 286f  xtend_mul_div_(o
-00017960: 7468 6572 2c20 6b69 6e64 3d6b 696e 642c  ther, kind=kind,
-00017970: 2072 6967 6874 3d72 6967 6874 290a 0a20   right=right).. 
-00017980: 2020 2064 6566 205f 6d61 6b65 5f64 696d     def _make_dim
-00017990: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
-000179a0: 6e64 293a 0a20 2020 2020 2020 2022 2222  nd):.        """
-000179b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000179c0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-000179d0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-000179e0: 7220 6b69 6e64 3a0a 2020 2020 2020 2020  r kind:.        
-000179f0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-00017a00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00017a10: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
-00017a20: 6865 722c 2069 6e74 293a 0a20 2020 2020  her, int):.     
-00017a30: 2020 2020 2020 2062 6173 655f 7461 6720         base_tag 
-00017a40: 3d20 7365 6c66 2e72 6570 7265 7365 6e74  = self.represent
-00017a50: 6174 6976 655f 7461 6728 290a 2020 2020  ative_tag().    
-00017a60: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00017a70: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-00017a80: 6174 6963 5f64 696d 286f 7468 6572 2c20  atic_dim(other, 
-00017a90: 6b69 6e64 3d62 6173 655f 7461 672e 6b69  kind=base_tag.ki
-00017aa0: 6e64 2069 6620 6261 7365 5f74 6167 2065  nd if base_tag e
-00017ab0: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
-00017ac0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00017ad0: 6528 6f74 6865 722c 205f 642e 4469 6d29  e(other, _d.Dim)
-00017ae0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00017af0: 7475 726e 206f 7468 6572 2e67 6574 5f73  turn other.get_s
-00017b00: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
-00017b10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00017b20: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-00017b30: 7272 6f72 2822 2573 2025 7320 2573 2069  rror("%s %s %s i
-00017b40: 6e76 616c 6964 2066 6f72 2074 7970 6520  nvalid for type 
-00017b50: 2573 2220 2520 2873 656c 662c 206b 696e  %s" % (self, kin
-00017b60: 642c 206f 7468 6572 2c20 7479 7065 286f  d, other, type(o
-00017b70: 7468 6572 2929 290a 0a20 2020 2064 6566  ther)))..    def
-00017b80: 2072 6570 7265 7365 6e74 6174 6976 655f   representative_
-00017b90: 7461 6728 7365 6c66 293a 0a20 2020 2020  tag(self):.     
-00017ba0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00017bb0: 7274 7970 653a 2044 696d 7c4e 6f6e 650a  rtype: Dim|None.
-00017bc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017bd0: 2020 2020 2320 4669 7273 7420 6669 6e64      # First find
-00017be0: 2061 6e79 2064 796e 616d 6963 2e0a 2020   any dynamic..  
-00017bf0: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
-00017c00: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
-00017c10: 2020 2020 2020 2020 2020 666f 7220 7465            for te
-00017c20: 726d 5f20 696e 2074 6572 6d2e 7465 726d  rm_ in term.term
-00017c30: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00017c40: 2020 2069 6620 7465 726d 5f2e 6973 5f64     if term_.is_d
-00017c50: 796e 616d 6963 2829 3a0a 2020 2020 2020  ynamic():.      
-00017c60: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00017c70: 7475 726e 2074 6572 6d5f 0a20 2020 2020  turn term_.     
-00017c80: 2020 2023 204e 6f77 2066 696e 6420 6e6f     # Now find no
-00017c90: 6e2d 756e 7370 6563 6966 6965 642e 0a20  n-unspecified.. 
-00017ca0: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
-00017cb0: 696e 2073 656c 662e 7465 726d 733a 0a20  in self.terms:. 
-00017cc0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-00017cd0: 6572 6d5f 2069 6e20 7465 726d 2e74 6572  erm_ in term.ter
-00017ce0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00017cf0: 2020 2020 6966 2074 6572 6d5f 2e6b 696e      if term_.kin
-00017d00: 6420 213d 2044 696d 5479 7065 732e 556e  d != DimTypes.Un
-00017d10: 7370 6563 6966 6965 643a 0a20 2020 2020  specified:.     
-00017d20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017d30: 6574 7572 6e20 7465 726d 5f0a 2020 2020  eturn term_.    
-00017d40: 2020 2020 2320 4e6f 7720 6669 6e64 2061      # Now find a
-00017d50: 6e79 2e0a 2020 2020 2020 2020 666f 7220  ny..        for 
-00017d60: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
-00017d70: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00017d80: 666f 7220 7465 726d 5f20 696e 2074 6572  for term_ in ter
-00017d90: 6d2e 7465 726d 733a 0a20 2020 2020 2020  m.terms:.       
-00017da0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00017db0: 7465 726d 5f0a 2020 2020 2020 2020 7265  term_.        re
-00017dc0: 7475 726e 204e 6f6e 650a 0a0a 6465 6620  turn None...def 
-00017dd0: 5f67 6574 5f6d 6572 6765 645f 6469 6d5f  _get_merged_dim_
-00017de0: 6b69 6e64 2864 696d 5f74 6167 7329 3a0a  kind(dim_tags):.
-00017df0: 2020 2020 2222 220a 2020 2020 3a70 6172      """.    :par
-00017e00: 616d 206c 6973 745b 4469 6d5d 7c74 7570  am list[Dim]|tup
-00017e10: 6c65 5b44 696d 5d20 6469 6d5f 7461 6773  le[Dim] dim_tags
-00017e20: 3a0a 2020 2020 3a72 6574 7572 6e3a 2064  :.    :return: d
-00017e30: 696d 206b 696e 640a 2020 2020 3a72 7479  im kind.    :rty
-00017e40: 7065 3a20 456e 7469 7479 0a20 2020 2022  pe: Entity.    "
-00017e50: 2222 0a20 2020 2069 6620 616e 7928 7461  "".    if any(ta
-00017e60: 672e 6973 5f62 6174 6368 5f64 696d 2829  g.is_batch_dim()
-00017e70: 2066 6f72 2074 6167 2069 6e20 6469 6d5f   for tag in dim_
-00017e80: 7461 6773 293a 0a20 2020 2020 2020 2072  tags):.        r
-00017e90: 6574 7572 6e20 4469 6d54 7970 6573 2e42  eturn DimTypes.B
-00017ea0: 6174 6368 0a20 2020 2065 6c69 6620 616e  atch.    elif an
-00017eb0: 7928 7461 672e 6973 5f66 6561 7475 7265  y(tag.is_feature
-00017ec0: 5f64 696d 2829 2066 6f72 2074 6167 2069  _dim() for tag i
-00017ed0: 6e20 6469 6d5f 7461 6773 293a 0a20 2020  n dim_tags):.   
-00017ee0: 2020 2020 2072 6574 7572 6e20 4469 6d54       return DimT
-00017ef0: 7970 6573 2e46 6561 7475 7265 0a20 2020  ypes.Feature.   
-00017f00: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-00017f10: 6574 7572 6e20 4469 6d54 7970 6573 2e53  eturn DimTypes.S
-00017f20: 7061 7469 616c 0a0a 0a64 6566 2064 696d  patial...def dim
-00017f30: 5f63 6d70 5f76 616c 7565 286f 626a 293a  _cmp_value(obj):
-00017f40: 0a20 2020 2022 2222 0a20 2020 203a 7061  .    """.    :pa
-00017f50: 7261 6d20 4469 6d7c 5f4d 6172 6b65 6444  ram Dim|_MarkedD
-00017f60: 696d 206f 626a 3a0a 2020 2020 3a72 6574  im obj:.    :ret
-00017f70: 7572 6e3a 2061 6e79 7468 696e 6720 7768  urn: anything wh
-00017f80: 6963 6820 6361 6e20 6265 2063 6f6d 7061  ich can be compa
-00017f90: 7265 640a 2020 2020 2222 220a 2020 2020  red.    """.    
-00017fa0: 2320 4d61 6b65 2044 696d 2061 6e64 205f  # Make Dim and _
-00017fb0: 4d61 726b 6564 4469 6d20 636f 6d70 6172  MarkedDim compar
-00017fc0: 6162 6c65 2074 6f20 6561 6368 206f 7468  able to each oth
-00017fd0: 6572 2e0a 2020 2020 2320 4e6f 7465 2074  er..    # Note t
-00017fe0: 6861 7420 7468 6520 6f72 6465 7220 6973  hat the order is
-00017ff0: 2072 6561 6c6c 7920 6172 6269 7472 6172   really arbitrar
-00018000: 7920 616e 6420 646f 6573 206e 6f74 206d  y and does not m
-00018010: 6174 7465 722e 0a20 2020 2069 6620 6973  atter..    if is
-00018020: 696e 7374 616e 6365 286f 626a 2c20 5f64  instance(obj, _d
-00018030: 2e44 696d 293a 0a20 2020 2020 2020 206f  .Dim):.        o
-00018040: 626a 203d 206f 626a 2e67 6574 5f73 616d  bj = obj.get_sam
-00018050: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
-00018060: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-00018070: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
-00018080: 2020 2020 2020 6f62 6a2e 6465 7363 7269        obj.descri
-00018090: 7074 696f 6e2c 0a20 2020 2020 2020 2020  ption,.         
-000180a0: 2020 206f 626a 2e6b 696e 642c 0a20 2020     obj.kind,.   
-000180b0: 2020 2020 2020 2020 206f 626a 2e64 696d           obj.dim
-000180c0: 656e 7369 6f6e 2c0a 2020 2020 2020 2020  ension,.        
-000180d0: 2020 2020 6f62 6a2e 6479 6e5f 7369 7a65      obj.dyn_size
-000180e0: 5f65 7874 2e64 696d 7320 6966 206f 626a  _ext.dims if obj
-000180f0: 2e64 796e 5f73 697a 655f 6578 7420 6973  .dyn_size_ext is
-00018100: 206e 6f74 204e 6f6e 6520 656c 7365 204e   not None else N
-00018110: 6f6e 652c 0a20 2020 2020 2020 2029 0a20  one,.        ). 
-00018120: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00018130: 286f 626a 2c20 5f6d 2e4d 6172 6b65 6444  (obj, _m.MarkedD
-00018140: 696d 293a 0a20 2020 2020 2020 2072 6574  im):.        ret
-00018150: 7572 6e20 6f62 6a2e 5f5f 636c 6173 735f  urn obj.__class_
-00018160: 5f2e 5f5f 6e61 6d65 5f5f 2c20 6f62 6a2e  _.__name__, obj.
-00018170: 7461 670a 2020 2020 7265 7475 726e 206f  tag.    return o
-00018180: 626a 0a                                  bj.
+000093b0: 6b0a 0a20 2020 2020 2020 2073 697a 655f  k..        size_
+000093c0: 6474 7970 6520 3d20 4e6f 6e65 0a20 2020  dtype = None.   
+000093d0: 2020 2020 2066 6f72 2078 2069 6e20 6f70       for x in op
+000093e0: 2e69 6e70 7574 733a 0a20 2020 2020 2020  .inputs:.       
+000093f0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+00009400: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+00009410: 2020 2020 7820 3d20 782e 6765 745f 666f      x = x.get_fo
+00009420: 725f 6261 7463 685f 6374 7828 7365 6c66  r_batch_ctx(self
+00009430: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
+00009440: 7472 6f6c 5f66 6c6f 775f 6374 7829 0a20  trol_flow_ctx). 
+00009450: 2020 2020 2020 2020 2020 2069 6620 782e             if x.
+00009460: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+00009470: 2020 2020 2020 2020 2020 2020 2020 7369                si
+00009480: 7a65 5f64 7479 7065 203d 2078 2e64 796e  ze_dtype = x.dyn
+00009490: 5f73 697a 655f 6578 742e 6474 7970 650a  _size_ext.dtype.
+000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094b0: 6272 6561 6b0a 2020 2020 2020 2020 6966  break.        if
+000094c0: 206e 6f74 2073 697a 655f 6474 7970 653a   not size_dtype:
+000094d0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+000094e0: 655f 6474 7970 6520 3d20 5f74 2e54 656e  e_dtype = _t.Ten
+000094f0: 736f 722e 7369 7a65 5f64 7479 7065 0a0a  sor.size_dtype..
+00009500: 2020 2020 2020 2020 696d 706f 7274 206e          import n
+00009510: 756d 7079 0a20 2020 2020 2020 2069 6d70  umpy.        imp
+00009520: 6f72 7420 7265 7475 726e 6e2e 6672 6f6e  ort returnn.fron
+00009530: 7465 6e64 2061 7320 7266 0a20 2020 2020  tend as rf.     
+00009540: 2020 2066 726f 6d20 7265 7475 726e 6e2e     from returnn.
+00009550: 7465 6e73 6f72 2069 6d70 6f72 7420 5465  tensor import Te
+00009560: 6e73 6f72 0a0a 2020 2020 2020 2020 7466  nsor..        tf
+00009570: 203d 2074 665f 7574 696c 203d 2074 656e   = tf_util = ten
+00009580: 736f 725f 7574 696c 203d 204e 6f6e 650a  sor_util = None.
+00009590: 2020 2020 2020 2020 6966 2062 6163 6b65          if backe
+000095a0: 6e64 2061 6e64 2062 6163 6b65 6e64 2e69  nd and backend.i
+000095b0: 735f 7465 6e73 6f72 666c 6f77 3a0a 2020  s_tensorflow:.  
+000095c0: 2020 2020 2020 2020 2020 696d 706f 7274            import
+000095d0: 2074 656e 736f 7266 6c6f 7720 6173 2074   tensorflow as t
+000095e0: 660a 0a20 2020 2020 2020 2020 2020 2069  f..            i
+000095f0: 6620 6261 636b 656e 642e 5261 7754 656e  f backend.RawTen
+00009600: 736f 7254 7970 6520 3d3d 2074 662e 5465  sorType == tf.Te
+00009610: 6e73 6f72 3a0a 2020 2020 2020 2020 2020  nsor:.          
+00009620: 2020 2020 2020 6672 6f6d 2072 6574 7572        from retur
+00009630: 6e6e 2e74 662e 7574 696c 2069 6d70 6f72  nn.tf.util impor
+00009640: 7420 6261 7369 6320 6173 2074 665f 7574  t basic as tf_ut
+00009650: 696c 0a20 2020 2020 2020 2020 2020 2020  il.             
+00009660: 2020 2066 726f 6d20 7465 6e73 6f72 666c     from tensorfl
+00009670: 6f77 2e70 7974 686f 6e2e 6672 616d 6577  ow.python.framew
+00009680: 6f72 6b20 696d 706f 7274 2074 656e 736f  ork import tenso
+00009690: 725f 7574 696c 0a20 2020 2020 2020 2020  r_util.         
+000096a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000096b0: 2020 2020 2020 2020 2074 6620 3d20 4e6f           tf = No
+000096c0: 6e65 0a0a 2020 2020 2020 2020 6b69 6e64  ne..        kind
+000096d0: 203d 206f 702e 6b69 6e64 0a20 2020 2020   = op.kind.     
+000096e0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
+000096f0: 6974 6828 225f 7269 6768 7422 293a 0a20  ith("_right"):. 
+00009700: 2020 2020 2020 2020 2020 206b 696e 6420             kind 
+00009710: 3d20 6b69 6e64 5b3a 202d 6c65 6e28 225f  = kind[: -len("_
+00009720: 7269 6768 7422 295d 2020 2320 6f72 6465  right")]  # orde
+00009730: 7220 646f 6573 206e 6f74 206d 6174 7465  r does not matte
+00009740: 7220 6865 7265 0a20 2020 2020 2020 2069  r here.        i
+00009750: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
+00009760: 225f 6c65 6674 2229 3a0a 2020 2020 2020  "_left"):.      
+00009770: 2020 2020 2020 6b69 6e64 203d 206b 696e        kind = kin
+00009780: 645b 3a20 2d6c 656e 2822 5f6c 6566 7422  d[: -len("_left"
+00009790: 295d 0a0a 2020 2020 2020 2020 6465 6620  )]..        def 
+000097a0: 5f69 735f 6e65 6761 7469 7665 2878 5f5f  _is_negative(x__
+000097b0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+000097c0: 6620 6973 696e 7374 616e 6365 2878 5f5f  f isinstance(x__
+000097d0: 2c20 6e75 6d70 792e 6e64 6172 7261 7929  , numpy.ndarray)
+000097e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000097f0: 2020 7265 7475 726e 2028 785f 5f20 3c20    return (x__ < 
+00009800: 3029 2e61 6e79 2829 0a20 2020 2020 2020  0).any().       
+00009810: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00009820: 6365 2878 5f5f 2c20 2869 6e74 2c20 666c  ce(x__, (int, fl
+00009830: 6f61 742c 206e 756d 7079 2e6e 756d 6265  oat, numpy.numbe
+00009840: 7229 293a 0a20 2020 2020 2020 2020 2020  r)):.           
+00009850: 2020 2020 2072 6574 7572 6e20 785f 5f20       return x__ 
+00009860: 3c20 300a 2020 2020 2020 2020 2020 2020  < 0.            
+00009870: 6966 206e 6f74 2074 663a 0a20 2020 2020  if not tf:.     
+00009880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009890: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+000098a0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+000098b0: 7461 6e63 6528 785f 5f2c 2074 662e 5465  tance(x__, tf.Te
+000098c0: 6e73 6f72 290a 2020 2020 2020 2020 2020  nsor).          
+000098d0: 2020 785f 5f20 3d20 7465 6e73 6f72 5f75    x__ = tensor_u
+000098e0: 7469 6c2e 636f 6e73 7461 6e74 5f76 616c  til.constant_val
+000098f0: 7565 2878 5f5f 290a 2020 2020 2020 2020  ue(x__).        
+00009900: 2020 2020 6966 2078 5f5f 2069 7320 6e6f      if x__ is no
+00009910: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009920: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00009930: 6973 5f6e 6567 6174 6976 6528 785f 5f29  is_negative(x__)
+00009940: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009950: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
+00009960: 2020 2064 6566 205f 6269 6e5f 6f70 5f74     def _bin_op_t
+00009970: 6628 612c 2062 293a 0a20 2020 2020 2020  f(a, b):.       
+00009980: 2020 2020 2069 6620 7465 6d70 6c61 7465       if template
+00009990: 5f6f 6e6c 793a 0a20 2020 2020 2020 2020  _only:.         
+000099a0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000099b0: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
+000099c0: 6620 6120 6973 204e 6f6e 6520 6f72 2062  f a is None or b
+000099d0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000099e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000099f0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00009a00: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00009a10: 6e63 6528 612c 2074 662e 5465 6e73 6f72  nce(a, tf.Tensor
+00009a20: 2920 616e 6420 6973 696e 7374 616e 6365  ) and isinstance
+00009a30: 2862 2c20 2869 6e74 2c20 7466 2e54 656e  (b, (int, tf.Ten
+00009a40: 736f 7229 290a 2020 2020 2020 2020 2020  sor)).          
+00009a50: 2020 7769 7468 2074 665f 7574 696c 2e73    with tf_util.s
+00009a60: 616d 655f 636f 6e74 726f 6c5f 666c 6f77  ame_control_flow
+00009a70: 5f63 7478 285b 612c 2062 5d29 3a0a 2020  _ctx([a, b]):.  
+00009a80: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009a90: 206b 696e 6420 3d3d 2022 6164 6422 3a0a   kind == "add":.
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 7573 655f 7265 6c75 203d 205f      use_relu = _
+00009ac0: 6973 5f6e 6567 6174 6976 6528 6129 206f  is_negative(a) o
+00009ad0: 7220 5f69 735f 6e65 6761 7469 7665 2862  r _is_negative(b
+00009ae0: 2920 2023 2066 6f72 2064 796e 616d 6963  )  # for dynamic
+00009af0: 2074 656e 736f 7273 2c20 6173 7375 6d65   tensors, assume
+00009b00: 2061 6c6c 2070 6f73 6974 6976 650a 2020   all positive.  
+00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 2020 6966 2075 7365 5f72 656c 753a 0a20    if use_relu:. 
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b40: 2020 2020 2020 2072 6574 7572 6e20 7466         return tf
+00009b50: 2e63 6f6e 7665 7274 5f74 6f5f 7465 6e73  .convert_to_tens
+00009b60: 6f72 2874 665f 7574 696c 2e73 696d 706c  or(tf_util.simpl
+00009b70: 6966 795f 6e6f 6e5f 6e65 6761 7469 7665  ify_non_negative
+00009b80: 5f73 6571 5f6c 656e 6774 6828 6120 2b20  _seq_length(a + 
+00009b90: 6229 290a 2020 2020 2020 2020 2020 2020  b)).            
+00009ba0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00009bb0: 202b 2062 0a20 2020 2020 2020 2020 2020   + b.           
+00009bc0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+00009bd0: 3d20 2273 7562 223a 0a20 2020 2020 2020  = "sub":.       
+00009be0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00009bf0: 7572 6e20 7466 2e63 6f6e 7665 7274 5f74  urn tf.convert_t
+00009c00: 6f5f 7465 6e73 6f72 2874 665f 7574 696c  o_tensor(tf_util
+00009c10: 2e73 696d 706c 6966 795f 6e6f 6e5f 6e65  .simplify_non_ne
+00009c20: 6761 7469 7665 5f73 6571 5f6c 656e 6774  gative_seq_lengt
+00009c30: 6828 6120 2d20 6229 290a 2020 2020 2020  h(a - b)).      
+00009c40: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+00009c50: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
+00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c70: 2020 7265 7475 726e 2061 202a 2062 0a20    return a * b. 
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00009c90: 6c69 6620 6b69 6e64 2069 6e20 2822 666c  lif kind in ("fl
+00009ca0: 6f6f 7264 6976 222c 2022 7472 7565 6469  oordiv", "truedi
+00009cb0: 7622 293a 2020 2320 7472 7565 6469 7620  v"):  # truediv 
+00009cc0: 6173 7375 6d65 7320 7468 6572 6520 6973  assumes there is
+00009cd0: 206e 6f20 7265 6d61 696e 6465 720a 2020   no remainder.  
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 7265 7475 726e 2061 202f 2f20 620a    return a // b.
+00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d10: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
+00009d20: 696c 6469 7622 3a0a 2020 2020 2020 2020  ildiv":.        
+00009d30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009d40: 726e 202d 282d 6120 2f2f 2062 290a 2020  rn -(-a // b).  
+00009d50: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009d60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009d70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00009d80: 6c75 6545 7272 6f72 2822 756e 6b6e 6f77  lueError("unknow
+00009d90: 6e20 6f70 206b 696e 6420 2572 2220 2520  n op kind %r" % 
+00009da0: 6f70 2e6b 696e 6429 0a0a 2020 2020 2020  op.kind)..      
+00009db0: 2020 6465 6620 5f62 696e 5f6f 7028 612c    def _bin_op(a,
+00009dc0: 2062 293a 0a20 2020 2020 2020 2020 2020   b):.           
+00009dd0: 2069 6620 7465 6d70 6c61 7465 5f6f 6e6c   if template_onl
+00009de0: 7920 6f72 206e 6f74 2062 6163 6b65 6e64  y or not backend
+00009df0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009e00: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00009e10: 612c 205f 742e 5465 6e73 6f72 2920 616e  a, _t.Tensor) an
+00009e20: 6420 6973 696e 7374 616e 6365 2862 2c20  d isinstance(b, 
+00009e30: 5f74 2e54 656e 736f 7229 3a0a 2020 2020  _t.Tensor):.    
+00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e50: 7265 7475 726e 205f 742e 5465 6e73 6f72  return _t.Tensor
+00009e60: 2e67 6574 5f63 6f6d 6d6f 6e5f 6461 7461  .get_common_data
+00009e70: 285b 612c 2062 5d2c 2061 6c6c 6f77 5f62  ([a, b], allow_b
+00009e80: 726f 6164 6361 7374 5f61 6c6c 5f73 6f75  roadcast_all_sou
+00009e90: 7263 6573 3d54 7275 6529 0a20 2020 2020  rces=True).     
+00009ea0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00009eb0: 696e 7374 616e 6365 2861 2c20 5f74 2e54  instance(a, _t.T
+00009ec0: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
+00009ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009ee0: 726e 2061 0a20 2020 2020 2020 2020 2020  rn a.           
+00009ef0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00009f00: 6365 2862 2c20 5f74 2e54 656e 736f 7229  ce(b, _t.Tensor)
+00009f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009f20: 2020 2020 2020 7265 7475 726e 2062 0a20        return b. 
+00009f30: 2020 2020 2020 2020 2020 2069 6620 6b69             if ki
+00009f40: 6e64 203d 3d20 2261 6464 223a 0a20 2020  nd == "add":.   
+00009f50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00009f60: 7572 6e20 6120 2b20 620a 2020 2020 2020  urn a + b.      
+00009f70: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
+00009f80: 3d3d 2022 7375 6222 3a0a 2020 2020 2020  == "sub":.      
+00009f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009fa0: 2061 202d 2062 0a20 2020 2020 2020 2020   a - b.         
+00009fb0: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
+00009fc0: 226d 756c 223a 0a20 2020 2020 2020 2020  "mul":.         
+00009fd0: 2020 2020 2020 2072 6574 7572 6e20 6120         return a 
+00009fe0: 2a20 620a 2020 2020 2020 2020 2020 2020  * b.            
+00009ff0: 656c 6966 206b 696e 6420 696e 2028 2266  elif kind in ("f
+0000a000: 6c6f 6f72 6469 7622 2c20 2274 7275 6564  loordiv", "trued
+0000a010: 6976 2229 3a20 2023 2074 7275 6564 6976  iv"):  # truediv
+0000a020: 2061 7373 756d 6573 2074 6865 7265 2069   assumes there i
+0000a030: 7320 6e6f 2072 656d 6169 6e64 6572 0a20  s no remainder. 
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a050: 6574 7572 6e20 6120 2f2f 2062 0a20 2020  eturn a // b.   
+0000a060: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
+0000a070: 6e64 203d 3d20 2263 6569 6c64 6976 223a  nd == "ceildiv":
+0000a080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a090: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+0000a0a0: 2c20 5465 6e73 6f72 293a 0a20 2020 2020  , Tensor):.     
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a0c0: 6574 7572 6e20 7266 2e63 6569 6c5f 6469  eturn rf.ceil_di
+0000a0d0: 7669 6465 2861 2c20 6229 0a20 2020 2020  vide(a, b).     
+0000a0e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a0f0: 6e20 2d28 2d61 202f 2f20 6229 0a20 2020  n -(-a // b).   
+0000a100: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a120: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000a130: 2275 6e6b 6e6f 776e 206f 7020 6b69 6e64  "unknown op kind
+0000a140: 2025 7222 2025 206f 702e 6b69 6e64 290a   %r" % op.kind).
+0000a150: 0a20 2020 2020 2020 2079 5f6e 616d 6520  .        y_name 
+0000a160: 3d20 7365 6c66 2e64 6573 6372 6970 7469  = self.descripti
+0000a170: 6f6e 202b 2022 3a73 6571 2d6c 656e 6774  on + ":seq-lengt
+0000a180: 6822 0a20 2020 2020 2020 2079 3a20 4f70  h".        y: Op
+0000a190: 7469 6f6e 616c 5b5f 742e 5465 6e73 6f72  tional[_t.Tensor
+0000a1a0: 5d20 3d20 4e6f 6e65 2020 2320 7265 7375  ] = None  # resu
+0000a1b0: 6c74 696e 6720 6479 6e20 7369 7a65 0a20  lting dyn size. 
+0000a1c0: 2020 2020 2020 2069 6e70 7574 7320 3d20         inputs = 
+0000a1d0: 6c69 7374 286f 702e 696e 7075 7473 290a  list(op.inputs).
+0000a1e0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+0000a1f0: 6e70 7574 730a 2020 2020 2020 2020 7768  nputs.        wh
+0000a200: 696c 6520 696e 7075 7473 3a0a 2020 2020  ile inputs:.    
+0000a210: 2020 2020 2020 2020 7820 3d20 696e 7075          x = inpu
+0000a220: 7473 2e70 6f70 2830 290a 2020 2020 2020  ts.pop(0).      
+0000a230: 2020 2020 2020 6966 206e 6f74 2078 2e69        if not x.i
+0000a240: 735f 6479 6e61 6d69 6328 293a 2020 2320  s_dynamic():  # 
+0000a250: 7374 6174 6963 0a20 2020 2020 2020 2020  static.         
+0000a260: 2020 2020 2020 2061 7373 6572 7420 782e         assert x.
+0000a270: 6469 6d65 6e73 696f 6e20 6973 206e 6f74  dimension is not
+0000a280: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000a290: 2020 2020 2020 6966 2079 2069 7320 4e6f        if y is No
+0000a2a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a2b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
+0000a2c0: 656d 706c 6174 655f 6f6e 6c79 2061 6e64  emplate_only and
+0000a2d0: 2062 6163 6b65 6e64 2061 6e64 206e 6f74   backend and not
+0000a2e0: 2074 663a 0a20 2020 2020 2020 2020 2020   tf:.           
+0000a2f0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+0000a300: 2062 6163 6b65 6e64 2e63 6f6e 7665 7274   backend.convert
+0000a310: 5f74 6f5f 7465 6e73 6f72 2878 2e64 696d  _to_tensor(x.dim
+0000a320: 656e 7369 6f6e 2c20 6469 6d73 3d5b 5d2c  ension, dims=[],
+0000a330: 2064 7479 7065 3d73 697a 655f 6474 7970   dtype=size_dtyp
+0000a340: 652c 206e 616d 653d 795f 6e61 6d65 290a  e, name=y_name).
+0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a360: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 7920 3d20 5f74 2e54 656e 736f 7228    y = _t.Tensor(
+0000a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a3a0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0000a3b0: 653d 795f 6e61 6d65 2c0a 2020 2020 2020  e=y_name,.      
+0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3d0: 2020 2020 2020 6469 6d5f 7461 6773 3d5b        dim_tags=[
+0000a3e0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000a400: 7479 7065 3d73 697a 655f 6474 7970 652c  type=size_dtype,
+0000a410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a420: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a440: 2020 2069 6620 6e6f 7420 7465 6d70 6c61     if not templa
+0000a450: 7465 5f6f 6e6c 7920 616e 6420 7466 3a0a  te_only and tf:.
+0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a470: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000a480: 2074 662e 636f 6e74 726f 6c5f 6465 7065   tf.control_depe
+0000a490: 6e64 656e 6369 6573 284e 6f6e 6529 3a20  ndencies(None): 
+0000a4a0: 2023 2074 6869 7320 7769 6c6c 2072 6573   # this will res
+0000a4b0: 6574 2074 6865 2063 6f6e 7465 7874 0a20  et the context. 
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+0000a4e0: 2e72 6177 5f74 656e 736f 7220 3d20 7466  .raw_tensor = tf
+0000a4f0: 2e63 6f6e 7374 616e 7428 782e 6469 6d65  .constant(x.dime
+0000a500: 6e73 696f 6e29 0a20 2020 2020 2020 2020  nsion).         
+0000a510: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000a520: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0000a530: 2020 2020 6966 2074 663a 0a20 2020 2020      if tf:.     
+0000a540: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+0000a550: 2e70 6c61 6365 686f 6c64 6572 203d 205f  .placeholder = _
+0000a560: 6269 6e5f 6f70 5f74 6628 792e 706c 6163  bin_op_tf(y.plac
+0000a570: 6568 6f6c 6465 722c 2078 2e64 696d 656e  eholder, x.dimen
+0000a580: 7369 6f6e 290a 2020 2020 2020 2020 2020  sion).          
+0000a590: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5b0: 7920 3d20 5f62 696e 5f6f 7028 792c 2078  y = _bin_op(y, x
+0000a5c0: 2e64 696d 656e 7369 6f6e 290a 2020 2020  .dimension).    
+0000a5d0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000a5e0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000a5f0: 2069 6620 7365 6c66 2e62 6174 6368 3a0a   if self.batch:.
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 7820 3d20 782e 6765 745f 666f 725f 6261  x = x.get_for_ba
+0000a620: 7463 685f 6374 7828 7365 6c66 2e62 6174  tch_ctx(self.bat
+0000a630: 6368 2c20 7365 6c66 2e63 6f6e 7472 6f6c  ch, self.control
+0000a640: 5f66 6c6f 775f 6374 7829 0a20 2020 2020  _flow_ctx).     
+0000a650: 2020 2020 2020 2078 2e63 6f6d 706c 6574         x.complet
+0000a660: 655f 6479 6e5f 7369 7a65 2874 656d 706c  e_dyn_size(templ
+0000a670: 6174 655f 6f6e 6c79 3d74 656d 706c 6174  ate_only=templat
+0000a680: 655f 6f6e 6c79 290a 2020 2020 2020 2020  e_only).        
+0000a690: 2020 2020 6966 206e 6f74 2078 2e64 796e      if not x.dyn
+0000a6a0: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+0000a6b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a6c0: 6e0a 2020 2020 2020 2020 2020 2020 7820  n.            x 
+0000a6d0: 3d20 782e 6479 6e5f 7369 7a65 5f65 7874  = x.dyn_size_ext
+0000a6e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a6f0: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
+0000a700: 2020 2020 2020 2020 2020 2079 203d 2078             y = x
+0000a710: 2e63 6f70 7928 6e61 6d65 3d79 5f6e 616d  .copy(name=y_nam
+0000a720: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000a730: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0000a740: 2020 2020 2020 2020 6966 2078 2e64 696d          if x.dim
+0000a750: 5f74 6167 7320 213d 2079 2e64 696d 5f74  _tags != y.dim_t
+0000a760: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+0000a770: 2020 2020 2063 6f6d 6d6f 6e20 3d20 5f74       common = _t
+0000a780: 2e54 656e 736f 722e 6765 745f 636f 6d6d  .Tensor.get_comm
+0000a790: 6f6e 5f64 6174 6128 5b78 2c20 795d 2c20  on_data([x, y], 
+0000a7a0: 616c 6c6f 775f 6272 6f61 6463 6173 745f  allow_broadcast_
+0000a7b0: 616c 6c5f 736f 7572 6365 733d 5472 7565  all_sources=True
+0000a7c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a7d0: 2020 785f 203d 2078 2e63 6f70 795f 636f    x_ = x.copy_co
+0000a7e0: 6d70 6174 6962 6c65 5f74 6f28 636f 6d6d  mpatible_to(comm
+0000a7f0: 6f6e 2920 6966 2078 2e64 696d 5f74 6167  on) if x.dim_tag
+0000a800: 7320 656c 7365 2078 0a20 2020 2020 2020  s else x.       
+0000a810: 2020 2020 2020 2020 2079 5f20 3d20 792e           y_ = y.
+0000a820: 636f 7079 5f63 6f6d 7061 7469 626c 655f  copy_compatible_
+0000a830: 746f 2863 6f6d 6d6f 6e29 2069 6620 792e  to(common) if y.
+0000a840: 6469 6d5f 7461 6773 2065 6c73 6520 790a  dim_tags else y.
+0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a860: 7920 3d20 636f 6d6d 6f6e 0a20 2020 2020  y = common.     
+0000a870: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a880: 2020 2020 2020 2020 2020 2020 2078 5f2c               x_,
+0000a890: 2079 5f20 3d20 782c 2079 0a20 2020 2020   y_ = x, y.     
+0000a8a0: 2020 2020 2020 2069 6620 7466 3a0a 2020         if tf:.  
+0000a8b0: 2020 2020 2020 2020 2020 2020 2020 792e                y.
+0000a8c0: 706c 6163 6568 6f6c 6465 7220 3d20 5f62  placeholder = _b
+0000a8d0: 696e 5f6f 705f 7466 2879 5f2e 706c 6163  in_op_tf(y_.plac
+0000a8e0: 6568 6f6c 6465 722c 2078 5f2e 706c 6163  eholder, x_.plac
+0000a8f0: 6568 6f6c 6465 7229 0a20 2020 2020 2020  eholder).       
+0000a900: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000a910: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
+0000a920: 6269 6e5f 6f70 2879 5f2c 2078 5f29 0a20  bin_op(y_, x_). 
+0000a930: 2020 2020 2020 2061 7373 6572 7420 792c         assert y,
+0000a940: 2066 226f 7020 7b6f 707d 3f22 0a20 2020   f"op {op}?".   
+0000a950: 2020 2020 2069 6620 7365 6c66 2e64 796e       if self.dyn
+0000a960: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+0000a970: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000a980: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
+0000a990: 6469 6d5f 7461 6773 203d 3d20 792e 6469  dim_tags == y.di
+0000a9a0: 6d5f 7461 6773 0a20 2020 2020 2020 2069  m_tags.        i
+0000a9b0: 6620 792e 6261 7463 683a 0a20 2020 2020  f y.batch:.     
+0000a9c0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0000a9d0: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+0000a9e0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+0000a9f0: 662e 6261 7463 6820 3d3d 2079 2e62 6174  f.batch == y.bat
+0000aa00: 6368 0a20 2020 2020 2020 2020 2020 2065  ch.            e
+0000aa10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000aa20: 2020 2020 2073 656c 662e 6261 7463 6820       self.batch 
+0000aa30: 3d20 792e 6261 7463 680a 2020 2020 2020  = y.batch.      
+0000aa40: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+0000aa50: 6578 7420 3d20 790a 2020 2020 2020 2020  ext = y.        
+0000aa60: 6966 2074 6620 616e 6420 792e 706c 6163  if tf and y.plac
+0000aa70: 6568 6f6c 6465 7220 6973 206e 6f74 204e  eholder is not N
+0000aa80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000aa90: 2073 656c 662e 7365 745f 7461 675f 6f6e   self.set_tag_on
+0000aaa0: 5f73 697a 655f 7465 6e73 6f72 2879 2e70  _size_tensor(y.p
+0000aab0: 6c61 6365 686f 6c64 6572 290a 0a20 2020  laceholder)..   
+0000aac0: 2064 6566 2069 735f 6571 7561 6c28 0a20   def is_equal(. 
+0000aad0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000aae0: 2020 2020 206f 7468 6572 2c0a 2020 2020       other,.    
+0000aaf0: 2020 2020 6967 6e6f 7265 5f66 6561 7475      ignore_featu
+0000ab00: 7265 5f64 696d 3d46 616c 7365 2c0a 2020  re_dim=False,.  
+0000ab10: 2020 2020 2020 616c 6c6f 775f 7361 6d65        allow_same
+0000ab20: 5f66 6561 7475 7265 5f64 696d 3d46 616c  _feature_dim=Fal
+0000ab30: 7365 2c0a 2020 2020 2020 2020 616c 6c6f  se,.        allo
+0000ab40: 775f 7361 6d65 5f73 7061 7469 616c 5f64  w_same_spatial_d
+0000ab50: 696d 3d4e 6f6e 652c 0a20 2020 2020 2020  im=None,.       
+0000ab60: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
+0000ab70: 735f 7370 6174 6961 6c3d 4661 6c73 652c  s_spatial=False,
+0000ab80: 0a20 2020 2020 2020 2062 726f 6164 6361  .        broadca
+0000ab90: 7374 5f6d 6174 6368 6573 3d46 616c 7365  st_matches=False
+0000aba0: 2c0a 2020 2020 2020 2020 756e 6b6e 6f77  ,.        unknow
+0000abb0: 6e5f 7370 6174 6961 6c5f 6d61 7463 6865  n_spatial_matche
+0000abc0: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
+0000abd0: 2075 6e64 6566 696e 6564 5f6d 6174 6368   undefined_match
+0000abe0: 6573 3d46 616c 7365 2c0a 2020 2020 2020  es=False,.      
+0000abf0: 2020 6465 7269 7665 645f 6d61 7463 6865    derived_matche
+0000ac00: 733d 4661 6c73 652c 0a20 2020 2029 3a0a  s=False,.    ):.
+0000ac10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000ac20: 2020 2020 436f 6d70 6172 6573 2073 656c      Compares sel
+0000ac30: 6620 746f 206f 7468 6572 2066 6f72 2065  f to other for e
+0000ac40: 7175 616c 6974 792e 0a0a 2020 2020 2020  quality...      
+0000ac50: 2020 4e6f 7465 2074 6861 7420 7468 6520    Note that the 
+0000ac60: 6465 6661 756c 7420 6265 6861 7669 6f72  default behavior
+0000ac70: 2069 7320 7665 7279 2072 6573 7472 6963   is very restric
+0000ac80: 7469 7665 2e0a 2020 2020 2020 2020 5573  tive..        Us
+0000ac90: 6520 6675 6e63 7469 6f6e 7320 7375 6368  e functions such
+0000aca0: 2061 7320 3a66 756e 633a 6067 6574 5f61   as :func:`get_a
+0000acb0: 6c6c 5f64 696d 656e 7369 6f6e 5f74 6167  ll_dimension_tag
+0000acc0: 7360 206f 7220 3a66 756e 633a 6067 6574  s` or :func:`get
+0000acd0: 5f65 7869 7374 696e 675f 7461 675f 6672  _existing_tag_fr
+0000ace0: 6f6d 5f63 6f6c 6c65 6374 696f 6e60 0a20  om_collection`. 
+0000acf0: 2020 2020 2020 2074 6f20 6578 706c 6963         to explic
+0000ad00: 6974 6c79 2073 7065 6369 6679 2074 6865  itly specify the
+0000ad10: 2062 6568 6176 696f 7220 666f 7220 7468   behavior for th
+0000ad20: 6520 636f 6d70 6172 6973 6f6e 2e0a 0a20  e comparison... 
+0000ad30: 2020 2020 2020 2041 6c73 6f20 6e6f 7465         Also note
+0000ad40: 2074 6861 7420 7468 6520 6465 6669 6e69   that the defini
+0000ad50: 7469 6f6e 2069 7320 736c 6967 6874 6c79  tion is slightly
+0000ad60: 2061 642d 686f 6320 666f 7220 736f 6d65   ad-hoc for some
+0000ad70: 2063 6173 6573 2c0a 2020 2020 2020 2020   cases,.        
+0000ad80: 616e 6420 6d69 6768 7420 706f 7465 6e74  and might potent
+0000ad90: 6961 6c6c 7920 6368 616e 6765 2069 6e20  ially change in 
+0000ada0: 7468 6520 6675 7475 7265 2e0a 2020 2020  the future..    
+0000adb0: 2020 2020 2020 6874 7470 733a 2f2f 6769        https://gi
+0000adc0: 7468 7562 2e63 6f6d 2f72 7774 682d 6936  thub.com/rwth-i6
+0000add0: 2f72 6574 7572 6e6e 2f69 7373 7565 732f  /returnn/issues/
+0000ade0: 3633 340a 0a20 2020 2020 2020 203a 7061  634..        :pa
+0000adf0: 7261 6d20 4469 6d20 6f74 6865 723a 0a20  ram Dim other:. 
+0000ae00: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+0000ae10: 6f6c 2069 676e 6f72 655f 6665 6174 7572  ol ignore_featur
+0000ae20: 655f 6469 6d3a 0a20 2020 2020 2020 203a  e_dim:.        :
+0000ae30: 7061 7261 6d20 626f 6f6c 2061 6c6c 6f77  param bool allow
+0000ae40: 5f73 616d 655f 6665 6174 7572 655f 6469  _same_feature_di
+0000ae50: 6d3a 0a20 2020 2020 2020 203a 7061 7261  m:.        :para
+0000ae60: 6d20 626f 6f6c 7c4e 6f6e 6520 616c 6c6f  m bool|None allo
+0000ae70: 775f 7361 6d65 5f73 7061 7469 616c 5f64  w_same_spatial_d
+0000ae80: 696d 3a0a 2020 2020 2020 2020 3a70 6172  im:.        :par
+0000ae90: 616d 2062 6f6f 6c20 7472 6561 745f 6665  am bool treat_fe
+0000aea0: 6174 7572 655f 6173 5f73 7061 7469 616c  ature_as_spatial
+0000aeb0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+0000aec0: 2062 6f6f 6c20 6272 6f61 6463 6173 745f   bool broadcast_
+0000aed0: 6d61 7463 6865 733a 0a20 2020 2020 2020  matches:.       
+0000aee0: 203a 7061 7261 6d20 626f 6f6c 2075 6e6b   :param bool unk
+0000aef0: 6e6f 776e 5f73 7061 7469 616c 5f6d 6174  nown_spatial_mat
+0000af00: 6368 6573 3a0a 2020 2020 2020 2020 3a70  ches:.        :p
+0000af10: 6172 616d 2062 6f6f 6c20 756e 6465 6669  aram bool undefi
+0000af20: 6e65 645f 6d61 7463 6865 733a 0a20 2020  ned_matches:.   
+0000af30: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+0000af40: 2064 6572 6976 6564 5f6d 6174 6368 6573   derived_matches
+0000af50: 3a0a 2020 2020 2020 2020 3a72 7479 7065  :.        :rtype
+0000af60: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+0000af70: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
+0000af80: 7265 7475 726e 6e2e 7574 696c 2069 6d70  returnn.util imp
+0000af90: 6f72 7420 4265 6861 7669 6f72 5665 7273  ort BehaviorVers
+0000afa0: 696f 6e0a 0a20 2020 2020 2020 2069 6620  ion..        if 
+0000afb0: 7365 6c66 2069 7320 6f74 6865 723a 2020  self is other:  
+0000afc0: 2320 6669 7273 7420 736f 6d65 2066 6173  # first some fas
+0000afd0: 7420 7061 7468 2063 6865 636b 0a20 2020  t path check.   
+0000afe0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000aff0: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+0000b000: 7365 6c66 2e73 7065 6369 616c 206f 7220  self.special or 
+0000b010: 6f74 6865 722e 7370 6563 6961 6c3a 0a20  other.special:. 
+0000b020: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b030: 6e20 4661 6c73 6520 2023 206f 6e6c 7920  n False  # only 
+0000b040: 7472 7565 2069 6620 7361 6d65 2069 6e73  true if same ins
+0000b050: 7461 6e63 652c 2063 6865 636b 2061 626f  tance, check abo
+0000b060: 7665 0a20 2020 2020 2020 2069 6620 616c  ve.        if al
+0000b070: 6c6f 775f 7361 6d65 5f73 7061 7469 616c  low_same_spatial
+0000b080: 5f64 696d 2069 7320 4e6f 6e65 3a0a 2020  _dim is None:.  
+0000b090: 2020 2020 2020 2020 2020 616c 6c6f 775f            allow_
+0000b0a0: 7361 6d65 5f73 7061 7469 616c 5f64 696d  same_spatial_dim
+0000b0b0: 203d 2061 6c6c 6f77 5f73 616d 655f 6665   = allow_same_fe
+0000b0c0: 6174 7572 655f 6469 6d0a 2020 2020 2020  ature_dim.      
+0000b0d0: 2020 7365 6c66 5f62 6173 6520 3d20 7365    self_base = se
+0000b0e0: 6c66 2e67 6574 5f73 616d 655f 6465 7269  lf.get_same_deri
+0000b0f0: 7665 645f 6261 7365 2829 2069 6620 6465  ved_base() if de
+0000b100: 7269 7665 645f 6d61 7463 6865 7320 656c  rived_matches el
+0000b110: 7365 2073 656c 662e 6765 745f 7361 6d65  se self.get_same
+0000b120: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
+0000b130: 6f74 6865 725f 6261 7365 203d 206f 7468  other_base = oth
+0000b140: 6572 2e67 6574 5f73 616d 655f 6465 7269  er.get_same_deri
+0000b150: 7665 645f 6261 7365 2829 2069 6620 6465  ved_base() if de
+0000b160: 7269 7665 645f 6d61 7463 6865 7320 656c  rived_matches el
+0000b170: 7365 206f 7468 6572 2e67 6574 5f73 616d  se other.get_sam
+0000b180: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
+0000b190: 2069 6620 7365 6c66 5f62 6173 6520 6973   if self_base is
+0000b1a0: 206f 7468 6572 5f62 6173 653a 0a20 2020   other_base:.   
+0000b1b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000b1c0: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+0000b1d0: 7365 6c66 5f62 6173 652e 6465 7269 7665  self_base.derive
+0000b1e0: 645f 6672 6f6d 5f6f 7020 616e 6420 6f74  d_from_op and ot
+0000b1f0: 6865 725f 6261 7365 2e64 6572 6976 6564  her_base.derived
+0000b200: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
+0000b210: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
+0000b220: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
+0000b230: 6f70 203d 3d20 6f74 6865 725f 6261 7365  op == other_base
+0000b240: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000b250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b260: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b270: 2020 2020 2020 7365 6c66 5f6b 696e 6420        self_kind 
+0000b280: 3d20 7365 6c66 2e6b 696e 640a 2020 2020  = self.kind.    
+0000b290: 2020 2020 6f74 6865 725f 6b69 6e64 203d      other_kind =
+0000b2a0: 206f 7468 6572 2e6b 696e 640a 2020 2020   other.kind.    
+0000b2b0: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
+0000b2c0: 203d 3d20 6f74 6865 725f 6b69 6e64 203d   == other_kind =
+0000b2d0: 3d20 4469 6d54 7970 6573 2e46 6561 7475  = DimTypes.Featu
+0000b2e0: 7265 2061 6e64 2069 676e 6f72 655f 6665  re and ignore_fe
+0000b2f0: 6174 7572 655f 6469 6d3a 0a20 2020 2020  ature_dim:.     
+0000b300: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0000b310: 7565 0a20 2020 2020 2020 2069 6620 7472  ue.        if tr
+0000b320: 6561 745f 6665 6174 7572 655f 6173 5f73  eat_feature_as_s
+0000b330: 7061 7469 616c 3a0a 2020 2020 2020 2020  patial:.        
+0000b340: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
+0000b350: 203d 3d20 4469 6d54 7970 6573 2e46 6561   == DimTypes.Fea
+0000b360: 7475 7265 3a0a 2020 2020 2020 2020 2020  ture:.          
+0000b370: 2020 2020 2020 7365 6c66 5f6b 696e 6420        self_kind 
+0000b380: 3d20 4469 6d54 7970 6573 2e53 7061 7469  = DimTypes.Spati
+0000b390: 616c 0a20 2020 2020 2020 2020 2020 2069  al.            i
+0000b3a0: 6620 6f74 6865 725f 6b69 6e64 203d 3d20  f other_kind == 
+0000b3b0: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
+0000b3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b3d0: 2020 6f74 6865 725f 6b69 6e64 203d 2044    other_kind = D
+0000b3e0: 696d 5479 7065 732e 5370 6174 6961 6c0a  imTypes.Spatial.
+0000b3f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000b400: 6469 6d65 6e73 696f 6e20 213d 206f 7468  dimension != oth
+0000b410: 6572 2e64 696d 656e 7369 6f6e 3a0a 2020  er.dimension:.  
+0000b420: 2020 2020 2020 2020 2020 6966 2062 726f            if bro
+0000b430: 6164 6361 7374 5f6d 6174 6368 6573 2061  adcast_matches a
+0000b440: 6e64 2028 7365 6c66 2e64 696d 656e 7369  nd (self.dimensi
+0000b450: 6f6e 203d 3d20 3120 6f72 206f 7468 6572  on == 1 or other
+0000b460: 2e64 696d 656e 7369 6f6e 203d 3d20 3129  .dimension == 1)
+0000b470: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b480: 2020 7061 7373 2020 2320 7061 7373 206f    pass  # pass o
+0000b490: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
+0000b4a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000b4b0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0000b4c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000b4d0: 5f6b 696e 6420 213d 206f 7468 6572 5f6b  _kind != other_k
+0000b4e0: 696e 643a 0a20 2020 2020 2020 2020 2020  ind:.           
+0000b4f0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0000b500: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
+0000b510: 6e64 203d 3d20 6f74 6865 725f 6b69 6e64  nd == other_kind
+0000b520: 203d 3d20 4469 6d54 7970 6573 2e42 6174   == DimTypes.Bat
+0000b530: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+0000b540: 2320 4e6f 7465 3a20 5468 6973 206d 6967  # Note: This mig
+0000b550: 6874 2062 6520 696e 636f 7272 6563 7420  ht be incorrect 
+0000b560: 696e 2073 6f6d 6520 6361 7365 732c 0a20  in some cases,. 
+0000b570: 2020 2020 2020 2020 2020 2023 2065 2e67             # e.g
+0000b580: 2e20 666f 7220 6265 616d 2073 6561 7263  . for beam searc
+0000b590: 6820 7768 656e 2077 6520 6861 7665 2074  h when we have t
+0000b5a0: 6865 2062 6561 6d20 6869 6464 656e 2069  he beam hidden i
+0000b5b0: 6e20 7468 6520 6261 7463 6820 6469 6d2c  n the batch dim,
+0000b5c0: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
+0000b5d0: 7220 7768 656e 2077 6520 7573 6564 204d  r when we used M
+0000b5e0: 6572 6765 4469 6d73 4c61 7965 7220 6f6e  ergeDimsLayer on
+0000b5f0: 2074 6865 2062 6174 6368 2061 7869 732c   the batch axis,
+0000b600: 206f 7220 736f 2e0a 2020 2020 2020 2020   or so..        
+0000b610: 2020 2020 2320 5765 206d 6967 6874 206e      # We might n
+0000b620: 6565 6420 746f 2065 7874 656e 6420 7468  eed to extend th
+0000b630: 6520 6c6f 6769 6320 6865 7265 206c 6174  e logic here lat
+0000b640: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+0000b650: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+0000b660: 2020 2020 6966 2042 6568 6176 696f 7256      if BehaviorV
+0000b670: 6572 7369 6f6e 2e67 6574 2829 203e 3d20  ersion.get() >= 
+0000b680: 3136 3a0a 2020 2020 2020 2020 2020 2020  16:.            
+0000b690: 2320 4569 7468 6572 2073 656c 6620 6f72  # Either self or
+0000b6a0: 206f 7468 6572 2069 7320 736f 6d65 2064   other is some d
+0000b6b0: 696d 2074 6167 2065 7870 6c69 6369 746c  im tag explicitl
+0000b6c0: 7920 6372 6561 7465 6420 6279 2074 6865  y created by the
+0000b6d0: 2075 7365 722c 0a20 2020 2020 2020 2020   user,.         
+0000b6e0: 2020 2023 2061 6e64 2074 6865 7920 6172     # and they ar
+0000b6f0: 6520 6e6f 7420 7468 6520 7361 6d65 2c20  e not the same, 
+0000b700: 736f 2077 6520 6e65 7665 7220 7472 6561  so we never trea
+0000b710: 7420 7468 656d 2061 7320 6571 7561 6c2e  t them as equal.
+0000b720: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b730: 6e6f 7420 7365 6c66 2e61 7574 6f5f 6765  not self.auto_ge
+0000b740: 6e65 7261 7465 6420 6f72 206e 6f74 206f  nerated or not o
+0000b750: 7468 6572 2e61 7574 6f5f 6765 6e65 7261  ther.auto_genera
+0000b760: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
+0000b770: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
+0000b780: 745f 6d61 7463 6865 7320 616e 6420 280a  t_matches and (.
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 2020 2020 2873 656c 662e 6469 6d65 6e73      (self.dimens
+0000b7b0: 696f 6e20 3d3d 2031 2061 6e64 2073 656c  ion == 1 and sel
+0000b7c0: 662e 6175 746f 5f67 656e 6572 6174 6564  f.auto_generated
+0000b7d0: 2920 6f72 2028 6f74 6865 722e 6469 6d65  ) or (other.dime
+0000b7e0: 6e73 696f 6e20 3d3d 2031 2061 6e64 206f  nsion == 1 and o
+0000b7f0: 7468 6572 2e61 7574 6f5f 6765 6e65 7261  ther.auto_genera
+0000b800: 7465 6429 0a20 2020 2020 2020 2020 2020  ted).           
+0000b810: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+0000b820: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0000b830: 2020 2320 6578 6365 7074 696f 6e2c 2061    # exception, a
+0000b840: 6c6c 6f77 2062 726f 6164 6361 7374 206c  llow broadcast l
+0000b850: 6f67 6963 0a20 2020 2020 2020 2020 2020  ogic.           
+0000b860: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b870: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b880: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0000b890: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
+0000b8a0: 203d 3d20 6f74 6865 725f 6b69 6e64 203d   == other_kind =
+0000b8b0: 3d20 4469 6d54 7970 6573 2e46 6561 7475  = DimTypes.Featu
+0000b8c0: 7265 3a0a 2020 2020 2020 2020 2020 2020  re:.            
+0000b8d0: 6966 2061 6c6c 6f77 5f73 616d 655f 6665  if allow_same_fe
+0000b8e0: 6174 7572 655f 6469 6d3a 0a20 2020 2020  ature_dim:.     
+0000b8f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b900: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
+0000b910: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
+0000b920: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
+0000b930: 5479 7065 732e 5370 6174 6961 6c3a 0a20  Types.Spatial:. 
+0000b940: 2020 2020 2020 2020 2020 2069 6620 616c             if al
+0000b950: 6c6f 775f 7361 6d65 5f73 7061 7469 616c  low_same_spatial
+0000b960: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
+0000b970: 2020 2020 2020 6966 2073 656c 662e 6469        if self.di
+0000b980: 6d65 6e73 696f 6e20 6973 206e 6f74 204e  mension is not N
+0000b990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b9a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000b9b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000b9c0: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
+0000b9d0: 745f 6d61 7463 6865 7320 616e 6420 2873  t_matches and (s
+0000b9e0: 656c 662e 6469 6d65 6e73 696f 6e20 3d3d  elf.dimension ==
+0000b9f0: 2031 206f 7220 6f74 6865 722e 6469 6d65   1 or other.dime
+0000ba00: 6e73 696f 6e20 3d3d 2031 293a 0a20 2020  nsion == 1):.   
+0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba20: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+0000ba30: 2020 2020 2020 2020 2069 6620 756e 6b6e           if unkn
+0000ba40: 6f77 6e5f 7370 6174 6961 6c5f 6d61 7463  own_spatial_matc
+0000ba50: 6865 7320 616e 6420 2828 7365 6c66 2e64  hes and ((self.d
+0000ba60: 796e 5f73 697a 6520 6973 204e 6f6e 6529  yn_size is None)
+0000ba70: 206f 7220 286f 7468 6572 2e64 796e 5f73   or (other.dyn_s
+0000ba80: 697a 6520 6973 204e 6f6e 6529 293a 0a20  ize is None)):. 
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000baa0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0000bab0: 2020 2020 2020 2069 6620 756e 6465 6669         if undefi
+0000bac0: 6e65 645f 6d61 7463 6865 7320 616e 6420  ned_matches and 
+0000bad0: 2873 656c 662e 756e 6465 6669 6e65 6420  (self.undefined 
+0000bae0: 6f72 206f 7468 6572 2e75 6e64 6566 696e  or other.undefin
+0000baf0: 6564 293a 0a20 2020 2020 2020 2020 2020  ed):.           
+0000bb00: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0000bb10: 0a20 2020 2020 2020 2023 2049 6e20 7072  .        # In pr
+0000bb20: 696e 6369 706c 652c 2077 6520 776f 756c  inciple, we woul
+0000bb30: 6420 7761 6e74 2074 6f20 6368 6563 6b20  d want to check 
+0000bb40: 666f 7220 6964 656e 7469 7479 2028 7365  for identity (se
+0000bb50: 6c66 2069 7320 6f74 6865 7229 2e0a 2020  lf is other)..  
+0000bb60: 2020 2020 2020 2320 5765 2063 7572 7265        # We curre
+0000bb70: 6e74 6c79 2075 7365 2074 6865 2064 6573  ntly use the des
+0000bb80: 6372 6970 7469 6f6e 2062 6563 6175 7365  cription because
+0000bb90: 2074 6865 2069 6465 6e74 6974 7920 776f   the identity wo
+0000bba0: 756c 6420 6e6f 7420 6265 2074 6865 2073  uld not be the s
+0000bbb0: 616d 650a 2020 2020 2020 2020 2320 696e  ame.        # in
+0000bbc0: 2063 6173 6520 6f66 2074 656d 706c 6174   case of templat
+0000bbd0: 6520 636f 6e73 7472 7563 7469 6f6e 2077  e construction w
+0000bbe0: 6865 7265 2061 2064 696d 2074 6167 2069  here a dim tag i
+0000bbf0: 7320 6f6e 6365 2063 7265 6174 6564 2066  s once created f
+0000bc00: 6f72 2061 2074 656d 706c 6174 6520 6c61  or a template la
+0000bc10: 7965 722c 0a20 2020 2020 2020 2023 2061  yer,.        # a
+0000bc20: 6e64 2074 6865 6e20 6c61 7465 7220 6167  nd then later ag
+0000bc30: 6169 6e20 666f 7220 7468 6520 7265 616c  ain for the real
+0000bc40: 206c 6179 6572 2e0a 2020 2020 2020 2020   layer..        
+0000bc50: 6966 2073 656c 662e 6175 746f 5f67 656e  if self.auto_gen
+0000bc60: 6572 6174 6564 2061 6e64 206f 7468 6572  erated and other
+0000bc70: 2e61 7574 6f5f 6765 6e65 7261 7465 6420  .auto_generated 
+0000bc80: 616e 6420 7365 6c66 2e64 6573 6372 6970  and self.descrip
+0000bc90: 7469 6f6e 203d 3d20 6f74 6865 722e 6465  tion == other.de
+0000bca0: 7363 7269 7074 696f 6e3a 0a20 2020 2020  scription:.     
+0000bcb0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0000bcc0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+0000bcd0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+0000bce0: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
+0000bcf0: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
+0000bd00: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+0000bd10: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
+0000bd20: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+0000bd30: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000bd40: 3a20 3a66 756e 633a 6069 735f 6571 7561  : :func:`is_equa
+0000bd50: 6c60 2077 6974 6820 6465 6661 756c 7420  l` with default 
+0000bd60: 6f70 7469 6f6e 730a 2020 2020 2020 2020  options.        
+0000bd70: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+0000bd80: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
+0000bd90: 6865 722c 205f 642e 4469 6d29 3a0a 2020  her, _d.Dim):.  
+0000bda0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000bdb0: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
+0000bdc0: 6574 7572 6e20 7365 6c66 2e69 735f 6571  eturn self.is_eq
+0000bdd0: 7561 6c28 6f74 6865 7229 0a0a 2020 2020  ual(other)..    
+0000bde0: 6465 6620 5f5f 6e65 5f5f 2873 656c 663a  def __ne__(self:
+0000bdf0: 2044 696d 2c20 6f74 6865 723a 2044 696d   Dim, other: Dim
+0000be00: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000be10: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+0000be20: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+0000be30: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+0000be40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000be50: 2020 7265 7475 726e 206e 6f74 2028 7365    return not (se
+0000be60: 6c66 203d 3d20 6f74 6865 7229 0a0a 2020  lf == other)..  
+0000be70: 2020 6465 6620 5f5f 6861 7368 5f5f 2873    def __hash__(s
+0000be80: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000be90: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+0000bea0: 3a20 696e 740a 2020 2020 2020 2020 3a72  : int.        :r
+0000beb0: 6574 7572 6e3a 2068 6173 682c 206d 6174  eturn: hash, mat
+0000bec0: 6368 696e 6720 746f 203a 6675 6e63 3a60  ching to :func:`
+0000bed0: 5f5f 6571 5f5f 600a 2020 2020 2020 2020  __eq__`.        
+0000bee0: 2222 220a 2020 2020 2020 2020 2320 5468  """.        # Th
+0000bef0: 6973 206d 7573 7420 6d61 7463 6820 7468  is must match th
+0000bf00: 6520 6265 6861 7669 6f72 2069 6e20 5f5f  e behavior in __
+0000bf10: 6571 5f5f 2c20 7768 6963 6820 6973 2069  eq__, which is i
+0000bf20: 735f 6571 7561 6c20 7769 7468 2064 6566  s_equal with def
+0000bf30: 6175 6c74 206f 7074 696f 6e73 2e0a 2020  ault options..  
+0000bf40: 2020 2020 2020 2320 492e 652e 2064 6966        # I.e. dif
+0000bf50: 6665 7265 6e74 2068 6173 6820 696d 706c  ferent hash impl
+0000bf60: 6965 7320 6e6f 7420 6571 7561 6c20 2862  ies not equal (b
+0000bf70: 7574 2073 616d 6520 6861 7368 206e 6f74  ut same hash not
+0000bf80: 206e 6563 6573 7361 7269 6c79 2065 7175   necessarily equ
+0000bf90: 616c 292e 0a20 2020 2020 2020 2069 6620  al)..        if 
+0000bfa0: 7365 6c66 2e73 7065 6369 616c 3a0a 2020  self.special:.  
+0000bfb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000bfc0: 2068 6173 6828 6964 2873 656c 6629 290a   hash(id(self)).
+0000bfd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000bfe0: 6973 5f62 6174 6368 5f64 696d 2829 3a0a  is_batch_dim():.
+0000bff0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c000: 726e 2068 6173 6828 2829 290a 2020 2020  rn hash(()).    
+0000c010: 2020 2020 7769 7468 2075 7469 6c2e 6775      with util.gu
+0000c020: 6172 645f 696e 6669 6e69 7465 5f72 6563  ard_infinite_rec
+0000c030: 7572 7369 6f6e 285f 642e 4469 6d2e 5f5f  ursion(_d.Dim.__
+0000c040: 6861 7368 5f5f 2c20 7365 6c66 293a 0a20  hash__, self):. 
+0000c050: 2020 2020 2020 2020 2020 2062 6173 6520             base 
+0000c060: 3d20 7365 6c66 2e67 6574 5f73 616d 655f  = self.get_same_
+0000c070: 6261 7365 2829 0a20 2020 2020 2020 2020  base().         
+0000c080: 2020 2069 6620 6261 7365 2069 7320 6e6f     if base is no
+0000c090: 7420 7365 6c66 3a0a 2020 2020 2020 2020  t self:.        
+0000c0a0: 2020 2020 2020 2020 7265 7475 726e 2068          return h
+0000c0b0: 6173 6828 6261 7365 290a 2020 2020 2020  ash(base).      
+0000c0c0: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
+0000c0d0: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000c0f0: 6574 7572 6e20 6861 7368 2873 656c 662e  eturn hash(self.
+0000c100: 6465 7269 7665 645f 6672 6f6d 5f6f 7029  derived_from_op)
+0000c110: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c120: 7365 6c66 2e61 7574 6f5f 6765 6e65 7261  self.auto_genera
+0000c130: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
+0000c140: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+0000c150: 2828 6261 7365 2e6b 696e 642c 2062 6173  ((base.kind, bas
+0000c160: 652e 6469 6d65 6e73 696f 6e2c 2062 6173  e.dimension, bas
+0000c170: 652e 6465 7363 7269 7074 696f 6e29 290a  e.description)).
+0000c180: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c190: 726e 2068 6173 6828 6964 2862 6173 6529  rn hash(id(base)
+0000c1a0: 290a 0a20 2020 2064 6566 205f 5f6c 745f  )..    def __lt_
+0000c1b0: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
+0000c1c0: 6572 3a20 4469 6d29 3a0a 2020 2020 2020  er: Dim):.      
+0000c1d0: 2020 2222 220a 2020 2020 2020 2020 4465    """.        De
+0000c1e0: 6669 6e65 2073 6f6d 6520 6f72 6465 722e  fine some order.
+0000c1f0: 2054 6869 7320 6973 206a 7573 7420 7375   This is just su
+0000c200: 6368 2074 6861 7420 6073 6f72 7465 6460  ch that `sorted`
+0000c210: 2077 6f72 6b73 2c20 6f72 2073 6f6d 6520   works, or some 
+0000c220: 6469 6666 2072 6570 6f72 7469 6e67 2c20  diff reporting, 
+0000c230: 6f72 2073 6f2e 0a20 2020 2020 2020 2049  or so..        I
+0000c240: 7420 6973 206f 6e20 7379 6d62 6f6c 6963  t is on symbolic
+0000c250: 206c 6576 656c 2c20 692e 652e 2069 7420   level, i.e. it 
+0000c260: 646f 6573 206e 6f74 2063 6f6e 7369 6465  does not conside
+0000c270: 7220 7468 6520 6163 7475 616c 2064 696d  r the actual dim
+0000c280: 656e 7369 6f6e 2076 616c 7565 2e0a 2020  ension value..  
+0000c290: 2020 2020 2020 5468 6520 6465 6669 6e65        The define
+0000c2a0: 6420 6f72 6465 7220 736f 6d65 7768 6174  d order somewhat
+0000c2b0: 2061 7262 6974 7261 7279 2c20 736f 2064   arbitrary, so d
+0000c2c0: 6f20 6e6f 7420 7265 6c79 206f 6e20 7468  o not rely on th
+0000c2d0: 6520 6578 6163 7420 6265 6861 7669 6f72  e exact behavior
+0000c2e0: 2c0a 2020 2020 2020 2020 6173 2074 6869  ,.        as thi
+0000c2f0: 7320 6d69 6768 7420 6368 616e 6765 2061  s might change a
+0000c300: 7420 736f 6d65 206c 6174 6572 2070 6f69  t some later poi
+0000c310: 6e74 2e0a 2020 2020 2020 2020 4375 7272  nt..        Curr
+0000c320: 656e 746c 792c 2069 7420 6465 7065 6e64  ently, it depend
+0000c330: 7320 6f6e 2074 6865 2063 7265 6174 696f  s on the creatio
+0000c340: 6e20 696e 6465 782e 0a0a 2020 2020 2020  n index...      
+0000c350: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
+0000c360: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
+0000c370: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
+0000c380: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0000c390: 6e6f 7420 6973 696e 7374 616e 6365 286f  not isinstance(o
+0000c3a0: 7468 6572 2c20 285f 642e 4469 6d2c 205f  ther, (_d.Dim, _
+0000c3b0: 6d2e 4d61 726b 6564 4469 6d29 293a 0a20  m.MarkedDim)):. 
+0000c3c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000c3d0: 2054 7970 6545 7272 6f72 2822 6361 6e6e   TypeError("cann
+0000c3e0: 6f74 2063 6f6d 7061 7265 2025 7220 7769  ot compare %r wi
+0000c3f0: 7468 2025 7222 2025 2028 7365 6c66 2c20  th %r" % (self, 
+0000c400: 6f74 6865 7229 290a 2020 2020 2020 2020  other)).        
+0000c410: 6966 2073 656c 6620 3d3d 206f 7468 6572  if self == other
+0000c420: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000c430: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+0000c440: 2020 2072 6574 7572 6e20 6469 6d5f 636d     return dim_cm
+0000c450: 705f 7661 6c75 6528 7365 6c66 2920 3c20  p_value(self) < 
+0000c460: 6469 6d5f 636d 705f 7661 6c75 6528 6f74  dim_cmp_value(ot
+0000c470: 6865 7229 0a0a 2020 2020 6465 6620 5f5f  her)..    def __
+0000c480: 6774 5f5f 2873 656c 662c 206f 7468 6572  gt__(self, other
+0000c490: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000c4a0: 2020 2020 2020 2053 6565 203a 6675 6e63         See :func
+0000c4b0: 3a60 5f5f 6c74 5f5f 602e 0a0a 2020 2020  :`__lt__`...    
+0000c4c0: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
+0000c4d0: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+0000c4e0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+0000c4f0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000c500: 6574 7572 6e20 6f74 6865 7220 3c20 7365  eturn other < se
+0000c510: 6c66 0a0a 2020 2020 6465 6620 5f5f 6765  lf..    def __ge
+0000c520: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+0000c530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c540: 6e6f 7420 7365 6c66 203c 206f 7468 6572  not self < other
+0000c550: 0a0a 2020 2020 6465 6620 5f5f 6c65 5f5f  ..    def __le__
+0000c560: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+0000c570: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+0000c580: 7420 7365 6c66 203e 206f 7468 6572 0a0a  t self > other..
+0000c590: 2020 2020 6465 6620 6765 745f 7361 6d65      def get_same
+0000c5a0: 5f62 6173 6528 7365 6c66 3a20 5f64 2e44  _base(self: _d.D
+0000c5b0: 696d 2920 2d3e 205f 642e 4469 6d3a 0a20  im) -> _d.Dim:. 
+0000c5c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c5d0: 2020 203a 7265 7475 726e 3a20 7361 6d65     :return: same
+0000c5e0: 2062 6173 650a 2020 2020 2020 2020 2222   base.        ""
+0000c5f0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000c600: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
+0000c610: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c620: 2073 656c 660a 2020 2020 2020 2020 6261   self.        ba
+0000c630: 7365 203d 2073 656c 660a 2020 2020 2020  se = self.      
+0000c640: 2020 7768 696c 6520 6261 7365 2e73 616d    while base.sam
+0000c650: 655f 6173 3a0a 2020 2020 2020 2020 2020  e_as:.          
+0000c660: 2020 6261 7365 203d 2062 6173 652e 7361    base = base.sa
+0000c670: 6d65 5f61 730a 2020 2020 2020 2020 7265  me_as.        re
+0000c680: 7475 726e 2062 6173 650a 0a20 2020 2064  turn base..    d
+0000c690: 6566 2067 6574 5f73 616d 655f 6465 7269  ef get_same_deri
+0000c6a0: 7665 645f 6261 7365 2873 656c 663a 205f  ved_base(self: _
+0000c6b0: 642e 4469 6d29 202d 3e20 5f64 2e44 696d  d.Dim) -> _d.Dim
+0000c6c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c6d0: 2020 2020 2020 3a72 6574 7572 6e3a 2073        :return: s
+0000c6e0: 616d 6520 6261 7365 2c20 6275 7420 616c  ame base, but al
+0000c6f0: 736f 2063 6f6e 7369 6465 7220 6465 7269  so consider deri
+0000c700: 7665 645f 6672 6f6d 5f2e 2e2e 0a20 2020  ved_from_....   
+0000c710: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c720: 2062 6173 6520 3d20 7365 6c66 0a20 2020   base = self.   
+0000c730: 2020 2020 2076 6973 6974 6564 203d 207b       visited = {
+0000c740: 7d0a 2020 2020 2020 2020 7768 696c 6520  }.        while 
+0000c750: 6261 7365 2e73 616d 655f 6173 206f 7220  base.same_as or 
+0000c760: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000c770: 6d5f 7461 673a 0a20 2020 2020 2020 2020  m_tag:.         
+0000c780: 2020 2061 7373 6572 7420 6964 2862 6173     assert id(bas
+0000c790: 6529 206e 6f74 2069 6e20 7669 7369 7465  e) not in visite
+0000c7a0: 6420 2023 2073 686f 756c 6420 6e6f 7420  d  # should not 
+0000c7b0: 6861 7665 2063 7963 6c65 732e 206e 6f72  have cycles. nor
+0000c7c0: 6d61 6c6c 7920 7468 6973 2073 686f 756c  mally this shoul
+0000c7d0: 6420 6e65 7665 7220 6265 2074 7269 6767  d never be trigg
+0000c7e0: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+0000c7f0: 2076 6973 6974 6564 5b69 6428 6261 7365   visited[id(base
+0000c800: 295d 203d 2062 6173 650a 2020 2020 2020  )] = base.      
+0000c810: 2020 2020 2020 6966 2062 6173 652e 7361        if base.sa
+0000c820: 6d65 5f61 733a 0a20 2020 2020 2020 2020  me_as:.         
+0000c830: 2020 2020 2020 2062 6173 6520 3d20 6261         base = ba
+0000c840: 7365 2e73 616d 655f 6173 0a20 2020 2020  se.same_as.     
+0000c850: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000c860: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0000c870: 6261 7365 203d 2062 6173 652e 6465 7269  base = base.deri
+0000c880: 7665 645f 6672 6f6d 5f74 6167 0a20 2020  ved_from_tag.   
+0000c890: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000c8a0: 6261 7365 0a20 2020 2020 2020 2072 6574  base.        ret
+0000c8b0: 7572 6e20 6261 7365 0a0a 2020 2020 6465  urn base..    de
+0000c8c0: 6620 6765 745f 6465 7269 7665 645f 6261  f get_derived_ba
+0000c8d0: 7365 735f 7365 7428 7365 6c66 293a 0a20  ses_set(self):. 
+0000c8e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c8f0: 2020 203a 7274 7970 653a 2073 6574 5b44     :rtype: set[D
+0000c900: 696d 5d0a 2020 2020 2020 2020 2222 220a  im].        """.
+0000c910: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+0000c920: 7428 290a 2020 2020 2020 2020 7175 6575  t().        queu
+0000c930: 6520 3d20 5b73 656c 665d 0a20 2020 2020  e = [self].     
+0000c940: 2020 2076 6973 6974 6564 203d 207b 7d20     visited = {} 
+0000c950: 2023 2074 7970 653a 2044 6963 745b 696e   # type: Dict[in
+0000c960: 742c 5f64 2e44 696d 5d20 2023 2062 7920  t,_d.Dim]  # by 
+0000c970: 6964 0a20 2020 2020 2020 2077 6869 6c65  id.        while
+0000c980: 2071 7565 7565 3a0a 2020 2020 2020 2020   queue:.        
+0000c990: 2020 2020 6261 7365 203d 2071 7565 7565      base = queue
+0000c9a0: 2e70 6f70 282d 3129 0a20 2020 2020 2020  .pop(-1).       
+0000c9b0: 2020 2020 2069 6620 6261 7365 2e73 616d       if base.sam
+0000c9c0: 655f 6173 3a0a 2020 2020 2020 2020 2020  e_as:.          
+0000c9d0: 2020 2020 2020 6261 7365 203d 2062 6173        base = bas
+0000c9e0: 652e 7361 6d65 5f61 730a 2020 2020 2020  e.same_as.      
+0000c9f0: 2020 2020 2020 6966 2069 6428 6261 7365        if id(base
+0000ca00: 2920 696e 2076 6973 6974 6564 3a0a 2020  ) in visited:.  
+0000ca10: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000ca20: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+0000ca30: 2020 2076 6973 6974 6564 5b69 6428 6261     visited[id(ba
+0000ca40: 7365 295d 203d 2062 6173 650a 2020 2020  se)] = base.    
+0000ca50: 2020 2020 2020 2020 7265 732e 6164 6428          res.add(
+0000ca60: 6261 7365 290a 2020 2020 2020 2020 2020  base).          
+0000ca70: 2020 6966 2062 6173 652e 6465 7269 7665    if base.derive
+0000ca80: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
+0000ca90: 2020 2020 2020 2020 2020 2071 7565 7565             queue
+0000caa0: 2e65 7874 656e 6428 6261 7365 2e64 6572  .extend(base.der
+0000cab0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+0000cac0: 7574 7329 0a20 2020 2020 2020 2020 2020  uts).           
+0000cad0: 2065 6c69 6620 6261 7365 2e64 6572 6976   elif base.deriv
+0000cae0: 6564 5f66 726f 6d5f 7461 673a 0a20 2020  ed_from_tag:.   
+0000caf0: 2020 2020 2020 2020 2020 2020 2071 7565               que
+0000cb00: 7565 2e61 7070 656e 6428 6261 7365 2e64  ue.append(base.d
+0000cb10: 6572 6976 6564 5f66 726f 6d5f 7461 6729  erived_from_tag)
+0000cb20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cb30: 7265 730a 0a20 2020 2040 7072 6f70 6572  res..    @proper
+0000cb40: 7479 0a20 2020 2064 6566 2075 6e64 6566  ty.    def undef
+0000cb50: 696e 6564 2873 656c 663a 205f 642e 4469  ined(self: _d.Di
+0000cb60: 6d29 202d 3e20 626f 6f6c 3a0a 2020 2020  m) -> bool:.    
+0000cb70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cb80: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
+0000cb90: 2074 6865 2075 6e64 6566 696e 6564 2066   the undefined f
+0000cba0: 6c61 6720 6973 2073 6574 2c20 696e 2073  lag is set, in s
+0000cbb0: 656c 662c 2062 6173 6573 2c20 6f72 2061  elf, bases, or a
+0000cbc0: 6e79 2064 6572 6976 6564 2062 6173 6573  ny derived bases
+0000cbd0: 2e20 616c 736f 2073 6565 203a 6675 6e63  . also see :func
+0000cbe0: 3a60 6973 5f64 696d 5f6b 6e6f 776e 600a  :`is_dim_known`.
+0000cbf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000cc00: 2020 2020 6261 7365 203d 2073 656c 660a      base = self.
+0000cc10: 2020 2020 2020 2020 7669 7369 7465 6420          visited 
+0000cc20: 3d20 7b7d 0a20 2020 2020 2020 2077 6869  = {}.        whi
+0000cc30: 6c65 2062 6173 652e 7361 6d65 5f61 7320  le base.same_as 
+0000cc40: 6f72 2062 6173 652e 6465 7269 7665 645f  or base.derived_
+0000cc50: 6672 6f6d 5f74 6167 3a0a 2020 2020 2020  from_tag:.      
+0000cc60: 2020 2020 2020 6173 7365 7274 2069 6428        assert id(
+0000cc70: 6261 7365 2920 6e6f 7420 696e 2076 6973  base) not in vis
+0000cc80: 6974 6564 2020 2320 7368 6f75 6c64 206e  ited  # should n
+0000cc90: 6f74 2068 6176 6520 6379 636c 6573 2e20  ot have cycles. 
+0000cca0: 6e6f 726d 616c 6c79 2074 6869 7320 7368  normally this sh
+0000ccb0: 6f75 6c64 206e 6576 6572 2062 6520 7472  ould never be tr
+0000ccc0: 6967 6765 7265 640a 2020 2020 2020 2020  iggered.        
+0000ccd0: 2020 2020 7669 7369 7465 645b 6964 2862      visited[id(b
+0000cce0: 6173 6529 5d20 3d20 6261 7365 0a20 2020  ase)] = base.   
+0000ccf0: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
+0000cd00: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
+0000cd10: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
+0000cd20: 2020 2020 2020 6966 2062 6173 652e 5f65        if base._e
+0000cd30: 7874 7261 2061 6e64 2062 6173 652e 5f65  xtra and base._e
+0000cd40: 7874 7261 2e75 6e64 6566 696e 6564 3a0a  xtra.undefined:.
+0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd60: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+0000cd70: 2020 2020 2020 2020 6966 2062 6173 652e          if base.
+0000cd80: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
+0000cd90: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
+0000cda0: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
+0000cdb0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000cdc0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+0000cdd0: 2020 6261 7365 203d 2062 6173 652e 6465    base = base.de
+0000cde0: 7269 7665 645f 6672 6f6d 5f74 6167 0a20  rived_from_tag. 
+0000cdf0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000ce00: 7420 6261 7365 0a20 2020 2020 2020 2023  t base.        #
+0000ce10: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+0000ce20: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+0000ce30: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+0000ce40: 6173 652e 5f65 7874 7261 2061 6e64 2062  ase._extra and b
+0000ce50: 6173 652e 5f65 7874 7261 2e75 6e64 6566  ase._extra.undef
+0000ce60: 696e 6564 0a0a 2020 2020 6465 6620 6465  ined..    def de
+0000ce70: 636c 6172 655f 7361 6d65 5f61 7328 7365  clare_same_as(se
+0000ce80: 6c66 3a20 5f64 2e44 696d 2c20 6f74 6865  lf: _d.Dim, othe
+0000ce90: 723a 205f 642e 4469 6d29 3a0a 2020 2020  r: _d.Dim):.    
+0000cea0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ceb0: 3a70 6172 616d 206f 7468 6572 3a0a 2020  :param other:.  
+0000cec0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ced0: 2020 6173 7365 7274 2073 656c 662e 6361    assert self.ca
+0000cee0: 6e5f 6265 5f75 7365 645f 6173 5f64 696d  n_be_used_as_dim
+0000cef0: 2829 2061 6e64 206f 7468 6572 2e63 616e  () and other.can
+0000cf00: 5f62 655f 7573 6564 5f61 735f 6469 6d28  _be_used_as_dim(
+0000cf10: 2920 2023 2064 6563 6c61 7265 5f73 616d  )  # declare_sam
+0000cf20: 655f 6173 2064 6f65 7320 6e6f 7420 6d61  e_as does not ma
+0000cf30: 6b65 2073 656e 7365 206f 7468 6572 7769  ke sense otherwi
+0000cf40: 7365 0a20 2020 2020 2020 2023 204e 6f74  se.        # Not
+0000cf50: 653a 2043 6865 636b 2060 6973 602c 206e  e: Check `is`, n
+0000cf60: 6f74 2060 3d3d 602e 2060 3d3d 6020 6361  ot `==`. `==` ca
+0000cf70: 6e20 6265 2074 7275 6520 6576 656e 2074  n be true even t
+0000cf80: 686f 7567 6820 7361 6d65 5f61 7320 6172  hough same_as ar
+0000cf90: 6520 6e6f 7420 7468 6520 7361 6d65 2069  e not the same i
+0000cfa0: 6e73 7461 6e63 652c 0a20 2020 2020 2020  nstance,.       
+0000cfb0: 2023 2065 2e67 2e20 7669 6120 6175 746f   # e.g. via auto
+0000cfc0: 5f67 656e 6572 6174 6564 2e0a 2020 2020  _generated..    
+0000cfd0: 2020 2020 6966 2073 656c 6620 6973 206f      if self is o
+0000cfe0: 7468 6572 3a0a 2020 2020 2020 2020 2020  ther:.          
+0000cff0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000d000: 2073 656c 662e 5f6d 6179 6265 5f75 7064   self._maybe_upd
+0000d010: 6174 6528 290a 2020 2020 2020 2020 7365  ate().        se
+0000d020: 6c66 2e5f 7661 6c69 6461 7465 5f69 6e5f  lf._validate_in_
+0000d030: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
+0000d040: 2020 2020 2020 2020 6f74 6865 722e 5f76          other._v
+0000d050: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
+0000d060: 6e74 5f67 7261 7068 2829 0a20 2020 2020  nt_graph().     
+0000d070: 2020 206f 7468 6572 5f73 616d 655f 6261     other_same_ba
+0000d080: 7365 203d 206f 7468 6572 2e67 6574 5f73  se = other.get_s
+0000d090: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
+0000d0a0: 2020 2069 6620 7365 6c66 2069 7320 6f74     if self is ot
+0000d0b0: 6865 725f 7361 6d65 5f62 6173 6520 6f72  her_same_base or
+0000d0c0: 2073 656c 662e 7361 6d65 5f61 7320 6973   self.same_as is
+0000d0d0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000d0e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000d0f0: 7475 726e 0a20 2020 2020 2020 2073 656c  turn.        sel
+0000d100: 665f 7361 6d65 5f61 7320 3d20 7365 6c66  f_same_as = self
+0000d110: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
+0000d120: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000d130: 5f73 616d 655f 6173 2069 7320 6f74 6865  _same_as is othe
+0000d140: 725f 7361 6d65 5f62 6173 653a 0a20 2020  r_same_base:.   
+0000d150: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000d160: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+0000d170: 5f73 616d 655f 6261 7365 2e67 6574 5f73  _same_base.get_s
+0000d180: 616d 655f 6465 7269 7665 645f 6261 7365  ame_derived_base
+0000d190: 2829 2069 7320 7365 6c66 5f73 616d 655f  () is self_same_
+0000d1a0: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
+0000d1b0: 2320 5765 2061 6374 7561 6c6c 7920 7761  # We actually wa
+0000d1c0: 6e74 2069 7420 746f 2062 6520 7468 6520  nt it to be the 
+0000d1d0: 6f74 6865 7220 7761 7920 6172 6f75 6e64  other way around
+0000d1e0: 2e0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+0000d1f0: 7468 2075 7469 6c2e 6775 6172 645f 696e  th util.guard_in
+0000d200: 6669 6e69 7465 5f72 6563 7572 7369 6f6e  finite_recursion
+0000d210: 285f 642e 4469 6d2e 6465 636c 6172 655f  (_d.Dim.declare_
+0000d220: 7361 6d65 5f61 732c 206f 7468 6572 2c20  same_as, other, 
+0000d230: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+0000d240: 2020 2020 2020 2072 6574 7572 6e20 6f74         return ot
+0000d250: 6865 722e 6465 636c 6172 655f 7361 6d65  her.declare_same
+0000d260: 5f61 7328 7365 6c66 290a 2020 2020 2020  _as(self).      
+0000d270: 2020 6966 2073 656c 662e 6261 7463 683a    if self.batch:
+0000d280: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+0000d290: 6620 7365 6c66 2069 7320 6465 6669 6e65  f self is define
+0000d2a0: 6420 2873 656c 662e 6973 5f64 696d 5f6b  d (self.is_dim_k
+0000d2b0: 6e6f 776e 292c 2062 6520 6661 6972 2074  nown), be fair t
+0000d2c0: 6f20 6f74 6865 722c 2061 6e64 2061 6461  o other, and ada
+0000d2d0: 7074 2069 7420 746f 2074 6865 2072 6967  pt it to the rig
+0000d2e0: 6874 2062 6174 6368 2c0a 2020 2020 2020  ht batch,.      
+0000d2f0: 2020 2020 2020 2320 7375 6368 2074 6861        # such tha
+0000d300: 7420 6f74 6865 722e 6973 5f64 696d 5f6b  t other.is_dim_k
+0000d310: 6e6f 776e 2069 7320 636f 7272 6563 742c  nown is correct,
+0000d320: 2062 7920 706f 7465 6e74 6961 6c6c 7920   by potentially 
+0000d330: 636f 6d70 6c65 7469 6e67 2069 742e 0a20  completing it.. 
+0000d340: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000d350: 5f20 3d20 6f74 6865 722e 6765 745f 666f  _ = other.get_fo
+0000d360: 725f 6261 7463 685f 6374 7828 7365 6c66  r_batch_ctx(self
+0000d370: 2e62 6174 6368 2c20 6374 783d 7365 6c66  .batch, ctx=self
+0000d380: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000d390: 7829 0a20 2020 2020 2020 2065 6c73 653a  x).        else:
+0000d3a0: 0a20 2020 2020 2020 2020 2020 206f 7468  .            oth
+0000d3b0: 6572 5f20 3d20 6f74 6865 720a 2020 2020  er_ = other.    
+0000d3c0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+0000d3d0: 2020 2020 2028 7365 6c66 2e69 735f 6469       (self.is_di
+0000d3e0: 6d5f 6b6e 6f77 6e28 2920 616e 6420 6e6f  m_known() and no
+0000d3f0: 7420 6f74 6865 725f 2e69 735f 6469 6d5f  t other_.is_dim_
+0000d400: 6b6e 6f77 6e28 2929 0a20 2020 2020 2020  known()).       
+0000d410: 2020 2020 206f 720a 2020 2020 2020 2020       or.        
+0000d420: 2020 2020 2320 4c69 6b65 2069 735f 6469      # Like is_di
+0000d430: 6d5f 6b6e 6f77 6e20 6275 7420 666f 7220  m_known but for 
+0000d440: 7374 6174 6963 2064 696d 732c 2077 6520  static dims, we 
+0000d450: 6d69 6768 7420 6b6e 6f77 2062 6f74 682c  might know both,
+0000d460: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
+0000d470: 7574 2074 6865 2064 6572 6976 6564 5f66  ut the derived_f
+0000d480: 726f 6d5f 6f70 2073 7469 6c6c 2077 6f75  rom_op still wou
+0000d490: 6c64 2070 726f 7669 6465 206d 6f72 6520  ld provide more 
+0000d4a0: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
+0000d4b0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+0000d4c0: 2020 2020 2020 2020 2020 2073 656c 665f             self_
+0000d4d0: 7361 6d65 5f61 732e 6465 7269 7665 645f  same_as.derived_
+0000d4e0: 6672 6f6d 5f6f 700a 2020 2020 2020 2020  from_op.        
+0000d4f0: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
+0000d500: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000d510: 6465 7269 7665 645f 6672 6f6d 5f6f 700a  derived_from_op.
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 616e 6420 6f74 6865 7220 6e6f 7420 696e  and other not in
+0000d540: 2073 656c 662e 6765 745f 6465 7269 7665   self.get_derive
+0000d550: 645f 6261 7365 735f 7365 7428 290a 2020  d_bases_set().  
+0000d560: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000d570: 2020 2020 2020 2020 6f72 2028 6e6f 7420          or (not 
+0000d580: 7365 6c66 2e75 6e64 6566 696e 6564 2061  self.undefined a
+0000d590: 6e64 206f 7468 6572 5f2e 756e 6465 6669  nd other_.undefi
+0000d5a0: 6e65 6429 0a20 2020 2020 2020 2029 3a0a  ned).        ):.
+0000d5b0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000d5c0: 2075 7469 6c2e 6775 6172 645f 696e 6669   util.guard_infi
+0000d5d0: 6e69 7465 5f72 6563 7572 7369 6f6e 285f  nite_recursion(_
+0000d5e0: 642e 4469 6d2e 6465 636c 6172 655f 7361  d.Dim.declare_sa
+0000d5f0: 6d65 5f61 732c 206f 7468 6572 2c20 7365  me_as, other, se
+0000d600: 6c66 293a 0a20 2020 2020 2020 2020 2020  lf):.           
+0000d610: 2020 2020 2072 6574 7572 6e20 6f74 6865       return othe
+0000d620: 722e 6465 636c 6172 655f 7361 6d65 5f61  r.declare_same_a
+0000d630: 7328 7365 6c66 290a 2020 2020 2020 2020  s(self).        
+0000d640: 6f74 6865 725f 6465 7269 7665 645f 6261  other_derived_ba
+0000d650: 7365 7320 3d20 6f74 6865 722e 6765 745f  ses = other.get_
+0000d660: 6465 7269 7665 645f 6261 7365 735f 7365  derived_bases_se
+0000d670: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000d680: 5f64 6572 6976 6564 5f62 6173 6573 203d  _derived_bases =
+0000d690: 2073 656c 662e 6765 745f 6465 7269 7665   self.get_derive
+0000d6a0: 645f 6261 7365 735f 7365 7428 290a 2020  d_bases_set().  
+0000d6b0: 2020 2020 2020 6966 206f 7468 6572 5f64        if other_d
+0000d6c0: 6572 6976 6564 5f62 6173 6573 2021 3d20  erived_bases != 
+0000d6d0: 7365 6c66 5f64 6572 6976 6564 5f62 6173  self_derived_bas
+0000d6e0: 6573 2061 6e64 2073 656c 665f 6465 7269  es and self_deri
+0000d6f0: 7665 645f 6261 7365 732e 6973 7375 6273  ved_bases.issubs
+0000d700: 6574 286f 7468 6572 5f64 6572 6976 6564  et(other_derived
+0000d710: 5f62 6173 6573 293a 0a20 2020 2020 2020  _bases):.       
+0000d720: 2020 2020 2023 2041 766f 6964 2063 7963       # Avoid cyc
+0000d730: 6c65 7320 6f6e 2064 6572 6976 6564 5f66  les on derived_f
+0000d740: 726f 6d5f 7461 672e 2068 7474 7073 3a2f  rom_tag. https:/
+0000d750: 2f67 6974 6875 622e 636f 6d2f 7277 7468  /github.com/rwth
+0000d760: 2d69 362f 7265 7475 726e 6e2f 6973 7375  -i6/returnn/issu
+0000d770: 6573 2f31 3035 340a 2020 2020 2020 2020  es/1054.        
+0000d780: 2020 2020 7769 7468 2075 7469 6c2e 6775      with util.gu
+0000d790: 6172 645f 696e 6669 6e69 7465 5f72 6563  ard_infinite_rec
+0000d7a0: 7572 7369 6f6e 285f 642e 4469 6d2e 6465  ursion(_d.Dim.de
+0000d7b0: 636c 6172 655f 7361 6d65 5f61 732c 206f  clare_same_as, o
+0000d7c0: 7468 6572 2c20 7365 6c66 293a 0a20 2020  ther, self):.   
+0000d7d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000d7e0: 7572 6e20 6f74 6865 722e 6465 636c 6172  urn other.declar
+0000d7f0: 655f 7361 6d65 5f61 7328 7365 6c66 290a  e_same_as(self).
+0000d800: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d810: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
+0000d820: 2020 2020 7365 6c66 2e5f 6578 7472 612e      self._extra.
+0000d830: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
+0000d840: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000d850: 2020 2073 656c 662e 5f65 7874 7261 2e64     self._extra.d
+0000d860: 6572 6976 6564 5f66 726f 6d5f 7461 6720  erived_from_tag 
+0000d870: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+0000d880: 6620 7365 6c66 5f73 616d 655f 6173 2069  f self_same_as i
+0000d890: 7320 6e6f 7420 7365 6c66 3a0a 2020 2020  s not self:.    
+0000d8a0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+0000d8b0: 6f74 2073 656c 665f 7361 6d65 5f61 732e  ot self_same_as.
+0000d8c0: 7361 6d65 5f61 730a 2020 2020 2020 2020  same_as.        
+0000d8d0: 2020 2020 6966 2073 656c 665f 7361 6d65      if self_same
+0000d8e0: 5f61 7320 6973 206f 7468 6572 5f73 616d  _as is other_sam
+0000d8f0: 655f 6261 7365 3a0a 2020 2020 2020 2020  e_base:.        
+0000d900: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000d910: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000d920: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
+0000d930: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
+0000d940: 2e44 696d 2e64 6563 6c61 7265 5f73 616d  .Dim.declare_sam
+0000d950: 655f 6173 2c20 7365 6c66 5f73 616d 655f  e_as, self_same_
+0000d960: 6173 2c20 6f74 6865 725f 7361 6d65 5f62  as, other_same_b
+0000d970: 6173 6529 3a0a 2020 2020 2020 2020 2020  ase):.          
+0000d980: 2020 2020 2020 7365 6c66 5f73 616d 655f        self_same_
+0000d990: 6173 2e64 6563 6c61 7265 5f73 616d 655f  as.declare_same_
+0000d9a0: 6173 286f 7468 6572 5f73 616d 655f 6261  as(other_same_ba
+0000d9b0: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+0000d9c0: 6966 2028 7365 6c66 2e64 796e 5f73 697a  if (self.dyn_siz
+0000d9d0: 655f 6578 7420 6973 204e 6f6e 6520 6f72  e_ext is None or
+0000d9e0: 206e 6f74 2073 656c 662e 5f76 616c 6964   not self._valid
+0000d9f0: 6174 655f 696e 5f63 7572 7265 6e74 5f67  ate_in_current_g
+0000da00: 7261 7068 2829 2920 616e 6420 7365 6c66  raph()) and self
+0000da10: 5f73 616d 655f 6173 2e64 796e 5f73 697a  _same_as.dyn_siz
+0000da20: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
+0000da30: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
+0000da40: 7369 7a65 5f65 7874 203d 2073 656c 665f  size_ext = self_
+0000da50: 7361 6d65 5f61 732e 6765 745f 6479 6e5f  same_as.get_dyn_
+0000da60: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
+0000da70: 6368 5f63 7478 280a 2020 2020 2020 2020  ch_ctx(.        
+0000da80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000da90: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
+0000daa0: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
+0000dab0: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
+0000dac0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000dad0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+0000dae0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000daf0: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
+0000db00: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000db10: 7220 6469 6d5f 2069 6e20 7365 6c66 2e5f  r dim_ in self._
+0000db20: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
+0000db30: 6174 6368 5f63 7478 2e76 616c 7565 7328  atch_ctx.values(
+0000db40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000db50: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
+0000db60: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+0000db70: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
+0000db80: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000db90: 696d 5f2e 5f65 7874 7261 3a0a 2020 2020  im_._extra:.    
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+0000dbc0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+0000dbd0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+0000dbe0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+0000dbf0: 5f2e 5f65 7874 7261 2e64 6572 6976 6564  _._extra.derived
+0000dc00: 5f66 726f 6d5f 6f70 203d 204e 6f6e 650a  _from_op = None.
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc20: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
+0000dc30: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
+0000dc40: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 2064 696d 5f2e 5f65 7874 7261 2e64 6572   dim_._extra.der
+0000dc70: 6976 6564 5f66 726f 6d5f 7461 6720 3d20  ived_from_tag = 
+0000dc80: 4e6f 6e65 0a20 2020 2020 2020 2023 204e  None.        # N
+0000dc90: 6f77 206d 6572 6765 2065 7869 7374 696e  ow merge existin
+0000dca0: 6720 7661 7269 616e 7473 2e20 4275 7420  g variants. But 
+0000dcb0: 6f6e 6c79 2069 6620 6e6f 7420 6465 7269  only if not deri
+0000dcc0: 7665 6420 7669 6120 6f70 2c20 6265 6361  ved via op, beca
+0000dcd0: 7573 6520 696e 2074 6861 7420 6361 7365  use in that case
+0000dce0: 2c20 7765 2063 616e 2028 616e 6420 7368  , we can (and sh
+0000dcf0: 6f75 6c64 2129 0a20 2020 2020 2020 2023  ould!).        #
+0000dd00: 2061 7574 6f6d 6174 6963 616c 6c79 2069   automatically i
+0000dd10: 6e66 6572 2069 742e 204e 6f74 6520 7468  nfer it. Note th
+0000dd20: 6174 2077 6520 6f6e 6c79 2067 6f74 2068  at we only got h
+0000dd30: 6572 6520 7768 656e 2074 6865 206f 7468  ere when the oth
+0000dd40: 6572 2069 7320 6e6f 7420 7468 6520 7361  er is not the sa
+0000dd50: 6d65 2064 696d 2c20 736f 2069 7420 6d65  me dim, so it me
+0000dd60: 616e 7320 7468 6174 0a20 2020 2020 2020  ans that.       
+0000dd70: 2023 2074 6865 206f 7468 6572 2069 7320   # the other is 
+0000dd80: 7265 616c 6c79 2064 6966 6665 7265 6e74  really different
+0000dd90: 2c20 7468 6520 7369 7a65 7320 6172 6520  , the sizes are 
+0000dda0: 706f 7465 6e74 6961 6c6c 7920 6469 6666  potentially diff
+0000ddb0: 6572 656e 742c 2062 7574 2077 6520 7761  erent, but we wa
+0000ddc0: 6e74 2074 6f20 6f76 6572 7461 6b65 2074  nt to overtake t
+0000ddd0: 6865 206f 7468 6572 2e0a 2020 2020 2020  he other..      
+0000dde0: 2020 6966 206f 7468 6572 5f73 616d 655f    if other_same_
+0000ddf0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000de00: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
+0000de10: 2020 2320 436c 6561 6e75 7020 6576 6572    # Cleanup ever
+0000de20: 7974 6869 6e67 2c20 6573 7020 706f 7465  ything, esp pote
+0000de30: 6e74 6961 6c20 616c 7265 6164 7920 636f  ntial already co
+0000de40: 6d70 7574 6564 2073 697a 6573 2c20 6173  mputed sizes, as
+0000de50: 2074 6865 7365 206d 6967 6874 2062 6520   these might be 
+0000de60: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
+0000de70: 2020 2020 2066 6f72 2064 696d 5f20 696e       for dim_ in
+0000de80: 205b 7365 6c66 5f73 616d 655f 6173 2c20   [self_same_as, 
+0000de90: 7365 6c66 5d20 2b20 286c 6973 7428 7365  self] + (list(se
+0000dea0: 6c66 2e5f 6578 7472 612e 7361 6d65 5f66  lf._extra.same_f
+0000deb0: 6f72 5f62 6174 6368 5f63 7478 2e76 616c  or_batch_ctx.val
+0000dec0: 7565 7328 2929 2069 6620 7365 6c66 2e5f  ues()) if self._
+0000ded0: 6578 7472 6120 656c 7365 205b 5d29 3a0a  extra else []):.
+0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000def0: 6966 2064 696d 5f2e 6479 6e5f 7369 7a65  if dim_.dyn_size
+0000df00: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
+0000df10: 2020 2020 2020 2020 2020 6469 6d5f 2e64            dim_.d
+0000df20: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
+0000df30: 6568 6f6c 6465 7220 3d20 4e6f 6e65 0a20  eholder = None. 
+0000df40: 2020 2020 2020 206f 7468 6572 5f73 616d         other_sam
+0000df50: 655f 6261 7365 2e5f 6d65 7267 655f 7361  e_base._merge_sa
+0000df60: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
+0000df70: 5f64 6963 7428 7365 6c66 290a 2020 2020  _dict(self).    
+0000df80: 2020 2020 6f74 6865 722e 5f6d 6179 6265      other._maybe
+0000df90: 5f75 7064 6174 6528 290a 2020 2020 2020  _update().      
+0000dfa0: 2020 7365 6c66 2e73 616d 655f 6173 203d    self.same_as =
+0000dfb0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000dfc0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+0000dfd0: 6179 6265 5f75 7064 6174 6528 290a 2020  aybe_update().  
+0000dfe0: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+0000dff0: 6e5f 7369 7a65 2069 7320 6e6f 7420 4e6f  n_size is not No
+0000e000: 6e65 2061 6e64 206f 7468 6572 5f73 616d  ne and other_sam
+0000e010: 655f 6261 7365 2e64 796e 5f73 697a 6520  e_base.dyn_size 
+0000e020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000e030: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000e040: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
+0000e050: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000e060: 2e64 796e 5f73 697a 653a 0a20 2020 2020  .dyn_size:.     
+0000e070: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000e080: 6c66 2e62 6174 6368 203d 3d20 6f74 6865  lf.batch == othe
+0000e090: 725f 7361 6d65 5f62 6173 652e 6261 7463  r_same_base.batc
+0000e0a0: 6820 616e 6420 7365 6c66 2e63 6f6e 7472  h and self.contr
+0000e0b0: 6f6c 5f66 6c6f 775f 6374 7820 3d3d 206f  ol_flow_ctx == o
+0000e0c0: 7468 6572 5f73 616d 655f 6261 7365 2e63  ther_same_base.c
+0000e0d0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 783a  ontrol_flow_ctx:
+0000e0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e0f0: 2020 2020 2023 204e 6f74 653a 2049 6e73       # Note: Ins
+0000e100: 7465 6164 206f 6620 6d61 6b69 6e67 2074  tead of making t
+0000e110: 6869 7320 6120 7761 726e 696e 672c 2077  his a warning, w
+0000e120: 6520 636f 756c 6420 616c 736f 2065 6e66  e could also enf
+0000e130: 6f72 6365 2074 6869 7320 6174 2073 6f6d  orce this at som
+0000e140: 6520 706f 696e 742e 0a20 2020 2020 2020  e point..       
+0000e150: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+0000e160: 2054 6865 2075 7365 7220 7368 6f75 6c64   The user should
+0000e170: 2062 6520 6162 6c65 2074 6f20 6669 7820   be able to fix 
+0000e180: 6065 7874 6572 6e5f 6461 7461 6020 696e  `extern_data` in
+0000e190: 2074 6865 2063 6f6e 6669 670a 2020 2020   the config.    
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1b0: 2320 2020 7375 6368 2074 6861 7420 7468  #   such that th
+0000e1c0: 6973 2069 7320 636f 7272 6563 7420 696e  is is correct in
+0000e1d0: 2074 6865 2066 6972 7374 2070 6c61 6365   the first place
+0000e1e0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e1f0: 2020 2020 2020 2320 2020 416c 736f 2c20        #   Also, 
+0000e200: 696e 2061 6464 6974 696f 6e20 746f 2074  in addition to t
+0000e210: 6869 7320 7761 726e 696e 672c 0a20 2020  his warning,.   
+0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e230: 2023 2020 2077 6520 6d69 6768 7420 7761   #   we might wa
+0000e240: 6e74 2074 6f20 6164 6420 736f 6d65 2072  nt to add some r
+0000e250: 756e 7469 6d65 2063 6865 636b 206f 6e20  untime check on 
+0000e260: 7468 6520 6571 206f 6620 7468 6520 6479  the eq of the dy
+0000e270: 6e20 7369 7a65 732e 0a20 2020 2020 2020  n sizes..       
+0000e280: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000e290: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+0000e2a0: 2020 2020 2020 2020 2020 2020 2257 6172              "War
+0000e2b0: 6e69 6e67 3a20 6173 7375 6d69 6e67 2064  ning: assuming d
+0000e2c0: 696d 2074 6167 7320 6172 6520 7361 6d65  im tags are same
+0000e2d0: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
+0000e2e0: 7369 7a65 2070 6c61 6365 686f 6c64 6572  size placeholder
+0000e2f0: 733a 2025 7220 7673 2025 7222 0a20 2020  s: %r vs %r".   
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 2020 2025 2028 7365 6c66 2e64 796e       % (self.dyn
+0000e320: 5f73 697a 652c 206f 7468 6572 5f73 616d  _size, other_sam
+0000e330: 655f 6261 7365 2e64 796e 5f73 697a 6529  e_base.dyn_size)
+0000e340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e350: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+0000e360: 2049 6620 7765 2068 6176 6520 6120 6465   If we have a de
+0000e370: 6669 6e65 6420 736f 7572 6365 2c20 616e  fined source, an
+0000e380: 6420 7468 6973 2069 7320 6120 6479 6e61  d this is a dyna
+0000e390: 6d69 6320 7370 6174 6961 6c20 6178 6973  mic spatial axis
+0000e3a0: 2c20 616e 6420 6974 2077 6173 2075 6e64  , and it was und
+0000e3b0: 6566 696e 6564 2062 6566 6f72 652c 0a20  efined before,. 
+0000e3c0: 2020 2020 2020 2023 206d 6179 6265 2077         # maybe w
+0000e3d0: 6520 6361 6e20 6f76 6572 7461 6b65 2074  e can overtake t
+0000e3e0: 6865 2073 697a 655f 706c 6163 6568 6f6c  he size_placehol
+0000e3f0: 6465 7220 6e6f 772e 0a20 2020 2020 2020  der now..       
+0000e400: 2069 6620 6f74 6865 725f 7361 6d65 5f62   if other_same_b
+0000e410: 6173 652e 6479 6e5f 7369 7a65 2069 7320  ase.dyn_size is 
+0000e420: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
+0000e430: 662e 5f65 7874 7261 2061 6e64 2073 656c  f._extra and sel
+0000e440: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
+0000e450: 613a 0a20 2020 2020 2020 2020 2020 2061  a:.            a
+0000e460: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+0000e470: 2873 656c 662e 5f65 7874 7261 2e73 7263  (self._extra.src
+0000e480: 5f61 7869 732c 2069 6e74 290a 2020 2020  _axis, int).    
+0000e490: 2020 2020 2020 2020 2320 4d61 7962 6520          # Maybe 
+0000e4a0: 6974 2063 6861 6e67 6564 2069 6e20 7468  it changed in th
+0000e4b0: 6520 6d65 616e 7768 696c 652c 2073 6f20  e meanwhile, so 
+0000e4c0: 6368 6563 6b2e 0a20 2020 2020 2020 2020  check..         
+0000e4d0: 2020 2074 6167 203d 2073 656c 662e 5f65     tag = self._e
+0000e4e0: 7874 7261 2e73 7263 5f64 6174 612e 6765  xtra.src_data.ge
+0000e4f0: 745f 6469 6d5f 7461 6728 7365 6c66 2e5f  t_dim_tag(self._
+0000e500: 6578 7472 612e 7372 635f 6178 6973 290a  extra.src_axis).
+0000e510: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0000e520: 6167 2e64 6573 6372 6970 7469 6f6e 203d  ag.description =
+0000e530: 3d20 7365 6c66 2e64 6573 6372 6970 7469  = self.descripti
+0000e540: 6f6e 2061 6e64 2028 6e6f 7420 7461 672e  on and (not tag.
+0000e550: 6479 6e5f 7369 7a65 5f65 7874 206f 7220  dyn_size_ext or 
+0000e560: 6e6f 7420 7461 672e 5f76 616c 6964 6174  not tag._validat
+0000e570: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
+0000e580: 7068 2829 293a 0a20 2020 2020 2020 2020  ph()):.         
+0000e590: 2020 2020 2020 2074 6167 2e64 796e 5f73         tag.dyn_s
+0000e5a0: 697a 655f 6578 7420 3d20 7365 6c66 2e67  ize_ext = self.g
+0000e5b0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
+0000e5c0: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2074 6167 2e62 6174 6368 2c20 7461     tag.batch, ta
+0000e5f0: 672e 636f 6e74 726f 6c5f 666c 6f77 5f63  g.control_flow_c
+0000e600: 7478 2c20 7465 6d70 6c61 7465 5f6f 6e6c  tx, template_onl
+0000e610: 793d 5472 7565 0a20 2020 2020 2020 2020  y=True.         
+0000e620: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000e630: 2020 2020 2020 2020 2074 6167 2e5f 6d61           tag._ma
+0000e640: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
+0000e650: 2020 2020 2023 2049 6620 6f74 6865 7273       # If others
+0000e660: 2064 796e 5f73 697a 6520 6973 204e 6f6e   dyn_size is Non
+0000e670: 6520 6275 7420 7765 2068 6176 6520 6120  e but we have a 
+0000e680: 6479 6e5f 7369 7a65 2c20 6d61 7962 6520  dyn_size, maybe 
+0000e690: 7570 6461 7465 206f 7468 6572 7320 6479  update others dy
+0000e6a0: 6e5f 7369 7a65 2e0a 2020 2020 2020 2020  n_size..        
+0000e6b0: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
+0000e6c0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000e6d0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000e6e0: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
+0000e6f0: 2073 656c 662e 6479 6e5f 7369 7a65 3a0a   self.dyn_size:.
+0000e700: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
+0000e710: 756c 6420 6265 2075 6e73 6574 2069 6620  uld be unset if 
+0000e720: 6974 2063 6f6d 6573 2066 726f 6d20 7468  it comes from th
+0000e730: 6520 636f 6e66 6967 2c20 6f72 2066 726f  e config, or fro
+0000e740: 6d20 7072 6576 2067 7261 7068 2063 7265  m prev graph cre
+0000e750: 6174 696f 6e2e 0a20 2020 2020 2020 2020  ation..         
+0000e760: 2020 2023 2054 6869 7320 6973 2069 6d70     # This is imp
+0000e770: 6f72 7461 6e74 2073 7563 6820 7468 6174  ortant such that
+0000e780: 2073 656c 662e 6361 6e5f 636f 6d70 6172   self.can_compar
+0000e790: 6528 2920 6973 2073 616e 652e 0a20 2020  e() is sane..   
+0000e7a0: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
+0000e7b0: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
+0000e7c0: 7369 7a65 2069 7320 4e6f 6e65 206f 7220  size is None or 
+0000e7d0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
+0000e7e0: 6173 652e 5f76 616c 6964 6174 655f 696e  ase._validate_in
+0000e7f0: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
+0000e800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e810: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
+0000e820: 652e 6479 6e5f 7369 7a65 5f65 7874 203d  e.dyn_size_ext =
+0000e830: 2073 656c 662e 6765 745f 6479 6e5f 7369   self.get_dyn_si
+0000e840: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
+0000e850: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
+0000e860: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+0000e870: 7361 6d65 5f62 6173 652e 6261 7463 682c  same_base.batch,
+0000e880: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000e890: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000e8a0: 782c 2074 656d 706c 6174 655f 6f6e 6c79  x, template_only
+0000e8b0: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
+0000e8c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000e8d0: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
+0000e8e0: 6d65 5f62 6173 652e 5f6d 6179 6265 5f75  me_base._maybe_u
+0000e8f0: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
+0000e900: 6966 206e 6f74 2073 656c 662e 6479 6e5f  if not self.dyn_
+0000e910: 7369 7a65 5f65 7874 206f 7220 6e6f 7420  size_ext or not 
+0000e920: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
+0000e930: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000e940: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000e950: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+0000e960: 203d 206f 7468 6572 5f73 616d 655f 6261   = other_same_ba
+0000e970: 7365 2e67 6574 5f64 796e 5f73 697a 655f  se.get_dyn_size_
+0000e980: 6578 745f 666f 725f 6261 7463 685f 6374  ext_for_batch_ct
+0000e990: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
+0000e9a0: 2020 2073 656c 662e 6261 7463 682c 2073     self.batch, s
+0000e9b0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+0000e9c0: 5f63 7478 2c20 7465 6d70 6c61 7465 5f6f  _ctx, template_o
+0000e9d0: 6e6c 793d 5472 7565 0a20 2020 2020 2020  nly=True.       
+0000e9e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000e9f0: 2020 2073 656c 662e 5f6d 6179 6265 5f75     self._maybe_u
+0000ea00: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
+0000ea10: 656c 6966 206f 7468 6572 5f73 616d 655f  elif other_same_
+0000ea20: 6261 7365 2e64 796e 5f73 697a 655f 6578  base.dyn_size_ex
+0000ea30: 7420 6973 204e 6f6e 6520 6f72 206e 6f74  t is None or not
+0000ea40: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000ea50: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000ea60: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
+0000ea70: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000ea80: 5f73 616d 655f 6261 7365 2e64 796e 5f73  _same_base.dyn_s
+0000ea90: 697a 655f 6578 7420 3d20 7365 6c66 2e67  ize_ext = self.g
+0000eaa0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
+0000eab0: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
+0000eac0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ead0: 7468 6572 5f73 616d 655f 6261 7365 2e62  ther_same_base.b
+0000eae0: 6174 6368 2c20 6f74 6865 725f 7361 6d65  atch, other_same
+0000eaf0: 5f62 6173 652e 636f 6e74 726f 6c5f 666c  _base.control_fl
+0000eb00: 6f77 5f63 7478 2c20 7465 6d70 6c61 7465  ow_ctx, template
+0000eb10: 5f6f 6e6c 793d 5472 7565 0a20 2020 2020  _only=True.     
+0000eb20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000eb30: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
+0000eb40: 6261 7365 2e5f 6d61 7962 655f 7570 6461  base._maybe_upda
+0000eb50: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
+0000eb60: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
+0000eb70: 6e28 2920 616e 6420 6f74 6865 722e 6973  n() and other.is
+0000eb80: 5f64 696d 5f6b 6e6f 776e 2829 3a0a 2020  _dim_known():.  
+0000eb90: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000eba0: 2073 656c 662e 6469 6d65 6e73 696f 6e20   self.dimension 
+0000ebb0: 3d3d 206f 7468 6572 2e64 696d 656e 7369  == other.dimensi
+0000ebc0: 6f6e 0a20 2020 2020 2020 2065 6c69 6620  on.        elif 
+0000ebd0: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
+0000ebe0: 6e28 2920 616e 6420 6e6f 7420 6f74 6865  n() and not othe
+0000ebf0: 722e 6973 5f64 696d 5f6b 6e6f 776e 2829  r.is_dim_known()
+0000ec00: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
+0000ec10: 6865 722e 6361 7061 6369 7479 203d 2073  her.capacity = s
+0000ec20: 656c 662e 6361 7061 6369 7479 0a20 2020  elf.capacity.   
+0000ec30: 2020 2020 2020 2020 206f 7468 6572 2e73           other.s
+0000ec40: 697a 6520 3d20 7365 6c66 2e73 697a 650a  ize = self.size.
+0000ec50: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
+0000ec60: 2073 656c 662e 6973 5f64 696d 5f6b 6e6f   self.is_dim_kno
+0000ec70: 776e 2829 2061 6e64 206f 7468 6572 2e69  wn() and other.i
+0000ec80: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
+0000ec90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eca0: 6361 7061 6369 7479 203d 206f 7468 6572  capacity = other
+0000ecb0: 2e63 6170 6163 6974 790a 2020 2020 2020  .capacity.      
+0000ecc0: 2020 2020 2020 7365 6c66 2e73 697a 6520        self.size 
+0000ecd0: 3d20 6f74 6865 722e 7369 7a65 0a20 2020  = other.size.   
+0000ece0: 2020 2020 2069 6620 7365 6c66 2e76 6f63       if self.voc
+0000ecf0: 6162 2061 6e64 206e 6f74 206f 7468 6572  ab and not other
+0000ed00: 5f73 616d 655f 6261 7365 2e76 6f63 6162  _same_base.vocab
+0000ed10: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
+0000ed20: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
+0000ed30: 6361 6220 3d20 7365 6c66 2e76 6f63 6162  cab = self.vocab
+0000ed40: 0a20 2020 2020 2020 2065 6c69 6620 6f74  .        elif ot
+0000ed50: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
+0000ed60: 6361 6220 616e 6420 6e6f 7420 7365 6c66  cab and not self
+0000ed70: 2e76 6f63 6162 3a0a 2020 2020 2020 2020  .vocab:.        
+0000ed80: 2020 2020 7365 6c66 2e76 6f63 6162 203d      self.vocab =
+0000ed90: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000eda0: 2e76 6f63 6162 0a20 2020 2020 2020 2073  .vocab.        s
+0000edb0: 656c 662e 5f6d 616b 655f 6578 7472 6128  elf._make_extra(
+0000edc0: 290a 2020 2020 2020 2020 7365 6c66 5f73  ).        self_s
+0000edd0: 616d 655f 6173 2e5f 6d61 6b65 5f65 7874  ame_as._make_ext
+0000ede0: 7261 2829 0a20 2020 2020 2020 2023 206e  ra().        # n
+0000edf0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
+0000ee00: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
+0000ee10: 2020 2020 2020 7365 6c66 2e5f 6578 7472        self._extr
+0000ee20: 612e 6175 746f 5f67 656e 6572 6174 6564  a.auto_generated
+0000ee30: 203d 2073 656c 665f 7361 6d65 5f61 732e   = self_same_as.
+0000ee40: 5f65 7874 7261 2e61 7574 6f5f 6765 6e65  _extra.auto_gene
+0000ee50: 7261 7465 6420 3d20 6f74 6865 725f 7361  rated = other_sa
+0000ee60: 6d65 5f62 6173 652e 6175 746f 5f67 656e  me_base.auto_gen
+0000ee70: 6572 6174 6564 0a20 2020 2020 2020 2023  erated.        #
+0000ee80: 2054 616b 6520 6f76 6572 2064 6572 6976   Take over deriv
+0000ee90: 6564 5f66 726f 6d5f 6f70 2e20 486f 7765  ed_from_op. Howe
+0000eea0: 7665 722c 206f 6e6c 7920 6966 2074 6869  ver, only if thi
+0000eeb0: 7320 776f 756c 6420 6e6f 7420 696e 7472  s would not intr
+0000eec0: 6f64 7563 6520 6379 636c 6573 210a 2020  oduce cycles!.  
+0000eed0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0000eee0: 665f 6465 7269 7665 645f 6261 7365 732e  f_derived_bases.
+0000eef0: 6973 7375 7065 7273 6574 286f 7468 6572  issuperset(other
+0000ef00: 5f64 6572 6976 6564 5f62 6173 6573 293a  _derived_bases):
+0000ef10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000ef20: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
+0000ef30: 6d5f 6f70 2061 6e64 206e 6f74 206f 7468  m_op and not oth
+0000ef40: 6572 5f73 616d 655f 6261 7365 2e64 6572  er_same_base.der
+0000ef50: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000ef70: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+0000ef80: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000efa0: 7468 6572 5f73 616d 655f 6261 7365 2e5f  ther_same_base._
+0000efb0: 6d61 6b65 5f65 7874 7261 2829 2e64 6572  make_extra().der
+0000efc0: 6976 6564 5f66 726f 6d5f 6f70 203d 2073  ived_from_op = s
+0000efd0: 656c 662e 6465 7269 7665 645f 6672 6f6d  elf.derived_from
+0000efe0: 5f6f 700a 2020 2020 2020 2020 2020 2020  _op.            
+0000eff0: 656c 6966 206f 7468 6572 5f73 616d 655f  elif other_same_
+0000f000: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000f010: 6d5f 6f70 2061 6e64 206e 6f74 2073 656c  m_op and not sel
+0000f020: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
+0000f030: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+0000f040: 2020 2073 656c 662e 5f6d 616b 655f 6578     self._make_ex
+0000f050: 7472 6128 292e 6465 7269 7665 645f 6672  tra().derived_fr
+0000f060: 6f6d 5f6f 7020 3d20 6f74 6865 725f 7361  om_op = other_sa
+0000f070: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
+0000f080: 6672 6f6d 5f6f 700a 2020 2020 2020 2020  from_op.        
+0000f090: 6966 2073 656c 662e 5f65 7874 7261 2061  if self._extra a
+0000f0a0: 6e64 206e 6f74 206f 7468 6572 5f73 616d  nd not other_sam
+0000f0b0: 655f 6261 7365 2e69 735f 6479 6e61 6d69  e_base.is_dynami
+0000f0c0: 6328 293a 0a20 2020 2020 2020 2020 2020  c():.           
+0000f0d0: 2023 2054 686f 7365 206d 6967 6874 2062   # Those might b
+0000f0e0: 6520 7365 7420 7669 6120 6765 745f 6261  e set via get_ba
+0000f0f0: 7463 685f 666f 725f 6374 7820 666f 7220  tch_for_ctx for 
+0000f100: 616e 2075 6e64 6566 696e 6564 2064 696d  an undefined dim
+0000f110: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0000f120: 7768 6963 6820 6e6f 7720 6265 636f 6d65  which now become
+0000f130: 7320 7374 6174 6963 2064 7565 2074 6f20  s static due to 
+0000f140: 606f 7468 6572 602e 0a20 2020 2020 2020  `other`..       
+0000f150: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
+0000f160: 2e62 6174 6368 203d 204e 6f6e 650a 2020  .batch = None.  
+0000f170: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000f180: 6578 7472 612e 636f 6e74 726f 6c5f 666c  extra.control_fl
+0000f190: 6f77 5f63 7478 203d 204e 6f6e 650a 2020  ow_ctx = None.  
+0000f1a0: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+0000f1b0: 792c 2064 696d 5f20 696e 2073 656c 662e  y, dim_ in self.
+0000f1c0: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000f1d0: 6261 7463 685f 6374 782e 6974 656d 7328  batch_ctx.items(
+0000f1e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000f1f0: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
+0000f200: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
+0000f210: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
+0000f220: 2020 2020 6469 6d5f 6578 7472 6120 3d20      dim_extra = 
+0000f230: 6469 6d5f 2e5f 6578 7472 610a 2020 2020  dim_._extra.    
+0000f240: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000f250: 696d 5f65 7874 7261 3a0a 2020 2020 2020  im_extra:.      
+0000f260: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0000f270: 6d5f 6578 7472 612e 6261 7463 6820 3d20  m_extra.batch = 
+0000f280: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000f290: 2020 2020 2020 2020 2064 696d 5f65 7874           dim_ext
+0000f2a0: 7261 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  ra.control_flow_
+0000f2b0: 6374 7820 3d20 4e6f 6e65 0a20 2020 2020  ctx = None.     
+0000f2c0: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+0000f2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f2e0: 6c66 5f20 3d20 7365 6c66 2e67 6574 5f66  lf_ = self.get_f
+0000f2f0: 6f72 5f62 6174 6368 5f63 7478 2862 6174  or_batch_ctx(bat
+0000f300: 6368 3d73 656c 662e 6261 7463 682c 2063  ch=self.batch, c
+0000f310: 7478 3d73 656c 662e 636f 6e74 726f 6c5f  tx=self.control_
+0000f320: 666c 6f77 5f63 7478 290a 2020 2020 2020  flow_ctx).      
+0000f330: 2020 2020 2020 6966 2073 656c 665f 2069        if self_ i
+0000f340: 7320 6e6f 7420 7365 6c66 3a0a 2020 2020  s not self:.    
+0000f350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f360: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000f370: 7820 3d20 7365 6c66 5f2e 636f 6e74 726f  x = self_.contro
+0000f380: 6c5f 666c 6f77 5f63 7478 2020 2320 6d69  l_flow_ctx  # mi
+0000f390: 6768 7420 6265 2064 6966 6665 7265 6e74  ght be different
+0000f3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f3b0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+0000f3c0: 7874 203d 2073 656c 665f 2e64 796e 5f73  xt = self_.dyn_s
+0000f3d0: 697a 655f 6578 7420 2023 206d 6967 6874  ize_ext  # might
+0000f3e0: 2062 6520 756e 7365 740a 0a20 2020 2064   be unset..    d
+0000f3f0: 6566 205f 6d65 7267 655f 7361 6d65 5f66  ef _merge_same_f
+0000f400: 6f72 5f62 6174 6368 5f63 7478 5f64 6963  or_batch_ctx_dic
+0000f410: 7428 7365 6c66 3a20 5f64 2e44 696d 2c20  t(self: _d.Dim, 
+0000f420: 6f74 6865 723a 205f 642e 4469 6d29 3a0a  other: _d.Dim):.
+0000f430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f440: 2020 2020 3a70 6172 616d 206f 7468 6572      :param other
+0000f450: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f460: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+0000f470: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+0000f480: 4d65 6d62 6572 0a20 2020 2020 2020 2069  Member.        i
+0000f490: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
+0000f4a0: 6120 616e 6420 6e6f 7420 6f74 6865 722e  a and not other.
+0000f4b0: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
+0000f4c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000f4d0: 2020 2073 656c 662e 5f76 616c 6964 6174     self._validat
+0000f4e0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
+0000f4f0: 7068 2829 0a20 2020 2020 2020 2069 6620  ph().        if 
+0000f500: 7365 6c66 2e5f 6578 7472 613a 0a20 2020  self._extra:.   
+0000f510: 2020 2020 2020 2020 2066 6f72 205f 2c20           for _, 
+0000f520: 6469 6d20 696e 206c 6973 7428 7365 6c66  dim in list(self
+0000f530: 2e5f 6578 7472 612e 7361 6d65 5f66 6f72  ._extra.same_for
+0000f540: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
+0000f550: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+0000f560: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+0000f570: 7374 616e 6365 2864 696d 2c20 5f64 2e44  stance(dim, _d.D
+0000f580: 696d 290a 2020 2020 2020 2020 2020 2020  im).            
+0000f590: 2020 2020 6469 6d2e 5f76 616c 6964 6174      dim._validat
+0000f5a0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
+0000f5b0: 7068 2829 0a20 2020 2020 2020 2023 206e  ph().        # n
+0000f5c0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
+0000f5d0: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
+0000f5e0: 2020 2020 2020 6966 206f 7468 6572 2e5f        if other._
+0000f5f0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+0000f600: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
+0000f610: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
+0000f620: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
+0000f630: 666f 7220 6b65 792c 2064 696d 2069 6e20  for key, dim in 
+0000f640: 6f74 6865 722e 5f65 7874 7261 2e73 616d  other._extra.sam
+0000f650: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
+0000f660: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0000f670: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000f680: 6469 6d2e 5f76 616c 6964 6174 655f 696e  dim._validate_in
+0000f690: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
+0000f6a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f6b0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f6d0: 656c 665f 6469 6d20 3d20 7365 6c66 2e5f  elf_dim = self._
+0000f6e0: 6d61 6b65 5f65 7874 7261 2829 2e73 616d  make_extra().sam
+0000f6f0: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
+0000f700: 6765 7428 6b65 792c 204e 6f6e 6529 0a20  get(key, None). 
+0000f710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f720: 6620 7365 6c66 5f64 696d 2061 6e64 2028  f self_dim and (
+0000f730: 7365 6c66 5f64 696d 2e64 796e 5f73 697a  self_dim.dyn_siz
+0000f740: 655f 6578 7420 6f72 206e 6f74 2064 696d  e_ext or not dim
+0000f750: 2e64 796e 5f73 697a 655f 6578 7429 3a0a  .dyn_size_ext):.
+0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f770: 2020 2020 636f 6e74 696e 7565 2020 2320      continue  # 
+0000f780: 6b65 6570 206f 7572 730a 2020 2020 2020  keep ours.      
+0000f790: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000f7a0: 2064 696d 2e64 796e 5f73 697a 655f 6578   dim.dyn_size_ex
+0000f7b0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000f7c0: 2020 2020 2020 2063 6f6e 7469 6e75 6520         continue 
+0000f7d0: 2023 2075 6e64 6566 696e 6564 2c20 646f   # undefined, do
+0000f7e0: 206e 6f74 206f 7665 7274 616b 650a 2020   not overtake.  
+0000f7f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f800: 6c66 2e5f 6578 7472 612e 7361 6d65 5f66  lf._extra.same_f
+0000f810: 6f72 5f62 6174 6368 5f63 7478 5b6b 6579  or_batch_ctx[key
+0000f820: 5d20 3d20 6469 6d0a 2020 2020 2020 2020  ] = dim.        
+0000f830: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+0000f840: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+0000f850: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+0000f860: 206f 7468 6572 2e5f 6578 7472 612e 7361   other._extra.sa
+0000f870: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
+0000f880: 2e63 6c65 6172 2829 2020 2320 7765 206f  .clear()  # we o
+0000f890: 6e6c 7920 7761 6e74 2074 6f20 6861 7665  nly want to have
+0000f8a0: 2069 7420 6f6e 6365 0a0a 2020 2020 2320   it once..    # 
+0000f8b0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+0000f8c0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+0000f8d0: 2020 2064 6566 2064 6572 6976 655f 6672     def derive_fr
+0000f8e0: 6f6d 2873 656c 663a 205f 642e 4469 6d2c  om(self: _d.Dim,
+0000f8f0: 2062 6173 653a 205f 642e 4469 6d2c 2073   base: _d.Dim, s
+0000f900: 6574 5f64 6572 6976 6564 5f66 726f 6d5f  et_derived_from_
+0000f910: 666c 6167 3a20 626f 6f6c 203d 2054 7275  flag: bool = Tru
+0000f920: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+0000f930: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+0000f940: 6173 653a 2064 696d 0a20 2020 2020 2020  ase: dim.       
+0000f950: 203a 7061 7261 6d20 7365 745f 6465 7269   :param set_deri
+0000f960: 7665 645f 6672 6f6d 5f66 6c61 673a 0a20  ved_from_flag:. 
+0000f970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f980: 2020 2073 656c 665f 6261 7365 203d 2073     self_base = s
+0000f990: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
+0000f9a0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000f9b0: 5f62 6173 655f 6578 7472 6120 3d20 7365  _base_extra = se
+0000f9c0: 6c66 5f62 6173 652e 5f6d 616b 655f 6578  lf_base._make_ex
+0000f9d0: 7472 6128 290a 2020 2020 2020 2020 6966  tra().        if
+0000f9e0: 2073 6574 5f64 6572 6976 6564 5f66 726f   set_derived_fro
+0000f9f0: 6d5f 666c 6167 3a0a 2020 2020 2020 2020  m_flag:.        
+0000fa00: 2020 2020 6966 2073 656c 665f 6261 7365      if self_base
+0000fa10: 5f65 7874 7261 2e64 6572 6976 6564 5f66  _extra.derived_f
+0000fa20: 726f 6d5f 7461 673a 0a20 2020 2020 2020  rom_tag:.       
+0000fa30: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000fa40: 7365 6c66 5f62 6173 655f 6578 7472 612e  self_base_extra.
+0000fa50: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+0000fa60: 203d 3d20 6261 7365 0a20 2020 2020 2020   == base.       
+0000fa70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000fa80: 2020 2020 2020 2020 2020 2073 656c 665f             self_
+0000fa90: 6261 7365 5f65 7874 7261 2e64 6572 6976  base_extra.deriv
+0000faa0: 6564 5f66 726f 6d5f 7461 6720 3d20 6261  ed_from_tag = ba
+0000fab0: 7365 0a20 2020 2020 2020 2069 6620 6e6f  se.        if no
+0000fac0: 7420 7365 6c66 2e62 6174 6368 2061 6e64  t self.batch and
+0000fad0: 2062 6173 652e 6261 7463 683a 0a20 2020   base.batch:.   
+0000fae0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+0000faf0: 7463 6820 3d20 6261 7365 2e62 6174 6368  tch = base.batch
+0000fb00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fb10: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+0000fb20: 7478 203d 2062 6173 652e 636f 6e74 726f  tx = base.contro
+0000fb30: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
+0000fb40: 2020 2020 2020 206b 6579 203d 2062 6173         key = bas
+0000fb50: 652e 6261 7463 682c 2062 6173 652e 636f  e.batch, base.co
+0000fb60: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a20  ntrol_flow_ctx. 
+0000fb70: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000fb80: 7420 6b65 7920 6e6f 7420 696e 2073 656c  t key not in sel
+0000fb90: 665f 6261 7365 5f65 7874 7261 2e73 616d  f_base_extra.sam
+0000fba0: 655f 666f 725f 6261 7463 685f 6374 780a  e_for_batch_ctx.
+0000fbb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fbc0: 5f62 6173 655f 6578 7472 612e 7361 6d65  _base_extra.same
+0000fbd0: 5f66 6f72 5f62 6174 6368 5f63 7478 5b6b  _for_batch_ctx[k
+0000fbe0: 6579 5d20 3d20 7365 6c66 0a20 2020 2020  ey] = self.     
+0000fbf0: 2020 2069 6620 7365 6c66 2e69 735f 6479     if self.is_dy
+0000fc00: 6e61 6d69 6328 2920 6f72 206e 6f74 2073  namic() or not s
+0000fc10: 656c 662e 6973 5f64 696d 5f6b 6e6f 776e  elf.is_dim_known
+0000fc20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000fc30: 6966 206e 6f74 2073 656c 662e 6479 6e5f  if not self.dyn_
+0000fc40: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
+0000fc50: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
+0000fc60: 652e 6479 6e5f 7369 7a65 5f65 7874 3a0a  e.dyn_size_ext:.
+0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc80: 2020 2020 6966 2062 6173 652e 6261 7463      if base.batc
+0000fc90: 6820 616e 6420 6261 7365 2e62 6174 6368  h and base.batch
+0000fca0: 203d 3d20 7365 6c66 2e62 6174 6368 2061   == self.batch a
+0000fcb0: 6e64 2062 6173 652e 636f 6e74 726f 6c5f  nd base.control_
+0000fcc0: 666c 6f77 5f63 7478 203d 3d20 7365 6c66  flow_ctx == self
+0000fcd0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000fce0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
+0000fcf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fd00: 6479 6e5f 7369 7a65 5f65 7874 203d 2062  dyn_size_ext = b
+0000fd10: 6173 652e 6479 6e5f 7369 7a65 5f65 7874  ase.dyn_size_ext
+0000fd20: 2e63 6f70 795f 7465 6d70 6c61 7465 286e  .copy_template(n
+0000fd30: 616d 653d 2225 733a 7369 7a65 2220 2520  ame="%s:size" % 
+0000fd40: 7365 6c66 5f62 6173 652e 6465 7363 7269  self_base.descri
+0000fd50: 7074 696f 6e29 0a20 2020 2020 2020 2020  ption).         
+0000fd60: 2020 2020 2020 2065 6c69 6620 6261 7365         elif base
+0000fd70: 2e69 735f 6261 7463 685f 6469 6d28 293a  .is_batch_dim():
+0000fd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fd90: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
+0000fda0: 7a65 5f65 7874 203d 205f 742e 5465 6e73  ze_ext = _t.Tens
+0000fdb0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000fdc0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000fdd0: 3d22 2573 3a62 6174 6368 2220 2520 7365  ="%s:batch" % se
+0000fde0: 6c66 5f62 6173 652e 6465 7363 7269 7074  lf_base.descript
+0000fdf0: 696f 6e2c 2073 6861 7065 3d28 292c 2064  ion, shape=(), d
+0000fe00: 7479 7065 3d22 696e 7433 3222 2c20 6261  type="int32", ba
+0000fe10: 7463 685f 6469 6d5f 6178 6973 3d4e 6f6e  tch_dim_axis=Non
+0000fe20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000fe30: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000fe40: 2063 6f70 795f 6672 6f6d 2873 656c 663a   copy_from(self:
+0000fe50: 2044 696d 2c20 6f74 6865 723a 2044 696d   Dim, other: Dim
+0000fe60: 293a 0a20 2020 2020 2020 2022 2222 6465  ):.        """de
+0000fe70: 6669 6e65 2222 220a 2020 2020 2020 2020  fine""".        
+0000fe80: 7365 6c66 2e73 697a 6520 3d20 6f74 6865  self.size = othe
+0000fe90: 722e 7369 7a65 0a20 2020 2020 2020 2073  r.size.        s
+0000fea0: 656c 662e 6361 7061 6369 7479 203d 206f  elf.capacity = o
+0000feb0: 7468 6572 2e63 6170 6163 6974 790a 2020  ther.capacity.  
+0000fec0: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
+0000fed0: 697a 655f 6578 7420 3d20 6f74 6865 722e  ize_ext = other.
+0000fee0: 6479 6e5f 7369 7a65 5f65 7874 0a20 2020  dyn_size_ext.   
+0000fef0: 2020 2020 2073 656c 662e 6465 7269 7665       self.derive
+0000ff00: 5f66 726f 6d28 6f74 6865 7229 0a0a 2020  _from(other)..  
+0000ff10: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+0000ff20: 2020 2064 6566 2067 6574 5f65 7869 7374     def get_exist
+0000ff30: 696e 675f 7461 675f 6672 6f6d 5f63 6f6c  ing_tag_from_col
+0000ff40: 6c65 6374 696f 6e28 636c 732c 206f 7468  lection(cls, oth
+0000ff50: 6572 2c20 7461 6773 2c20 6973 5f65 7175  er, tags, is_equ
+0000ff60: 616c 5f6f 7074 733d 4e6f 6e65 293a 0a20  al_opts=None):. 
+0000ff70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ff80: 2020 203a 7061 7261 6d20 4469 6d20 6f74     :param Dim ot
+0000ff90: 6865 723a 0a20 2020 2020 2020 203a 7061  her:.        :pa
+0000ffa0: 7261 6d20 6c69 7374 5b44 696d 5d7c 7475  ram list[Dim]|tu
+0000ffb0: 706c 655b 4469 6d5d 7c73 6574 5b44 696d  ple[Dim]|set[Dim
+0000ffc0: 5d20 7461 6773 3a0a 2020 2020 2020 2020  ] tags:.        
+0000ffd0: 3a70 6172 616d 2064 6963 745b 7374 725d  :param dict[str]
+0000ffe0: 7c4e 6f6e 6520 6973 5f65 7175 616c 5f6f  |None is_equal_o
+0000fff0: 7074 733a 2070 6173 7365 6420 746f 2044  pts: passed to D
+00010000: 696d 2e69 735f 6571 7561 6c0a 2020 2020  im.is_equal.    
+00010010: 2020 2020 3a72 7479 7065 3a20 4469 6d7c      :rtype: Dim|
+00010020: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+00010030: 0a20 2020 2020 2020 2069 6620 6973 5f65  .        if is_e
+00010040: 7175 616c 5f6f 7074 7320 6973 204e 6f6e  qual_opts is Non
+00010050: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00010060: 735f 6571 7561 6c5f 6f70 7473 203d 207b  s_equal_opts = {
+00010070: 7d0a 2020 2020 2020 2020 2320 5765 2064  }.        # We d
+00010080: 6f20 706f 7465 6e74 6961 6c20 6d75 6c74  o potential mult
+00010090: 6970 6c65 2072 6f75 6e64 732c 2073 7563  iple rounds, suc
+000100a0: 6820 7468 6174 2077 6520 7072 6566 6572  h that we prefer
+000100b0: 2022 6d6f 7265 2065 7175 616c 2220 2875   "more equal" (u
+000100c0: 7369 6e67 206c 6573 7320 6973 5f65 7175  sing less is_equ
+000100d0: 616c 5f6f 7074 7329 2e0a 2020 2020 2020  al_opts)..      
+000100e0: 2020 726f 756e 6473 203d 205b 7b7d 5d0a    rounds = [{}].
+000100f0: 2020 2020 2020 2020 6966 2069 735f 6571          if is_eq
+00010100: 7561 6c5f 6f70 7473 3a0a 2020 2020 2020  ual_opts:.      
+00010110: 2020 2020 2020 6966 2022 6272 6f61 6463        if "broadc
+00010120: 6173 745f 6d61 7463 6865 7322 2069 6e20  ast_matches" in 
+00010130: 6973 5f65 7175 616c 5f6f 7074 733a 0a20  is_equal_opts:. 
+00010140: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010150: 6f75 6e64 732e 6170 7065 6e64 287b 6b3a  ounds.append({k:
+00010160: 2076 2066 6f72 2028 6b2c 2076 2920 696e   v for (k, v) in
+00010170: 2069 735f 6571 7561 6c5f 6f70 7473 2e69   is_equal_opts.i
+00010180: 7465 6d73 2829 2069 6620 6b20 213d 2022  tems() if k != "
+00010190: 6272 6f61 6463 6173 745f 6d61 7463 6865  broadcast_matche
+000101a0: 7322 7d29 0a20 2020 2020 2020 2020 2020  s"}).           
+000101b0: 2072 6f75 6e64 732e 6170 7065 6e64 2869   rounds.append(i
+000101c0: 735f 6571 7561 6c5f 6f70 7473 290a 2020  s_equal_opts).  
+000101d0: 2020 2020 2020 666f 7220 5f69 735f 6571        for _is_eq
+000101e0: 7561 6c5f 6f70 7473 2069 6e20 726f 756e  ual_opts in roun
+000101f0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
+00010200: 666f 7220 5f74 6167 2069 6e20 7461 6773  for _tag in tags
+00010210: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010220: 2020 6966 205f 7461 672e 6973 5f65 7175    if _tag.is_equ
+00010230: 616c 286f 7468 6572 2c20 2a2a 5f69 735f  al(other, **_is_
+00010240: 6571 7561 6c5f 6f70 7473 293a 0a20 2020  equal_opts):.   
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 2072 6574 7572 6e20 5f74 6167 0a20 2020   return _tag.   
+00010270: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00010280: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00010290: 6f64 0a20 2020 2064 6566 2067 6574 5f61  od.    def get_a
+000102a0: 6c6c 5f64 696d 656e 7369 6f6e 5f74 6167  ll_dimension_tag
+000102b0: 7328 636c 732c 2064 6174 615f 6c69 7374  s(cls, data_list
+000102c0: 2c20 6973 5f65 7175 616c 5f6f 7074 733d  , is_equal_opts=
+000102d0: 4e6f 6e65 2c20 756e 6971 7565 5f73 6570  None, unique_sep
+000102e0: 6172 6174 655f 6178 6573 3d54 7275 6529  arate_axes=True)
+000102f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00010300: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
+00010310: 745b 5f74 2e54 656e 736f 725d 2064 6174  t[_t.Tensor] dat
+00010320: 615f 6c69 7374 3a0a 2020 2020 2020 2020  a_list:.        
+00010330: 3a70 6172 616d 2064 6963 745b 7374 725d  :param dict[str]
+00010340: 7c4e 6f6e 6520 6973 5f65 7175 616c 5f6f  |None is_equal_o
+00010350: 7074 733a 2070 6173 7365 6420 746f 2044  pts: passed to D
+00010360: 696d 2e69 735f 6571 7561 6c0a 2020 2020  im.is_equal.    
+00010370: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00010380: 756e 6971 7565 5f73 6570 6172 6174 655f  unique_separate_
+00010390: 6178 6573 3a20 652e 672e 2064 6174 615f  axes: e.g. data_
+000103a0: 6c69 7374 3d5b 4461 7461 2077 6974 6820  list=[Data with 
+000103b0: 7368 6170 6520 2842 2c35 2c35 2c31 3029  shape (B,5,5,10)
+000103c0: 5d20 7265 7375 6c74 7320 696e 2034 2064  ] results in 4 d
+000103d0: 696d 2074 6167 732c 206e 6f74 2033 2e0a  im tags, not 3..
+000103e0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000103f0: 206c 6973 7420 6f66 2064 696d 656e 7369   list of dimensi
+00010400: 6f6e 2074 6167 732c 2064 6963 7420 666f  on tags, dict fo
+00010410: 7220 6461 7461 202d 3e20 6c69 7374 206f  r data -> list o
+00010420: 6620 6469 6d65 6e73 696f 6e20 7461 6773  f dimension tags
+00010430: 2028 666f 7220 6561 6368 2061 7869 7329   (for each axis)
+00010440: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00010450: 2028 6c69 7374 5b44 696d 5d2c 2075 7469   (list[Dim], uti
+00010460: 6c2e 4469 6374 5265 664b 6579 735b 5f74  l.DictRefKeys[_t
+00010470: 2e54 656e 736f 722c 206c 6973 745b 4469  .Tensor, list[Di
+00010480: 6d5d 5d29 0a20 2020 2020 2020 2022 2222  m]]).        """
+00010490: 0a20 2020 2020 2020 2074 6167 7320 3d20  .        tags = 
+000104a0: 5b5d 0a20 2020 2020 2020 2064 6174 615f  [].        data_
+000104b0: 6178 6573 5f64 6963 7420 3d20 7574 696c  axes_dict = util
+000104c0: 2e44 6963 7452 6566 4b65 7973 2829 2020  .DictRefKeys()  
+000104d0: 2320 7479 7065 3a20 7574 696c 2e44 6963  # type: util.Dic
+000104e0: 7452 6566 4b65 7973 5b5f 742e 5465 6e73  tRefKeys[_t.Tens
+000104f0: 6f72 2c20 4c69 7374 5b44 696d 5d5d 0a20  or, List[Dim]]. 
+00010500: 2020 2020 2020 2066 6f72 2064 6174 6120         for data 
+00010510: 696e 2064 6174 615f 6c69 7374 3a0a 2020  in data_list:.  
+00010520: 2020 2020 2020 2020 2020 6461 7461 5f61            data_a
+00010530: 7865 735f 6469 6374 5b64 6174 615d 203d  xes_dict[data] =
+00010540: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+00010550: 6578 6973 7469 6e67 5f74 6167 5f63 6f6c  existing_tag_col
+00010560: 6c65 6374 696f 6e5f 666f 725f 6461 7461  lection_for_data
+00010570: 203d 206c 6973 7428 7461 6773 2920 6966   = list(tags) if
+00010580: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
+00010590: 5f61 7865 7320 656c 7365 2074 6167 730a  _axes else tags.
+000105a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000105b0: 6178 6973 2069 6e20 7261 6e67 6528 6461  axis in range(da
+000105c0: 7461 2e62 6174 6368 5f6e 6469 6d29 3a0a  ta.batch_ndim):.
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 7461 6720 3d20 6461 7461 2e67 6574 5f64  tag = data.get_d
+000105f0: 696d 5f74 6167 2861 7869 7329 0a20 2020  im_tag(axis).   
+00010600: 2020 2020 2020 2020 2020 2020 2065 7869               exi
+00010610: 7374 696e 675f 7461 6720 3d20 636c 732e  sting_tag = cls.
+00010620: 6765 745f 6578 6973 7469 6e67 5f74 6167  get_existing_tag
+00010630: 5f66 726f 6d5f 636f 6c6c 6563 7469 6f6e  _from_collection
+00010640: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010650: 2020 2020 2020 7461 672c 2074 6167 733d        tag, tags=
+00010660: 6578 6973 7469 6e67 5f74 6167 5f63 6f6c  existing_tag_col
+00010670: 6c65 6374 696f 6e5f 666f 725f 6461 7461  lection_for_data
+00010680: 2c20 6973 5f65 7175 616c 5f6f 7074 733d  , is_equal_opts=
+00010690: 6973 5f65 7175 616c 5f6f 7074 730a 2020  is_equal_opts.  
+000106a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106c0: 6966 2065 7869 7374 696e 675f 7461 673a  if existing_tag:
+000106d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106e0: 2020 2020 2069 6620 756e 6971 7565 5f73       if unique_s
+000106f0: 6570 6172 6174 655f 6178 6573 3a0a 2020  eparate_axes:.  
+00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010710: 2020 2020 2020 6578 6973 7469 6e67 5f74        existing_t
+00010720: 6167 5f63 6f6c 6c65 6374 696f 6e5f 666f  ag_collection_fo
+00010730: 725f 6461 7461 2e72 656d 6f76 6528 6578  r_data.remove(ex
+00010740: 6973 7469 6e67 5f74 6167 2920 2023 2064  isting_tag)  # d
+00010750: 6f6e 2774 2074 616b 6520 6974 2061 6761  on't take it aga
+00010760: 696e 2066 6f72 2074 6869 7320 6461 7461  in for this data
+00010770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010780: 2020 2020 2072 6570 6c61 6365 5f65 7869       replace_exi
+00010790: 7374 696e 6720 3d20 280a 2020 2020 2020  sting = (.      
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107b0: 2020 6578 6973 7469 6e67 5f74 6167 2e75    existing_tag.u
+000107c0: 6e64 6566 696e 6564 2061 6e64 206e 6f74  ndefined and not
+000107d0: 2074 6167 2e75 6e64 6566 696e 6564 2061   tag.undefined a
+000107e0: 6e64 2074 6167 2e64 696d 656e 7369 6f6e  nd tag.dimension
+000107f0: 203d 3d20 6578 6973 7469 6e67 5f74 6167   == existing_tag
+00010800: 2e64 696d 656e 7369 6f6e 0a20 2020 2020  .dimension.     
+00010810: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010830: 2020 2020 2069 6620 7265 706c 6163 655f       if replace_
+00010840: 6578 6973 7469 6e67 3a20 2023 2052 6570  existing:  # Rep
+00010850: 6c61 6365 2074 6865 2065 7869 7374 696e  lace the existin
+00010860: 6720 6279 2074 6865 206e 6577 2074 6167  g by the new tag
+00010870: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010880: 2020 2020 2020 2020 2020 7461 6773 5b74            tags[t
+00010890: 6167 732e 696e 6465 7828 6578 6973 7469  ags.index(existi
+000108a0: 6e67 5f74 6167 295d 203d 2074 6167 0a20  ng_tag)] = tag. 
+000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108c0: 2020 2020 2020 2066 6f72 205f 2c20 6469         for _, di
+000108d0: 6d73 5f20 696e 2064 6174 615f 6178 6573  ms_ in data_axes
+000108e0: 5f64 6963 742e 6974 656d 7328 293a 0a20  _dict.items():. 
+000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010900: 2020 2020 2020 2020 2020 2064 696d 735f             dims_
+00010910: 5b3a 5d20 3d20 5b74 6167 2069 6620 6420  [:] = [tag if d 
+00010920: 3d3d 2065 7869 7374 696e 675f 7461 6720  == existing_tag 
+00010930: 656c 7365 2064 2066 6f72 2064 2069 6e20  else d for d in 
+00010940: 6469 6d73 5f5d 0a20 2020 2020 2020 2020  dims_].         
+00010950: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00010960: 7869 7374 696e 675f 7461 6720 3d20 7461  xisting_tag = ta
+00010970: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00010980: 2020 656c 7365 3a20 2023 206e 6f20 6578    else:  # no ex
+00010990: 6973 7469 6e67 2074 6167 0a20 2020 2020  isting tag.     
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000109b0: 6167 732e 6170 7065 6e64 2874 6167 290a  ags.append(tag).
+000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109d0: 6461 7461 5f61 7865 735f 6469 6374 5b64  data_axes_dict[d
+000109e0: 6174 615d 2e61 7070 656e 6428 6578 6973  ata].append(exis
+000109f0: 7469 6e67 5f74 6167 206f 7220 7461 6729  ting_tag or tag)
+00010a00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010a10: 7461 6773 2c20 6461 7461 5f61 7865 735f  tags, data_axes_
+00010a20: 6469 6374 0a0a 2020 2020 4063 6c61 7373  dict..    @class
+00010a30: 6d65 7468 6f64 0a20 2020 2064 6566 2067  method.    def g
+00010a40: 6574 5f75 6e69 715f 636f 6c6c 6563 7469  et_uniq_collecti
+00010a50: 6f6e 2863 6c73 2c20 7461 6773 2c20 6973  on(cls, tags, is
+00010a60: 5f65 7175 616c 5f6f 7074 733d 4e6f 6e65  _equal_opts=None
+00010a70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00010a80: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
+00010a90: 7374 5b44 696d 5d7c 7475 706c 655b 4469  st[Dim]|tuple[Di
+00010aa0: 6d5d 7c73 6574 5b44 696d 5d20 7461 6773  m]|set[Dim] tags
+00010ab0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00010ac0: 2064 6963 745b 7374 725d 7c4e 6f6e 6520   dict[str]|None 
+00010ad0: 6973 5f65 7175 616c 5f6f 7074 733a 2070  is_equal_opts: p
+00010ae0: 6173 7365 6420 746f 2044 696d 2e69 735f  assed to Dim.is_
+00010af0: 6571 7561 6c0a 2020 2020 2020 2020 3a72  equal.        :r
+00010b00: 7479 7065 3a20 6c69 7374 5b44 696d 5d0a  type: list[Dim].
+00010b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010b20: 2020 2020 7265 7320 3d20 5b5d 0a20 2020      res = [].   
+00010b30: 2020 2020 2066 6f72 2074 6167 2069 6e20       for tag in 
+00010b40: 7461 6773 3a0a 2020 2020 2020 2020 2020  tags:.          
+00010b50: 2020 6578 203d 2063 6c73 2e67 6574 5f65    ex = cls.get_e
+00010b60: 7869 7374 696e 675f 7461 675f 6672 6f6d  xisting_tag_from
+00010b70: 5f63 6f6c 6c65 6374 696f 6e28 7461 672c  _collection(tag,
+00010b80: 2072 6573 2c20 6973 5f65 7175 616c 5f6f   res, is_equal_o
+00010b90: 7074 733d 6973 5f65 7175 616c 5f6f 7074  pts=is_equal_opt
+00010ba0: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
+00010bb0: 6620 6e6f 7420 6578 3a0a 2020 2020 2020  f not ex:.      
+00010bc0: 2020 2020 2020 2020 2020 7265 732e 6170            res.ap
+00010bd0: 7065 6e64 2874 6167 290a 2020 2020 2020  pend(tag).      
+00010be0: 2020 7265 7475 726e 2072 6573 0a0a 2020    return res..  
+00010bf0: 2020 6465 6620 6765 745f 7369 7a65 5f74    def get_size_t
+00010c00: 656e 736f 7228 7365 6c66 2920 2d3e 205f  ensor(self) -> _
+00010c10: 742e 5465 6e73 6f72 3a0a 2020 2020 2020  t.Tensor:.      
+00010c20: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00010c30: 6574 7572 6e3a 2073 697a 6520 7465 6e73  eturn: size tens
+00010c40: 6f72 2c20 6f72 2064 796e 5f73 697a 655f  or, or dyn_size_
+00010c50: 6578 7420 6966 2064 6566 696e 6564 0a20  ext if defined. 
+00010c60: 2020 2020 2020 203a 7274 7970 653a 205f         :rtype: _
+00010c70: 742e 5465 6e73 6f72 0a20 2020 2020 2020  t.Tensor.       
+00010c80: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00010c90: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00010ca0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00010cb0: 6574 7572 6e20 7365 6c66 2e64 796e 5f73  eturn self.dyn_s
+00010cc0: 697a 655f 6578 740a 0a20 2020 2020 2020  ize_ext..       
+00010cd0: 2069 6d70 6f72 7420 7265 7475 726e 6e2e   import returnn.
+00010ce0: 6672 6f6e 7465 6e64 2061 7320 7266 0a0a  frontend as rf..
+00010cf0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00010d00: 656c 662e 7369 7a65 2069 7320 6e6f 7420  elf.size is not 
+00010d10: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+00010d20: 7572 6e20 7266 2e63 6f6e 7665 7274 5f74  urn rf.convert_t
+00010d30: 6f5f 7465 6e73 6f72 2873 656c 662e 7369  o_tensor(self.si
+00010d40: 7a65 2c20 6e61 6d65 3d22 2573 3a73 697a  ze, name="%s:siz
+00010d50: 6522 2025 2073 656c 662e 6465 7363 7269  e" % self.descri
+00010d60: 7074 696f 6e29 0a0a 2020 2020 6465 6620  ption)..    def 
+00010d70: 6765 745f 6469 6d5f 7661 6c75 6528 7365  get_dim_value(se
+00010d80: 6c66 2920 2d3e 2055 6e69 6f6e 5b69 6e74  lf) -> Union[int
+00010d90: 2c20 5f74 2e52 6177 5465 6e73 6f72 5479  , _t.RawTensorTy
+00010da0: 7065 5d3a 0a20 2020 2020 2020 2022 2222  pe]:.        """
+00010db0: 0a20 2020 2020 2020 2049 6e66 6572 7320  .        Infers 
+00010dc0: 7468 6520 6469 6d20 7468 6973 2061 7869  the dim this axi
+00010dd0: 7320 7368 6f75 6c64 2068 6176 6520 6966  s should have if
+00010de0: 2075 6e62 726f 6164 6361 7374 6564 2e0a   unbroadcasted..
+00010df0: 2020 2020 2020 2020 4966 2060 7365 6c66          If `self
+00010e00: 2e73 7263 5f64 6174 6160 2068 6173 2061  .src_data` has a
+00010e10: 2070 6c61 6365 686f 6c64 6572 2c20 7769   placeholder, wi
+00010e20: 6c6c 2075 7365 2074 6865 2073 6861 7065  ll use the shape
+00010e30: 2066 726f 6d20 7468 6572 652e 0a20 2020   from there..   
+00010e40: 2020 2020 204f 7468 6572 7769 7365 2c20       Otherwise, 
+00010e50: 7573 6573 2060 7365 6c66 2e64 696d 656e  uses `self.dimen
+00010e60: 7369 6f6e 6020 2869 6620 7374 6174 6963  sion` (if static
+00010e70: 2920 6f72 2060 7365 6c66 2e64 796e 5f73  ) or `self.dyn_s
+00010e80: 697a 6560 2028 6966 2064 796e 616d 6963  ize` (if dynamic
+00010e90: 292e 0a0a 2020 2020 2020 2020 3a72 6574  )...        :ret
+00010ea0: 7572 6e3a 206d 6178 2873 697a 6520 6f72  urn: max(size or
+00010eb0: 2064 796e 5f73 697a 6529 0a20 2020 2020   dyn_size).     
+00010ec0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00010ed0: 6573 203d 2073 656c 662e 6765 745f 6469  es = self.get_di
+00010ee0: 6d5f 7661 6c75 655f 7465 6e73 6f72 2829  m_value_tensor()
+00010ef0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00010f00: 7374 616e 6365 2872 6573 2c20 5f74 2e54  stance(res, _t.T
+00010f10: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
+00010f20: 2020 2020 6173 7365 7274 2072 6573 2e64      assert res.d
+00010f30: 696d 7320 3d3d 2028 290a 2020 2020 2020  ims == ().      
+00010f40: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00010f50: 2e72 6177 5f74 656e 736f 720a 2020 2020  .raw_tensor.    
+00010f60: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00010f70: 7461 6e63 6528 7265 732c 2069 6e74 290a  tance(res, int).
+00010f80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00010f90: 6573 0a0a 2020 2020 6465 6620 6765 745f  es..    def get_
+00010fa0: 6469 6d5f 7661 6c75 655f 7465 6e73 6f72  dim_value_tensor
+00010fb0: 2873 656c 6629 202d 3e20 556e 696f 6e5b  (self) -> Union[
+00010fc0: 696e 742c 205f 742e 5465 6e73 6f72 5d3a  int, _t.Tensor]:
+00010fd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010fe0: 2020 2020 2049 6e66 6572 7320 7468 6520       Infers the 
+00010ff0: 6469 6d20 7468 6973 2061 7869 7320 7368  dim this axis sh
+00011000: 6f75 6c64 2068 6176 6520 6966 2075 6e62  ould have if unb
+00011010: 726f 6164 6361 7374 6564 2e0a 2020 2020  roadcasted..    
+00011020: 2020 2020 4966 2060 7365 6c66 2e73 7263      If `self.src
+00011030: 5f64 6174 6160 2068 6173 2061 2070 6c61  _data` has a pla
+00011040: 6365 686f 6c64 6572 2c20 7769 6c6c 2075  ceholder, will u
+00011050: 7365 2074 6865 2073 6861 7065 2066 726f  se the shape fro
+00011060: 6d20 7468 6572 652e 0a20 2020 2020 2020  m there..       
+00011070: 204f 7468 6572 7769 7365 2c20 7573 6573   Otherwise, uses
+00011080: 2060 7365 6c66 2e64 696d 656e 7369 6f6e   `self.dimension
+00011090: 6020 2869 6620 7374 6174 6963 2920 6f72  ` (if static) or
+000110a0: 2060 7365 6c66 2e64 796e 5f73 697a 6560   `self.dyn_size`
+000110b0: 2028 6966 2064 796e 616d 6963 292e 0a0a   (if dynamic)...
+000110c0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000110d0: 206d 6178 2873 697a 6520 6f72 2064 796e   max(size or dyn
+000110e0: 5f73 697a 6529 0a20 2020 2020 2020 2022  _size).        "
+000110f0: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
+00011100: 7420 7265 7475 726e 6e2e 6672 6f6e 7465  t returnn.fronte
+00011110: 6e64 2061 7320 7266 0a0a 2020 2020 2020  nd as rf..      
+00011120: 2020 6966 2073 656c 662e 6469 6d65 6e73    if self.dimens
+00011130: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00011140: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011150: 7572 6e20 7365 6c66 2e64 696d 656e 7369  urn self.dimensi
+00011160: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
+00011170: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
+00011180: 616e 6420 7365 6c66 2e64 796e 5f73 697a  and self.dyn_siz
+00011190: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
+000111a0: 7220 6973 206e 6f74 204e 6f6e 653a 2020  r is not None:  
+000111b0: 2320 6661 7374 2070 6174 680a 2020 2020  # fast path.    
+000111c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000111d0: 6479 6e5f 7369 7a65 5f65 7874 2e62 6174  dyn_size_ext.bat
+000111e0: 6368 5f6e 6469 6d20 3e20 303a 0a20 2020  ch_ndim > 0:.   
+000111f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00011200: 7572 6e20 7266 2e72 6564 7563 655f 6d61  urn rf.reduce_ma
+00011210: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
+00011220: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
+00011230: 7369 7a65 5f65 7874 2c0a 2020 2020 2020  size_ext,.      
+00011240: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00011250: 6973 3d73 656c 662e 6479 6e5f 7369 7a65  is=self.dyn_size
+00011260: 5f65 7874 2e64 696d 5f74 6167 732c 0a20  _ext.dim_tags,. 
+00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011280: 2020 2023 204d 6173 6b69 6e67 2069 7320     # Masking is 
+00011290: 6e6f 7420 616c 7761 7973 2070 6f73 7369  not always possi
+000112a0: 626c 6520 6865 7265 2c20 652e 672e 0a20  ble here, e.g.. 
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2023 2073 656c 6620 3d20 4469 6d7b     # self = Dim{
+000112d0: 2773 656c 662d 6174 742d 6b65 7973 275b  'self-att-keys'[
+000112e0: 2774 696d 653a 7661 723a 6578 7465 726e  'time:var:extern
+000112f0: 5f64 6174 613a 636c 6173 7365 7327 5b42  _data:classes'[B
+00011300: 5d5d 7d2e 0a20 2020 2020 2020 2020 2020  ]]}..           
+00011310: 2020 2020 2020 2020 2075 7365 5f6d 6173           use_mas
+00011320: 6b3d 4661 6c73 652c 0a20 2020 2020 2020  k=False,.       
+00011330: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00011340: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011350: 6c66 2e64 796e 5f73 697a 655f 6578 740a  lf.dyn_size_ext.
+00011360: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011370: 6973 5f62 6174 6368 5f64 696d 2829 3a0a  is_batch_dim():.
+00011380: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00011390: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+000113a0: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
+000113b0: 6120 616e 6420 7365 6c66 2e5f 6578 7472  a and self._extr
+000113c0: 612e 7372 635f 6461 7461 3a0a 2020 2020  a.src_data:.    
+000113d0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+000113e0: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
+000113f0: 635f 6461 7461 2e67 6574 5f62 6174 6368  c_data.get_batch
+00011400: 5f64 696d 2829 0a20 2020 2020 2020 2020  _dim().         
+00011410: 2020 2065 6c69 6620 7365 6c66 2e62 6174     elif self.bat
+00011420: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+00011430: 2020 2020 7265 7320 3d20 7365 6c66 2e62      res = self.b
+00011440: 6174 6368 2e64 696d 0a20 2020 2020 2020  atch.dim.       
+00011450: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00011460: 6365 2872 6573 2c20 696e 7429 3a0a 2020  ce(res, int):.  
+00011470: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00011480: 7475 726e 2072 6573 0a20 2020 2020 2020  turn res.       
+00011490: 2020 2020 2069 6620 7265 7320 6973 206e       if res is n
+000114a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000114b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000114c0: 5f74 2e54 656e 736f 7228 2262 6174 6368  _t.Tensor("batch
+000114d0: 222c 2064 696d 733d 2829 2c20 6474 7970  ", dims=(), dtyp
+000114e0: 653d 7266 2e67 6574 5f64 6566 6175 6c74  e=rf.get_default
+000114f0: 5f61 7272 6179 5f69 6e64 6578 5f64 7479  _array_index_dty
+00011500: 7065 2829 2c20 7261 775f 7465 6e73 6f72  pe(), raw_tensor
+00011510: 3d72 6573 290a 2020 2020 2020 2020 6966  =res).        if
+00011520: 2028 0a20 2020 2020 2020 2020 2020 2073   (.            s
+00011530: 656c 662e 5f65 7874 7261 0a20 2020 2020  elf._extra.     
+00011540: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
+00011550: 5f65 7874 7261 2e73 7263 5f64 6174 6120  _extra.src_data 
+00011560: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00011570: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
+00011580: 2e5f 6578 7472 612e 7372 635f 6178 6973  ._extra.src_axis
+00011590: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+000115a0: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
+000115b0: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
+000115c0: 612e 706c 6163 6568 6f6c 6465 7220 6973  a.placeholder is
+000115d0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+000115e0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+000115f0: 2072 6573 203d 2073 656c 662e 5f65 7874   res = self._ext
+00011600: 7261 2e73 7263 5f64 6174 612e 6765 745f  ra.src_data.get_
+00011610: 6469 6d28 7365 6c66 2e5f 6578 7472 612e  dim(self._extra.
+00011620: 7372 635f 6178 6973 290a 2020 2020 2020  src_axis).      
+00011630: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00011640: 6e63 6528 7265 732c 2069 6e74 293a 0a20  nce(res, int):. 
+00011650: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00011660: 6574 7572 6e20 7265 730a 2020 2020 2020  eturn res.      
+00011670: 2020 2020 2020 7265 7475 726e 205f 742e        return _t.
+00011680: 5465 6e73 6f72 2822 6261 7463 6822 2c20  Tensor("batch", 
+00011690: 6469 6d73 3d28 292c 2064 7479 7065 3d72  dims=(), dtype=r
+000116a0: 662e 6765 745f 6465 6661 756c 745f 6172  f.get_default_ar
+000116b0: 7261 795f 696e 6465 785f 6474 7970 6528  ray_index_dtype(
+000116c0: 292c 2072 6177 5f74 656e 736f 723d 7265  ), raw_tensor=re
+000116d0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+000116e0: 636f 6d70 6c65 7465 5f64 796e 5f73 697a  complete_dyn_siz
+000116f0: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
+00011700: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00011710: 2061 6e64 2073 656c 662e 6479 6e5f 7369   and self.dyn_si
+00011720: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
+00011730: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+00011740: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00011750: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00011760: 2e62 6174 6368 5f6e 6469 6d20 3e20 303a  .batch_ndim > 0:
+00011770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011780: 2072 6574 7572 6e20 7266 2e72 6564 7563   return rf.reduc
+00011790: 655f 6d61 7828 7365 6c66 2e64 796e 5f73  e_max(self.dyn_s
+000117a0: 697a 655f 6578 742c 2061 7869 733d 7365  ize_ext, axis=se
+000117b0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
+000117c0: 6469 6d5f 7461 6773 290a 2020 2020 2020  dim_tags).      
+000117d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000117e0: 662e 6479 6e5f 7369 7a65 5f65 7874 0a20  f.dyn_size_ext. 
+000117f0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+00011800: 6570 7469 6f6e 2822 2573 3a20 6e65 6564  eption("%s: need
+00011810: 2070 6c61 6365 686f 6c64 6572 2c20 7365   placeholder, se
+00011820: 6c66 2e64 696d 656e 7369 6f6e 206f 7220  lf.dimension or 
+00011830: 7365 6c66 2e64 796e 5f73 697a 6520 666f  self.dyn_size fo
+00011840: 7220 6469 6d20 7661 6c75 6522 2025 2073  r dim value" % s
+00011850: 656c 6629 0a0a 2020 2020 6465 6620 6178  elf)..    def ax
+00011860: 6973 5f73 706c 6974 5f69 6e66 6f28 7365  is_split_info(se
+00011870: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00011880: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00011890: 3a20 6178 6973 2073 706c 6974 2069 6e66  : axis split inf
+000118a0: 6f2e 2073 6565 203a 6675 6e63 3a60 6765  o. see :func:`ge
+000118b0: 745f 7061 7261 6d5f 6178 6573 5f73 706c  t_param_axes_spl
+000118c0: 6974 5f69 6e66 6f60 2061 6e64 2075 7361  it_info` and usa
+000118d0: 6765 2028 652e 672e 2070 7265 7472 6169  ge (e.g. pretrai
+000118e0: 6e69 6e67 290a 2020 2020 2020 2020 3a72  ning).        :r
+000118f0: 7479 7065 3a20 6c69 7374 5b69 6e74 7c4e  type: list[int|N
+00011900: 6f6e 655d 0a20 2020 2020 2020 2022 2222  one].        """
+00011910: 0a20 2020 2020 2020 2073 616d 655f 6261  .        same_ba
+00011920: 7365 203d 2073 656c 662e 6765 745f 7361  se = self.get_sa
+00011930: 6d65 5f62 6173 6528 290a 2020 2020 2020  me_base().      
+00011940: 2020 6f70 203d 2073 656c 662e 6465 7269    op = self.deri
+00011950: 7665 645f 6672 6f6d 5f6f 7020 6f72 2073  ved_from_op or s
+00011960: 616d 655f 6261 7365 2e64 6572 6976 6564  ame_base.derived
+00011970: 5f66 726f 6d5f 6f70 0a20 2020 2020 2020  _from_op.       
+00011980: 2069 6620 6e6f 7420 6f70 3a0a 2020 2020   if not op:.    
+00011990: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+000119a0: 7365 6c66 2e64 696d 656e 7369 6f6e 5d0a  self.dimension].
+000119b0: 2020 2020 2020 2020 6966 206f 702e 6b69          if op.ki
+000119c0: 6e64 203d 3d20 2261 6464 223a 0a20 2020  nd == "add":.   
+000119d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000119e0: 7375 6d28 5b78 2e61 7869 735f 7370 6c69  sum([x.axis_spli
+000119f0: 745f 696e 666f 2829 2066 6f72 2078 2069  t_info() for x i
+00011a00: 6e20 6f70 2e69 6e70 7574 735d 2c20 5b5d  n op.inputs], []
+00011a10: 2920 2023 2066 6c61 7474 656e 0a20 2020  )  # flatten.   
+00011a20: 2020 2020 2069 6620 6f70 2e6b 696e 6420       if op.kind 
+00011a30: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
+00011a40: 2020 2020 2020 7265 7320 3d20 5b31 5d0a        res = [1].
+00011a50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011a60: 7820 696e 206f 702e 696e 7075 7473 3a0a  x in op.inputs:.
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 7265 7320 3d20 7375 6d28 5b6e 202a 2078  res = sum([n * x
+00011a90: 2e61 7869 735f 7370 6c69 745f 696e 666f  .axis_split_info
+00011aa0: 2829 2069 6620 6e20 6973 206e 6f74 204e  () if n is not N
+00011ab0: 6f6e 6520 656c 7365 204e 6f6e 6520 666f  one else None fo
+00011ac0: 7220 6e20 696e 2072 6573 5d2c 205b 5d29  r n in res], [])
+00011ad0: 2020 2320 666c 6174 7465 6e0a 2020 2020    # flatten.    
+00011ae0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00011af0: 6573 0a20 2020 2020 2020 2072 6574 7572  es.        retur
+00011b00: 6e20 5b73 656c 662e 6469 6d65 6e73 696f  n [self.dimensio
+00011b10: 6e5d 0a0a 2020 2020 6465 6620 5f67 6574  n]..    def _get
+00011b20: 5f73 616d 655f 6261 7365 5f65 7874 7261  _same_base_extra
+00011b30: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00011b40: 616c 5b5f 4469 6d45 7874 7261 5d3a 0a20  al[_DimExtra]:. 
+00011b50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00011b60: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
+00011b70: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00011b80: 6e65 0a20 2020 2020 2020 2062 6173 6520  ne.        base 
+00011b90: 3d20 7365 6c66 2e67 6574 5f73 616d 655f  = self.get_same_
+00011ba0: 6261 7365 2829 0a20 2020 2020 2020 2023  base().        #
+00011bb0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+00011bc0: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+00011bd0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00011be0: 6173 652e 5f65 7874 7261 0a0a 2020 2020  ase._extra..    
+00011bf0: 6465 6620 5f6d 616b 655f 6578 7472 6128  def _make_extra(
+00011c00: 7365 6c66 3a20 5f64 2e44 696d 2920 2d3e  self: _d.Dim) ->
+00011c10: 205f 4469 6d45 7874 7261 3a0a 2020 2020   _DimExtra:.    
+00011c20: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00011c30: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
+00011c40: 2020 2020 7365 6c66 2e5f 6578 7472 6120      self._extra 
+00011c50: 3d20 5f44 696d 4578 7472 6128 6469 6d3d  = _DimExtra(dim=
+00011c60: 7365 6c66 290a 2020 2020 2020 2020 7265  self).        re
+00011c70: 7475 726e 2073 656c 662e 5f65 7874 7261  turn self._extra
+00011c80: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00011c90: 2020 2020 6465 6620 766f 6361 6228 7365      def vocab(se
+00011ca0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00011cb0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00011cc0: 2072 6574 7572 6e6e 2e64 6174 6173 6574   returnn.dataset
+00011cd0: 732e 7574 696c 2e76 6f63 6162 756c 6172  s.util.vocabular
+00011ce0: 792e 566f 6361 6275 6c61 7279 7c4e 6f6e  y.Vocabulary|Non
+00011cf0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+00011d00: 2020 2020 2020 6578 7472 6120 3d20 7365        extra = se
+00011d10: 6c66 2e5f 6765 745f 7361 6d65 5f62 6173  lf._get_same_bas
+00011d20: 655f 6578 7472 6128 290a 2020 2020 2020  e_extra().      
+00011d30: 2020 6966 2065 7874 7261 3a0a 2020 2020    if extra:.    
+00011d40: 2020 2020 2020 2020 7265 7475 726e 2065          return e
+00011d50: 7874 7261 2e76 6f63 6162 0a20 2020 2020  xtra.vocab.     
+00011d60: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00011d70: 2020 2020 4076 6f63 6162 2e73 6574 7465      @vocab.sette
+00011d80: 720a 2020 2020 6465 6620 766f 6361 6228  r.    def vocab(
+00011d90: 7365 6c66 2c20 766f 6361 6229 3a0a 2020  self, vocab):.  
+00011da0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011db0: 2020 3a70 6172 616d 2072 6574 7572 6e6e    :param returnn
+00011dc0: 2e64 6174 6173 6574 732e 7574 696c 2e76  .datasets.util.v
+00011dd0: 6f63 6162 756c 6172 792e 566f 6361 6275  ocabulary.Vocabu
+00011de0: 6c61 7279 7c4e 6f6e 6520 766f 6361 623a  lary|None vocab:
+00011df0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011e00: 2020 2020 2069 6620 766f 6361 6220 6973       if vocab is
+00011e10: 2073 656c 662e 766f 6361 623a 0a20 2020   self.vocab:.   
+00011e20: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00011e30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011e40: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
+00011e50: 2020 2020 2073 656c 662e 6765 745f 7361       self.get_sa
+00011e60: 6d65 5f62 6173 6528 292e 766f 6361 6220  me_base().vocab 
+00011e70: 3d20 766f 6361 620a 2020 2020 2020 2020  = vocab.        
+00011e80: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00011e90: 2020 2065 7874 7261 203d 2073 656c 662e     extra = self.
+00011ea0: 5f67 6574 5f73 616d 655f 6261 7365 5f65  _get_same_base_e
+00011eb0: 7874 7261 2829 0a20 2020 2020 2020 2069  xtra().        i
+00011ec0: 6620 6578 7472 613a 0a20 2020 2020 2020  f extra:.       
+00011ed0: 2020 2020 2065 7874 7261 2e76 6f63 6162       extra.vocab
+00011ee0: 203d 2076 6f63 6162 0a0a 2020 2020 2320   = vocab..    # 
+00011ef0: 5468 6520 6b69 6e64 206f 6620 6f70 6572  The kind of oper
+00011f00: 6174 696f 6e73 2077 6520 6861 7665 3a0a  ations we have:.
+00011f10: 2020 2020 2320 6120 2b20 623a 2070 6164      # a + b: pad
+00011f20: 6469 6e67 2c20 636f 6e63 6174 0a20 2020  ding, concat.   
+00011f30: 2023 2061 202d 2062 3a20 7769 6e64 6f77   # a - b: window
+00011f40: 2077 6974 6820 7661 6c69 6420 6672 616d   with valid fram
+00011f50: 6573 206f 6e6c 790a 2020 2020 2320 6120  es only.    # a 
+00011f60: 2a20 623a 206d 6572 6765 2064 696d 732c  * b: merge dims,
+00011f70: 2075 7073 616d 706c 652c 2074 7261 6e73   upsample, trans
+00011f80: 706f 7365 6420 636f 6e76 2077 6974 6820  posed conv with 
+00011f90: 7374 7269 6469 6e67 0a20 2020 2023 2061  striding.    # a
+00011fa0: 202f 2062 2028 7768 656e 2061 2025 2062   / b (when a % b
+00011fb0: 203d 3d20 3029 3a20 7370 6c69 7420 6469   == 0): split di
+00011fc0: 6d73 2c20 646f 776e 7361 6d70 6c65 2c20  ms, downsample, 
+00011fd0: 636f 6e76 2077 6974 6820 7374 7269 6469  conv with stridi
+00011fe0: 6e67 0a20 2020 2023 2063 6569 6c64 6976  ng.    # ceildiv
+00011ff0: 2861 2c20 6229 3a20 636f 6e76 2077 6974  (a, b): conv wit
+00012000: 6820 7374 7269 6469 6e67 0a20 2020 2023  h striding.    #
+00012010: 2063 7573 746f 6d3a 2072 6570 6561 742c   custom: repeat,
+00012020: 2072 656d 6f76 652c 206d 6173 6b2c 206c   remove, mask, l
+00012030: 6f6f 7020 7769 7468 2064 796e 2065 6e64  oop with dyn end
+00012040: 0a20 2020 2023 204e 6f74 6520 7468 6174  .    # Note that
+00012050: 2077 6520 6469 6666 6572 656e 7469 6174   we differentiat
+00012060: 6520 6265 7477 6565 6e20 7468 6520 6f72  e between the or
+00012070: 6465 722c 2069 2e65 2e20 6120 2b20 6220  der, i.e. a + b 
+00012080: 213d 2062 202b 2061 2e0a 2020 2020 2320  != b + a..    # 
+00012090: 4e6f 7465 2074 6861 7420 7765 2061 6c77  Note that we alw
+000120a0: 6179 7320 6861 7665 2074 6865 2061 7373  ays have the ass
+000120b0: 756d 7074 696f 6e20 7468 6174 2061 2064  umption that a d
+000120c0: 696d 656e 7369 6f6e 2069 7320 6e6f 6e2d  imension is non-
+000120d0: 6e65 6761 7469 7665 2e0a 2020 2020 2320  negative..    # 
+000120e0: 5468 6973 2061 7373 756d 7074 696f 6e20  This assumption 
+000120f0: 6973 206e 6563 6573 7361 7279 2066 6f72  is necessary for
+00012100: 2073 6f6d 6520 7369 6d70 6c69 6669 6361   some simplifica
+00012110: 7469 6f6e 732e 0a20 2020 2023 2068 7474  tions..    # htt
+00012120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00012130: 7277 7468 2d69 362f 7265 7475 726e 6e2f  rwth-i6/returnn/
+00012140: 7075 6c6c 2f38 3533 0a0a 2020 2020 6465  pull/853..    de
+00012150: 6620 5f5f 6164 645f 5f28 7365 6c66 3a20  f __add__(self: 
+00012160: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
+00012170: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012180: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
+00012190: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+000121a0: 7265 7475 726e 3a20 7365 6c66 202b 206f  return: self + o
+000121b0: 7468 6572 2e20 6e6f 7465 2074 6861 7420  ther. note that 
+000121c0: 7468 6973 2069 7320 6e6f 7420 636f 6d6d  this is not comm
+000121d0: 7574 6174 6976 652c 2069 2e65 2e20 6469  utative, i.e. di
+000121e0: 6666 6572 656e 7420 6672 6f6d 206f 7468  fferent from oth
+000121f0: 6572 202b 2073 656c 662e 0a20 2020 2020  er + self..     
+00012200: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
+00012210: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012220: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
+00012230: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
+00012240: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
+00012250: 6572 6d2e 6578 7465 6e64 5f61 6464 5f73  erm.extend_add_s
+00012260: 7562 5f28 6f74 6865 722c 206b 696e 643d  ub_(other, kind=
+00012270: 2261 6464 222c 2072 6967 6874 3d54 7275  "add", right=Tru
+00012280: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00012290: 6e20 7465 726d 2e61 735f 6469 6d28 290a  n term.as_dim().
+000122a0: 0a20 2020 2064 6566 205f 5f72 6164 645f  .    def __radd_
+000122b0: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
+000122c0: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
+000122d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000122e0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
+000122f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00012300: 6f74 6865 7220 2b20 7365 6c66 0a20 2020  other + self.   
+00012310: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00012320: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012330: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
+00012340: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
+00012350: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
+00012360: 2074 6572 6d2e 6578 7465 6e64 5f61 6464   term.extend_add
+00012370: 5f73 7562 5f28 6f74 6865 722c 206b 696e  _sub_(other, kin
+00012380: 643d 2261 6464 222c 2072 6967 6874 3d46  d="add", right=F
+00012390: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
+000123a0: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
+000123b0: 2829 0a0a 2020 2020 6465 6620 5f5f 7375  ()..    def __su
+000123c0: 625f 5f28 7365 6c66 2c20 6f74 6865 7229  b__(self, other)
+000123d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000123e0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+000123f0: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+00012400: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+00012410: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012420: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00012430: 7375 625f 7269 6768 7428 6f74 6865 7229  sub_right(other)
+00012440: 0a0a 2020 2020 6465 6620 7375 625f 7269  ..    def sub_ri
+00012450: 6768 7428 7365 6c66 3a20 4469 6d2c 206f  ght(self: Dim, o
+00012460: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012470: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012480: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012490: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000124a0: 3a20 7365 6c66 202d 206f 7468 6572 0a20  : self - other. 
+000124b0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+000124c0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+000124d0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
+000124e0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
+000124f0: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
+00012500: 2020 2074 6572 6d2e 6578 7465 6e64 5f61     term.extend_a
+00012510: 6464 5f73 7562 5f28 6f74 6865 722c 206b  dd_sub_(other, k
+00012520: 696e 643d 2273 7562 222c 2072 6967 6874  ind="sub", right
+00012530: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00012540: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
+00012550: 6d28 290a 0a20 2020 2064 6566 2073 7562  m()..    def sub
+00012560: 5f6c 6566 7428 7365 6c66 3a20 4469 6d2c  _left(self: Dim,
+00012570: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00012580: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+00012590: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
+000125a0: 723a 0a20 2020 2020 2020 203a 7265 7475  r:.        :retu
+000125b0: 726e 3a20 282d 6f74 6865 7229 202b 2073  rn: (-other) + s
+000125c0: 656c 660a 2020 2020 2020 2020 3a72 7479  elf.        :rty
+000125d0: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
+000125e0: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
+000125f0: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
+00012600: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
+00012610: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+00012620: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
+00012630: 6572 2c20 6b69 6e64 3d22 7375 6222 2c20  er, kind="sub", 
+00012640: 7269 6768 743d 4661 6c73 6529 0a20 2020  right=False).   
+00012650: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
+00012660: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
+00012670: 6566 205f 5f6d 756c 5f5f 2873 656c 663a  ef __mul__(self:
+00012680: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
+00012690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000126a0: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
+000126b0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+000126c0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
+000126d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000126e0: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
+000126f0: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
+00012700: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
+00012710: 2e65 7874 656e 645f 6d75 6c5f 6469 765f  .extend_mul_div_
+00012720: 286f 7468 6572 2c20 6b69 6e64 3d22 6d75  (other, kind="mu
+00012730: 6c22 2c20 7269 6768 743d 5472 7565 290a  l", right=True).
+00012740: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00012750: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
+00012760: 2020 6465 6620 5f5f 726d 756c 5f5f 2873    def __rmul__(s
+00012770: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
+00012780: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012790: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+000127a0: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+000127b0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+000127c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000127d0: 2020 2020 7465 726d 203d 205f 4f70 4c69      term = _OpLi
+000127e0: 6e65 6172 5465 726d 2e66 726f 6d5f 6469  nearTerm.from_di
+000127f0: 6d28 7365 6c66 290a 2020 2020 2020 2020  m(self).        
+00012800: 7465 726d 2e65 7874 656e 645f 6d75 6c5f  term.extend_mul_
+00012810: 6469 765f 286f 7468 6572 2c20 6b69 6e64  div_(other, kind
+00012820: 3d22 6d75 6c22 2c20 7269 6768 743d 4661  ="mul", right=Fa
+00012830: 6c73 6529 0a20 2020 2020 2020 2072 6574  lse).        ret
+00012840: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
+00012850: 290a 0a20 2020 2064 6566 205f 5f66 6c6f  )..    def __flo
+00012860: 6f72 6469 765f 5f28 7365 6c66 3a20 4469  ordiv__(self: Di
+00012870: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
+00012880: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00012890: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+000128a0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+000128b0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+000128c0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+000128d0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+000128e0: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+000128f0: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+00012900: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
+00012910: 6865 722c 206b 696e 643d 2266 6c6f 6f72  her, kind="floor
+00012920: 6469 7622 2c20 7269 6768 743d 5472 7565  div", right=True
+00012930: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012940: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
+00012950: 2020 2020 6465 6620 5f5f 7472 7565 6469      def __truedi
+00012960: 765f 5f28 7365 6c66 2c20 6f74 6865 7229  v__(self, other)
+00012970: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012980: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00012990: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+000129a0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+000129b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000129c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000129d0: 6469 765f 7269 6768 7428 6f74 6865 7229  div_right(other)
+000129e0: 0a0a 2020 2020 6465 6620 6469 765f 6c65  ..    def div_le
+000129f0: 6674 2873 656c 663a 2044 696d 2c20 6f74  ft(self: Dim, ot
+00012a00: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
+00012a10: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00012a20: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
+00012a30: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00012a40: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
+00012a50: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
+00012a60: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+00012a70: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
+00012a80: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
+00012a90: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
+00012aa0: 6b69 6e64 3d22 7472 7565 6469 7622 2c20  kind="truediv", 
+00012ab0: 7269 6768 743d 4661 6c73 6529 0a20 2020  right=False).   
+00012ac0: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
+00012ad0: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
+00012ae0: 6566 2064 6976 5f72 6967 6874 2873 656c  ef div_right(sel
+00012af0: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
+00012b00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012b10: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
+00012b20: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
+00012b30: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+00012b40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012b50: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
+00012b60: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
+00012b70: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
+00012b80: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
+00012b90: 765f 286f 7468 6572 2c20 6b69 6e64 3d22  v_(other, kind="
+00012ba0: 7472 7565 6469 7622 2c20 7269 6768 743d  truediv", right=
+00012bb0: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
+00012bc0: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
+00012bd0: 2829 0a0a 2020 2020 6465 6620 6365 696c  ()..    def ceil
+00012be0: 6469 765f 6c65 6674 2873 656c 663a 2044  div_left(self: D
+00012bf0: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
+00012c00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012c10: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
+00012c20: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+00012c30: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00012c40: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
+00012c50: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
+00012c60: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
+00012c70: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
+00012c80: 7874 656e 645f 6d75 6c5f 6469 765f 286f  xtend_mul_div_(o
+00012c90: 7468 6572 2c20 6b69 6e64 3d22 6365 696c  ther, kind="ceil
+00012ca0: 6469 7622 2c20 7269 6768 743d 4661 6c73  div", right=Fals
+00012cb0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00012cc0: 6e20 7465 726d 2e61 735f 6469 6d28 290a  n term.as_dim().
+00012cd0: 0a20 2020 2064 6566 2063 6569 6c64 6976  .    def ceildiv
+00012ce0: 5f72 6967 6874 2873 656c 663a 2044 696d  _right(self: Dim
+00012cf0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00012d00: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00012d10: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
+00012d20: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
+00012d30: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
+00012d40: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
+00012d50: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
+00012d60: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
+00012d70: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+00012d80: 656e 645f 6d75 6c5f 6469 765f 286f 7468  end_mul_div_(oth
+00012d90: 6572 2c20 6b69 6e64 3d22 6365 696c 6469  er, kind="ceildi
+00012da0: 7622 2c20 7269 6768 743d 5472 7565 290a  v", right=True).
+00012db0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00012dc0: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
+00012dd0: 2020 6465 6620 5f5f 6e65 675f 5f28 7365    def __neg__(se
+00012de0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00012df0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00012e00: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00012e10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012e20: 2d31 202a 2073 656c 660a 0a20 2020 2064  -1 * self..    d
+00012e30: 6566 2069 735f 636f 6e73 7461 6e74 5f73  ef is_constant_s
+00012e40: 7461 7469 635f 6469 6d28 7365 6c66 2920  tatic_dim(self) 
+00012e50: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00012e60: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
+00012e70: 7475 726e 3a20 6465 7269 7665 6420 6f70  turn: derived op
+00012e80: 206f 6620 7479 7065 2063 6f6e 7374 616e   of type constan
+00012e90: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00012ea0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00012eb0: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
+00012ec0: 7020 616e 6420 7365 6c66 2e64 6572 6976  p and self.deriv
+00012ed0: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
+00012ee0: 3d3d 2022 636f 6e73 7461 6e74 220a 0a0a  == "constant"...
+00012ef0: 6465 6620 5f6d 616b 655f 636f 6e73 7461  def _make_consta
+00012f00: 6e74 5f73 7461 7469 635f 6469 6d28 7661  nt_static_dim(va
+00012f10: 6c75 652c 206b 696e 643d 4e6f 6e65 293a  lue, kind=None):
+00012f20: 0a20 2020 2022 2222 0a20 2020 203a 7061  .    """.    :pa
+00012f30: 7261 6d20 696e 7420 7661 6c75 653a 0a20  ram int value:. 
+00012f40: 2020 203a 7061 7261 6d20 456e 7469 7479     :param Entity
+00012f50: 7c4e 6f6e 6520 6b69 6e64 3a0a 2020 2020  |None kind:.    
+00012f60: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
+00012f70: 2222 220a 2020 2020 7265 7475 726e 205f  """.    return _
+00012f80: 642e 4469 6d28 0a20 2020 2020 2020 2064  d.Dim(.        d
+00012f90: 696d 656e 7369 6f6e 3d76 616c 7565 2c0a  imension=value,.
+00012fa0: 2020 2020 2020 2020 6b69 6e64 3d6b 696e          kind=kin
+00012fb0: 6420 6f72 2044 696d 5479 7065 732e 556e  d or DimTypes.Un
+00012fc0: 7370 6563 6966 6965 642c 0a20 2020 2020  specified,.     
+00012fd0: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00012fe0: 756e 6e61 6d65 645f 2573 6469 6d5f 2569  unnamed_%sdim_%i
+00012ff0: 2220 2520 286b 696e 642e 6e61 6d65 202b  " % (kind.name +
+00013000: 2022 5f22 2069 6620 6b69 6e64 2065 6c73   "_" if kind els
+00013010: 6520 2222 2c20 7661 6c75 6529 2c0a 2020  e "", value),.  
+00013020: 2020 2020 2020 6465 7269 7665 645f 6672        derived_fr
+00013030: 6f6d 5f6f 703d 4f70 286b 696e 643d 2263  om_op=Op(kind="c
+00013040: 6f6e 7374 616e 7422 2c20 696e 7075 7473  onstant", inputs
+00013050: 3d5b 5d2c 2061 7474 7269 6273 3d7b 2276  =[], attribs={"v
+00013060: 616c 7565 223a 2076 616c 7565 7d29 2c0a  alue": value}),.
+00013070: 2020 2020 2020 2020 6175 746f 5f67 656e          auto_gen
+00013080: 6572 6174 6564 3d54 7275 652c 0a20 2020  erated=True,.   
+00013090: 2029 0a0a 0a63 6c61 7373 204f 703a 0a20   )...class Op:. 
+000130a0: 2020 2022 2222 0a20 2020 204f 7020 6f6e     """.    Op on
+000130b0: 203a 636c 6173 733a 6044 696d 6020 7768   :class:`Dim` wh
+000130c0: 6963 6820 7265 7375 6c74 7320 696e 2061  ich results in a
+000130d0: 2064 6572 6976 6564 203a 636c 6173 733a   derived :class:
+000130e0: 6044 696d 602e 0a20 2020 2022 2222 0a0a  `Dim`..    """..
+000130f0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00013100: 2873 656c 662c 206b 696e 642c 2069 6e70  (self, kind, inp
+00013110: 7574 732c 2061 7474 7269 6273 3d4e 6f6e  uts, attribs=Non
+00013120: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00013130: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+00013140: 7472 206b 696e 643a 2022 6164 6422 2c20  tr kind: "add", 
+00013150: 2273 7562 222c 2022 6d75 6c22 2c20 2263  "sub", "mul", "c
+00013160: 6569 6c64 6976 220a 2020 2020 2020 2020  eildiv".        
+00013170: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
+00013180: 2069 6e70 7574 733a 0a20 2020 2020 2020   inputs:.       
+00013190: 203a 7061 7261 6d20 6469 6374 5b73 7472   :param dict[str
+000131a0: 5d7c 4e6f 6e65 2061 7474 7269 6273 3a0a  ]|None attribs:.
+000131b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000131c0: 2020 2020 7365 6c66 2e6b 696e 6420 3d20      self.kind = 
+000131d0: 6b69 6e64 0a20 2020 2020 2020 2073 656c  kind.        sel
+000131e0: 662e 696e 7075 7473 203d 2069 6e70 7574  f.inputs = input
+000131f0: 730a 2020 2020 2020 2020 7365 6c66 2e6f  s.        self.o
+00013200: 7574 7075 7420 3d20 4e6f 6e65 2020 2320  utput = None  # 
+00013210: 7479 7065 3a20 4f70 7469 6f6e 616c 5b5f  type: Optional[_
+00013220: 642e 4469 6d5d 0a20 2020 2020 2020 2073  d.Dim].        s
+00013230: 656c 662e 6174 7472 6962 7320 3d20 6174  elf.attribs = at
+00013240: 7472 6962 730a 0a20 2020 2064 6566 205f  tribs..    def _
+00013250: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
+00013260: 2020 2020 2020 2061 7474 7269 6273 203d         attribs =
+00013270: 2028 2220 2572 2220 2520 7365 6c66 2e61   (" %r" % self.a
+00013280: 7474 7269 6273 2920 6966 2073 656c 662e  ttribs) if self.
+00013290: 6174 7472 6962 7320 656c 7365 2022 220a  attribs else "".
+000132a0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+000132b0: 3c44 696d 2e4f 7020 2572 2025 7325 733e  <Dim.Op %r %s%s>
+000132c0: 2220 2520 2873 656c 662e 6b69 6e64 2c20  " % (self.kind, 
+000132d0: 7365 6c66 2e69 6e70 7574 732c 2061 7474  self.inputs, att
+000132e0: 7269 6273 290a 0a20 2020 2064 6566 205f  ribs)..    def _
+000132f0: 7661 6c75 6528 7365 6c66 293a 0a20 2020  value(self):.   
+00013300: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00013310: 2e6b 696e 642c 2074 7570 6c65 2873 656c  .kind, tuple(sel
+00013320: 662e 696e 7075 7473 292c 2066 726f 7a65  f.inputs), froze
+00013330: 6e73 6574 2873 656c 662e 6174 7472 6962  nset(self.attrib
+00013340: 732e 6974 656d 7328 2929 2069 6620 7365  s.items()) if se
+00013350: 6c66 2e61 7474 7269 6273 2065 6c73 6520  lf.attribs else 
+00013360: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f5f  None..    def __
+00013370: 6861 7368 5f5f 2873 656c 6629 3a0a 2020  hash__(self):.  
+00013380: 2020 2020 2020 7265 7475 726e 2068 6173        return has
+00013390: 6828 7365 6c66 2e5f 7661 6c75 6528 2929  h(self._value())
+000133a0: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
+000133b0: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+000133c0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+000133d0: 616e 6365 286f 7468 6572 2c20 4f70 293a  ance(other, Op):
+000133e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000133f0: 7572 6e20 7365 6c66 2e5f 7661 6c75 6528  urn self._value(
+00013400: 2920 3d3d 206f 7468 6572 2e5f 7661 6c75  ) == other._valu
+00013410: 6528 290a 2020 2020 2020 2020 7265 7475  e().        retu
+00013420: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
+00013430: 6620 5f5f 6e65 5f5f 2873 656c 662c 206f  f __ne__(self, o
+00013440: 7468 6572 293a 0a20 2020 2020 2020 2072  ther):.        r
+00013450: 6574 7572 6e20 6e6f 7420 7365 6c66 2e5f  eturn not self._
+00013460: 5f65 715f 5f28 6f74 6865 7229 0a0a 0a64  _eq__(other)...d
+00013470: 6566 205f 6765 745f 6465 7363 7269 7074  ef _get_descript
+00013480: 696f 6e28 6469 6d2c 2062 7261 636b 6574  ion(dim, bracket
+00013490: 733d 5472 7565 293a 0a20 2020 2022 2222  s=True):.    """
+000134a0: 0a20 2020 203a 7061 7261 6d20 4469 6d20  .    :param Dim 
+000134b0: 6469 6d3a 0a20 2020 203a 7061 7261 6d20  dim:.    :param 
+000134c0: 626f 6f6c 2062 7261 636b 6574 733a 2061  bool brackets: a
+000134d0: 6464 2062 7261 636b 6574 7320 7768 656e  dd brackets when
+000134e0: 206e 6563 6573 7361 7279 0a20 2020 203a   necessary.    :
+000134f0: 7274 7970 653a 2073 7472 0a20 2020 2022  rtype: str.    "
+00013500: 2222 0a20 2020 2069 6620 6469 6d2e 6465  "".    if dim.de
+00013510: 7363 7269 7074 696f 6e20 616e 6420 6469  scription and di
+00013520: 6d2e 6465 7363 7269 7074 696f 6e2e 7374  m.description.st
+00013530: 6172 7473 7769 7468 2822 756e 6e61 6d65  artswith("unname
+00013540: 645f 2229 2061 6e64 2064 696d 2e64 696d  d_") and dim.dim
+00013550: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
+00013560: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
+00013570: 726e 2073 7472 2864 696d 2e64 696d 656e  rn str(dim.dimen
+00013580: 7369 6f6e 290a 2020 2020 6966 2064 696d  sion).    if dim
+00013590: 2e64 6573 6372 6970 7469 6f6e 3a0a 2020  .description:.  
+000135a0: 2020 2020 2020 6966 2062 7261 636b 6574        if bracket
+000135b0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+000135c0: 6d70 6f72 7420 7265 0a0a 2020 2020 2020  mport re..      
+000135d0: 2020 2020 2020 6966 2072 652e 7365 6172        if re.sear
+000135e0: 6368 2822 5b2b 5c5c 2d2f 205d 222c 2064  ch("[+\\-/ ]", d
+000135f0: 696d 2e64 6573 6372 6970 7469 6f6e 293a  im.description):
+00013600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013610: 2072 6574 7572 6e20 2228 2573 2922 2025   return "(%s)" %
+00013620: 2064 696d 2e64 6573 6372 6970 7469 6f6e   dim.description
+00013630: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013640: 6469 6d2e 6465 7363 7269 7074 696f 6e0a  dim.description.
+00013650: 2020 2020 7265 7475 726e 2022 756e 6e61      return "unna
+00013660: 6d65 645f 2573 5f64 696d 2573 2220 2520  med_%s_dim%s" % 
+00013670: 2864 696d 2e6b 696e 642c 2064 696d 2e64  (dim.kind, dim.d
+00013680: 696d 656e 7369 6f6e 2069 6620 6469 6d2e  imension if dim.
+00013690: 6469 6d65 6e73 696f 6e20 6973 206e 6f74  dimension is not
+000136a0: 204e 6f6e 6520 656c 7365 2022 3f22 290a   None else "?").
+000136b0: 0a0a 636c 6173 7320 5f4f 704d 756c 7454  ..class _OpMultT
+000136c0: 6572 6d3a 0a20 2020 2022 2222 0a20 2020  erm:.    """.   
+000136d0: 2072 6570 7265 7365 6e74 7320 7374 6820   represents sth 
+000136e0: 6c69 6b65 2061 202a 2062 202a 2063 0a20  like a * b * c. 
+000136f0: 2020 2022 2222 0a0a 2020 2020 4063 6c61     """..    @cla
+00013700: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00013710: 2066 726f 6d5f 6469 6d28 636c 732c 2064   from_dim(cls, d
+00013720: 696d 3a20 5f64 2e44 696d 2920 2d3e 205f  im: _d.Dim) -> _
+00013730: 4f70 4d75 6c74 5465 726d 3a0a 2020 2020  OpMultTerm:.    
+00013740: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013750: 3a70 6172 616d 2064 696d 3a0a 2020 2020  :param dim:.    
+00013760: 2020 2020 3a72 6574 7572 6e3a 206f 7020      :return: op 
+00013770: 6d75 6c74 2074 6572 6d0a 2020 2020 2020  mult term.      
+00013780: 2020 2222 220a 2020 2020 2020 2020 6469    """.        di
+00013790: 6d20 3d20 6469 6d2e 6765 745f 7361 6d65  m = dim.get_same
+000137a0: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
+000137b0: 6966 2064 696d 2e64 696d 656e 7369 6f6e  if dim.dimension
+000137c0: 203d 3d20 3120 616e 6420 6469 6d2e 6973   == 1 and dim.is
+000137d0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+000137e0: 5f64 696d 2829 3a0a 2020 2020 2020 2020  _dim():.        
+000137f0: 2020 2020 7265 7475 726e 2063 6c73 2e6f      return cls.o
+00013800: 6e65 2829 0a20 2020 2020 2020 2069 6620  ne().        if 
+00013810: 6469 6d2e 6465 7269 7665 645f 6672 6f6d  dim.derived_from
+00013820: 5f6f 7020 616e 6420 6469 6d2e 6465 7269  _op and dim.deri
+00013830: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00013840: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+00013850: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
+00013860: 7328 6c69 7374 2864 696d 2e64 6572 6976  s(list(dim.deriv
+00013870: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00013880: 7329 290a 2020 2020 2020 2020 7265 7475  s)).        retu
+00013890: 726e 2063 6c73 285b 6469 6d5d 290a 0a20  rn cls([dim]).. 
+000138a0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000138b0: 2020 2020 6465 6620 6672 6f6d 5f64 696d      def from_dim
+000138c0: 5f66 6163 746f 7273 2863 6c73 2c20 6469  _factors(cls, di
+000138d0: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+000138e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000138f0: 6c69 7374 5b44 696d 5d20 6469 6d73 3a0a  list[Dim] dims:.
+00013900: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00013910: 4469 6d2e 5f4f 704d 756c 7454 6572 6d0a  Dim._OpMultTerm.
+00013920: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013930: 2020 2020 7265 7320 3d20 636c 732e 6f6e      res = cls.on
+00013940: 6528 290a 2020 2020 2020 2020 666f 7220  e().        for 
+00013950: 6420 696e 2064 696d 733a 0a20 2020 2020  d in dims:.     
+00013960: 2020 2020 2020 2072 6573 2e65 7874 656e         res.exten
+00013970: 645f 6d75 6c5f 6469 765f 2864 2c20 6b69  d_mul_div_(d, ki
+00013980: 6e64 3d22 6d75 6c22 2c20 7269 6768 743d  nd="mul", right=
+00013990: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
+000139a0: 7475 726e 2072 6573 0a0a 2020 2020 4063  turn res..    @c
+000139b0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+000139c0: 6566 206f 6e65 2863 6c73 293a 0a20 2020  ef one(cls):.   
+000139d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000139e0: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
+000139f0: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
+00013a00: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00013a10: 7572 6e20 636c 7328 5b5d 290a 0a20 2020  urn cls([])..   
+00013a20: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00013a30: 6c66 2c20 7465 726d 7329 3a0a 2020 2020  lf, terms):.    
+00013a40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013a50: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
+00013a60: 2074 6572 6d73 3a0a 2020 2020 2020 2020   terms:.        
+00013a70: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+00013a80: 2e74 6572 6d73 203d 2074 6572 6d73 0a0a  .terms = terms..
+00013a90: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
+00013aa0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00013ab0: 7265 7475 726e 2068 6173 6828 7475 706c  return hash(tupl
+00013ac0: 6528 7365 6c66 2e74 6572 6d73 2929 0a0a  e(self.terms))..
+00013ad0: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
+00013ae0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+00013af0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013b00: 203a 7061 7261 6d20 4469 6d7c 4469 6d2e   :param Dim|Dim.
+00013b10: 5f4f 704d 756c 7454 6572 6d20 6f74 6865  _OpMultTerm othe
+00013b20: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+00013b30: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00013b40: 616e 6365 286f 7468 6572 2c20 5f4f 704d  ance(other, _OpM
+00013b50: 756c 7454 6572 6d29 3a0a 2020 2020 2020  ultTerm):.      
+00013b60: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00013b70: 662e 7465 726d 7320 3d3d 206f 7468 6572  f.terms == other
+00013b80: 2e74 6572 6d73 0a20 2020 2020 2020 2072  .terms.        r
+00013b90: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00013ba0: 2064 6566 205f 5f6e 655f 5f28 7365 6c66   def __ne__(self
+00013bb0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00013bc0: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
+00013bd0: 662e 5f5f 6571 5f5f 286f 7468 6572 290a  f.__eq__(other).
+00013be0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+00013bf0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00013c00: 2072 6574 7572 6e20 2244 696d 2e5f 4f70   return "Dim._Op
+00013c10: 4d75 6c74 5465 726d 2825 7229 2220 2520  MultTerm(%r)" % 
+00013c20: 2873 656c 662e 7465 726d 732c 290a 0a20  (self.terms,).. 
+00013c30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00013c40: 2064 6566 2064 696d 656e 7369 6f6e 2873   def dimension(s
+00013c50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00013c60: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+00013c70: 3a20 696e 747c 4e6f 6e65 0a20 2020 2020  : int|None.     
+00013c80: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+00013c90: 696d 203d 2031 0a20 2020 2020 2020 2066  im = 1.        f
+00013ca0: 6f72 2070 6172 7420 696e 2073 656c 662e  or part in self.
+00013cb0: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00013cc0: 2020 2069 6620 7061 7274 2e64 696d 656e     if part.dimen
+00013cd0: 7369 6f6e 2069 7320 4e6f 6e65 3a0a 2020  sion is None:.  
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00013cf0: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+00013d00: 2020 2020 2020 6469 6d20 2a3d 2070 6172        dim *= par
+00013d10: 742e 6469 6d65 6e73 696f 6e0a 2020 2020  t.dimension.    
+00013d20: 2020 2020 7265 7475 726e 2064 696d 0a0a      return dim..
+00013d30: 2020 2020 6465 6620 6261 7365 5f74 6572      def base_ter
+00013d40: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
+00013d50: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00013d60: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00013d70: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
+00013d80: 6572 7420 7365 6c66 2e74 6572 6d73 0a20  ert self.terms. 
+00013d90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00013da0: 6c66 2e74 6572 6d73 5b2d 315d 0a0a 2020  lf.terms[-1]..  
+00013db0: 2020 6465 6620 6973 5f6f 6e65 2873 656c    def is_one(sel
+00013dc0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00013dd0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00013de0: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
+00013df0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013e00: 6e6f 7420 7365 6c66 2e74 6572 6d73 0a0a  not self.terms..
+00013e10: 2020 2020 6465 6620 6973 5f63 6f6e 7374      def is_const
+00013e20: 616e 745f 7374 6174 6963 5f64 696d 2873  ant_static_dim(s
+00013e30: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00013e40: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+00013e50: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+00013e60: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00013e70: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
+00013e80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00013e90: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+00013ea0: 7475 726e 2061 6c6c 2874 6572 6d2e 6973  turn all(term.is
+00013eb0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+00013ec0: 5f64 696d 2829 2066 6f72 2074 6572 6d20  _dim() for term 
+00013ed0: 696e 2073 656c 662e 7465 726d 7329 0a0a  in self.terms)..
+00013ee0: 2020 2020 6465 6620 636f 7079 2873 656c      def copy(sel
+00013ef0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00013f00: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00013f10: 4469 6d2e 5f4f 704d 756c 7454 6572 6d0a  Dim._OpMultTerm.
+00013f20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013f30: 2020 2020 7265 7475 726e 205f 4f70 4d75      return _OpMu
+00013f40: 6c74 5465 726d 286c 6973 7428 7365 6c66  ltTerm(list(self
+00013f50: 2e74 6572 6d73 2929 0a0a 2020 2020 6465  .terms))..    de
+00013f60: 6620 6e65 6761 7469 7665 2873 656c 6629  f negative(self)
+00013f70: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013f80: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+00013f90: 6d2e 5f4f 704d 756c 7454 6572 6d0a 2020  m._OpMultTerm.  
+00013fa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013fb0: 2020 6966 2073 656c 662e 7465 726d 7320    if self.terms 
+00013fc0: 616e 6420 7365 6c66 2e74 6572 6d73 5b30  and self.terms[0
+00013fd0: 5d2e 6973 5f63 6f6e 7374 616e 745f 7374  ].is_constant_st
+00013fe0: 6174 6963 5f64 696d 2829 2061 6e64 2073  atic_dim() and s
+00013ff0: 656c 662e 7465 726d 735b 305d 2e64 696d  elf.terms[0].dim
+00014000: 656e 7369 6f6e 203d 3d20 2d31 3a0a 2020  ension == -1:.  
+00014010: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014020: 205f 4f70 4d75 6c74 5465 726d 2873 656c   _OpMultTerm(sel
+00014030: 662e 7465 726d 735b 313a 5d29 0a20 2020  f.terms[1:]).   
+00014040: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00014050: 636f 7079 2829 0a20 2020 2020 2020 2072  copy().        r
+00014060: 6573 2e65 7874 656e 645f 6d75 6c5f 6469  es.extend_mul_di
+00014070: 765f 285f 6d61 6b65 5f63 6f6e 7374 616e  v_(_make_constan
+00014080: 745f 7374 6174 6963 5f64 696d 282d 3129  t_static_dim(-1)
+00014090: 2c20 6b69 6e64 3d22 6d75 6c22 2c20 7269  , kind="mul", ri
+000140a0: 6768 743d 4661 6c73 6529 0a20 2020 2020  ght=False).     
+000140b0: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
+000140c0: 2020 2064 6566 2064 6976 6973 6962 6c65     def divisible
+000140d0: 2873 656c 662c 206f 7468 6572 2c20 7269  (self, other, ri
+000140e0: 6768 7429 3a0a 2020 2020 2020 2020 2222  ght):.        ""
+000140f0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00014100: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
+00014110: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00014120: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
+00014130: 7265 7475 726e 3a20 7768 6574 6865 7220  return: whether 
+00014140: 7765 2063 616e 2064 6976 6964 6520 6f74  we can divide ot
+00014150: 6865 722c 2077 6974 686f 7574 2072 656d  her, without rem
+00014160: 6169 6e64 6572 0a20 2020 2020 2020 203a  ainder.        :
+00014170: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+00014180: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014190: 6966 206e 6f74 2073 656c 662e 7465 726d  if not self.term
+000141a0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+000141b0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+000141c0: 2020 2020 6966 206f 7468 6572 2e64 6572      if other.der
+000141d0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
+000141e0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+000141f0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
+00014200: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
+00014210: 2020 746d 7020 3d20 7365 6c66 2e63 6f70    tmp = self.cop
+00014220: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+00014230: 666f 7220 7465 726d 2069 6e20 6f74 6865  for term in othe
+00014240: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00014250: 702e 696e 7075 7473 2069 6620 7269 6768  p.inputs if righ
+00014260: 7420 656c 7365 2072 6576 6572 7365 6428  t else reversed(
+00014270: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00014280: 6f6d 5f6f 702e 696e 7075 7473 293a 0a20  om_op.inputs):. 
+00014290: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000142a0: 6620 6e6f 7420 746d 702e 6469 7669 7369  f not tmp.divisi
+000142b0: 626c 6528 7465 726d 2c20 7269 6768 743d  ble(term, right=
+000142c0: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
+000142d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000142e0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+000142f0: 2020 2020 2020 2020 2074 6d70 2e65 7874           tmp.ext
+00014300: 656e 645f 6d75 6c5f 6469 765f 2874 6572  end_mul_div_(ter
+00014310: 6d2c 206b 696e 643d 2274 7275 6564 6976  m, kind="truediv
+00014320: 222c 2072 6967 6874 3d72 6967 6874 290a  ", right=right).
+00014330: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014340: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+00014350: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+00014360: 203d 2073 656c 662e 7465 726d 735b 2d31   = self.terms[-1
+00014370: 2069 6620 7269 6768 7420 656c 7365 2030   if right else 0
+00014380: 5d0a 2020 2020 2020 2020 6966 206f 7468  ].        if oth
+00014390: 6572 203d 3d20 6d6f 7374 5f72 6563 656e  er == most_recen
+000143a0: 745f 7465 726d 3a0a 2020 2020 2020 2020  t_term:.        
+000143b0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000143c0: 2020 2020 2020 2020 6966 206d 6f73 745f          if most_
+000143d0: 7265 6365 6e74 5f74 6572 6d2e 6469 6d65  recent_term.dime
+000143e0: 6e73 696f 6e20 6973 206e 6f74 204e 6f6e  nsion is not Non
+000143f0: 6520 616e 6420 6f74 6865 722e 6469 6d65  e and other.dime
+00014400: 6e73 696f 6e20 6973 206e 6f74 204e 6f6e  nsion is not Non
+00014410: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00014420: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
+00014430: 726d 2e64 696d 656e 7369 6f6e 2025 206f  rm.dimension % o
+00014440: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
+00014450: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00014460: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00014470: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014480: 4661 6c73 650a 0a20 2020 2064 6566 2063  False..    def c
+00014490: 616e 5f73 696d 706c 6966 7928 7365 6c66  an_simplify(self
+000144a0: 2c20 6f74 6865 722c 206b 696e 642c 2072  , other, kind, r
+000144b0: 6967 6874 293a 0a20 2020 2020 2020 2022  ight):.        "
+000144c0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+000144d0: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
+000144e0: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+000144f0: 6b69 6e64 3a0a 2020 2020 2020 2020 3a70  kind:.        :p
+00014500: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
+00014510: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00014520: 3a20 7768 6574 6865 7220 7765 2063 616e  : whether we can
+00014530: 2073 696d 706c 6966 7920 7768 656e 2061   simplify when a
+00014540: 7070 6c79 696e 6720 7468 6973 206f 7065  pplying this ope
+00014550: 7261 7469 6f6e 0a20 2020 2020 2020 203a  ration.        :
+00014560: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+00014570: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014580: 6966 206f 7468 6572 2e64 6572 6976 6564  if other.derived
+00014590: 5f66 726f 6d5f 6f70 2061 6e64 206f 7468  _from_op and oth
+000145a0: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+000145b0: 6f70 2e6b 696e 6420 3d3d 2022 6d75 6c22  op.kind == "mul"
+000145c0: 3a0a 2020 2020 2020 2020 2020 2020 746d  :.            tm
+000145d0: 7020 3d20 7365 6c66 2e63 6f70 7928 290a  p = self.copy().
+000145e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000145f0: 7465 726d 2069 6e20 6f74 6865 722e 6465  term in other.de
+00014600: 7269 7665 645f 6672 6f6d 5f6f 702e 696e  rived_from_op.in
+00014610: 7075 7473 2069 6620 7269 6768 7420 656c  puts if right el
+00014620: 7365 2072 6576 6572 7365 6428 6f74 6865  se reversed(othe
+00014630: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00014640: 702e 696e 7075 7473 293a 0a20 2020 2020  p.inputs):.     
+00014650: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00014660: 7420 746d 702e 6361 6e5f 7369 6d70 6c69  t tmp.can_simpli
+00014670: 6679 2874 6572 6d2c 206b 696e 643d 6b69  fy(term, kind=ki
+00014680: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
+00014690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000146a0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000146b0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+000146c0: 2020 2074 6d70 2e65 7874 656e 645f 6d75     tmp.extend_mu
+000146d0: 6c5f 6469 765f 2874 6572 6d2c 206b 696e  l_div_(term, kin
+000146e0: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+000146f0: 6768 7429 0a20 2020 2020 2020 2020 2020  ght).           
+00014700: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00014710: 2020 2020 2069 6478 203d 2073 656c 662e       idx = self.
+00014720: 5f73 696d 706c 6966 795f 7465 726d 5f69  _simplify_term_i
+00014730: 6478 286f 7468 6572 2c20 6b69 6e64 3d6b  dx(other, kind=k
+00014740: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00014750: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00014760: 2069 6478 2069 7320 6e6f 7420 4e6f 6e65   idx is not None
+00014770: 0a0a 2020 2020 6465 6620 5f73 696d 706c  ..    def _simpl
+00014780: 6966 795f 7465 726d 5f69 6478 2873 656c  ify_term_idx(sel
+00014790: 662c 206f 7468 6572 2c20 6b69 6e64 2c20  f, other, kind, 
+000147a0: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
+000147b0: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+000147c0: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
+000147d0: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+000147e0: 206b 696e 643a 0a20 2020 2020 2020 203a   kind:.        :
+000147f0: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
+00014800: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
+00014810: 6e3a 2069 6e64 6578 206f 6620 7465 726d  n: index of term
+00014820: 2074 6f20 7369 6d70 6c69 6679 0a20 2020   to simplify.   
+00014830: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
+00014840: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
+00014850: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+00014860: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00014870: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00014880: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00014890: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
+000148a0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+000148b0: 7761 6e74 2028 6220 2a20 6129 202f 2f20  want (b * a) // 
+000148c0: 6220 213d 2061 2e0a 2020 2020 2020 2020  b != a..        
+000148d0: 2020 2020 2320 486f 7765 7665 722c 2077      # However, w
+000148e0: 6520 7761 6e74 2068 202a 2028 3220 2a20  e want h * (2 * 
+000148f0: 6120 2f2f 2068 2920 3d3d 2032 202a 2061  a // h) == 2 * a
+00014900: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00014910: 536f 2c20 666f 7220 606d 756c 602c 2061  So, for `mul`, a
+00014920: 6e64 206f 6e6c 7920 666f 7220 606d 756c  nd only for `mul
+00014930: 602c 2063 6865 636b 2061 6c6c 2074 6572  `, check all ter
+00014940: 6d73 2c20 7768 6574 6865 7220 7765 2063  ms, whether we c
+00014950: 616e 2073 696d 706c 6966 7920 736f 6d65  an simplify some
+00014960: 2064 6976 6973 696f 6e2d 7465 726d 2e0a   division-term..
+00014970: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00014980: 692c 2074 6572 6d20 696e 2072 6576 6572  i, term in rever
+00014990: 7365 6428 6c69 7374 2865 6e75 6d65 7261  sed(list(enumera
+000149a0: 7465 2873 656c 662e 7465 726d 7329 2929  te(self.terms)))
+000149b0: 2069 6620 7269 6768 7420 656c 7365 2065   if right else e
+000149c0: 6e75 6d65 7261 7465 2873 656c 662e 7465  numerate(self.te
+000149d0: 726d 7329 3a0a 2020 2020 2020 2020 2020  rms):.          
+000149e0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+000149f0: 6e73 7461 6e63 6528 7465 726d 2c20 5f64  nstance(term, _d
+00014a00: 2e44 696d 290a 2020 2020 2020 2020 2020  .Dim).          
+00014a10: 2020 2020 2020 6966 2074 6572 6d2e 6465        if term.de
+00014a20: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a40: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
+00014a50: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
+00014a60: 3d3d 2022 7472 7565 6469 765f 2220 2b20  == "truediv_" + 
+00014a70: 2822 7269 6768 7422 2069 6620 7269 6768  ("right" if righ
+00014a80: 7420 656c 7365 2022 6c65 6674 2229 3a0a  t else "left"):.
+00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014aa0: 2020 2020 2020 2020 6966 2074 6572 6d2e          if term.
+00014ab0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00014ac0: 696e 7075 7473 5b2d 315d 203d 3d20 6f74  inputs[-1] == ot
+00014ad0: 6865 723a 0a20 2020 2020 2020 2020 2020  her:.           
+00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014af0: 2072 6574 7572 6e20 690a 2020 2020 2020   return i.      
+00014b00: 2020 2020 2020 2020 2020 6966 206f 7468            if oth
+00014b10: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+00014b20: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+00014b30: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+00014b40: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00014b50: 2e6b 696e 6420 3d3d 2022 7472 7565 6469  .kind == "truedi
+00014b60: 765f 2220 2b20 2822 7269 6768 7422 2069  v_" + ("right" i
+00014b70: 6620 6e6f 7420 7269 6768 7420 656c 7365  f not right else
+00014b80: 2022 6c65 6674 2229 3a0a 2020 2020 2020   "left"):.      
+00014b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ba0: 2020 6966 206f 7468 6572 2e64 6572 6976    if other.deriv
+00014bb0: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00014bc0: 735b 2d31 5d20 3d3d 2074 6572 6d3a 0a20  s[-1] == term:. 
+00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014be0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014bf0: 6e20 690a 2020 2020 2020 2020 2020 2020  n i.            
+00014c00: 2020 2020 6966 2074 6572 6d2e 6973 5f63      if term.is_c
+00014c10: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+00014c20: 696d 2829 2061 6e64 206f 7468 6572 2e69  im() and other.i
+00014c30: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
+00014c40: 635f 6469 6d28 293a 0a20 2020 2020 2020  c_dim():.       
+00014c50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00014c60: 7572 6e20 690a 2020 2020 2020 2020 2320  urn i.        # 
+00014c70: 466f 7220 7468 6520 6c61 7374 2f66 6972  For the last/fir
+00014c80: 7374 2074 6572 6d2c 2065 7874 7261 2063  st term, extra c
+00014c90: 6865 636b 732e 0a20 2020 2020 2020 2069  hecks..        i
+00014ca0: 203d 206c 656e 2873 656c 662e 7465 726d   = len(self.term
+00014cb0: 7329 202d 2031 2069 6620 7269 6768 7420  s) - 1 if right 
+00014cc0: 656c 7365 2030 0a20 2020 2020 2020 2074  else 0.        t
+00014cd0: 6572 6d20 3d20 7365 6c66 2e74 6572 6d73  erm = self.terms
+00014ce0: 5b69 5d0a 2020 2020 2020 2020 6966 206b  [i].        if k
+00014cf0: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
+00014d00: 7622 2920 616e 6420 6f74 6865 7220 3d3d  v") and other ==
+00014d10: 2074 6572 6d3a 0a20 2020 2020 2020 2020   term:.         
+00014d20: 2020 2072 6574 7572 6e20 690a 2020 2020     return i.    
+00014d30: 2020 2020 6f70 5f6b 696e 6420 3d20 6b69      op_kind = ki
+00014d40: 6e64 202b 2022 5f22 202b 2028 2272 6967  nd + "_" + ("rig
+00014d50: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
+00014d60: 6520 226c 6566 7422 290a 2020 2020 2020  e "left").      
+00014d70: 2020 6966 2074 6572 6d2e 6465 7269 7665    if term.derive
+00014d80: 645f 6672 6f6d 5f6f 7020 616e 6420 7465  d_from_op and te
+00014d90: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
+00014da0: 6f70 2e6b 696e 6420 3d3d 206f 705f 6b69  op.kind == op_ki
+00014db0: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
+00014dc0: 7265 7475 726e 2069 0a20 2020 2020 2020  return i.       
+00014dd0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00014de0: 2020 6465 6620 6578 7465 6e64 5f6d 756c    def extend_mul
+00014df0: 5f64 6976 5f28 7365 6c66 2c20 6f74 6865  _div_(self, othe
+00014e00: 722c 206b 696e 642c 2072 6967 6874 293a  r, kind, right):
+00014e10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014e20: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
+00014e30: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+00014e40: 7061 7261 6d20 7374 7220 6b69 6e64 3a0a  param str kind:.
+00014e50: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+00014e60: 6f6f 6c20 7269 6768 743a 0a20 2020 2020  ool right:.     
+00014e70: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+00014e80: 7373 6572 7420 6b69 6e64 2069 6e20 7b22  ssert kind in {"
+00014e90: 6d75 6c22 2c20 2266 6c6f 6f72 6469 7622  mul", "floordiv"
+00014ea0: 2c20 2274 7275 6564 6976 222c 2022 6365  , "truediv", "ce
+00014eb0: 696c 6469 7622 7d0a 2020 2020 2020 2020  ildiv"}.        
+00014ec0: 6966 206f 7468 6572 2e69 735f 636f 6e73  if other.is_cons
+00014ed0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
+00014ee0: 2920 616e 6420 6f74 6865 722e 6469 6d65  ) and other.dime
+00014ef0: 6e73 696f 6e20 3d3d 2031 3a0a 2020 2020  nsion == 1:.    
+00014f00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00014f10: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00014f20: 6c66 2e74 6572 6d73 3a0a 2020 2020 2020  lf.terms:.      
+00014f30: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00014f40: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
+00014f50: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+00014f60: 6d73 2e61 7070 656e 6428 6f74 6865 7229  ms.append(other)
+00014f70: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00014f80: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
+00014f90: 2264 6976 2229 3a0a 2020 2020 2020 2020  "div"):.        
+00014fa0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+00014fb0: 6d73 203d 205b 5f4f 704d 756c 7454 6572  ms = [_OpMultTer
+00014fc0: 6d2e 6e65 775f 6469 765f 6469 6d28 7365  m.new_div_dim(se
+00014fd0: 6c66 2e61 735f 6469 6d28 292c 206f 7468  lf.as_dim(), oth
+00014fe0: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
+00014ff0: 6967 6874 3d72 6967 6874 295d 0a20 2020  ight=right)].   
+00015000: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00015010: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+00015020: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015030: 2061 6e64 206f 7468 6572 2e64 6572 6976   and other.deriv
+00015040: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
+00015050: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
+00015060: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
+00015070: 6e20 6f74 6865 722e 6465 7269 7665 645f  n other.derived_
+00015080: 6672 6f6d 5f6f 702e 696e 7075 7473 2069  from_op.inputs i
+00015090: 6620 7269 6768 7420 656c 7365 2072 6576  f right else rev
+000150a0: 6572 7365 6428 6f74 6865 722e 6465 7269  ersed(other.deri
+000150b0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+000150c0: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+000150d0: 2020 2020 2073 656c 662e 6578 7465 6e64       self.extend
+000150e0: 5f6d 756c 5f64 6976 5f28 7465 726d 2c20  _mul_div_(term, 
+000150f0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
+00015100: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
+00015110: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00015120: 2020 2069 6478 203d 2073 656c 662e 5f73     idx = self._s
+00015130: 696d 706c 6966 795f 7465 726d 5f69 6478  implify_term_idx
+00015140: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
+00015150: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
+00015160: 2020 2020 2020 2020 6966 2069 6478 2069          if idx i
+00015170: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00015180: 2020 2020 2020 2020 7465 726d 203d 2073          term = s
+00015190: 656c 662e 7465 726d 735b 6964 785d 0a20  elf.terms[idx]. 
+000151a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000151b0: 7420 6973 696e 7374 616e 6365 2874 6572  t isinstance(ter
+000151c0: 6d2c 205f 642e 4469 6d29 0a20 2020 2020  m, _d.Dim).     
+000151d0: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
+000151e0: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
+000151f0: 6e64 206f 7468 6572 203d 3d20 7465 726d  nd other == term
+00015200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015210: 2020 7365 6c66 2e74 6572 6d73 2e70 6f70    self.terms.pop
+00015220: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
+00015230: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00015240: 2020 2020 2020 2020 2069 6620 6b69 6e64           if kind
+00015250: 203d 3d20 226d 756c 2220 616e 6420 7465   == "mul" and te
+00015260: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
+00015270: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+00015280: 2020 2020 6966 2074 6572 6d2e 6465 7269      if term.deri
+00015290: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+000152a0: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
+000152b0: 2028 2272 6967 6874 2220 6966 2072 6967   ("right" if rig
+000152c0: 6874 2065 6c73 6520 226c 6566 7422 293a  ht else "left"):
+000152d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000152e0: 2020 2020 2069 6620 7465 726d 2e64 6572       if term.der
+000152f0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00015300: 7574 735b 2d31 5d20 3d3d 206f 7468 6572  uts[-1] == other
+00015310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015320: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00015330: 6572 6d73 5b69 6478 5d20 3d20 7465 726d  erms[idx] = term
+00015340: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015350: 2e69 6e70 7574 735b 305d 0a20 2020 2020  .inputs[0].     
+00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015370: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00015380: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00015390: 2022 6d75 6c22 2061 6e64 206f 7468 6572   "mul" and other
+000153a0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+000153b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000153c0: 2020 6966 206f 7468 6572 2e64 6572 6976    if other.deriv
+000153d0: 6564 5f66 726f 6d5f 6f70 2e6b 696e 6420  ed_from_op.kind 
+000153e0: 3d3d 2022 7472 7565 6469 765f 2220 2b20  == "truediv_" + 
+000153f0: 2822 7269 6768 7422 2069 6620 6e6f 7420  ("right" if not 
+00015400: 7269 6768 7420 656c 7365 2022 6c65 6674  right else "left
+00015410: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00015420: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+00015430: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015440: 2e69 6e70 7574 735b 2d31 5d20 3d3d 2074  .inputs[-1] == t
+00015450: 6572 6d3a 0a20 2020 2020 2020 2020 2020  erm:.           
+00015460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015470: 662e 7465 726d 735b 6964 785d 203d 206f  f.terms[idx] = o
+00015480: 7468 6572 2e64 6572 6976 6564 5f66 726f  ther.derived_fro
+00015490: 6d5f 6f70 2e69 6e70 7574 735b 305d 0a20  m_op.inputs[0]. 
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000154c0: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
+000154d0: 6d2e 6973 5f63 6f6e 7374 616e 745f 7374  m.is_constant_st
+000154e0: 6174 6963 5f64 696d 2829 2061 6e64 206f  atic_dim() and o
+000154f0: 7468 6572 2e69 735f 636f 6e73 7461 6e74  ther.is_constant
+00015500: 5f73 7461 7469 635f 6469 6d28 293a 0a20  _static_dim():. 
+00015510: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015520: 6620 6b69 6e64 203d 3d20 226d 756c 223a  f kind == "mul":
+00015530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015540: 2020 2020 2069 6620 7465 726d 2e64 696d       if term.dim
+00015550: 656e 7369 6f6e 202a 206f 7468 6572 2e64  ension * other.d
+00015560: 696d 656e 7369 6f6e 203d 3d20 313a 0a20  imension == 1:. 
+00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015580: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+00015590: 732e 706f 7028 6964 7829 0a20 2020 2020  s.pop(idx).     
+000155a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155b0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+000155c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000155d0: 6c66 2e74 6572 6d73 5b69 6478 5d20 3d20  lf.terms[idx] = 
+000155e0: 5f6d 616b 655f 636f 6e73 7461 6e74 5f73  _make_constant_s
+000155f0: 7461 7469 635f 6469 6d28 7465 726d 2e64  tatic_dim(term.d
+00015600: 696d 656e 7369 6f6e 202a 206f 7468 6572  imension * other
+00015610: 2e64 696d 656e 7369 6f6e 2c20 6b69 6e64  .dimension, kind
+00015620: 3d74 6572 6d2e 6b69 6e64 290a 2020 2020  =term.kind).    
+00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015640: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00015650: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
+00015660: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
+00015670: 6e64 2074 6572 6d2e 6469 6d65 6e73 696f  nd term.dimensio
+00015680: 6e20 2520 6f74 6865 722e 6469 6d65 6e73  n % other.dimens
+00015690: 696f 6e20 3d3d 2030 3a0a 2020 2020 2020  ion == 0:.      
+000156a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000156b0: 6c66 2e74 6572 6d73 5b69 6478 5d20 3d20  lf.terms[idx] = 
+000156c0: 5f6d 616b 655f 636f 6e73 7461 6e74 5f73  _make_constant_s
+000156d0: 7461 7469 635f 6469 6d28 7465 726d 2e64  tatic_dim(term.d
+000156e0: 696d 656e 7369 6f6e 202f 2f20 6f74 6865  imension // othe
+000156f0: 722e 6469 6d65 6e73 696f 6e2c 206b 696e  r.dimension, kin
+00015700: 643d 7465 726d 2e6b 696e 6429 0a20 2020  d=term.kind).   
+00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015720: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00015730: 2020 2020 2020 2020 2320 4661 6c6c 6261          # Fallba
+00015740: 636b 2077 6974 6820 6765 6e65 7269 6320  ck with generic 
+00015750: 6861 6e64 6c69 6e67 2e0a 2020 2020 2020  handling..      
+00015760: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
+00015770: 6b69 6e64 202b 2022 5f22 202b 2028 2272  kind + "_" + ("r
+00015780: 6967 6874 2220 6966 2072 6967 6874 2065  ight" if right e
+00015790: 6c73 6520 226c 6566 7422 290a 2020 2020  lse "left").    
+000157a0: 2020 2020 2020 2020 6966 206b 696e 642e          if kind.
+000157b0: 656e 6473 7769 7468 2822 6469 7622 2920  endswith("div") 
+000157c0: 616e 6420 7465 726d 2e64 6572 6976 6564  and term.derived
+000157d0: 5f66 726f 6d5f 6f70 2061 6e64 2074 6572  _from_op and ter
+000157e0: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
+000157f0: 702e 6b69 6e64 203d 3d20 6f70 5f6b 696e  p.kind == op_kin
+00015800: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00015810: 2020 206e 756d 6572 6174 6f72 203d 2074     numerator = t
+00015820: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
+00015830: 5f6f 702e 696e 7075 7473 5b30 5d0a 2020  _op.inputs[0].  
+00015840: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00015850: 6e6f 6d69 6e61 746f 7220 3d20 7465 726d  nominator = term
+00015860: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015870: 2e69 6e70 7574 735b 315d 0a20 2020 2020  .inputs[1].     
+00015880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015890: 7465 726d 735b 6964 785d 203d 205f 4f70  terms[idx] = _Op
+000158a0: 4d75 6c74 5465 726d 2e6e 6577 5f64 6976  MultTerm.new_div
+000158b0: 5f64 696d 286e 756d 6572 6174 6f72 2c20  _dim(numerator, 
+000158c0: 6465 6e6f 6d69 6e61 746f 7220 2a20 6f74  denominator * ot
+000158d0: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
+000158e0: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
+000158f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00015900: 7572 6e0a 2020 2020 2020 2020 6966 206b  urn.        if k
+00015910: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
+00015920: 7622 293a 0a20 2020 2020 2020 2020 2020  v"):.           
+00015930: 2073 656c 662e 7465 726d 7320 3d20 5b5f   self.terms = [_
+00015940: 4f70 4d75 6c74 5465 726d 2e6e 6577 5f64  OpMultTerm.new_d
+00015950: 6976 5f64 696d 2873 656c 662e 6173 5f64  iv_dim(self.as_d
+00015960: 696d 2829 2c20 6f74 6865 722c 206b 696e  im(), other, kin
+00015970: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+00015980: 6768 7429 5d0a 2020 2020 2020 2020 2020  ght)].          
+00015990: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+000159a0: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
+000159b0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
+000159c0: 6620 7269 6768 743a 0a20 2020 2020 2020  f right:.       
+000159d0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+000159e0: 726d 732e 6170 7065 6e64 286f 7468 6572  rms.append(other
+000159f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00015a00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00015a10: 2020 2020 7365 6c66 2e74 6572 6d73 2e69      self.terms.i
+00015a20: 6e73 6572 7428 302c 206f 7468 6572 290a  nsert(0, other).
+00015a30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015a40: 726e 0a20 2020 2020 2020 2061 7373 6572  rn.        asser
+00015a50: 7420 4661 6c73 650a 0a20 2020 2040 636c  t False..    @cl
+00015a60: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00015a70: 6620 6e65 775f 6469 765f 6469 6d28 636c  f new_div_dim(cl
+00015a80: 732c 206e 756d 6572 6174 6f72 2c20 6465  s, numerator, de
+00015a90: 6e6f 6d69 6e61 746f 722c 206b 696e 642c  nominator, kind,
+00015aa0: 2072 6967 6874 293a 0a20 2020 2020 2020   right):.       
+00015ab0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+00015ac0: 7261 6d20 4469 6d20 6e75 6d65 7261 746f  ram Dim numerato
+00015ad0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
+00015ae0: 6d20 4469 6d20 6465 6e6f 6d69 6e61 746f  m Dim denominato
+00015af0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
+00015b00: 6d20 7374 7220 6b69 6e64 3a20 2266 6c6f  m str kind: "flo
+00015b10: 6f72 6469 7622 206f 7220 2263 6569 6c64  ordiv" or "ceild
+00015b20: 6976 2220 6f72 2022 7472 7565 6469 7622  iv" or "truediv"
+00015b30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00015b40: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
+00015b50: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+00015b60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015b70: 2020 2020 6469 6d5f 7661 6c75 6520 3d20      dim_value = 
+00015b80: 4e6f 6e65 0a20 2020 2020 2020 2061 203d  None.        a =
+00015b90: 206e 756d 6572 6174 6f72 2e64 696d 656e   numerator.dimen
+00015ba0: 7369 6f6e 0a20 2020 2020 2020 2062 203d  sion.        b =
+00015bb0: 2064 656e 6f6d 696e 6174 6f72 2e64 696d   denominator.dim
+00015bc0: 656e 7369 6f6e 0a20 2020 2020 2020 2069  ension.        i
+00015bd0: 6620 6120 6973 206e 6f74 204e 6f6e 6520  f a is not None 
+00015be0: 616e 6420 6220 6973 206e 6f74 204e 6f6e  and b is not Non
+00015bf0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00015c00: 6620 6b69 6e64 203d 3d20 2266 6c6f 6f72  f kind == "floor
+00015c10: 6469 7622 3a0a 2020 2020 2020 2020 2020  div":.          
+00015c20: 2020 2020 2020 6469 6d5f 7661 6c75 6520        dim_value 
+00015c30: 3d20 6120 2f2f 2062 0a20 2020 2020 2020  = a // b.       
+00015c40: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+00015c50: 3d20 2263 6569 6c64 6976 223a 0a20 2020  = "ceildiv":.   
+00015c60: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+00015c70: 5f76 616c 7565 203d 202d 282d 6120 2f2f  _value = -(-a //
+00015c80: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
+00015c90: 2020 2020 6966 2061 2025 2062 203d 3d20      if a % b == 
+00015ca0: 3020 616e 6420 7269 6768 743a 0a20 2020  0 and right:.   
+00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cc0: 206b 696e 6420 3d20 2266 6c6f 6f72 6469   kind = "floordi
+00015cd0: 7622 2020 2320 666f 7220 6e69 6365 7220  v"  # for nicer 
+00015ce0: 6465 7363 7269 7074 696f 6e2c 2061 6e64  description, and
+00015cf0: 2064 6f65 7320 6e6f 7420 6d61 7474 6572   does not matter
+00015d00: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00015d10: 6620 6b69 6e64 203d 3d20 2274 7275 6564  f kind == "trued
+00015d20: 6976 223a 0a20 2020 2020 2020 2020 2020  iv":.           
+00015d30: 2020 2020 2069 6620 6120 2520 6220 213d       if a % b !=
+00015d40: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00015d50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00015d60: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00015d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d80: 2020 2225 7320 7472 7565 6469 7620 2573    "%s truediv %s
+00015d90: 206f 6e6c 7920 616c 6c6f 7765 6420 6966   only allowed if
+00015da0: 2074 6865 2072 6573 756c 7420 6973 2061   the result is a
+00015db0: 6e20 696e 7465 6765 7222 2025 2028 6e75  n integer" % (nu
+00015dc0: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
+00015dd0: 6174 6f72 290a 2020 2020 2020 2020 2020  ator).          
+00015de0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015df0: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
+00015e00: 7661 6c75 6520 3d20 6120 2f2f 2062 0a20  value = a // b. 
+00015e10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015e20: 6620 7269 6768 743a 0a20 2020 2020 2020  f right:.       
+00015e30: 2020 2020 2020 2020 2020 2020 206b 696e               kin
+00015e40: 6420 3d20 2266 6c6f 6f72 6469 7622 2020  d = "floordiv"  
+00015e50: 2320 666f 7220 6e69 6365 7220 6465 7363  # for nicer desc
+00015e60: 7269 7074 696f 6e2c 2061 6e64 2064 6f65  ription, and doe
+00015e70: 7320 6e6f 7420 6d61 7474 6572 0a20 2020  s not matter.   
+00015e80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00015e90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015ea0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00015eb0: 2269 6e76 616c 6964 206b 696e 6420 2572  "invalid kind %r
+00015ec0: 2220 2520 286b 696e 642c 2929 0a20 2020  " % (kind,)).   
+00015ed0: 2020 2020 2069 6620 6b69 6e64 203d 3d20       if kind == 
+00015ee0: 2266 6c6f 6f72 6469 7622 2061 6e64 2072  "floordiv" and r
+00015ef0: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
+00015f00: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
+00015f10: 2225 732f 2f25 7322 2025 2028 5f67 6574  "%s//%s" % (_get
+00015f20: 5f64 6573 6372 6970 7469 6f6e 286e 756d  _description(num
+00015f30: 6572 6174 6f72 292c 205f 6765 745f 6465  erator), _get_de
+00015f40: 7363 7269 7074 696f 6e28 6465 6e6f 6d69  scription(denomi
+00015f50: 6e61 746f 7229 290a 2020 2020 2020 2020  nator)).        
+00015f60: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
+00015f70: 696c 6469 7622 2061 6e64 2072 6967 6874  ildiv" and right
+00015f80: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00015f90: 7363 7269 7074 696f 6e20 3d20 22e2 8c88  scription = "...
+00015fa0: 2573 2f25 73e2 8c89 2220 2520 285f 6765  %s/%s..." % (_ge
+00015fb0: 745f 6465 7363 7269 7074 696f 6e28 6e75  t_description(nu
+00015fc0: 6d65 7261 746f 7229 2c20 5f67 6574 5f64  merator), _get_d
+00015fd0: 6573 6372 6970 7469 6f6e 2864 656e 6f6d  escription(denom
+00015fe0: 696e 6174 6f72 2929 0a20 2020 2020 2020  inator)).       
+00015ff0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00016000: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
+00016010: 2022 2573 5f25 7328 2573 2c20 2573 2922   "%s_%s(%s, %s)"
+00016020: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
+00016030: 2020 2020 206b 696e 642c 0a20 2020 2020       kind,.     
+00016040: 2020 2020 2020 2020 2020 2022 7269 6768             "righ
+00016050: 7422 2069 6620 7269 6768 7420 656c 7365  t" if right else
+00016060: 2022 6c65 6674 222c 0a20 2020 2020 2020   "left",.       
+00016070: 2020 2020 2020 2020 205f 6765 745f 6465           _get_de
+00016080: 7363 7269 7074 696f 6e28 6e75 6d65 7261  scription(numera
+00016090: 746f 722c 2062 7261 636b 6574 733d 4661  tor, brackets=Fa
+000160a0: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
+000160b0: 2020 2020 2020 5f67 6574 5f64 6573 6372        _get_descr
+000160c0: 6970 7469 6f6e 2864 656e 6f6d 696e 6174  iption(denominat
+000160d0: 6f72 2c20 6272 6163 6b65 7473 3d46 616c  or, brackets=Fal
+000160e0: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
+000160f0: 2029 0a20 2020 2020 2020 206f 705f 6b69   ).        op_ki
+00016100: 6e64 203d 206b 696e 640a 2020 2020 2020  nd = kind.      
+00016110: 2020 6966 2061 2069 7320 6e6f 7420 4e6f    if a is not No
+00016120: 6e65 2061 6e64 2062 2069 7320 6e6f 7420  ne and b is not 
+00016130: 4e6f 6e65 2061 6e64 2061 2025 2062 203d  None and a % b =
+00016140: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00016150: 206f 705f 6b69 6e64 203d 2022 7472 7565   op_kind = "true
+00016160: 6469 7622 2020 2320 6d61 6b65 7320 736f  div"  # makes so
+00016170: 6d65 206f 7468 6572 2063 6865 636b 7320  me other checks 
+00016180: 7369 6d70 6c65 720a 2020 2020 2020 2020  simpler.        
+00016190: 6f70 5f6b 696e 6420 2b3d 2022 5f22 202b  op_kind += "_" +
+000161a0: 2028 2272 6967 6874 2220 6966 2072 6967   ("right" if rig
+000161b0: 6874 2065 6c73 6520 226c 6566 7422 290a  ht else "left").
+000161c0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000161d0: 642e 4469 6d28 0a20 2020 2020 2020 2020  d.Dim(.         
+000161e0: 2020 2064 6573 6372 6970 7469 6f6e 3d64     description=d
+000161f0: 6573 6372 6970 7469 6f6e 2c0a 2020 2020  escription,.    
+00016200: 2020 2020 2020 2020 6b69 6e64 3d6e 756d          kind=num
+00016210: 6572 6174 6f72 2e6b 696e 642c 0a20 2020  erator.kind,.   
+00016220: 2020 2020 2020 2020 2064 696d 656e 7369           dimensi
+00016230: 6f6e 3d64 696d 5f76 616c 7565 2c0a 2020  on=dim_value,.  
+00016240: 2020 2020 2020 2020 2020 6465 7269 7665            derive
+00016250: 645f 6672 6f6d 5f6f 703d 4f70 286b 696e  d_from_op=Op(kin
+00016260: 643d 6f70 5f6b 696e 642c 2069 6e70 7574  d=op_kind, input
+00016270: 733d 5b6e 756d 6572 6174 6f72 2c20 6465  s=[numerator, de
+00016280: 6e6f 6d69 6e61 746f 725d 292c 0a20 2020  nominator]),.   
+00016290: 2020 2020 2020 2020 2064 6572 6976 6564           derived
+000162a0: 5f66 726f 6d5f 7461 673d 6e75 6d65 7261  _from_tag=numera
+000162b0: 746f 722c 0a20 2020 2020 2020 2029 0a0a  tor,.        )..
+000162c0: 2020 2020 6465 6620 6173 5f64 696d 2873      def as_dim(s
+000162d0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000162e0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+000162f0: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
+00016300: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00016310: 662e 6973 5f6f 6e65 2829 3a0a 2020 2020  f.is_one():.    
+00016320: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00016330: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
+00016340: 6174 6963 5f64 696d 2831 290a 2020 2020  atic_dim(1).    
+00016350: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00016360: 7465 726d 7329 203d 3d20 313a 0a20 2020  terms) == 1:.   
+00016370: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00016380: 7365 6c66 2e74 6572 6d73 5b30 5d0a 2020  self.terms[0].  
+00016390: 2020 2020 2020 6469 6d5f 6b69 6e64 203d        dim_kind =
+000163a0: 205f 6765 745f 6d65 7267 6564 5f64 696d   _get_merged_dim
+000163b0: 5f6b 696e 6428 7365 6c66 2e74 6572 6d73  _kind(self.terms
+000163c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000163d0: 205f 642e 4469 6d28 0a20 2020 2020 2020   _d.Dim(.       
+000163e0: 2020 2020 206b 696e 643d 6469 6d5f 6b69       kind=dim_ki
+000163f0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
+00016400: 6465 7363 7269 7074 696f 6e3d 222a 222e  description="*".
+00016410: 6a6f 696e 286d 6170 285f 6765 745f 6465  join(map(_get_de
+00016420: 7363 7269 7074 696f 6e2c 2073 656c 662e  scription, self.
+00016430: 7465 726d 7329 292c 0a20 2020 2020 2020  terms)),.       
+00016440: 2020 2020 2064 696d 656e 7369 6f6e 3d73       dimension=s
+00016450: 656c 662e 6469 6d65 6e73 696f 6e2c 0a20  elf.dimension,. 
+00016460: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
+00016470: 6564 5f66 726f 6d5f 6f70 3d4f 7028 6b69  ed_from_op=Op(ki
+00016480: 6e64 3d22 6d75 6c22 2c20 696e 7075 7473  nd="mul", inputs
+00016490: 3d6c 6973 7428 7365 6c66 2e74 6572 6d73  =list(self.terms
+000164a0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+000164b0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+000164c0: 3d73 656c 662e 7265 7072 6573 656e 7461  =self.representa
+000164d0: 7469 7665 5f74 6167 2829 2c0a 2020 2020  tive_tag(),.    
+000164e0: 2020 2020 290a 0a20 2020 2064 6566 2072      )..    def r
+000164f0: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
+00016500: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+00016510: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00016520: 7970 653a 2044 696d 7c4e 6f6e 650a 2020  ype: Dim|None.  
+00016530: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00016540: 2020 2320 416c 736f 2073 6565 2044 696d    # Also see Dim
+00016550: 2e5f 4f70 4c69 6e65 6172 5465 726d 2e72  ._OpLinearTerm.r
+00016560: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
+00016570: 6728 292e 0a20 2020 2020 2020 2023 2046  g()..        # F
+00016580: 6972 7374 2066 696e 6420 616e 7920 6479  irst find any dy
+00016590: 6e61 6d69 632e 0a20 2020 2020 2020 2066  namic..        f
+000165a0: 6f72 2074 6572 6d5f 2069 6e20 7365 6c66  or term_ in self
+000165b0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+000165c0: 2020 2020 6966 2074 6572 6d5f 2e69 735f      if term_.is_
+000165d0: 6479 6e61 6d69 6328 293a 0a20 2020 2020  dynamic():.     
+000165e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000165f0: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
+00016600: 2320 4e6f 7720 6669 6e64 206e 6f6e 2d75  # Now find non-u
+00016610: 6e73 7065 6369 6669 6564 2e0a 2020 2020  nspecified..    
+00016620: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
+00016630: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00016640: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00016650: 5f2e 6b69 6e64 2021 3d20 4469 6d54 7970  _.kind != DimTyp
+00016660: 6573 2e55 6e73 7065 6369 6669 6564 3a0a  es.Unspecified:.
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 7265 7475 726e 2074 6572 6d5f 0a20 2020  return term_.   
+00016690: 2020 2020 2023 204e 6f77 2066 696e 6420       # Now find 
+000166a0: 616e 792e 0a20 2020 2020 2020 2066 6f72  any..        for
+000166b0: 2074 6572 6d5f 2069 6e20 7365 6c66 2e74   term_ in self.t
+000166c0: 6572 6d73 3a0a 2020 2020 2020 2020 2020  erms:.          
+000166d0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
+000166e0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000166f0: 6e65 0a0a 0a63 6c61 7373 205f 4f70 4c69  ne...class _OpLi
+00016700: 6e65 6172 5465 726d 3a0a 2020 2020 2222  nearTerm:.    ""
+00016710: 220a 2020 2020 7265 7072 6573 656e 7473  ".    represents
+00016720: 2073 7468 206c 696b 6520 6120 2a20 6220   sth like a * b 
+00016730: 2b20 630a 2020 2020 2222 220a 0a20 2020  + c.    """..   
+00016740: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00016750: 2020 6465 6620 6672 6f6d 5f64 696d 2863    def from_dim(c
+00016760: 6c73 2c20 6469 6d29 3a0a 2020 2020 2020  ls, dim):.      
+00016770: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00016780: 6172 616d 2044 696d 2064 696d 3a0a 2020  aram Dim dim:.  
+00016790: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+000167a0: 6d2e 5f4f 704c 696e 6561 7254 6572 6d0a  m._OpLinearTerm.
+000167b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000167c0: 2020 2020 7265 7320 3d20 636c 732e 7a65      res = cls.ze
+000167d0: 726f 2829 0a20 2020 2020 2020 2072 6573  ro().        res
+000167e0: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
+000167f0: 2864 696d 2c20 6b69 6e64 3d22 6164 6422  (dim, kind="add"
+00016800: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
+00016810: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00016820: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00016830: 6f64 0a20 2020 2064 6566 207a 6572 6f28  od.    def zero(
+00016840: 636c 7329 3a0a 2020 2020 2020 2020 2222  cls):.        ""
+00016850: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+00016860: 3a20 4469 6d2e 5f4f 704c 696e 6561 7254  : Dim._OpLinearT
+00016870: 6572 6d0a 2020 2020 2020 2020 2222 220a  erm.        """.
+00016880: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00016890: 4f70 4c69 6e65 6172 5465 726d 285b 5d29  OpLinearTerm([])
+000168a0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+000168b0: 5f5f 2873 656c 662c 2074 6572 6d73 293a  __(self, terms):
+000168c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000168d0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
+000168e0: 5b44 696d 2e5f 4f70 4d75 6c74 5465 726d  [Dim._OpMultTerm
+000168f0: 5d20 7465 726d 733a 0a20 2020 2020 2020  ] terms:.       
+00016900: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00016910: 662e 7465 726d 7320 3d20 7465 726d 730a  f.terms = terms.
+00016920: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
+00016930: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00016940: 2072 6574 7572 6e20 6861 7368 2874 7570   return hash(tup
+00016950: 6c65 2873 656c 662e 7465 726d 7329 290a  le(self.terms)).
+00016960: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
+00016970: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+00016980: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00016990: 6e63 6528 6f74 6865 722c 205f 4f70 4c69  nce(other, _OpLi
+000169a0: 6e65 6172 5465 726d 293a 0a20 2020 2020  nearTerm):.     
+000169b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000169c0: 6c66 2e74 6572 6d73 203d 3d20 6f74 6865  lf.terms == othe
+000169d0: 722e 7465 726d 730a 2020 2020 2020 2020  r.terms.        
+000169e0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
+000169f0: 2020 6465 6620 5f5f 6e65 5f5f 2873 656c    def __ne__(sel
+00016a00: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+00016a10: 2020 2072 6574 7572 6e20 6e6f 7420 7365     return not se
+00016a20: 6c66 2e5f 5f65 715f 5f28 6f74 6865 7229  lf.__eq__(other)
+00016a30: 0a0a 2020 2020 6465 6620 6173 5f64 696d  ..    def as_dim
+00016a40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00016a50: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
+00016a60: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
+00016a70: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00016a80: 656c 662e 6973 5f7a 6572 6f28 293a 0a20  elf.is_zero():. 
+00016a90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016aa0: 6e20 5f6d 616b 655f 636f 6e73 7461 6e74  n _make_constant
+00016ab0: 5f73 7461 7469 635f 6469 6d28 3029 0a20  _static_dim(0). 
+00016ac0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+00016ad0: 6c66 2e74 6572 6d73 2920 3d3d 2031 3a0a  lf.terms) == 1:.
+00016ae0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00016af0: 726e 2073 656c 662e 7465 726d 735b 305d  rn self.terms[0]
+00016b00: 2e61 735f 6469 6d28 290a 2020 2020 2020  .as_dim().      
+00016b10: 2020 6164 645f 7061 7274 7320 3d20 5b5d    add_parts = []
+00016b20: 0a20 2020 2020 2020 2064 6573 635f 7061  .        desc_pa
+00016b30: 7274 7320 3d20 5b5d 0a20 2020 2020 2020  rts = [].       
+00016b40: 2064 696d 203d 2030 0a20 2020 2020 2020   dim = 0.       
+00016b50: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
+00016b60: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
+00016b70: 2020 2020 2073 203d 2074 6572 6d2e 6173       s = term.as
+00016b80: 5f64 696d 2829 0a20 2020 2020 2020 2020  _dim().         
+00016b90: 2020 2061 6464 5f70 6172 7473 2e61 7070     add_parts.app
+00016ba0: 656e 6428 7329 0a20 2020 2020 2020 2020  end(s).         
+00016bb0: 2020 2064 6573 635f 7061 7274 732e 6170     desc_parts.ap
+00016bc0: 7065 6e64 285f 6765 745f 6465 7363 7269  pend(_get_descri
+00016bd0: 7074 696f 6e28 7329 290a 2020 2020 2020  ption(s)).      
+00016be0: 2020 2020 2020 6966 2064 696d 2069 7320        if dim is 
+00016bf0: 6e6f 7420 4e6f 6e65 2061 6e64 2073 2e64  not None and s.d
+00016c00: 696d 656e 7369 6f6e 2069 7320 6e6f 7420  imension is not 
+00016c10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016c20: 2020 2020 2020 6469 6d20 2b3d 2073 2e64        dim += s.d
+00016c30: 696d 656e 7369 6f6e 0a20 2020 2020 2020  imension.       
+00016c40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00016c50: 2020 2020 2020 2020 2020 2064 696d 203d             dim =
+00016c60: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00016c70: 206c 656e 2861 6464 5f70 6172 7473 2920   len(add_parts) 
+00016c80: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00016c90: 2020 7265 7475 726e 2061 6464 5f70 6172    return add_par
+00016ca0: 7473 5b30 5d0a 2020 2020 2020 2020 7265  ts[0].        re
+00016cb0: 7475 726e 205f 642e 4469 6d28 0a20 2020  turn _d.Dim(.   
+00016cc0: 2020 2020 2020 2020 206b 696e 643d 5f67           kind=_g
+00016cd0: 6574 5f6d 6572 6765 645f 6469 6d5f 6b69  et_merged_dim_ki
+00016ce0: 6e64 2861 6464 5f70 6172 7473 292c 0a20  nd(add_parts),. 
+00016cf0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00016d00: 6970 7469 6f6e 3d22 2b22 2e6a 6f69 6e28  iption="+".join(
+00016d10: 6465 7363 5f70 6172 7473 292c 0a20 2020  desc_parts),.   
+00016d20: 2020 2020 2020 2020 2064 696d 656e 7369           dimensi
+00016d30: 6f6e 3d64 696d 2c0a 2020 2020 2020 2020  on=dim,.        
+00016d40: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
+00016d50: 5f6f 703d 4f70 286b 696e 643d 2261 6464  _op=Op(kind="add
+00016d60: 222c 2069 6e70 7574 733d 6164 645f 7061  ", inputs=add_pa
+00016d70: 7274 7329 2c0a 2020 2020 2020 2020 2020  rts),.          
+00016d80: 2020 6465 7269 7665 645f 6672 6f6d 5f74    derived_from_t
+00016d90: 6167 3d73 656c 662e 7265 7072 6573 656e  ag=self.represen
+00016da0: 7461 7469 7665 5f74 6167 2829 2c0a 2020  tative_tag(),.  
+00016db0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00016dc0: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
+00016dd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016de0: 2244 696d 2e5f 4f70 4c69 6e65 6172 5465  "Dim._OpLinearTe
+00016df0: 726d 2825 7229 2220 2520 2873 656c 662e  rm(%r)" % (self.
+00016e00: 7465 726d 732c 290a 0a20 2020 2064 6566  terms,)..    def
+00016e10: 2069 735f 7a65 726f 2873 656c 6629 3a0a   is_zero(self):.
+00016e20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00016e30: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00016e40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016e50: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
+00016e60: 7365 6c66 2e74 6572 6d73 0a0a 2020 2020  self.terms..    
+00016e70: 6465 6620 6578 7465 6e64 5f61 6464 5f73  def extend_add_s
+00016e80: 7562 5f28 7365 6c66 2c20 6f74 6865 722c  ub_(self, other,
+00016e90: 206b 696e 642c 2072 6967 6874 293a 0a20   kind, right):. 
+00016ea0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016eb0: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00016ec0: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00016ed0: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
+00016ee0: 3a20 2261 6464 2220 6f72 2022 7375 6222  : "add" or "sub"
+00016ef0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00016f00: 626f 6f6c 2072 6967 6874 3a20 6f72 206c  bool right: or l
+00016f10: 6566 742e 2072 6967 6874 206d 6561 6e73  eft. right means
+00016f20: 2073 656c 6620 2b20 6f74 6865 722c 206c   self + other, l
+00016f30: 6566 7420 6d65 616e 7320 6f74 6865 7220  eft means other 
+00016f40: 2b20 7365 6c66 0a20 2020 2020 2020 2022  + self.        "
+00016f50: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
+00016f60: 7420 6b69 6e64 2069 6e20 7b22 6164 6422  t kind in {"add"
+00016f70: 2c20 2273 7562 227d 0a20 2020 2020 2020  , "sub"}.       
+00016f80: 206f 7468 6572 203d 2073 656c 662e 5f6d   other = self._m
+00016f90: 616b 655f 6469 6d28 6f74 6865 722c 206b  ake_dim(other, k
+00016fa0: 696e 643d 6b69 6e64 290a 2020 2020 2020  ind=kind).      
+00016fb0: 2020 6966 206f 7468 6572 2e69 735f 636f    if other.is_co
+00016fc0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00016fd0: 6d28 2920 616e 6420 6f74 6865 722e 6469  m() and other.di
+00016fe0: 6d65 6e73 696f 6e20 3d3d 2030 3a0a 2020  mension == 0:.  
+00016ff0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017000: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+00017010: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00017020: 7020 616e 6420 6f74 6865 722e 6465 7269  p and other.deri
+00017030: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00017040: 203d 3d20 2261 6464 223a 0a20 2020 2020   == "add":.     
+00017050: 2020 2020 2020 2066 6f72 206f 7468 6572         for other
+00017060: 5f20 696e 206f 7468 6572 2e64 6572 6976  _ in other.deriv
+00017070: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00017080: 7320 6966 2072 6967 6874 2065 6c73 6520  s if right else 
+00017090: 7265 7665 7273 6564 286f 7468 6572 2e64  reversed(other.d
+000170a0: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
+000170b0: 6e70 7574 7329 3a0a 2020 2020 2020 2020  nputs):.        
+000170c0: 2020 2020 2020 2020 7365 6c66 2e65 7874          self.ext
+000170d0: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
+000170e0: 6572 5f2c 206b 696e 643d 6b69 6e64 2c20  er_, kind=kind, 
+000170f0: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
+00017100: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00017110: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
+00017120: 4f70 4d75 6c74 5465 726d 2e66 726f 6d5f  OpMultTerm.from_
+00017130: 6469 6d28 6f74 6865 7229 0a20 2020 2020  dim(other).     
+00017140: 2020 206e 6567 5f74 6572 6d20 3d20 7465     neg_term = te
+00017150: 726d 2e6e 6567 6174 6976 6528 290a 2020  rm.negative().  
+00017160: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00017170: 2022 7375 6222 3a0a 2020 2020 2020 2020   "sub":.        
+00017180: 2020 2020 7465 726d 2c20 6e65 675f 7465      term, neg_te
+00017190: 726d 203d 206e 6567 5f74 6572 6d2c 2074  rm = neg_term, t
+000171a0: 6572 6d0a 2020 2020 2020 2020 6d6f 7374  erm.        most
+000171b0: 5f72 6563 656e 745f 7465 726d 203d 2073  _recent_term = s
+000171c0: 656c 662e 7465 726d 735b 2d31 2069 6620  elf.terms[-1 if 
+000171d0: 7269 6768 7420 656c 7365 2030 5d20 6966  right else 0] if
+000171e0: 2073 656c 662e 7465 726d 7320 656c 7365   self.terms else
+000171f0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00017200: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
+00017210: 6d3a 0a20 2020 2020 2020 2020 2020 2069  m:.            i
+00017220: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
+00017230: 726d 203d 3d20 6e65 675f 7465 726d 3a0a  rm == neg_term:.
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 7365 6c66 2e74 6572 6d73 2e70 6f70 282d  self.terms.pop(-
+00017260: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00017270: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+00017280: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00017290: 2020 2020 2020 6966 206d 6f73 745f 7265        if most_re
+000172a0: 6365 6e74 5f74 6572 6d2e 6973 5f63 6f6e  cent_term.is_con
+000172b0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+000172c0: 2829 2061 6e64 2074 6572 6d2e 6973 5f63  () and term.is_c
+000172d0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000172e0: 696d 2829 3a0a 2020 2020 2020 2020 2020  im():.          
+000172f0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00017300: 5b2d 3120 6966 2072 6967 6874 2065 6c73  [-1 if right els
+00017310: 6520 305d 203d 205f 4f70 4d75 6c74 5465  e 0] = _OpMultTe
+00017320: 726d 2e66 726f 6d5f 6469 6d28 0a20 2020  rm.from_dim(.   
+00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017340: 205f 6d61 6b65 5f63 6f6e 7374 616e 745f   _make_constant_
+00017350: 7374 6174 6963 5f64 696d 286d 6f73 745f  static_dim(most_
+00017360: 7265 6365 6e74 5f74 6572 6d2e 6469 6d65  recent_term.dime
+00017370: 6e73 696f 6e20 2b20 7465 726d 2e64 696d  nsion + term.dim
+00017380: 656e 7369 6f6e 2c20 6b69 6e64 3d6f 7468  ension, kind=oth
+00017390: 6572 2e6b 696e 6429 0a20 2020 2020 2020  er.kind).       
+000173a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000173b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000173c0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+000173d0: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
+000173e0: 6d2e 7465 726d 7320 616e 6420 7465 726d  m.terms and term
+000173f0: 2e74 6572 6d73 2061 6e64 206d 6f73 745f  .terms and most_
+00017400: 7265 6365 6e74 5f74 6572 6d2e 7465 726d  recent_term.term
+00017410: 735b 2d31 5d20 3d3d 2074 6572 6d2e 7465  s[-1] == term.te
+00017420: 726d 735b 2d31 5d3a 0a20 2020 2020 2020  rms[-1]:.       
+00017430: 2020 2020 2020 2020 2023 204d 6572 6765           # Merge
+00017440: 2074 6572 6d73 0a20 2020 2020 2020 2020   terms.         
+00017450: 2020 2020 2020 2061 203d 205f 4f70 4d75         a = _OpMu
+00017460: 6c74 5465 726d 2e66 726f 6d5f 6469 6d5f  ltTerm.from_dim_
+00017470: 6661 6374 6f72 7328 6d6f 7374 5f72 6563  factors(most_rec
+00017480: 656e 745f 7465 726d 2e74 6572 6d73 5b3a  ent_term.terms[:
+00017490: 2d31 5d29 2e61 735f 6469 6d28 290a 2020  -1]).as_dim().  
+000174a0: 2020 2020 2020 2020 2020 2020 2020 6220                b 
+000174b0: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
+000174c0: 6f6d 5f64 696d 5f66 6163 746f 7273 2874  om_dim_factors(t
+000174d0: 6572 6d2e 7465 726d 735b 3a2d 315d 292e  erm.terms[:-1]).
+000174e0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
+000174f0: 2020 2020 2020 2020 2072 6573 203d 205f           res = _
+00017500: 4f70 4d75 6c74 5465 726d 2e66 726f 6d5f  OpMultTerm.from_
+00017510: 6469 6d28 2861 202b 2062 2920 6966 2072  dim((a + b) if r
+00017520: 6967 6874 2065 6c73 6520 2862 202b 2061  ight else (b + a
+00017530: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00017540: 2020 2072 6573 2e65 7874 656e 645f 6d75     res.extend_mu
+00017550: 6c5f 6469 765f 2874 6572 6d2e 7465 726d  l_div_(term.term
+00017560: 735b 2d31 5d2c 206b 696e 643d 226d 756c  s[-1], kind="mul
+00017570: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
+00017580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017590: 656c 662e 7465 726d 735b 2d31 2069 6620  elf.terms[-1 if 
+000175a0: 7269 6768 7420 656c 7365 2030 5d20 3d20  right else 0] = 
+000175b0: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
+000175c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+000175d0: 2020 2069 6620 7269 6768 743a 0a20 2020     if right:.   
+000175e0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+000175f0: 726d 732e 6170 7065 6e64 2874 6572 6d29  rms.append(term)
+00017600: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00017610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017620: 7465 726d 732e 696e 7365 7274 2830 2c20  terms.insert(0, 
+00017630: 7465 726d 290a 0a20 2020 2064 6566 2065  term)..    def e
+00017640: 7874 656e 645f 6d75 6c5f 6469 765f 2873  xtend_mul_div_(s
+00017650: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
+00017660: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
+00017670: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00017680: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
+00017690: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
+000176a0: 616d 2073 7472 206b 696e 643a 2022 6d75  am str kind: "mu
+000176b0: 6c22 206f 7220 2263 6569 6c64 6976 220a  l" or "ceildiv".
+000176c0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+000176d0: 6f6f 6c20 7269 6768 743a 206f 7220 6c65  ool right: or le
+000176e0: 6674 2e20 7269 6768 7420 6d65 616e 7320  ft. right means 
+000176f0: 7365 6c66 202a 206f 7468 6572 2c20 6c65  self * other, le
+00017700: 6674 206d 6561 6e73 206f 7468 6572 202a  ft means other *
+00017710: 2073 656c 660a 2020 2020 2020 2020 2222   self.        ""
+00017720: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+00017730: 206b 696e 6420 696e 207b 226d 756c 222c   kind in {"mul",
+00017740: 2022 666c 6f6f 7264 6976 222c 2022 7472   "floordiv", "tr
+00017750: 7565 6469 7622 2c20 2263 6569 6c64 6976  uediv", "ceildiv
+00017760: 227d 0a20 2020 2020 2020 206f 7468 6572  "}.        other
+00017770: 203d 2073 656c 662e 5f6d 616b 655f 6469   = self._make_di
+00017780: 6d28 6f74 6865 722c 206b 696e 643d 6b69  m(other, kind=ki
+00017790: 6e64 290a 2020 2020 2020 2020 6966 206b  nd).        if k
+000177a0: 696e 6420 3d3d 2022 6d75 6c22 2061 6e64  ind == "mul" and
+000177b0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
+000177c0: 2020 2020 6966 206e 6f74 2061 6c6c 2874      if not all(t
+000177d0: 6572 6d2e 6361 6e5f 7369 6d70 6c69 6679  erm.can_simplify
+000177e0: 286f 7468 6572 2c20 6b69 6e64 3d6b 696e  (other, kind=kin
+000177f0: 642c 2072 6967 6874 3d72 6967 6874 2920  d, right=right) 
+00017800: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
+00017810: 2e74 6572 6d73 293a 0a20 2020 2020 2020  .terms):.       
+00017820: 2020 2020 2020 2020 2023 2044 6f20 6974           # Do it
+00017830: 2074 6865 206f 7468 6572 2077 6179 2061   the other way a
+00017840: 726f 756e 640a 2020 2020 2020 2020 2020  round.          
+00017850: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00017860: 2c20 6f74 6865 7220 3d20 5f4f 704c 696e  , other = _OpLin
+00017870: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
+00017880: 286f 7468 6572 292e 7465 726d 732c 2073  (other).terms, s
+00017890: 656c 662e 6173 5f64 696d 2829 0a20 2020  elf.as_dim().   
+000178a0: 2020 2020 2020 2020 2020 2020 2072 6967               rig
+000178b0: 6874 203d 2046 616c 7365 0a20 2020 2020  ht = False.     
+000178c0: 2020 2069 6620 6f74 6865 722e 6973 5f63     if other.is_c
+000178d0: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000178e0: 696d 2829 2061 6e64 206f 7468 6572 2e64  im() and other.d
+000178f0: 696d 656e 7369 6f6e 203d 3d20 313a 0a20  imension == 1:. 
+00017900: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017910: 6e0a 2020 2020 2020 2020 6966 206b 696e  n.        if kin
+00017920: 642e 656e 6473 7769 7468 2822 6469 7622  d.endswith("div"
+00017930: 2920 616e 6420 6c65 6e28 7365 6c66 2e74  ) and len(self.t
+00017940: 6572 6d73 2920 3e3d 2032 3a0a 2020 2020  erms) >= 2:.    
+00017950: 2020 2020 2020 2020 6966 2061 6e79 286e          if any(n
+00017960: 6f74 2074 6572 6d2e 6469 7669 7369 626c  ot term.divisibl
+00017970: 6528 6f74 6865 722c 2072 6967 6874 3d72  e(other, right=r
+00017980: 6967 6874 2920 666f 7220 7465 726d 2069  ight) for term i
+00017990: 6e20 7365 6c66 2e74 6572 6d73 293a 0a20  n self.terms):. 
+000179a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000179b0: 656c 662e 7465 726d 7320 3d20 5b0a 2020  elf.terms = [.  
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179d0: 2020 5f4f 704d 756c 7454 6572 6d2e 6672    _OpMultTerm.fr
+000179e0: 6f6d 5f64 696d 285f 4f70 4d75 6c74 5465  om_dim(_OpMultTe
+000179f0: 726d 2e6e 6577 5f64 6976 5f64 696d 2873  rm.new_div_dim(s
+00017a00: 656c 662e 6173 5f64 696d 2829 2c20 6f74  elf.as_dim(), ot
+00017a10: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
+00017a20: 7269 6768 743d 7269 6768 7429 290a 2020  right=right)).  
+00017a30: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a50: 7265 7475 726e 0a20 2020 2020 2020 2066  return.        f
+00017a60: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
+00017a70: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00017a80: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
+00017a90: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
+00017aa0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
+00017ab0: 7269 6768 7429 0a0a 2020 2020 6465 6620  right)..    def 
+00017ac0: 5f6d 616b 655f 6469 6d28 7365 6c66 2c20  _make_dim(self, 
+00017ad0: 6f74 6865 722c 206b 696e 6429 3a0a 2020  other, kind):.  
+00017ae0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00017af0: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
+00017b00: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00017b10: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
+00017b20: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00017b30: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00017b40: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00017b50: 7374 616e 6365 286f 7468 6572 2c20 696e  stance(other, in
+00017b60: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00017b70: 6261 7365 5f74 6167 203d 2073 656c 662e  base_tag = self.
+00017b80: 7265 7072 6573 656e 7461 7469 7665 5f74  representative_t
+00017b90: 6167 2829 0a20 2020 2020 2020 2020 2020  ag().           
+00017ba0: 2072 6574 7572 6e20 5f6d 616b 655f 636f   return _make_co
+00017bb0: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00017bc0: 6d28 6f74 6865 722c 206b 696e 643d 6261  m(other, kind=ba
+00017bd0: 7365 5f74 6167 2e6b 696e 6420 6966 2062  se_tag.kind if b
+00017be0: 6173 655f 7461 6720 656c 7365 204e 6f6e  ase_tag else Non
+00017bf0: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
+00017c00: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+00017c10: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
+00017c20: 2020 2020 2020 2072 6574 7572 6e20 6f74         return ot
+00017c30: 6865 722e 6765 745f 7361 6d65 5f62 6173  her.get_same_bas
+00017c40: 6528 290a 2020 2020 2020 2020 656c 7365  e().        else
+00017c50: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00017c60: 6973 6520 5479 7065 4572 726f 7228 2225  ise TypeError("%
+00017c70: 7320 2573 2025 7320 696e 7661 6c69 6420  s %s %s invalid 
+00017c80: 666f 7220 7479 7065 2025 7322 2025 2028  for type %s" % (
+00017c90: 7365 6c66 2c20 6b69 6e64 2c20 6f74 6865  self, kind, othe
+00017ca0: 722c 2074 7970 6528 6f74 6865 7229 2929  r, type(other)))
+00017cb0: 0a0a 2020 2020 6465 6620 7265 7072 6573  ..    def repres
+00017cc0: 656e 7461 7469 7665 5f74 6167 2873 656c  entative_tag(sel
+00017cd0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00017ce0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00017cf0: 4469 6d7c 4e6f 6e65 0a20 2020 2020 2020  Dim|None.       
+00017d00: 2022 2222 0a20 2020 2020 2020 2023 2046   """.        # F
+00017d10: 6972 7374 2066 696e 6420 616e 7920 6479  irst find any dy
+00017d20: 6e61 6d69 632e 0a20 2020 2020 2020 2066  namic..        f
+00017d30: 6f72 2074 6572 6d20 696e 2073 656c 662e  or term in self.
+00017d40: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00017d50: 2020 2066 6f72 2074 6572 6d5f 2069 6e20     for term_ in 
+00017d60: 7465 726d 2e74 6572 6d73 3a0a 2020 2020  term.terms:.    
+00017d70: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00017d80: 6572 6d5f 2e69 735f 6479 6e61 6d69 6328  erm_.is_dynamic(
+00017d90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00017da0: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00017db0: 726d 5f0a 2020 2020 2020 2020 2320 4e6f  rm_.        # No
+00017dc0: 7720 6669 6e64 206e 6f6e 2d75 6e73 7065  w find non-unspe
+00017dd0: 6369 6669 6564 2e0a 2020 2020 2020 2020  cified..        
+00017de0: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
+00017df0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00017e00: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
+00017e10: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
+00017e20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017e30: 7465 726d 5f2e 6b69 6e64 2021 3d20 4469  term_.kind != Di
+00017e40: 6d54 7970 6573 2e55 6e73 7065 6369 6669  mTypes.Unspecifi
+00017e50: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00017e60: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00017e70: 6572 6d5f 0a20 2020 2020 2020 2023 204e  erm_.        # N
+00017e80: 6f77 2066 696e 6420 616e 792e 0a20 2020  ow find any..   
+00017e90: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
+00017ea0: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00017eb0: 2020 2020 2020 2020 2066 6f72 2074 6572           for ter
+00017ec0: 6d5f 2069 6e20 7465 726d 2e74 6572 6d73  m_ in term.terms
+00017ed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017ee0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
+00017ef0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00017f00: 6e65 0a0a 0a64 6566 205f 6765 745f 6d65  ne...def _get_me
+00017f10: 7267 6564 5f64 696d 5f6b 696e 6428 6469  rged_dim_kind(di
+00017f20: 6d5f 7461 6773 293a 0a20 2020 2022 2222  m_tags):.    """
+00017f30: 0a20 2020 203a 7061 7261 6d20 6c69 7374  .    :param list
+00017f40: 5b44 696d 5d7c 7475 706c 655b 4469 6d5d  [Dim]|tuple[Dim]
+00017f50: 2064 696d 5f74 6167 733a 0a20 2020 203a   dim_tags:.    :
+00017f60: 7265 7475 726e 3a20 6469 6d20 6b69 6e64  return: dim kind
+00017f70: 0a20 2020 203a 7274 7970 653a 2045 6e74  .    :rtype: Ent
+00017f80: 6974 790a 2020 2020 2222 220a 2020 2020  ity.    """.    
+00017f90: 6966 2061 6e79 2874 6167 2e69 735f 6261  if any(tag.is_ba
+00017fa0: 7463 685f 6469 6d28 2920 666f 7220 7461  tch_dim() for ta
+00017fb0: 6720 696e 2064 696d 5f74 6167 7329 3a0a  g in dim_tags):.
+00017fc0: 2020 2020 2020 2020 7265 7475 726e 2044          return D
+00017fd0: 696d 5479 7065 732e 4261 7463 680a 2020  imTypes.Batch.  
+00017fe0: 2020 656c 6966 2061 6e79 2874 6167 2e69    elif any(tag.i
+00017ff0: 735f 6665 6174 7572 655f 6469 6d28 2920  s_feature_dim() 
+00018000: 666f 7220 7461 6720 696e 2064 696d 5f74  for tag in dim_t
+00018010: 6167 7329 3a0a 2020 2020 2020 2020 7265  ags):.        re
+00018020: 7475 726e 2044 696d 5479 7065 732e 4665  turn DimTypes.Fe
+00018030: 6174 7572 650a 2020 2020 656c 7365 3a0a  ature.    else:.
+00018040: 2020 2020 2020 2020 7265 7475 726e 2044          return D
+00018050: 696d 5479 7065 732e 5370 6174 6961 6c0a  imTypes.Spatial.
+00018060: 0a0a 6465 6620 6469 6d5f 636d 705f 7661  ..def dim_cmp_va
+00018070: 6c75 6528 6f62 6a29 3a0a 2020 2020 2222  lue(obj):.    ""
+00018080: 220a 2020 2020 3a70 6172 616d 2044 696d  ".    :param Dim
+00018090: 7c5f 4d61 726b 6564 4469 6d20 6f62 6a3a  |_MarkedDim obj:
+000180a0: 0a20 2020 203a 7265 7475 726e 3a20 616e  .    :return: an
+000180b0: 7974 6869 6e67 2077 6869 6368 2063 616e  ything which can
+000180c0: 2062 6520 636f 6d70 6172 6564 0a20 2020   be compared.   
+000180d0: 2022 2222 0a20 2020 2023 204d 616b 6520   """.    # Make 
+000180e0: 4469 6d20 616e 6420 5f4d 6172 6b65 6444  Dim and _MarkedD
+000180f0: 696d 2063 6f6d 7061 7261 626c 6520 746f  im comparable to
+00018100: 2065 6163 6820 6f74 6865 722e 0a20 2020   each other..   
+00018110: 2023 204e 6f74 6520 7468 6174 2074 6865   # Note that the
+00018120: 206f 7264 6572 2069 7320 7265 616c 6c79   order is really
+00018130: 2061 7262 6974 7261 7279 2061 6e64 2064   arbitrary and d
+00018140: 6f65 7320 6e6f 7420 6d61 7474 6572 2e0a  oes not matter..
+00018150: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00018160: 6528 6f62 6a2c 205f 642e 4469 6d29 3a0a  e(obj, _d.Dim):.
+00018170: 2020 2020 2020 2020 6f62 6a20 3d20 6f62          obj = ob
+00018180: 6a2e 6765 745f 7361 6d65 5f62 6173 6528  j.get_same_base(
+00018190: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000181a0: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
+000181b0: 222c 0a20 2020 2020 2020 2020 2020 206f  ",.            o
+000181c0: 626a 2e64 6573 6372 6970 7469 6f6e 2c0a  bj.description,.
+000181d0: 2020 2020 2020 2020 2020 2020 6f62 6a2e              obj.
+000181e0: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
+000181f0: 2020 6f62 6a2e 6469 6d65 6e73 696f 6e2c    obj.dimension,
+00018200: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
+00018210: 2e64 796e 5f73 697a 655f 6578 742e 6469  .dyn_size_ext.di
+00018220: 6d73 2069 6620 6f62 6a2e 6479 6e5f 7369  ms if obj.dyn_si
+00018230: 7a65 5f65 7874 2069 7320 6e6f 7420 4e6f  ze_ext is not No
+00018240: 6e65 2065 6c73 6520 4e6f 6e65 2c0a 2020  ne else None,.  
+00018250: 2020 2020 2020 290a 2020 2020 6966 2069        ).    if i
+00018260: 7369 6e73 7461 6e63 6528 6f62 6a2c 205f  sinstance(obj, _
+00018270: 6d2e 4d61 726b 6564 4469 6d29 3a0a 2020  m.MarkedDim):.  
+00018280: 2020 2020 2020 7265 7475 726e 206f 626a        return obj
+00018290: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+000182a0: 655f 5f2c 206f 626a 2e74 6167 0a20 2020  e__, obj.tag.   
+000182b0: 2072 6574 7572 6e20 6f62 6a0a             return obj.
```

### Comparing `returnn-1.20230428.123018/returnn/tensor/_tensor_extra.py` & `returnn-1.20230428.134452/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230428.134452/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230428.134452/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230428.134452/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/dim.py` & `returnn-1.20230428.134452/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/marked_dim.py` & `returnn-1.20230428.134452/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/tensor.py` & `returnn-1.20230428.134452/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tensor/tensor_dict.py` & `returnn-1.20230428.134452/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/compat.py` & `returnn-1.20230428.134452/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/data_pipeline.py` & `returnn-1.20230428.134452/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/distributed.py` & `returnn-1.20230428.134452/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/engine.py` & `returnn-1.20230428.134452/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230428.134452/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230428.134452/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/horovod.py` & `returnn-1.20230428.134452/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230428.134452/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/layers/base.py` & `returnn-1.20230428.134452/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/layers/basic.py` & `returnn-1.20230428.134452/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/layers/rec.py` & `returnn-1.20230428.134452/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/layers/segmental_model.py` & `returnn-1.20230428.134452/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/layers/signal_processing.py` & `returnn-1.20230428.134452/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/native_op.py` & `returnn-1.20230428.134452/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/network.py` & `returnn-1.20230428.134452/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/sprint.py` & `returnn-1.20230428.134452/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/updater.py` & `returnn-1.20230428.134452/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/util/basic.py` & `returnn-1.20230428.134452/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/util/data.py` & `returnn-1.20230428.134452/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/util/ken_lm.py` & `returnn-1.20230428.134452/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/tf/util/open_fst.py` & `returnn-1.20230428.134452/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/data/pipeline.py` & `returnn-1.20230428.134452/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230428.134452/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/data/tensor_utils.py` & `returnn-1.20230428.134452/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/engine.py` & `returnn-1.20230428.134452/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/frontend/_backend.py` & `returnn-1.20230428.134452/returnn/torch/frontend/_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1221,18 +1221,17 @@
             # PyTorch anyway uses a window with size = n_fft internally.
             # So we just explicitly handle the window logic.
             win_length=fft_length,
             window=window_pt,
             center=False,
             return_complex=True,
         )
-
         y = Tensor("stft", dims=batch_dims + [out_dim, out_spatial_dim], dtype=TorchBackend.get_dtype_name_raw(y_raw))
         y.feature_dim = out_dim
-        y.raw_tensor = y_raw
+        y.raw_tensor = torch.reshape(y_raw, [d.get_dim_value() for d in y.dims])
         return y
 
     @staticmethod
     def lstm(
         source: _TT,
         *,
         state_h: _TT,
```

### Comparing `returnn-1.20230428.123018/returnn/torch/frontend/_rand.py` & `returnn-1.20230428.134452/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/frontend/bridge.py` & `returnn-1.20230428.134452/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/torch/updater.py` & `returnn-1.20230428.134452/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/basic.py` & `returnn-1.20230428.134452/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/better_exchook.py` & `returnn-1.20230428.134452/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/bpe.py` & `returnn-1.20230428.134452/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/debug.py` & `returnn-1.20230428.134452/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/debug_helpers.py` & `returnn-1.20230428.134452/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/fsa.py` & `returnn-1.20230428.134452/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230428.134452/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/pprint.py` & `returnn-1.20230428.134452/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/py-to-pickle.cpp` & `returnn-1.20230428.134452/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/sig_proc.py` & `returnn-1.20230428.134452/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn/util/task_system.py` & `returnn-1.20230428.134452/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/returnn.egg-info/PKG-INFO` & `returnn-1.20230428.134452/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230428.123018
+Version: 1.20230428.134452
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230428.123018/returnn.egg-info/SOURCES.txt` & `returnn-1.20230428.134452/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/setup.py` & `returnn-1.20230428.134452/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/DummySprintExec.py` & `returnn-1.20230428.134452/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230428.134452/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230428.134452/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230428.134452/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/_set_num_threads1.py` & `returnn-1.20230428.134452/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/_setup_test_env.py` & `returnn-1.20230428.134452/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/bpe-unicode-demo.codes` & `returnn-1.20230428.134452/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/bpe-unicode-demo.vocab` & `returnn-1.20230428.134452/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/lexicon_opt.isyms` & `returnn-1.20230428.134452/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/lexicon_opt.jpg` & `returnn-1.20230428.134452/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/lint_common.py` & `returnn-1.20230428.134452/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/pycharm-inspect.py` & `returnn-1.20230428.134452/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/pylint.py` & `returnn-1.20230428.134452/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/returnn-as-framework.py` & `returnn-1.20230428.134452/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/rf_utils.py` & `returnn-1.20230428.134452/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/spelling.dic` & `returnn-1.20230428.134452/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_Config.py` & `returnn-1.20230428.134452/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_Dataset.py` & `returnn-1.20230428.134452/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_Fsa.py` & `returnn-1.20230428.134452/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_GeneratingDataset.py` & `returnn-1.20230428.134452/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_HDFDataset.py` & `returnn-1.20230428.134452/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_LearningRateControl.py` & `returnn-1.20230428.134452/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_Log.py` & `returnn-1.20230428.134452/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_MultiProcDataset.py` & `returnn-1.20230428.134452/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_PTDataset.py` & `returnn-1.20230428.134452/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_Pretrain.py` & `returnn-1.20230428.134452/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_ResNet.py` & `returnn-1.20230428.134452/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_SprintDataset.py` & `returnn-1.20230428.134452/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_SprintInterface.py` & `returnn-1.20230428.134452/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFEngine.py` & `returnn-1.20230428.134452/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFNativeOp.py` & `returnn-1.20230428.134452/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFNetworkLayer.py` & `returnn-1.20230428.134452/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230428.134452/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230428.134452/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFUpdater.py` & `returnn-1.20230428.134452/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TFUtil.py` & `returnn-1.20230428.134452/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TF_determinism.py` & `returnn-1.20230428.134452/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TaskSystem.py` & `returnn-1.20230428.134452/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230428.134452/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_TranslationDataset.py` & `returnn-1.20230428.134452/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_Util.py` & `returnn-1.20230428.134452/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_demos.py` & `returnn-1.20230428.134452/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_fork_exec.py` & `returnn-1.20230428.134452/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_hdf_dump.py` & `returnn-1.20230428.134452/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_array.py` & `returnn-1.20230428.134452/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_attention.py` & `returnn-1.20230428.134452/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_base.py` & `returnn-1.20230428.134452/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_container.py` & `returnn-1.20230428.134452/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_conv.py` & `returnn-1.20230428.134452/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_encoder_conformer.py` & `returnn-1.20230428.134452/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_math.py` & `returnn-1.20230428.134452/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_normalization.py` & `returnn-1.20230428.134452/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_rec.py` & `returnn-1.20230428.134452/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_rf_signal.py` & `returnn-1.20230428.134452/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_tensor.py` & `returnn-1.20230428.134452/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_tools.py` & `returnn-1.20230428.134452/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_torch_frontend.py` & `returnn-1.20230428.134452/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tests/test_torch_internal_frontend.py` & `returnn-1.20230428.134452/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/analyze-dataset-batches.py` & `returnn-1.20230428.134452/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/bliss-collect-seq-lens.py` & `returnn-1.20230428.134452/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/bliss-dump-text.py` & `returnn-1.20230428.134452/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/bliss-get-segment-names.py` & `returnn-1.20230428.134452/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/bliss-to-ogg-zip.py` & `returnn-1.20230428.134452/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/bpe-create-lexicon.py` & `returnn-1.20230428.134452/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/calculate-word-error-rate.py` & `returnn-1.20230428.134452/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/cleanup-old-models.py` & `returnn-1.20230428.134452/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/collect-orth-symbols.py` & `returnn-1.20230428.134452/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/collect-words.py` & `returnn-1.20230428.134452/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/compile_native_op.py` & `returnn-1.20230428.134452/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/compile_tf_graph.py` & `returnn-1.20230428.134452/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/debug-dump-search-scores.py` & `returnn-1.20230428.134452/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/debug-plot-search-scores.py` & `returnn-1.20230428.134452/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/dump-dataset-raw-strings.py` & `returnn-1.20230428.134452/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/dump-dataset.py` & `returnn-1.20230428.134452/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/dump-forward-stats.py` & `returnn-1.20230428.134452/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/dump-forward.py` & `returnn-1.20230428.134452/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/dump-network-json.py` & `returnn-1.20230428.134452/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/dump-pickle.py` & `returnn-1.20230428.134452/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230428.134452/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/get-attention-weights.py` & `returnn-1.20230428.134452/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/get-best-model-epoch.py` & `returnn-1.20230428.134452/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/hdf_dump.py` & `returnn-1.20230428.134452/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230428.134452/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/import-blocks-mt-model.py` & `returnn-1.20230428.134452/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/import-t2t-mt-model.py` & `returnn-1.20230428.134452/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/Makefile` & `returnn-1.20230428.134452/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/README.md` & `returnn-1.20230428.134452/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/example/README.md` & `returnn-1.20230428.134452/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230428.134452/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230428.134452/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230428.134452/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/file.h` & `returnn-1.20230428.134452/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230428.134452/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230428.134452/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/main.cc` & `returnn-1.20230428.134452/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230428.134452/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230428.134452/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230428.134452/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/tf_avg_checkpoints.py` & `returnn-1.20230428.134452/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/tf_inspect_checkpoint.py` & `returnn-1.20230428.134452/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230428.123018/tools/tf_inspect_summary_log.py` & `returnn-1.20230428.134452/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

