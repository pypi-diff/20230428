# Comparing `tmp/vectorlab-1.0.1.tar.gz` & `tmp/vectorlab-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorlab-1.0.1.tar", last modified: Thu Apr 13 14:55:08 2023, max compression
+gzip compressed data, was "vectorlab-1.0.2.tar", last modified: Fri Apr 28 08:11:35 2023, max compression
```

## Comparing `vectorlab-1.0.1.tar` & `vectorlab-1.0.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     1544 2022-10-19 08:15:02.000000 vectorlab-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2212 2023-04-13 14:52:09.284268 vectorlab-1.0.1/README.md
--rw-r--r--   0        0        0     1331 2023-04-13 14:52:09.292262 vectorlab-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8196 2022-11-24 06:03:57.630870 vectorlab-1.0.1/vectorlab/.DS_Store
--rw-r--r--   0        0        0      272 2023-04-13 14:53:42.990467 vectorlab-1.0.1/vectorlab/__init__.py
--rw-r--r--   0        0        0    11168 2023-04-13 14:52:09.294277 vectorlab-1.0.1/vectorlab/base.py
--rw-r--r--   0        0        0      113 2022-10-25 03:41:44.000000 vectorlab-1.0.1/vectorlab/data/__init__.py
--rw-r--r--   0        0        0     1129 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/_argument_generator.py
--rw-r--r--   0        0        0     1308 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/_data_generator.py
--rw-r--r--   0        0        0       76 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/dataloader/__init__.py
--rw-r--r--   0        0        0     3809 2023-04-13 14:52:09.294877 vectorlab-1.0.1/vectorlab/data/dataloader/_torch_dataloader.py
--rw-r--r--   0        0        0     4801 2023-04-13 14:52:09.295769 vectorlab-1.0.1/vectorlab/data/dataloader/_torch_geometric_dataloader.py
--rw-r--r--   0        0        0     1662 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/dataloader/tests/test_torch_dataloader.py
--rw-r--r--   0        0        0       57 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/dataset/__init__.py
--rw-r--r--   0        0        0     6196 2023-04-13 14:52:09.296470 vectorlab-1.0.1/vectorlab/data/dataset/_torch_dataset.py
--rw-r--r--   0        0        0    31856 2023-04-13 14:52:09.297053 vectorlab-1.0.1/vectorlab/data/dataset/_ts_dataset.py
--rw-r--r--   0        0        0      385 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/tests/test_argument_generator.py
--rw-r--r--   0        0        0      533 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/tests/test_data_generator.py
--rw-r--r--   0        0        0       23 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/ensemble/__init__.py
--rw-r--r--   0        0        0     3677 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/ensemble/_voting.py
--rw-r--r--   0        0        0     4070 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/ensemble/tests/test_ensemble_voting.py
--rw-r--r--   0        0        0       70 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/__init__.py
--rw-r--r--   0        0        0    11604 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/_generator.py
--rw-r--r--   0        0        0    15921 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/_utils.py
--rw-r--r--   0        0        0     1169 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/tests/test_graph_generator.py
--rw-r--r--   0        0        0     6818 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/tests/test_graph_utils.py
--rw-r--r--   0        0        0       68 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/__init__.py
--rw-r--r--   0        0        0     1920 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/_bfs.py
--rw-r--r--   0        0        0     1869 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/_dfs.py
--rw-r--r--   0        0        0     1275 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/_random_walk.py
--rw-r--r--   0        0        0     2235 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/tests/test_graph_walking.py
--rw-r--r--   0        0        0       23 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/__init__.py
--rw-r--r--   0        0        0       87 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/__init__.py
--rw-r--r--   0        0        0     8721 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/_dtw.py
--rw-r--r--   0        0        0     3329 2023-04-13 14:52:09.297651 vectorlab-1.0.1/vectorlab/metrics/pairwise/_kl_div.py
--rw-r--r--   0        0        0     1183 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/_lp_norm.py
--rw-r--r--   0        0        0     3206 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/_sbd.py
--rw-r--r--   0        0        0     2365 2023-04-13 14:52:09.298082 vectorlab-1.0.1/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py
--rw-r--r--   0        0        0      119 2023-04-13 14:52:09.298380 vectorlab-1.0.1/vectorlab/nn/__init__.py
--rw-r--r--   0        0        0     4305 2023-04-13 14:52:09.298680 vectorlab-1.0.1/vectorlab/nn/_earlystopping.py
--rw-r--r--   0        0        0     6318 2023-04-13 14:52:09.299021 vectorlab-1.0.1/vectorlab/nn/_resolver.py
--rw-r--r--   0        0        0    46446 2023-04-13 14:52:09.299466 vectorlab-1.0.1/vectorlab/nn/explorer.py
--rw-r--r--   0        0        0     2906 2023-04-13 14:52:09.299821 vectorlab-1.0.1/vectorlab/nn/functional.py
--rw-r--r--   0        0        0      201 2023-04-13 14:52:09.300127 vectorlab-1.0.1/vectorlab/nn/models/__init__.py
--rw-r--r--   0        0        0    18081 2023-04-13 14:52:09.300609 vectorlab-1.0.1/vectorlab/nn/models/_autoencoder.py
--rw-r--r--   0        0        0     2303 2023-04-13 14:52:09.300957 vectorlab-1.0.1/vectorlab/nn/models/_basic_gnn.py
--rw-r--r--   0        0        0     3679 2023-04-13 14:52:09.301388 vectorlab-1.0.1/vectorlab/nn/models/_classifier.py
--rw-r--r--   0        0        0    11804 2023-04-13 14:52:09.301831 vectorlab-1.0.1/vectorlab/nn/models/_decoder.py
--rw-r--r--   0        0        0    32841 2023-04-13 14:52:09.302107 vectorlab-1.0.1/vectorlab/nn/models/_encoder.py
--rw-r--r--   0        0        0     2571 2023-04-13 14:52:09.302342 vectorlab-1.0.1/vectorlab/nn/models/_gnn_decoder.py
--rw-r--r--   0        0        0     7574 2023-04-13 14:52:09.303205 vectorlab-1.0.1/vectorlab/nn/models/_mlp.py
--rw-r--r--   0        0        0     5855 2023-04-13 14:52:09.303721 vectorlab-1.0.1/vectorlab/nn/models/_seq2seq.py
--rw-r--r--   0        0        0     2155 2023-04-13 14:52:09.304252 vectorlab-1.0.1/vectorlab/nn/models/tests/test_decoder.py
--rw-r--r--   0        0        0     2255 2023-04-13 14:52:09.304596 vectorlab-1.0.1/vectorlab/nn/models/tests/test_encoder.py
--rw-r--r--   0        0        0     1276 2023-04-13 14:52:09.304912 vectorlab-1.0.1/vectorlab/nn/models/tests/test_seq2seq.py
--rw-r--r--   0        0        0       44 2023-04-13 14:52:09.306267 vectorlab-1.0.1/vectorlab/nn/modules/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-13 14:52:09.306669 vectorlab-1.0.1/vectorlab/nn/modules/gnn_loss.py
--rw-r--r--   0        0        0     2556 2023-04-13 14:52:09.306963 vectorlab-1.0.1/vectorlab/nn/modules/loss.py
--rw-r--r--   0        0        0      743 2023-04-13 14:52:09.307274 vectorlab-1.0.1/vectorlab/nn/tests/test_explorer.py
--rw-r--r--   0        0        0      873 2023-04-13 14:52:09.307569 vectorlab-1.0.1/vectorlab/nn/tests/test_functional.py
--rw-r--r--   0        0        0       45 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/optimize/__init__.py
--rw-r--r--   0        0        0     6294 2023-04-13 14:52:09.308010 vectorlab-1.0.1/vectorlab/optimize/_estimate.py
--rw-r--r--   0        0        0    16484 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/optimize/_qap.py
--rw-r--r--   0        0        0     2521 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/optimize/tests/test_estimate.py
--rw-r--r--   0        0        0       69 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/__init__.py
--rw-r--r--   0        0        0      412 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/_helper.py
--rw-r--r--   0        0        0     2980 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/_palettes.py
--rw-r--r--   0        0        0    16083 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/_plot.py
--rw-r--r--   0        0        0      732 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/tests/test_plot.py
--rw-r--r--   0        0        0       76 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/__init__.py
--rw-r--r--   0        0        0     8732 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/_preprocessing.py
--rw-r--r--   0        0        0     2796 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/_utils.py
--rw-r--r--   0        0        0      116 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/smoothing/__init__.py
--rw-r--r--   0        0        0     6298 2023-04-13 14:52:09.308452 vectorlab-1.0.1/vectorlab/series/smoothing/_arima.py
--rw-r--r--   0        0        0     7438 2023-04-13 14:52:09.308890 vectorlab-1.0.1/vectorlab/series/smoothing/_holt_winters.py
--rw-r--r--   0        0        0    12319 2023-04-13 14:52:09.309332 vectorlab-1.0.1/vectorlab/series/smoothing/_moving_average.py
--rw-r--r--   0        0        0     6832 2023-04-13 14:52:09.310075 vectorlab-1.0.1/vectorlab/series/smoothing/_spectral_residual.py
--rw-r--r--   0        0        0     2333 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/smoothing/tests/test_series_smoothing.py
--rw-r--r--   0        0        0     1520 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/tests/test_series_preprocessing.py
--rw-r--r--   0        0        0       77 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/__init__.py
--rw-r--r--   0        0        0    15478 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/_deg_graph.py
--rw-r--r--   0        0        0    18242 2023-04-13 14:52:09.310614 vectorlab-1.0.1/vectorlab/stats/_freq_tree.py
--rw-r--r--   0        0        0    14207 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/_t_digest.py
--rw-r--r--   0        0        0     1312 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/tests/test_deg_graph.py
--rw-r--r--   0        0        0     1311 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/tests/test_freq_tree.py
--rw-r--r--   0        0        0     1310 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/tests/test_t_digest.py
--rw-r--r--   0        0        0      110 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/__init__.py
--rw-r--r--   0        0        0     9958 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_check.py
--rw-r--r--   0        0        0      617 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_env.py
--rw-r--r--   0        0        0     2026 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_loading.py
--rw-r--r--   0        0        0     2707 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_parser.py
--rw-r--r--   0        0        0     5089 2023-04-13 14:52:09.311123 vectorlab-1.0.1/vectorlab/utils/_time.py
--rw-r--r--   0        0        0     1123 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/tests/test_time.py
--rw-r--r--   0        0        0       45 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/__init__.py
--rw-r--r--   0        0        0    11924 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/_array.py
--rw-r--r--   0        0        0     2933 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/_tensor.py
--rw-r--r--   0        0        0     4140 2023-04-13 14:52:09.311629 vectorlab-1.0.1/vectorlab/vector/tests/test_array.py
--rw-r--r--   0        0        0     1217 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/tests/test_tensor.py
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 vectorlab-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1544 2023-04-24 06:07:52.194842 vectorlab-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2212 2023-04-24 06:07:52.194842 vectorlab-1.0.2/README.md
+-rw-r--r--   0        0        0     1352 2023-04-28 08:09:16.372051 vectorlab-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/__init__.py
+-rw-r--r--   0        0        0    11168 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/base.py
+-rw-r--r--   0        0        0      113 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/__init__.py
+-rw-r--r--   0        0        0     1129 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/_argument_generator.py
+-rw-r--r--   0        0        0     1308 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/_data_generator.py
+-rw-r--r--   0        0        0       76 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/__init__.py
+-rw-r--r--   0        0        0     3809 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/_torch_dataloader.py
+-rw-r--r--   0        0        0     4801 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/_torch_geometric_dataloader.py
+-rw-r--r--   0        0        0     1662 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/tests/test_torch_dataloader.py
+-rw-r--r--   0        0        0       57 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataset/__init__.py
+-rw-r--r--   0        0        0     6196 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataset/_torch_dataset.py
+-rw-r--r--   0        0        0    31856 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataset/_ts_dataset.py
+-rw-r--r--   0        0        0      385 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/tests/test_argument_generator.py
+-rw-r--r--   0        0        0      533 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/tests/test_data_generator.py
+-rw-r--r--   0        0        0       23 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/ensemble/__init__.py
+-rw-r--r--   0        0        0     3677 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/ensemble/_voting.py
+-rw-r--r--   0        0        0     4070 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/ensemble/tests/test_ensemble_voting.py
+-rw-r--r--   0        0        0       70 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/__init__.py
+-rw-r--r--   0        0        0    11604 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/_generator.py
+-rw-r--r--   0        0        0    15921 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/_utils.py
+-rw-r--r--   0        0        0     1169 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/tests/test_graph_generator.py
+-rw-r--r--   0        0        0     6818 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/tests/test_graph_utils.py
+-rw-r--r--   0        0        0       68 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/__init__.py
+-rw-r--r--   0        0        0     1920 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/_bfs.py
+-rw-r--r--   0        0        0     1869 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/_dfs.py
+-rw-r--r--   0        0        0     1275 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/_random_walk.py
+-rw-r--r--   0        0        0     2235 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/tests/test_graph_walking.py
+-rw-r--r--   0        0        0       23 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/__init__.py
+-rw-r--r--   0        0        0       87 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/__init__.py
+-rw-r--r--   0        0        0     8721 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_dtw.py
+-rw-r--r--   0        0        0     3329 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_kl_div.py
+-rw-r--r--   0        0        0     1183 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_lp_norm.py
+-rw-r--r--   0        0        0     3206 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_sbd.py
+-rw-r--r--   0        0        0     2365 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py
+-rw-r--r--   0        0        0      119 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/nn/__init__.py
+-rw-r--r--   0        0        0     4302 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/_earlystopping.py
+-rw-r--r--   0        0        0     7110 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/_logger.py
+-rw-r--r--   0        0        0     7154 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/_resolver.py
+-rw-r--r--   0        0        0    45671 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/explorer.py
+-rw-r--r--   0        0        0     2906 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/functional.py
+-rw-r--r--   0        0        0      201 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/__init__.py
+-rw-r--r--   0        0        0    18081 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_autoencoder.py
+-rw-r--r--   0        0        0     2303 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_basic_gnn.py
+-rw-r--r--   0        0        0     3679 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_classifier.py
+-rw-r--r--   0        0        0    11804 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_decoder.py
+-rw-r--r--   0        0        0    32841 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_encoder.py
+-rw-r--r--   0        0        0     2571 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_gnn_decoder.py
+-rw-r--r--   0        0        0     7574 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_mlp.py
+-rw-r--r--   0        0        0     5855 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_seq2seq.py
+-rw-r--r--   0        0        0     2155 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/tests/test_decoder.py
+-rw-r--r--   0        0        0     2255 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/tests/test_encoder.py
+-rw-r--r--   0        0        0     1276 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/tests/test_seq2seq.py
+-rw-r--r--   0        0        0       44 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/modules/__init__.py
+-rw-r--r--   0        0        0     1529 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/modules/gnn_loss.py
+-rw-r--r--   0        0        0     2556 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/modules/loss.py
+-rw-r--r--   0        0        0      743 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/tests/test_explorer.py
+-rw-r--r--   0        0        0      873 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/tests/test_functional.py
+-rw-r--r--   0        0        0       45 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/__init__.py
+-rw-r--r--   0        0        0     6294 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/_estimate.py
+-rw-r--r--   0        0        0    16484 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/_qap.py
+-rw-r--r--   0        0        0     2521 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/tests/test_estimate.py
+-rw-r--r--   0        0        0       69 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/_helper.py
+-rw-r--r--   0        0        0     2980 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/_palettes.py
+-rw-r--r--   0        0        0    16083 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/_plot.py
+-rw-r--r--   0        0        0      732 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/tests/test_plot.py
+-rw-r--r--   0        0        0       76 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/__init__.py
+-rw-r--r--   0        0        0     8732 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/_preprocessing.py
+-rw-r--r--   0        0        0     2796 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/_utils.py
+-rw-r--r--   0        0        0      116 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/__init__.py
+-rw-r--r--   0        0        0     6298 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_arima.py
+-rw-r--r--   0        0        0     7438 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_holt_winters.py
+-rw-r--r--   0        0        0    12319 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_moving_average.py
+-rw-r--r--   0        0        0     6832 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_spectral_residual.py
+-rw-r--r--   0        0        0     2333 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/tests/test_series_smoothing.py
+-rw-r--r--   0        0        0     1520 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/tests/test_series_preprocessing.py
+-rw-r--r--   0        0        0       77 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/__init__.py
+-rw-r--r--   0        0        0    15478 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/_deg_graph.py
+-rw-r--r--   0        0        0    18242 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/_freq_tree.py
+-rw-r--r--   0        0        0    14207 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/_t_digest.py
+-rw-r--r--   0        0        0     1312 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/tests/test_deg_graph.py
+-rw-r--r--   0        0        0     1311 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/tests/test_freq_tree.py
+-rw-r--r--   0        0        0     1310 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/tests/test_t_digest.py
+-rw-r--r--   0        0        0      110 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/__init__.py
+-rw-r--r--   0        0        0     9958 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_check.py
+-rw-r--r--   0        0        0      617 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_env.py
+-rw-r--r--   0        0        0     2026 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_loading.py
+-rw-r--r--   0        0        0     2707 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_parser.py
+-rw-r--r--   0        0        0     5089 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_time.py
+-rw-r--r--   0        0        0     1123 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/tests/test_time.py
+-rw-r--r--   0        0        0       45 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/__init__.py
+-rw-r--r--   0        0        0    11924 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/_array.py
+-rw-r--r--   0        0        0     2933 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/_tensor.py
+-rw-r--r--   0        0        0     4140 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/tests/test_array.py
+-rw-r--r--   0        0        0     1217 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/tests/test_tensor.py
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 vectorlab-1.0.2/PKG-INFO
```

### Comparing `vectorlab-1.0.1/LICENSE.txt` & `vectorlab-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/README.md` & `vectorlab-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/pyproject.toml` & `vectorlab-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "matplotlib>=3.5.3",
     "seaborn>=0.11.2",
     "pillow>=9.2.0",
     "pytz>=2022.2.1",
     "dill>=0.3.5.1",
     "halo>=0.0.31",
     "pyyaml>=6.0",
+    "wandb>=0.15.0",
     "torchinfo>=1.6.3",
     "tensorboard>=2.6.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1.2",
```

### Comparing `vectorlab-1.0.1/vectorlab/base.py` & `vectorlab-1.0.2/vectorlab/base.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/_argument_generator.py` & `vectorlab-1.0.2/vectorlab/data/_argument_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/_data_generator.py` & `vectorlab-1.0.2/vectorlab/data/_data_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/dataloader/_torch_dataloader.py` & `vectorlab-1.0.2/vectorlab/data/dataloader/_torch_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/dataloader/_torch_geometric_dataloader.py` & `vectorlab-1.0.2/vectorlab/data/dataloader/_torch_geometric_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/dataloader/tests/test_torch_dataloader.py` & `vectorlab-1.0.2/vectorlab/data/dataloader/tests/test_torch_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/dataset/_torch_dataset.py` & `vectorlab-1.0.2/vectorlab/data/dataset/_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/dataset/_ts_dataset.py` & `vectorlab-1.0.2/vectorlab/data/dataset/_ts_dataset.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/data/tests/test_data_generator.py` & `vectorlab-1.0.2/vectorlab/data/tests/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/ensemble/_voting.py` & `vectorlab-1.0.2/vectorlab/ensemble/_voting.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/ensemble/tests/test_ensemble_voting.py` & `vectorlab-1.0.2/vectorlab/ensemble/tests/test_ensemble_voting.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/_generator.py` & `vectorlab-1.0.2/vectorlab/graph/_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/_utils.py` & `vectorlab-1.0.2/vectorlab/graph/_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/tests/test_graph_generator.py` & `vectorlab-1.0.2/vectorlab/graph/tests/test_graph_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/tests/test_graph_utils.py` & `vectorlab-1.0.2/vectorlab/graph/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/walking/_bfs.py` & `vectorlab-1.0.2/vectorlab/graph/walking/_bfs.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/walking/_dfs.py` & `vectorlab-1.0.2/vectorlab/graph/walking/_dfs.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/walking/_random_walk.py` & `vectorlab-1.0.2/vectorlab/graph/walking/_random_walk.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/graph/walking/tests/test_graph_walking.py` & `vectorlab-1.0.2/vectorlab/graph/walking/tests/test_graph_walking.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/metrics/pairwise/_dtw.py` & `vectorlab-1.0.2/vectorlab/metrics/pairwise/_dtw.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/metrics/pairwise/_kl_div.py` & `vectorlab-1.0.2/vectorlab/metrics/pairwise/_kl_div.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/metrics/pairwise/_lp_norm.py` & `vectorlab-1.0.2/vectorlab/metrics/pairwise/_lp_norm.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/metrics/pairwise/_sbd.py` & `vectorlab-1.0.2/vectorlab/metrics/pairwise/_sbd.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py` & `vectorlab-1.0.2/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/_earlystopping.py` & `vectorlab-1.0.2/vectorlab/nn/_earlystopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from ..base import SLMixin
 from ..utils._check import check_valid_option
 
 
-class _EarlyStopping(SLMixin):
+class EarlyStopping(SLMixin):
     r"""The EarlyStopping class to stop training in advance.
 
     The EarlyStopping is a form of regularization used to avoid
     overfitting when a certain metric performance stop improving.
 
     Parameters
     ----------
@@ -114,15 +114,15 @@
             self.laziness_cnt_ >= self.laziness_
         ):
             return True
 
         return False
 
 
-class AscES(_EarlyStopping):
+class AscES(EarlyStopping):
     r"""The ascending type of EarlyStopping class to stop training in advance.
 
     Parameters
     ----------
     warmup : int
         The warmup iteration for training.
     laziness : int
@@ -141,15 +141,15 @@
             warmup=warmup, laziness=laziness,
             tolerance=tolerance
         )
 
         return
 
 
-class DescES(_EarlyStopping):
+class DescES(EarlyStopping):
     r"""The descending type of EarlyStopping class to stop training in advance.
 
     Parameters
     ----------
     warmup : int
         The warmup iteration for training.
     laziness : int
```

### Comparing `vectorlab-1.0.1/vectorlab/nn/_resolver.py` & `vectorlab-1.0.2/vectorlab/nn/_resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import torch
 import torch_geometric
+import importlib.metadata as importlib_metadata
 
-from . import _earlystopping
+from packaging.version import parse
+
+from . import _earlystopping, _logger
 from ..data import dataloader as _dataloader
 
+_torch_version = importlib_metadata.version('torch')
+
 
 def normalize_string(s):
     r"""Normalize an input string.
 
     This function will normalize a string, remove all '-', '_', ' '.
 
     Parameters
@@ -147,15 +152,18 @@
 
     Returns
     -------
     torch.optim.lr_scheduler._LRScheduler
         The resolved scheduler class.
     """
 
-    base_class = torch.optim.lr_scheduler._LRScheduler  # noqa
+    if parse(_torch_version) >= parse('2.0.0'):
+        base_class = torch.optim.lr_scheduler.LRScheduler
+    else:
+        base_class = torch.optim.lr_scheduler._LRScheduler  # noqa
 
     schedulers = [
         scheduler
         for scheduler in vars(torch.optim.lr_scheduler).values()
         if isinstance(scheduler, type) and issubclass(scheduler, base_class)
     ]
     schedulers_dict = {}
@@ -172,30 +180,59 @@
     Parameters
     ----------
     query : str
         Input earlystopping query.
 
     Returns
     -------
-    _earlystopping._EarlyStopping
+    _earlystopping.EarlyStopping
         The resolved earlystopping class.
     """
 
-    base_class = _earlystopping._EarlyStopping  # noqa
+    base_class = _earlystopping.EarlyStopping
 
     earlystoppings = [
         es
         for es in vars(_earlystopping).values()
         if isinstance(es, type) and issubclass(es, base_class)
     ]
     earlystoppings_dict = {}
 
     return resolver(query, earlystoppings, earlystoppings_dict)
 
 
+def logger_resolver(query):
+    r"""A logger resolver.
+
+    List all loggers supported by vectorlab.nn._logger and find
+    corresponding logger.
+
+    Parameters
+    ----------
+    query : str
+        Input logger query.
+
+    Returns
+    -------
+    _logger.BaseLogger
+        The resolved logger class.
+    """
+
+    base_class = _logger.BaseLogger
+
+    loggers = [
+        logger
+        for logger in vars(_logger).values()
+        if isinstance(logger, type) and issubclass(logger, base_class)
+    ]
+    loggers_dict = {}
+
+    return resolver(query, loggers, loggers_dict)
+
+
 def activation_resolver(query):
     r"""An activation resolver.
 
     List all activations supported by torch.nn.modules.activation and
     find corresponding activation.
 
     Parameters
```

### Comparing `vectorlab-1.0.1/vectorlab/nn/explorer.py` & `vectorlab-1.0.2/vectorlab/nn/explorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import time
+import uuid
 import numpy as np
 
 from tqdm.auto import tqdm
 from sklearn.model_selection import KFold
 
 import torch
 
 from torchinfo import summary
 from torch.utils.data import Subset
-from torch.utils.tensorboard import SummaryWriter
 from torch_geometric.data import Data, Batch
 
 from ..base import SLMixin, Accumulator
 from ._resolver import (
     dataloader_resolver,
-    optimizer_resolver, scheduler_resolver, earlystopping_resolver
+    optimizer_resolver, scheduler_resolver, earlystopping_resolver,
+    logger_resolver
 )
 
 
 class Explorer(SLMixin):
     r"""The Explorer class to train a neural network.
 
     The Explorer helps to train a model with a certain set of arguments.
@@ -78,24 +79,26 @@
         The extra arguments for initialize the scheduler.
     earlystopping_fn : str, callable
         The earlystopping to be used to avoid overfitting.
     earlystopping_metric : str
         The montior metric for earlystopping.
     earlystopping_kwarg : dict
         The extra arguments for initialize the earlystopping.
+    logger_fn : str, callable
+        The logger to be used to log the metrics.
+    logger_project : str
+        The name of the current project.
+    logger_id : str
+        The name of the current experiment id.
+    logger_freq : int
+        The frequency to log the metrics.
     device : str, list, optional
         If given specified device or a list of devices, the explorer will use
         such device(s) as desired. If no device is specified, the explorer
         will automatically choose the device(s).
-    writer : bool
-        Whether to use summary writer or not.
-    writer_dir : str
-        The directory to store the information from summary writer.
-    writer_comment : str
-        The extra comment used to initialize the summary writer.
     parameters_dict : dict
         The extra parameters dictionary to specify.
 
     Attributes
     ----------
     net_ : torch.nn.Module
         The defined neural network.
@@ -145,28 +148,26 @@
         The earlystopping to be used to avoid overfitting.
     earlystopping_metric_ : str
         The montior metric for earlystopping.
     earlystopping_kwarg_ : dict
         The extra arguments for initialize the earlystopping.
     earlystopping_ : callable
         The earlystopping to break epoch iteration.
+    logger_fn_ : str, callable
+        The logger to be used to log the metrics.
+    logger_project_ : str
+        The name of the current project.
+    logger_id_ : str
+        The name of the current experiment id.
+    logger_freq_ : int
+        The frequency to log the metrics.
     device_ : torch.device
         The first device used to store the neural network and data.
     devices_ : list
         The list of potential devices that would be used.
-    writer_ : bool
-        If use summary writer of tensorboard to log the process.
-    train_writer_ : torch.utils.tensorboard.SummaryWriter
-        The summary writer for training process.
-    valid_writer_ : torch.utils.tensorboard.SummaryWriter
-        The summary writer for validation process.
-    writer_dir_ : str
-        The log directory for summary writer.
-    writer_comment : str
-        The comment used to identify the summary writer.
     parameters_dict_ : dict
         The dictionary stored the parameters that initialized the
         explorer.
     train_loss_ : float
         The loss criterion of trained neural network over the training
         dataset.
     valid_loss_ : float
@@ -197,16 +198,18 @@
                  test_loader_fn=None, test_loader_kwargs=None,
                  optimizer_fn='adamw',
                  learning_rate=0.1, weight_decay=0, optimizer_kwargs=None,
                  scheduler_fn='cosine_annealing_lr',
                  scheduler_kwargs=None,
                  earlystopping_fn='desc_es',
                  earlystopping_metric='loss', earlystopping_kwargs=None,
+                 logger_fn='tensorboard',
+                 logger_project='vectorlab_explorer_project', logger_id=None,
+                 logger_freq=1,
                  device=None,
-                 writer=False, writer_dir=None, writer_comment='',
                  parameters_dict=None):
 
         super().__init__()
 
         self._init_devices_(device)
 
         self.k_ = int(k)
@@ -257,17 +260,19 @@
         self._init_scheduler()
 
         self.earlystopping_fn_ = earlystopping_fn
         self.earlystopping_kwargs_ = earlystopping_kwargs
         self.earlystopping_metric_ = earlystopping_metric
         self._init_earlystopping()
 
-        self.writer_ = writer
-        self.writer_dir_ = writer_dir
-        self.writer_comment_ = writer_comment
+        self.logger_fn_ = logger_fn
+        self.logger_project_ = logger_project
+        self.logger_id_ = logger_id
+        self.logger_freq_ = logger_freq
+        self._init_logger()
 
         self._init_parameters_dict_(parameters_dict)
 
         return
 
     def _init_devices_(self, device=None):
         r"""Automatically initialize the devices used to store the data
@@ -400,14 +405,29 @@
         else:
             self.earlystopping_ = self.earlystopping_fn_(
                 **self.earlystopping_kwargs_
             )
 
         return self
 
+    def _init_logger(self):
+        r"""Initialize proper logger
+
+        Returns
+        -------
+        self : Explorer
+            Return itself.
+        """
+        self.logger_fn_ = logger_resolver(self.logger_fn_)
+
+        if self.logger_id_ is None:
+            self.logger_id_ = str(uuid.uuid4())
+
+        return self
+
     def _init_input_format(self):
         r"""Automatically analysis the data input format.
 
         Firstly, analysis the batch data input format, and generate
         corresponding data indices for net input and loss input.
 
         Returns
@@ -736,14 +756,52 @@
         loader : torch.utils.data.DataLoader
             The data loader containing validation data to evaluate the trained
             neural network.
         """
 
         return self._loss_evaluate(loader)
 
+    def _metrics(self, train_loader, valid_loader=None):
+        """Return the evaluated metrics from train and valid loader.
+
+        Parameters
+        ----------
+        train_loader : torch.utils.data.DataLoader
+            The data loader containing training data to evaluate the trained
+            neural network
+        valid_loader : torch.utils.data.DataLoader
+            The data loader containing validation data to evaluate the trained
+            neural network.
+
+        Returns
+        -------
+        metrics : dict
+            The dictionary contained the evaluation metrics for verfication.
+            If valid_loader is provided, it will be valid_metrics, otherwise,
+            it will be train_metrics.
+        nested_metrics : dict
+            The dictionary contained the evaluation metrics. The metrics are
+            in a nested representation of
+            {'train': {train_metrics}, 'valid': {valid_metrics}}.
+        """
+
+        train_metrics = self._evaluate(train_loader)
+
+        if valid_loader is None:
+            metrics = train_metrics
+            nested_metrics = {'train': train_metrics}
+
+            return metrics, nested_metrics
+
+        valid_metrics = self._evaluate(valid_loader)
+        metrics = valid_metrics
+        nested_metrics = {'train': train_metrics, 'valid': valid_metrics}
+
+        return metrics, nested_metrics
+
     def _inference(self, loader, verbose=0):
         r"""This is the abstract inference method.
 
         This is the abstract inference method that should be implemented in
         children class, that it will inference the result of inputs using
         trained neural network.
 
@@ -852,15 +910,15 @@
             If save the model parameters with best loss.
         save_last : bool, optional
             If save the last model parameters.
         verbose : int, optional
             If show the progress of training process.
             0 : quite mode
             1 : show basic summary
-            2 : show progress bar of inferring all data
+            2 : show progress bar of training all data
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
@@ -868,32 +926,34 @@
             print(
                 f'Training with parameters: {self.__repr_parameters__()} '
                 f'on devices {self.devices_}'
             )
 
         self.best_loss_ = np.Inf
 
-        if self.writer_:
-            self.train_writer_ = SummaryWriter(
-                log_dir=f'{self.writer_dir_}{self.writer_comment_}_train'
-                        if self.writer_dir_ else self.writer_dir_,
-                comment=f'{self.writer_comment_}_train'
+        if self.logger_fn_ is not None:
+            logger = self.logger_fn_(
+                self.logger_project_, self.logger_id_,
+                freq=self.logger_freq_
             )
+        else:
+            logger = None
 
-            if valid_dataset is not None:
-                self.valid_writer_ = SummaryWriter(
-                    log_dir=f'{self.writer_dir_}{self.writer_comment_}_valid'
-                            if self.writer_dir_ else self.writer_dir_,
-                    comment=f'{self.writer_comment_}_valid'
-                )
+        if logger or self.earlystopping_ or save_best or verbose > 1:
+            _calc_metrics = True
+        else:
+            _calc_metrics = False
 
         self.net_.to(self.device_)
         if hasattr(self.loss_fn_, 'to'):
             self.loss_fn_.to(self.device_)
 
+        if logger:
+            logger.watch(self.net_, self.loss_fn_)
+
         train_loader = self.train_loader_fn_(
             train_dataset,
             batch_size=self.batch_size_,
             num_workers=self.num_workers_,
             shuffle=True,
             **self.train_loader_kwargs_
         )
@@ -902,103 +962,71 @@
             valid_loader = self.valid_loader_fn_(
                 valid_dataset,
                 batch_size=self.batch_size_,
                 num_workers=self.num_workers_,
                 shuffle=False,
                 **self.valid_loader_kwargs_
             )
+        else:
+            valid_loader = None
 
         pbar = tqdm(
             range(self.num_epochs_),
             ascii=True,
             disable=(verbose <= 1)
         )
         for epoch in pbar:
             self._train(train_loader)
 
-            if self.writer_ or self.earlystopping_ or save_best or verbose > 1:
-                train_metrics_ = self._evaluate(train_loader)
+            if _calc_metrics:
+                metrics_, nested_metrics_ = self._metrics(
+                    train_loader, valid_loader
+                )
                 metric_repr_ = ', '.join(
                     [
                         f'{key}: {value:.3f}'
-                        for key, value in train_metrics_.items()
+                        for key, value in metrics_.items()
                     ]
                 )
 
-                if valid_dataset is not None:
-                    valid_metrics_ = self._evaluate(valid_loader)
-                    metric_repr_ = ', '.join(
-                        [
-                            f'{key}: {value:.3f}'
-                            for key, value in train_metrics_.items()
-                        ]
-                    )
-
                 pbar.set_description(
                     f'Epoch: {epoch:0{self.epochs_len_}d}, {metric_repr_}'
                 )
 
             if self.earlystopping_:
-                if valid_dataset is None:
-                    self.earlystopping_.record_metric(
-                        train_metrics_[self.earlystopping_metric_]
-                    )
-                else:
-                    self.earlystopping_.record_metric(
-                        valid_metrics_[self.earlystopping_metric_]
-                    )
+                self.earlystopping_.record_metric(
+                    metrics_[self.earlystopping_metric_]
+                )
 
-            if self.writer_:
-                for metric, value in train_metrics_.items():
-                    self.train_writer_.add_scalar(metric, value, epoch)
-
-                if valid_dataset is not None:
-                    for metric, value in valid_metrics_.items():
-                        self.valid_writer_.add_scalar(metric, value, epoch)
+            if logger and (epoch % logger.freq_ == 0):
+                logger.log(nested_metrics_, step=epoch)
 
             if save_best:
-                if valid_dataset is None:
-                    if train_metrics_['loss'] < self.best_loss_:
-                        self.best_loss_ = train_metrics_['loss']
-                        self._save_best_model()
-                else:
-                    if valid_metrics_['loss'] < self.best_loss_:
-                        self.best_loss_ = valid_metrics_['loss']
-                        self._save_best_model()
+                if metrics_['loss'] < self.best_loss_:
+                    self.best_loss_ = metrics_['loss']
+                    self._save_best_model()
 
             if self.earlystopping_ and self.earlystopping_.is_done():
                 break
 
-        train_metrics_ = self._evaluate(train_loader)
-        self.train_loss_ = train_metrics_['loss']
+        _, nested_metrics_ = self._metrics(
+            train_loader, valid_loader
+        )
 
-        if self.writer_:
-            self.train_writer_.add_hparams(
-                self.parameters_dict_,
-                {
-                    'hparam/' + metric: value
-                    for metric, value in train_metrics_.items()
-                }
-            )
+        self.train_loss_ = nested_metrics_['train']['loss']
 
-        if valid_dataset is not None:
-            valid_metrics_ = self._evaluate(valid_loader)
-            self.valid_loss_ = valid_metrics_['loss']
-
-            if self.writer_:
-                self.valid_writer_.add_hparams(
-                    self.parameters_dict_,
-                    {
-                        'hparam/' + metric: value
-                        for metric, value in valid_metrics_.items()
-                    }
-                )
+        if valid_loader:
+            self.valid_loss_ = nested_metrics_['valid']['loss']
         else:
             self.valid_loss_ = np.Inf
 
+        if logger:
+            logger.log_params(self.parameters_dict_, nested_metrics_)
+            logger.close()
+
         if save_last:
             self._save_last_model()
 
         if verbose:
             print(
                 f'Result: train loss {self.train_loss_:.6f}, '
                 f'valid loss {self.valid_loss_:.6f}'
@@ -1018,15 +1046,15 @@
         ----------
         train_dataset : torch.utils.data.Dataset
             The training dataset.
         verbose : int, optional
             If show the progress of k-fold training process.
             0 : quite mode
             1 : show basic summary
-            2 : show progress bar of inferring all data
+            2 : show progress bar of training all data
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
@@ -1040,34 +1068,36 @@
         accumulator = Accumulator(3, ['k_train_loss', 'k_valid_loss', 'k'])
 
         kf = KFold(n_splits=self.k_)
         for k, index in enumerate(kf.split(train_dataset)):
 
             (train_index, valid_index) = index
 
-            if self.writer_:
-                k_train_writer = SummaryWriter(
-                    log_dir=f'{self.writer_dir_}{self.writer_comment_}_'
-                            f'k_fold_{k}_train'
-                            if self.writer_dir_ else self.writer_dir_,
-                    comment=f'{self.writer_comment_}_k_fold_{k}_train'
-                )
-                k_valid_writer = SummaryWriter(
-                    log_dir=f'{self.writer_dir_}{self.writer_comment_}_'
-                            f'k_fold_{k}_valid'
-                            if self.writer_dir_ else self.writer_dir_,
-                    comment=f'{self.writer_comment_}_k_fold_{k}_valid'
+            if self.logger_fn_ is not None:
+                logger = self.logger_fn_(
+                    self.logger_project_, f'{self.logger_id_}-kfold-{k}',
+                    freq=self.logger_freq_
                 )
+            else:
+                logger = None
+
+            if logger or self.earlystopping_ or verbose > 1:
+                _calc_metrics = True
+            else:
+                _calc_metrics = False
 
             self.reset()
 
             self.net_.to(self.device_)
             if hasattr(self.loss_fn_, 'to'):
                 self.loss_fn_.to(self.device_)
 
+            if logger:
+                logger.watch(self.net_, self.loss_fn_)
+
             k_train_dataset = Subset(train_dataset, train_index)
             k_valid_dataset = Subset(train_dataset, valid_index)
 
             k_train_dataloader = self.train_loader_fn_(
                 k_train_dataset,
                 batch_size=self.batch_size_,
                 num_workers=self.num_workers_,
@@ -1086,73 +1116,59 @@
                 range(self.num_epochs_),
                 ascii=True,
                 disable=(verbose <= 1)
             )
             for epoch in pbar:
                 self._train(k_train_dataloader)
 
-                if self.writer_ or self.earlystopping_ or verbose > 1:
-                    k_train_metrics_ = self._evaluate(k_train_dataloader)
-                    k_valid_metrics_ = self._evaluate(k_valid_dataloader)
-
+                if _calc_metrics:
+                    k_metrics_, k_nested_metrics_ = self._metrics(
+                        k_train_dataloader, k_valid_dataloader
+                    )
                     metric_repr_ = ', '.join(
                         [
                             f'{key}: {value:.3f}'
-                            for key, value in k_valid_metrics_.items()
+                            for key, value in k_metrics_.items()
                         ]
                     )
+
                     pbar.set_description(
                         f'Epoch: {epoch:0{self.epochs_len_}d}, {metric_repr_}'
                     )
 
                 if self.earlystopping_:
                     self.earlystopping_.record_metric(
-                        k_valid_metrics_[self.earlystopping_metric_]
+                        k_metrics_[self.earlystopping_metric_]
                     )
 
-                if self.writer_:
-                    for metric, value in k_train_metrics_.items():
-                        k_train_writer.add_scalar(metric, value, epoch)
-
-                    for metric, value in k_valid_metrics_.items():
-                        k_valid_writer.add_scalar(metric, value, epoch)
+                if logger and (epoch % logger.freq_ == 0):
+                    logger.log(k_nested_metrics_, step=epoch)
 
                 if self.earlystopping_ and self.earlystopping_.is_done():
                     break
 
-            k_train_metrics_ = self._evaluate(k_train_dataloader)
-            k_valid_metrics_ = self._evaluate(k_valid_dataloader)
+            _, k_nested_metrics_ = self._metrics(
+                k_train_dataloader, k_valid_dataloader
+            )
 
-            if self.writer_:
-                k_train_writer.add_hparams(
-                    self.parameters_dict_,
-                    {
-                        'hparam/' + metric: value
-                        for metric, value in k_train_metrics_.items()
-                    }
-                )
-                k_valid_writer.add_hparams(
-                    self.parameters_dict_,
-                    {
-                        'hparam/' + metric: value
-                        for metric, value in k_valid_metrics_.items()
-                    }
-                )
+            if logger:
+                logger.log_params(self.parameters_dict_, k_nested_metrics_)
+                logger.close()
 
             accumulator.add(
                 {
-                    'k_train_loss': k_train_metrics_['loss'],
-                    'k_valid_loss': k_valid_metrics_['loss'],
+                    'k_train_loss': k_nested_metrics_['train']['loss'],
+                    'k_valid_loss': k_nested_metrics_['valid']['loss'],
                     'k': 1
                 }
             )
 
             if verbose:
-                k_train_loss_ = k_train_metrics_['loss']
-                k_valid_loss_ = k_valid_metrics_['loss']
+                k_train_loss_ = k_nested_metrics_['train']['loss']
+                k_valid_loss_ = k_nested_metrics_['valid']['loss']
                 print(
                     f'Fold {k}: train loss {k_train_loss_:.6f}, '
                     f'valid loss {k_valid_loss_:.6f}'
                 )
 
         self.k_train_loss_ = \
             accumulator.get('k_train_loss') / accumulator.get('k')
```

### Comparing `vectorlab-1.0.1/vectorlab/nn/functional.py` & `vectorlab-1.0.2/vectorlab/nn/functional.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_autoencoder.py` & `vectorlab-1.0.2/vectorlab/nn/models/_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_basic_gnn.py` & `vectorlab-1.0.2/vectorlab/nn/models/_basic_gnn.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_classifier.py` & `vectorlab-1.0.2/vectorlab/nn/models/_classifier.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_decoder.py` & `vectorlab-1.0.2/vectorlab/nn/models/_decoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_encoder.py` & `vectorlab-1.0.2/vectorlab/nn/models/_encoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_gnn_decoder.py` & `vectorlab-1.0.2/vectorlab/nn/models/_gnn_decoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_mlp.py` & `vectorlab-1.0.2/vectorlab/nn/models/_mlp.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/_seq2seq.py` & `vectorlab-1.0.2/vectorlab/nn/models/_seq2seq.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/tests/test_decoder.py` & `vectorlab-1.0.2/vectorlab/nn/models/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/tests/test_encoder.py` & `vectorlab-1.0.2/vectorlab/nn/models/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/models/tests/test_seq2seq.py` & `vectorlab-1.0.2/vectorlab/nn/models/tests/test_seq2seq.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/modules/gnn_loss.py` & `vectorlab-1.0.2/vectorlab/nn/modules/gnn_loss.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/modules/loss.py` & `vectorlab-1.0.2/vectorlab/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/tests/test_explorer.py` & `vectorlab-1.0.2/vectorlab/nn/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/nn/tests/test_functional.py` & `vectorlab-1.0.2/vectorlab/nn/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/optimize/_estimate.py` & `vectorlab-1.0.2/vectorlab/optimize/_estimate.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/optimize/_qap.py` & `vectorlab-1.0.2/vectorlab/optimize/_qap.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/optimize/tests/test_estimate.py` & `vectorlab-1.0.2/vectorlab/optimize/tests/test_estimate.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/plot/_palettes.py` & `vectorlab-1.0.2/vectorlab/plot/_palettes.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/plot/_plot.py` & `vectorlab-1.0.2/vectorlab/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/plot/tests/test_plot.py` & `vectorlab-1.0.2/vectorlab/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/_preprocessing.py` & `vectorlab-1.0.2/vectorlab/series/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/_utils.py` & `vectorlab-1.0.2/vectorlab/series/_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/smoothing/_arima.py` & `vectorlab-1.0.2/vectorlab/series/smoothing/_arima.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/smoothing/_holt_winters.py` & `vectorlab-1.0.2/vectorlab/series/smoothing/_holt_winters.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/smoothing/_moving_average.py` & `vectorlab-1.0.2/vectorlab/series/smoothing/_moving_average.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/smoothing/_spectral_residual.py` & `vectorlab-1.0.2/vectorlab/series/smoothing/_spectral_residual.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/smoothing/tests/test_series_smoothing.py` & `vectorlab-1.0.2/vectorlab/series/smoothing/tests/test_series_smoothing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/series/tests/test_series_preprocessing.py` & `vectorlab-1.0.2/vectorlab/series/tests/test_series_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/stats/_deg_graph.py` & `vectorlab-1.0.2/vectorlab/stats/_deg_graph.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/stats/_freq_tree.py` & `vectorlab-1.0.2/vectorlab/stats/_freq_tree.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/stats/_t_digest.py` & `vectorlab-1.0.2/vectorlab/stats/_t_digest.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/stats/tests/test_deg_graph.py` & `vectorlab-1.0.2/vectorlab/stats/tests/test_deg_graph.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/stats/tests/test_freq_tree.py` & `vectorlab-1.0.2/vectorlab/stats/tests/test_freq_tree.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/stats/tests/test_t_digest.py` & `vectorlab-1.0.2/vectorlab/stats/tests/test_t_digest.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/utils/_check.py` & `vectorlab-1.0.2/vectorlab/utils/_check.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/utils/_env.py` & `vectorlab-1.0.2/vectorlab/utils/_env.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/utils/_loading.py` & `vectorlab-1.0.2/vectorlab/utils/_loading.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/utils/_parser.py` & `vectorlab-1.0.2/vectorlab/utils/_parser.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/utils/_time.py` & `vectorlab-1.0.2/vectorlab/utils/_time.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/utils/tests/test_time.py` & `vectorlab-1.0.2/vectorlab/utils/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/vector/_array.py` & `vectorlab-1.0.2/vectorlab/vector/_array.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/vector/_tensor.py` & `vectorlab-1.0.2/vectorlab/vector/_tensor.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/vector/tests/test_array.py` & `vectorlab-1.0.2/vectorlab/vector/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/vectorlab/vector/tests/test_tensor.py` & `vectorlab-1.0.2/vectorlab/vector/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.1/PKG-INFO` & `vectorlab-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorlab
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lab for vectors.
 Author-email: Kyle Yang <kyle.yang1995@gmail.com>, Emma Qin <emmaqin0722@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +20,15 @@
 Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: pillow>=9.2.0
 Requires-Dist: pytz>=2022.2.1
 Requires-Dist: dill>=0.3.5.1
 Requires-Dist: halo>=0.0.31
 Requires-Dist: pyyaml>=6.0
+Requires-Dist: wandb>=0.15.0
 Requires-Dist: torchinfo>=1.6.3
 Requires-Dist: tensorboard>=2.6.0
 Requires-Dist: torch>=1.10.0 ; extra == "full"
 Requires-Dist: torch-sparse>=0.6.12 ; extra == "full"
 Requires-Dist: torch-cluster>=1.6.0 ; extra == "full"
 Requires-Dist: torch-scatter>=2.0.9 ; extra == "full"
 Requires-Dist: torch-spline-conv>=1.2.1 ; extra == "full"
```

