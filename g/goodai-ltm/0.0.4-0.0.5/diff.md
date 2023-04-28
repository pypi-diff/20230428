# Comparing `tmp/goodai-ltm-0.0.4.tar.gz` & `tmp/goodai-ltm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.0.4.tar", last modified: Wed Apr 19 18:51:42 2023, max compression
+gzip compressed data, was "goodai-ltm-0.0.5.tar", last modified: Thu Apr 20 20:20:40 2023, max compression
```

## Comparing `goodai-ltm-0.0.4.tar` & `goodai-ltm-0.0.5.tar`

### file list

```diff
@@ -1,79 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.009989 goodai-ltm-0.0.4/
--rw-rw-rw-   0        0        0      184 2023-04-19 18:51:42.009989 goodai-ltm-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-04-19 18:49:15.000000 goodai-ltm-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.929559 goodai-ltm-0.0.4/goodai/
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.952550 goodai-ltm-0.0.4/goodai/ltm/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.953550 goodai-ltm-0.0.4/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.954550 goodai-ltm-0.0.4/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     2000 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/names/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.963550 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     1518 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      323 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     2426 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      175 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    10899 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1861 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa_tok_entry.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.965549 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0     2531 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     6800 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/wiki.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.974550 goodai-ltm-0.0.4/goodai/ltm/embedding_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/__init__.py
--rw-rw-rw-   0        0        0      839 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/auto.py
--rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/contrast_classifier.py
--rw-rw-rw-   0        0        0     5290 2023-04-19 16:47:44.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/default.py
--rw-rw-rw-   0        0        0     1533 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     2648 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/openai_emb.py
--rw-rw-rw-   0        0        0     2081 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/st_emb.py
--rw-rw-rw-   0        0        0     5252 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/trainable.py
--rw-rw-rw-   0        0        0     1312 2023-04-19 16:11:12.000000 goodai-ltm-0.0.4/goodai/ltm/embeddings.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.977550 goodai-ltm-0.0.4/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0     3926 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     3006 2023-04-18 23:54:27.000000 goodai-ltm-0.0.4/goodai/ltm/eval/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.984550 goodai-ltm-0.0.4/goodai/ltm/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/collections_helper.py
--rw-rw-rw-   0        0        0      868 2023-04-18 21:34:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/json_helper.py
--rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/torch_helper.py
--rw-rw-rw-   0        0        0     1044 2023-04-19 16:11:46.000000 goodai-ltm-0.0.4/goodai/ltm/matching.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.988550 goodai-ltm-0.0.4/goodai/ltm/matching_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/__init__.py
--rw-rw-rw-   0        0        0      187 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/auto.py
--rw-rw-rw-   0        0        0    10023 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/default.py
--rw-rw-rw-   0        0        0      623 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/prob_model.py
--rw-rw-rw-   0        0        0     1144 2023-04-19 16:12:29.000000 goodai-ltm-0.0.4/goodai/ltm/memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.997990 goodai-ltm-0.0.4/goodai/ltm/memory_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/auto.py
--rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk.py
--rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_mixin.py
--rw-rw-rw-   0        0        0    10289 2023-04-19 18:19:26.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_queue.py
--rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/config.py
--rw-rw-rw-   0        0        0     5566 2023-04-19 18:20:54.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/default.py
--rw-rw-rw-   0        0        0     5723 2023-04-19 18:18:01.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/mem_foundation.py
--rw-rw-rw-   0        0        0     2896 2023-04-19 18:16:19.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.000988 goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/
--rw-rw-rw-   0        0        0     3101 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/TestChunkQueue.py
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.001987 goodai-ltm-0.0.4/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.003989 goodai-ltm-0.0.4/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/training/query_passage/trainer.py
--rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/training/sched_opt.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.008988 goodai-ltm-0.0.4/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0      184 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2225 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 18:51:42.009989 goodai-ltm-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-04-19 18:51:37.000000 goodai-ltm-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.141632 goodai-ltm-0.0.5/
+-rw-rw-rw-   0        0        0      184 2023-04-20 20:20:40.141632 goodai-ltm-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-04-19 21:51:49.000000 goodai-ltm-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.037632 goodai-ltm-0.0.5/goodai/
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.055631 goodai-ltm-0.0.5/goodai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/collections_helper.py
+-rw-rw-rw-   0        0        0      717 2023-04-19 20:33:13.000000 goodai-ltm-0.0.5/goodai/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.060632 goodai-ltm-0.0.5/goodai/ltm/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.063631 goodai-ltm-0.0.5/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.064632 goodai-ltm-0.0.5/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     1996 2023-04-19 22:25:12.000000 goodai-ltm-0.0.5/goodai/ltm/data/names/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.075632 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      485 2023-04-20 19:49:15.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     2422 2023-04-19 22:26:45.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      331 2023-04-20 19:47:41.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    11044 2023-04-20 19:51:43.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1857 2023-04-19 22:30:12.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa_tok_entry.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.077631 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     2527 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
+-rw-rw-rw-   0        0        0     6936 2023-04-20 19:54:07.000000 goodai-ltm-0.0.5/goodai/ltm/data/query_passage/wiki.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.090632 goodai-ltm-0.0.5/goodai/ltm/embedding_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/auto.py
+-rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5366 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/default.py
+-rw-rw-rw-   0        0        0     1533 2023-04-19 16:47:45.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     2785 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/openai_emb.py
+-rw-rw-rw-   0        0        0     2224 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/st_emb.py
+-rw-rw-rw-   0        0        0     5440 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embedding_models/trainable.py
+-rw-rw-rw-   0        0        0     1584 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/embeddings.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.100632 goodai-ltm-0.0.5/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/eval/auto.py
+-rw-rw-rw-   0        0        0     4450 2023-04-20 19:42:22.000000 goodai-ltm-0.0.5/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     2716 2023-04-19 23:22:15.000000 goodai-ltm-0.0.5/goodai/ltm/eval/metrics.py
+-rw-rw-rw-   0        0        0     1901 2023-04-19 23:26:29.000000 goodai-ltm-0.0.5/goodai/ltm/eval/qrecc.py
+-rw-rw-rw-   0        0        0     2072 2023-04-20 20:01:17.000000 goodai-ltm-0.0.5/goodai/ltm/eval/strategy_qa.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.102631 goodai-ltm-0.0.5/goodai/ltm/eval/tests/
+-rw-rw-rw-   0        0        0     1420 2023-04-19 23:22:33.000000 goodai-ltm-0.0.5/goodai/ltm/eval/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     1188 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/matching.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.110633 goodai-ltm-0.0.5/goodai/ltm/matching_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/auto.py
+-rw-rw-rw-   0        0        0    10019 2023-04-19 22:29:29.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/default.py
+-rw-rw-rw-   0        0        0      706 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/prob_model.py
+-rw-rw-rw-   0        0        0      658 2023-04-19 21:49:37.000000 goodai-ltm-0.0.5/goodai/ltm/matching_models/st_ce.py
+-rw-rw-rw-   0        0        0     1208 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.126632 goodai-ltm-0.0.5/goodai/ltm/memory_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/auto.py
+-rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk.py
+-rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_mixin.py
+-rw-rw-rw-   0        0        0    10364 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_queue.py
+-rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/config.py
+-rw-rw-rw-   0        0        0     5562 2023-04-19 22:25:35.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/default.py
+-rw-rw-rw-   0        0        0     5784 2023-04-19 22:27:29.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/mem_foundation.py
+-rw-rw-rw-   0        0        0     2960 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.128631 goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/__init__.py
+-rw-rw-rw-   0        0        0     3101 2023-04-20 15:19:11.000000 goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/test_chunk_queue.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.131636 goodai-ltm-0.0.5/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.134632 goodai-ltm-0.0.5/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.5/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.5/goodai/ltm/training/query_passage/trainer.py
+-rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.5/goodai/ltm/training/sched_opt.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:20:40.140632 goodai-ltm-0.0.5/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2357 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 20:20:39.000000 goodai-ltm-0.0.5/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:20:40.141632 goodai-ltm-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-04-20 19:37:55.000000 goodai-ltm-0.0.5/setup.py
```

### Comparing `goodai-ltm-0.0.4/README.md` & `goodai-ltm-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ## Installation
 
     pip install goodai-ltm
 
 ## Quick start
 
+    from goodai.ltm.memory_models.auto import AutoTextMemory
+
     mem = AutoTextMemory.create()
     mem.add_text("Lorem ipsum dolor sit amet, consectetur adipiscing elit\n")
     mem.add_text("Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore\n",
                  metadata={'timestamp': '2023-04-19', 'type': 'generic'})
     r_memories = mem.retrieve(query='dolorem eum fugiat quo voluptas nulla pariatur?', k=3)
     for r_mem in r_memories:
         print(r_mem)
@@ -36,17 +38,17 @@
 
 ## Loading a query-passage matching model
 
 Recommended:
 
     tmm = AutoTextMatchingModel.from_pretrained('default')
 
-Huggingface reranking cross-encoders:
+Huggingface reranking cross-encoders from the sentence-transformers library:
 
-    tmm = AutoTextMatchingModel.from_pretrained('ce:cross-encoder/mmarco-mMiniLMv2-L12-H384-v1')
+    tmm = AutoTextMatchingModel.from_pretrained('st:cross-encoder/mmarco-mMiniLMv2-L12-H384-v1')
 
 ## Query-passage matching model usage
 
 ## Loading a text memory instance:
 
 Recommended:
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/cloud.py` & `goodai-ltm-0.0.5/goodai/ltm/data/cloud.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.0.5/goodai/ltm/data/names/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import List
 
 import numpy as np
 
-from goodai.ltm.helpers.json_helper import load_json
+from goodai.helpers.json_helper import load_json
 
 _instance_attr = '__instance'
 _names_dir = os.path.join(os.path.dirname(__file__))
 _names_path = os.path.join(_names_dir, 'wikidata-names.json')
 
 
 class NameSource:
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/auto_data_source.py` & `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/auto_data_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from goodai.ltm.data.query_passage.qa import QAQueryPassageDataSource
 
 from goodai.ltm.data.query_passage.data_source import BaseQueryPassageDataSource
 from transformers import PreTrainedTokenizer
 
 
 class AutoQueryPassageDataSource:
+    """
+    Factory class for training and evaluation data sources for query-passage matching.
+    """
+
     def __init__(self):
         pass
 
     @staticmethod
     def create(name: str, random: np.random.RandomState, tokenizer: PreTrainedTokenizer,
                max_query_tokens=40, min_passage_tokens=24,
                max_passage_tokens=36) -> Tuple[BaseQueryPassageDataSource, BaseQueryPassageDataSource]:
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
+
+from goodai.helpers.tokenizer_helper import get_model_inputs
 from goodai.ltm.data.query_passage.data_source import BaseQueryPassageDataSource
 from torch.utils.data import Dataset
 from typing import List, Tuple
 from transformers import PreTrainedTokenizer
 
-from goodai.ltm.helpers.tokenizer_helper import get_model_inputs
-
 
 class QueryPassageDataset(Dataset):
     def __init__(
         self,
         data_sources: List[Tuple[BaseQueryPassageDataSource, float]],
         tokenizer: PreTrainedTokenizer,
         num_examples: int,
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 from typing import List, Dict, Tuple, Iterable
 
 import numpy as np
 from datasets import load_dataset, DatasetDict, Dataset
+
+from goodai.helpers.tokenizer_helper import get_sentence_punctuation_ids
 from goodai.ltm.data.query_passage.example import QueryPassageExample
 from transformers import PreTrainedTokenizer
 
 from goodai.ltm.data.names import NameSource
 from goodai.ltm.data.query_passage.data_source import BaseQueryPassageDataSource
 from goodai.ltm.data.query_passage.qa_tok_entry import QATokenizedEntry
-from goodai.ltm.helpers.tokenizer_helper import get_sentence_punctuation_ids
 
 
 class QAQueryPassageDataSource(BaseQueryPassageDataSource):
     def __init__(self, random: np.random.RandomState, tokenizer: PreTrainedTokenizer,
                  qa_examples: List[dict],
                  max_query_tokens: int, min_passage_tokens: int, max_passage_tokens: int,
                  min_query_tokens=6, min_answer_start_leeway: int = 16, answer_leeway_min_tokens: int = 32):
@@ -187,25 +188,24 @@
             passage_start = r.randint(0, p_to)
         passage_end = passage_start + num_tokens
         result = context_ids[passage_start:passage_end]
         if len(result) < self.min_passage_tokens:
             return None
         return result
 
-    def sample_item(self, use_different_p=0.5) -> QueryPassageExample:
+    def sample_item(self, is_match: bool, use_different_p=0.5) -> QueryPassageExample:
         r = self.random
         n = len(self.qa_examples)
         for attempt in range(100):
             pos_index = r.randint(0, n)
             pos_tok_entry = self.get_tokenization(pos_index)
             if pos_tok_entry.answer_seq_index == -1:
                 logging.warning(f'Did not find location of answer excerpt in example with id {pos_tok_entry.e_id}')
                 continue
             query_token_ids, nqn = self.get_query_token_ids(pos_tok_entry)
-            is_match = r.choice([True, False])
             if is_match:
                 passage_tok_entry = pos_tok_entry
                 non_answer = False
             else:
                 use_different = r.uniform() < use_different_p
                 if use_different:
                     neg_index = r.randint(0, n)
@@ -218,9 +218,11 @@
             passage_token_ids = self.get_passage_token_ids(passage_tok_entry, is_match, non_answer, nqn)
             if passage_token_ids is None:
                 continue
             return QueryPassageExample(query_token_ids, passage_token_ids, is_match)
 
         raise SystemError('Unable to find suitable qa_example!')
 
-    def sample_items(self, count: int) -> List[QueryPassageExample]:
-        return [self.sample_item() for _ in range(count)]
+    def sample_items(self, count: int, approx_positive_fraction: float = 0.5) -> List[QueryPassageExample]:
+        rnd_samples = self.random.uniform(size=count)
+        is_match = rnd_samples <= approx_positive_fraction
+        return [self.sample_item(is_match[i]) for i, _ in enumerate(range(count))]
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import List, Optional, Tuple
 from transformers import PreTrainedTokenizer
 
-from goodai.ltm.helpers.tokenizer_helper import get_token_index
+from goodai.helpers.tokenizer_helper import get_token_index
 
 
 @dataclass
 class QATokenizedEntry:
     ds_name: str
     e_id: str
     context: str
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py` & `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 import os
 import unittest
 from pathlib import Path
 from goodai.ltm.data.query_passage.auto_data_source import AutoQueryPassageDataSource
 from transformers import PreTrainedTokenizer, AutoTokenizer
 import numpy as np
-from goodai.ltm.helpers.html_helper import text_to_html
+from goodai.helpers.html_helper import text_to_html
 
 
 class TestQueryPassageDataSource(unittest.TestCase):
     def test_show_examples(self):
         tokenizer: PreTrainedTokenizer = AutoTokenizer.from_pretrained('distilroberta-base')
         random = np.random.RandomState(1)
         ds_names = ['adversarial_qa', 'coqa', 'squad_v2']
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.0.5/goodai/ltm/data/query_passage/wiki.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from typing import List, Optional, Any, Dict, Tuple
 
 import numpy as np
 from transformers import PreTrainedTokenizer
 
 from goodai.ltm.data.query_passage.data_source import BaseQueryPassageDataSource
+from goodai.ltm.data.query_passage.example import QueryPassageExample
 
 
 class WikiQueryPassageDataSource(BaseQueryPassageDataSource):
     def __init__(self, random: np.random.RandomState, tokenizer: PreTrainedTokenizer, articles: List[Any],
                  max_query_tokens: int, min_passage_tokens: int, max_passage_tokens: int,
                  gap_leeway=12, min_query_tokens=16):
         super().__init__()
@@ -100,25 +101,25 @@
         neg_par_token_ids = self.neg_article_token_ids[neg_par_id]
         flex = len(neg_par_token_ids) - num_passage_tokens
         passage_start = r.randint(0, flex + 1)
         passage_end = passage_start + num_passage_tokens
         passage_ids = neg_par_token_ids[passage_start:passage_end]
         return passage_ids
 
-    def sample_items(self, count: int) -> List[QueryPassageExample]:
+    def sample_items(self, count: int, approx_positive_fraction: float = 0.5) -> List[QueryPassageExample]:
         r = self.random
         result = []
         for i in range(count):
             if self.is_new_article_needed():
                 self.init_current_article()
             par_token_ids = self.pos_article_token_ids[self.current_par_idx]
             num_query_tokens = r.randint(self.min_query_tokens, self.max_query_tokens + 1)
             num_gap_tokens = r.randint(0, self.gap_leeway + 1)
             num_passage_tokens = r.randint(self.min_passage_tokens, self.max_passage_tokens + 1)
-            is_match = r.choice([True, False])
+            is_match = self.random.uniform() <= approx_positive_fraction
             if is_match:
                 total_tokens = num_query_tokens + num_gap_tokens + num_passage_tokens
             else:
                 total_tokens = num_query_tokens
             flex = len(par_token_ids) - total_tokens
             start = r.randint(0, flex + 1)
             query_end = start + num_query_tokens
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embedding_models/contrast_classifier.py` & `goodai-ltm-0.0.5/goodai/ltm/embedding_models/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embedding_models/default.py` & `goodai-ltm-0.0.5/goodai/ltm/embedding_models/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 from transformers import PreTrainedModel, PreTrainedTokenizer, PretrainedConfig
 from transformers.modeling_outputs import BaseModelOutput
+
+from goodai.helpers.tokenizer_helper import get_attention_after_token
 from goodai.ltm.embedding_models.trainable import TrainableEmbeddingModel
-from goodai.ltm.helpers.tokenizer_helper import get_attention_after_token
 
 
 class DefaultEmbeddingModel(TrainableEmbeddingModel):
+    """
+    Default implementation of trainable text embeddings.
+    """
+
     def __init__(self, lang_model: PreTrainedModel, tokenizer: PreTrainedTokenizer,
                  num_retrieval_emb: int, num_storage_emb: int,
                  num_end_chars_lb_ignore=18):
         super(DefaultEmbeddingModel, self).__init__(tokenizer)
         lb_token_ids = tokenizer.encode('\n', add_special_tokens=False)
         if len(lb_token_ids) != 1:
             raise ValueError(f'Tokenizer {tokenizer.name_or_path} does not have a line break token!')
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embedding_models/emb_qp_prob_model.py` & `goodai-ltm-0.0.5/goodai/ltm/embedding_models/emb_qp_prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embedding_models/openai_emb.py` & `goodai-ltm-0.0.5/goodai/ltm/embedding_models/openai_emb.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 from goodai.ltm.embeddings import BaseTextEmbeddingModel
 
 _openai_lock = threading.Lock()
 
 
 class OpenAIEmbeddingModel(BaseTextEmbeddingModel):
+    """
+    Text embedding model based on OpenAI text embeddings.
+
+    https://platform.openai.com/docs/guides/embeddings
+    """
+
     def __init__(self, api_key: str = None, model_name: str = 'text-embedding-ada-002', emb_dim: int = 1536):
         self.api_key = api_key
         self.emb_dim = emb_dim
         self.model_name = model_name
 
     def get_embedding_dim(self) -> int:
         return self.emb_dim
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embedding_models/st_emb.py` & `goodai-ltm-0.0.5/goodai/ltm/embedding_models/st_emb.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from sentence_transformers import SentenceTransformer
 from goodai.ltm.embeddings import BaseTextEmbeddingModel
 
 _openai_lock = threading.Lock()
 
 
 class SentenceTransformerEmbeddingModel(BaseTextEmbeddingModel):
+    """
+    Text embedding model based on Hugging Face Sentence Transformers.
+
+    https://huggingface.co/sentence-transformers
+    """
+
     def __init__(self, model_name: str):
         self.st = SentenceTransformer(model_name)
 
     def get_embedding_dim(self) -> int:
         return self.st.get_sentence_embedding_dimension()
 
     def get_num_retrieval_embeddings(self) -> int:
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embedding_models/trainable.py` & `goodai-ltm-0.0.5/goodai/ltm/embedding_models/trainable.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 
 import numpy as np
 import torch
 from torch import nn
 from tqdm import tqdm
 from transformers import PreTrainedTokenizer
 
+from goodai.helpers.tokenizer_helper import get_pad_token_id, get_model_inputs
 from goodai.ltm.embeddings import BaseTextEmbeddingModel
-from goodai.ltm.helpers.tokenizer_helper import get_model_inputs, get_pad_token_id
 
 
 class TrainableEmbeddingModel(BaseTextEmbeddingModel, nn.Module):
+    """
+    Abstract base class for locally trainable text embeddings.
+
+    Trainable embedding models support multiple retrieval and storage embeddings for a query or passage.
+    """
+
     def __init__(self, tokenizer: PreTrainedTokenizer):
         super(BaseTextEmbeddingModel, self).__init__()
         super(nn.Module, self).__init__()
         self.dummy = nn.Parameter()
         self.tokenizer = tokenizer
         self.pad_token_id = get_pad_token_id(tokenizer)
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/embeddings.py` & `goodai-ltm-0.0.5/goodai/ltm/embeddings.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 from typing import List, Union
 
 import numpy as np
 import torch
 
 
 class BaseTextEmbeddingModel(ABC):
+    """
+    Abstract base class for text embedding models.
+
+    The interface allows different embeddings for queries (retrieval embeddings) and passages
+    (storage embeddings) as well as multiple retrieval and storage embeddings for a query or passage.
+    """
+
     @abstractmethod
     def get_embedding_dim(self) -> int:
         """
         :return: The number of dimensions of embedding vectors.
         """
         pass
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/eval/mem.py` & `goodai-ltm-0.0.5/goodai/ltm/eval/mem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import abc
 from abc import ABC
+from dataclasses import dataclass
 from typing import List, Dict, Tuple
 
 import numpy as np
 from tqdm import tqdm
 from transformers import PreTrainedTokenizer
 
 from goodai.ltm.data.names import NameSource
 from goodai.ltm.eval.metrics import get_correctness_score
 from goodai.ltm.memory import BaseTextMemory
 
 
+@dataclass
 class QAScenario:
     context: List[str]
     supportingFacts: List[str]
     question: str
 
 
 class BaseMemEvaluator(ABC):
+    """
+    Abstract base class for text memory model evaluators.
+    """
+
     def __init__(self, tokenizer: PreTrainedTokenizer, top_ks: List[int],
                  max_query_tokens: int, has_query_noise: bool,
-                 add_names_to_context: bool = True, correctness_threshold=80):
+                 add_names_to_context: bool = True, correctness_threshold=70):
         if len(top_ks) == 0:
             raise ValueError('At least one top-k must be provided')
         self.top_ks = top_ks
         self.correctness_threshold = correctness_threshold
         self.tokenizer = tokenizer
         self.max_query_tokens = max_query_tokens
         self.has_query_noise = has_query_noise
@@ -44,28 +50,35 @@
         name1, name2 = tuple(NameSource.get_instance().sample_first_names(self.rnd1, count=2))
         names = [name1, name2]
         names_context = [f'{names[i % 2]}: {ctx}' for i, ctx in enumerate(scenario.context)]
         c_len = len(names_context)
         q_name = names[c_len % 2]
         a_name = names[(c_len + 1) % 2]
         query = f'{q_name}: {scenario.question}\n{a_name}:'
+        truncate_q_ids_at = self.max_query_tokens
         if self.has_query_noise:
+            no_noise_ids = self.tokenizer.encode(query, add_special_tokens=False)
+            len_nni = len(no_noise_ids)
+            if len_nni < self.max_query_tokens:
+                truncate_q_ids_at = self.rnd2.randint(max(1, len_nni), self.max_query_tokens + 1)
             context_as_text = '\n'.join(names_context[-3:])
             query = context_as_text + '\n' + query
-        plain_query_token_ids = self.tokenizer.encode(query, add_special_tokens=False)
-        plain_query_token_ids = plain_query_token_ids[-self.max_query_tokens:]
-        return self.tokenizer.decode(plain_query_token_ids, skip_special_tokens=True)
-
-    def get_queries_and_support(self, scenarios: List[QAScenario]) -> List[Tuple[str, List[str]]]:
-        result = []
+        query_token_ids = self.tokenizer.encode(query, add_special_tokens=False)
+        query_token_ids = query_token_ids[-truncate_q_ids_at:]
+        return self.tokenizer.decode(query_token_ids, skip_special_tokens=True)
+
+    def get_queries_and_support(self, scenarios: List[QAScenario]) -> Tuple[List[str], List[List[str]]]:
+        queries = []
+        supports_list: List[List[str]] = []
         for scenario in scenarios:
             query = self.get_query(scenario)
             support = scenario.supportingFacts
-            result.append((query, support))
-        return result
+            queries.append(query)
+            supports_list.append(support)
+        return queries, supports_list,
 
     def cross_max_correctness(self, retrieved_texts: List[str], supporting_facts: List[str]):
         result = []
         for rt in retrieved_texts:
             scores = [get_correctness_score(self.tokenizer, rt, f) for f in supporting_facts]
             result.append(max(scores))
         return result
@@ -83,8 +96,8 @@
             s_retrieved_texts = [r.passage for r in s_retrieved]
             correctness_values = self.cross_max_correctness(s_retrieved_texts, s_supports)
             for top_k in self.top_ks:
                 selected_cv = correctness_values[:top_k]
                 if max(selected_cv) >= self.correctness_threshold:
                     top_k_map[top_k] = top_k_map.get(top_k, 0) + 1
         item_count = len(retrieved)
-        return {f'MR@{top_k}': v / item_count for top_k, v in top_k_map.items()}
+        return {f'ACC@{top_k}': v / item_count for top_k, v in top_k_map.items()}
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.0.5/goodai/ltm/eval/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,39 +28,37 @@
 def get_correctness_score(tokenizer: PreTrainedTokenizer, predicted_answer: str, expected_answer: str):
     predicted_raw_tokens = tokenizer.tokenize(' ' + predicted_answer, add_special_tokens=False)
     return _get_correctness_score_for_tokens_ea(tokenizer, predicted_raw_tokens, expected_answer)
 
 
 def _get_correctness_score_for_tokens_ea(tokenizer: PreTrainedTokenizer, predicted_raw_tokens: List[str],
                                          expected_answer: str):
-    expected_raw_tokens_1 = tokenizer.tokenize(' ' + expected_answer.lower(), add_special_tokens=False)
     expected_raw_tokens_2 = tokenizer.tokenize(' ' + expected_answer, add_special_tokens=False)
-    correctness_1 = _get_correctness_score_for_tokens(predicted_raw_tokens, expected_raw_tokens_1)
     correctness_2 = _get_correctness_score_for_tokens(predicted_raw_tokens, expected_raw_tokens_2)
-    correctness = max(correctness_1, correctness_2)
-    return correctness
+    return correctness_2
 
 
 def _get_correctness_score_for_tokens(predicted_raw_tokens: List[str], expected_raw_tokens: List[str]):
     predicted_tokens = _norm_tokens(predicted_raw_tokens)
     expected_tokens = _norm_tokens(expected_raw_tokens)
     if len(expected_tokens) == 0:
         return 0.0
     else:
         s_distance = _subseq_distance(predicted_tokens, expected_tokens)
         max_distance = len(expected_tokens)
         return 100.0 * (1 - s_distance / max_distance)
 
 
 def _subseq_distance(s_pred: List[str], t_exp: List[str]):
-    # TODO subsequences of length at least len(t_exp)
-    pred_subseqs = [s_pred[i: j] for i in range(len(s_pred))
-                    for j in range(i + 1, len(s_pred) + 1)]
-    if len(pred_subseqs) == 0:
-        pred_subseqs = [[]]
+    min_s_len = len(t_exp)
+    i_max = len(s_pred) - min_s_len
+    if i_max <= 0:
+        pred_subseqs = [s_pred]
+    else:
+        pred_subseqs = [s_pred[i:i + min_s_len] for i in range(i_max + 1)]
     distances = [levenshtein_distance(s, t_exp) for s in pred_subseqs]
     return min(distances)
 
 
 def _norm_token(token: str):
     if token.startswith('Ġ'):
         token = token[1:]
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/helpers/collections_helper.py` & `goodai-ltm-0.0.5/goodai/helpers/collections_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/helpers/tokenizer_helper.py` & `goodai-ltm-0.0.5/goodai/helpers/tokenizer_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/matching.py` & `goodai-ltm-0.0.5/goodai/ltm/matching.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 
 class BaseTextMatchingModel(ABC):
+    """
+    Abstract base class for text matching models.
+
+    A matching model measures the match between queries and passages.
+    """
+
     def get_match_confidence(self, query: str, passages: List[str], batch_size: int = 32,
                              show_progress_bar: bool = False) -> List[float]:
         """
         :param query: A string representing a query.
         :param passages: A list of strings representing passages that should be matched with the provided query.
         :param show_progress_bar: Whether a progress bar should be shown.
         :param batch_size: The inference batch size.
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/matching_models/default.py` & `goodai-ltm-0.0.5/goodai/ltm/matching_models/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import torch
 from torch import nn
 import torch.nn.functional as F
 from tqdm import tqdm
 from transformers import AutoModel, AutoTokenizer, PreTrainedTokenizer
 from typing import List, Optional, Tuple
 
+from goodai.helpers.tokenizer_helper import get_attention_after_token, get_model_inputs
 from goodai.ltm.embedding_models.contrast_classifier import ContrastClassifier
-from goodai.ltm.helpers.tokenizer_helper import get_attention_after_token, get_model_inputs
 from goodai.ltm.matching import BaseTextMatchingModel
 from goodai.ltm.matching_models.prob_model import BaseQueryPassageProbModel
 
 
 class DefaultRerankingCrossEncoder(nn.Module, BaseQueryPassageProbModel, BaseTextMatchingModel):
     sep_id_tensor: torch.Tensor
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/matching_models/prob_model.py` & `goodai-ltm-0.0.5/goodai/ltm/matching_models/prob_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from abc import ABC, abstractmethod
 
 import torch
 from torch import nn
 
 
 class BaseQueryPassageProbModel(ABC):
+    """
+    Abstract base class for query-passage probability models.
+    """
+
     @abstractmethod
     def forward(self, query_input_ids: torch.Tensor, query_attention_mask: torch.Tensor,
                 query_token_lengths: torch.Tensor,
                 passage_input_ids: torch.Tensor, passage_attention_mask: torch.Tensor) -> torch.Tensor:
         pass
 
     @abstractmethod
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory.py` & `goodai-ltm-0.0.5/goodai/ltm/memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     metadata: Any
     """
     Metadata associated with the retrieved text
     """
 
 
 class BaseTextMemory(ABC):
+    """
+    Abstract base class for text memories.
+    """
+
     @abstractmethod
     def add_text(self, text: str, metadata: Optional[Any] = None):
         pass
 
     @abstractmethod
     def retrieve_multiple(self, queries: List[str], k: int, show_progress_bar: bool = False,
                           **kwargs) -> List[List[RetrievedMemory]]:
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/auto.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from goodai.ltm.memory import BaseTextMemory
 from goodai.ltm.memory_models.config import TextMemoryConfig
 from goodai.ltm.memory_models.default import DefaultTextMemory
 from goodai.ltm.memory_models.simple_vector_db import SimpleVectorDb
 
 
 class AutoTextMemory:
+    """
+    Factory class for text memory.
+    """
+
     @staticmethod
     def create(**kwargs) -> BaseTextMemory:
         new_kwargs = dict(kwargs)
         if 'vector_db' not in new_kwargs:
             new_kwargs['vector_db'] = SimpleVectorDb()
         if 'tokenizer' not in new_kwargs:
             new_kwargs['tokenizer'] = AutoTokenizer.from_pretrained('sentence-transformers/all-distilroberta-v1')
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_mixin.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_mixin.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_queue.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/chunk_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from typing import List, Tuple, Set, Dict, Optional, Any
 
 from goodai.ltm.memory_models.chunk import Chunk
 from goodai.ltm.memory_models.chunk_mixin import ChunkMixin
 
 
 class BaseChunkQueue(ABC):
+    """
+    Abstract base class for text memory chunk queues.
+    """
+
     def __init__(self):
         super().__init__()
 
     @abstractmethod
     def get_capacity(self) -> int:
         pass
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/default.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import gc
 from typing import List, Union, Any, Callable, Set, Optional
 import numpy as np
 import torch
 from faiss import Index
 from transformers import PreTrainedTokenizer
 
+from goodai.helpers.tokenizer_helper import get_pad_token_id, get_sentence_punctuation_ids
 from goodai.ltm.embeddings import BaseTextEmbeddingModel
-from goodai.ltm.helpers.tokenizer_helper import get_sentence_punctuation_ids, get_pad_token_id
 from goodai.ltm.matching import BaseTextMatchingModel
 from goodai.ltm.memory_models.chunk_queue import ChunkQueue, BaseChunkQueue
 from goodai.ltm.memory_models.config import TextMemoryConfig
 from goodai.ltm.memory_models.mem_foundation import BaseTextMemoryFoundation
 from goodai.ltm.memory_models.simple_vector_db import SimpleVectorDb
 
 _vector_db_type = Union[Index, SimpleVectorDb]
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/mem_foundation.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/mem_foundation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import faiss
 import numpy as np
 import torch
 from tqdm import tqdm
 from transformers import PreTrainedTokenizer
 
-from goodai.ltm.helpers.collections_helper import remove_duplicates, num_visited_to_get_expected_count, \
+from goodai.helpers.collections_helper import remove_duplicates, num_visited_to_get_expected_count, \
     get_non_adjacent
-from goodai.ltm.helpers.tokenizer_helper import get_sentence_punctuation_ids
+from goodai.helpers.tokenizer_helper import get_sentence_punctuation_ids
 from goodai.ltm.memory import BaseTextMemory, RetrievedMemory
 from goodai.ltm.memory_models.simple_vector_db import SimpleVectorDb
 
 _vector_db_type = Union[faiss.Index, SimpleVectorDb]
 
 
 class BaseTextMemoryFoundation(BaseTextMemory):
@@ -100,14 +100,15 @@
         expected_key_db_top_k = k
         if self.has_match_prob_model:
             expected_key_db_top_k *= mm_multiplier
         downstream_top_k = expected_key_db_top_k * self.num_storage_embeddings
         if not adjacent_chunks_ok:
             downstream_top_k *= 3
         distances, indexes = self.vector_db.search(rk_np, k=downstream_top_k)
+        assert distances.shape[0] == indexes.shape[0] == batch_size
         result = []
         rng = range(batch_size)
         if show_progress_bar:
             rng = tqdm(rng, desc='Retrieval', unit='query')
         for i in rng:
             flat_distances = distances[i]
             flat_indexes = indexes[i]
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/simple_vector_db.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/simple_vector_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Optional, Tuple
 
 import numpy as np
 
 
 class SimpleVectorDb:
+    """
+    Simple vector database implementation.
+    """
+
     def __init__(self):
         super().__init__()
         self.all_vectors: Optional[np.ndarray] = None
         self.all_ids: Optional[np.ndarray] = None
 
     def search(self, vectors: np.ndarray, k: int = 1) -> Tuple[np.ndarray, np.ndarray]:
         batch_size = vectors.shape[0]
```

### Comparing `goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/TestChunkQueue.py` & `goodai-ltm-0.0.5/goodai/ltm/memory_models/tests/test_chunk_queue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/training/query_passage/trainer.py` & `goodai-ltm-0.0.5/goodai/ltm/training/query_passage/trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai/ltm/training/sched_opt.py` & `goodai-ltm-0.0.5/goodai/ltm/training/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.4/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.0.5/goodai_ltm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 README.md
 setup.py
+goodai/helpers/__init__.py
+goodai/helpers/collections_helper.py
+goodai/helpers/file_helper.py
+goodai/helpers/html_helper.py
+goodai/helpers/json_helper.py
+goodai/helpers/tokenizer_helper.py
+goodai/helpers/torch_helper.py
 goodai/ltm/__init__.py
 goodai/ltm/embeddings.py
 goodai/ltm/matching.py
 goodai/ltm/memory.py
 goodai/ltm/data/__init__.py
 goodai/ltm/data/cloud.py
 goodai/ltm/data/names/__init__.py
@@ -11,49 +18,47 @@
 goodai/ltm/data/query_passage/auto_data_source.py
 goodai/ltm/data/query_passage/data_source.py
 goodai/ltm/data/query_passage/dataset.py
 goodai/ltm/data/query_passage/example.py
 goodai/ltm/data/query_passage/qa.py
 goodai/ltm/data/query_passage/qa_tok_entry.py
 goodai/ltm/data/query_passage/wiki.py
-goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py
 goodai/ltm/data/query_passage/tests/__init__.py
+goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
 goodai/ltm/embedding_models/__init__.py
 goodai/ltm/embedding_models/auto.py
 goodai/ltm/embedding_models/contrast_classifier.py
 goodai/ltm/embedding_models/default.py
 goodai/ltm/embedding_models/emb_qp_prob_model.py
 goodai/ltm/embedding_models/openai_emb.py
 goodai/ltm/embedding_models/st_emb.py
 goodai/ltm/embedding_models/trainable.py
 goodai/ltm/eval/__init__.py
+goodai/ltm/eval/auto.py
 goodai/ltm/eval/mem.py
 goodai/ltm/eval/metrics.py
-goodai/ltm/helpers/__init__.py
-goodai/ltm/helpers/collections_helper.py
-goodai/ltm/helpers/file_helper.py
-goodai/ltm/helpers/html_helper.py
-goodai/ltm/helpers/json_helper.py
-goodai/ltm/helpers/tokenizer_helper.py
-goodai/ltm/helpers/torch_helper.py
+goodai/ltm/eval/qrecc.py
+goodai/ltm/eval/strategy_qa.py
+goodai/ltm/eval/tests/test_metrics.py
 goodai/ltm/matching_models/__init__.py
 goodai/ltm/matching_models/auto.py
 goodai/ltm/matching_models/default.py
 goodai/ltm/matching_models/prob_model.py
+goodai/ltm/matching_models/st_ce.py
 goodai/ltm/memory_models/__init__.py
 goodai/ltm/memory_models/auto.py
 goodai/ltm/memory_models/chunk.py
 goodai/ltm/memory_models/chunk_mixin.py
 goodai/ltm/memory_models/chunk_queue.py
 goodai/ltm/memory_models/config.py
 goodai/ltm/memory_models/default.py
 goodai/ltm/memory_models/mem_foundation.py
 goodai/ltm/memory_models/simple_vector_db.py
-goodai/ltm/memory_models/tests/TestChunkQueue.py
 goodai/ltm/memory_models/tests/__init__.py
+goodai/ltm/memory_models/tests/test_chunk_queue.py
 goodai/ltm/training/__init__.py
 goodai/ltm/training/sched_opt.py
 goodai/ltm/training/query_passage/__init__.py
 goodai/ltm/training/query_passage/trainer.py
 goodai_ltm.egg-info/PKG-INFO
 goodai_ltm.egg-info/SOURCES.txt
 goodai_ltm.egg-info/dependency_links.txt
```

### Comparing `goodai-ltm-0.0.4/setup.py` & `goodai-ltm-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 packages = find_namespace_packages(include=['goodai.*'])
 
 setup(name='goodai-ltm',
       description='A text memory meant to be used with conversational language models.',
       url='https://github.com/GoodAI/goodai-ltm',
-      version='0.0.4',
+      version='0.0.5',
       packages=packages,
       package_data={},
       install_requires=['torch>=1.8.0', 'pytest>=7.0.0', 'numpy>=1.19.0', 'transformers>=4.0.0',
                         'openai>=0.27.0', 'faiss-cpu', 'datasets', 'boto3', 'python-dotenv',
                         'sentence-transformers>=2.2.2']
 )
```

