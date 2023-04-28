# Comparing `tmp/PaPie-0.4.1.tar.gz` & `tmp/PaPie-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaPie-0.4.1.tar", last modified: Thu Apr 27 11:35:16 2023, max compression
+gzip compressed data, was "PaPie-0.4.2.tar", last modified: Fri Apr 28 09:58:06 2023, max compression
```

## Comparing `PaPie-0.4.1.tar` & `PaPie-0.4.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1075 2021-05-20 08:00:23.000000 PaPie-0.4.1/LICENSE
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       68 2021-05-20 08:00:23.000000 PaPie-0.4.1/MANIFEST.in
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    15798 2023-04-27 11:35:16.433087 PaPie-0.4.1/PKG-INFO
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/PaPie.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    15798 2023-04-27 11:35:16.000000 PaPie-0.4.1/PaPie.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1259 2023-04-27 11:35:16.000000 PaPie-0.4.1/PaPie.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-04-27 11:35:16.000000 PaPie-0.4.1/PaPie.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       51 2023-04-27 11:35:16.000000 PaPie-0.4.1/PaPie.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      180 2023-04-27 11:35:16.000000 PaPie-0.4.1/PaPie.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        9 2023-04-27 11:35:16.000000 PaPie-0.4.1/PaPie.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    15050 2021-05-20 08:00:23.000000 PaPie-0.4.1/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/pie/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       45 2023-04-27 09:43:29.000000 PaPie-0.4.1/pie/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       18 2023-04-27 11:35:16.000000 PaPie-0.4.1/pie/commit_build.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       92 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/constants.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/pie/data/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      181 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3316 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/base_reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4257 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/conll_reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    26303 2023-02-04 16:32:10.000000 PaPie-0.4.1/pie/data/dataset.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/pie/data/preprocessors/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/preprocessors/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      245 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/preprocessors/edit_tree_tuples.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4940 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/preprocessors/edit_trees.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4272 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/preprocessors/greedy_scripts.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3114 2023-04-27 09:43:29.000000 PaPie-0.4.1/pie/data/reader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5414 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/data/tabreader.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8278 2021-06-08 10:30:41.000000 PaPie-0.4.1/pie/default_settings.json
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2445 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/initialization.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/pie/models/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      378 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/models/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6377 2023-04-27 09:43:29.000000 PaPie-0.4.1/pie/models/attention.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7189 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/models/base_model.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4018 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/models/beam_search.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    20129 2023-04-27 09:43:29.000000 PaPie-0.4.1/pie/models/decoder.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8320 2021-06-08 10:30:37.000000 PaPie-0.4.1/pie/models/embedding.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2356 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/models/encoder.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      970 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/models/highway.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5655 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/models/lstm.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    14659 2023-02-04 16:32:10.000000 PaPie-0.4.1/pie/models/model.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    15725 2023-04-27 09:43:29.000000 PaPie-0.4.1/pie/models/scorer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4661 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/optimize.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    15014 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/pretrain_encoder.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/pie/scripts/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/scripts/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4738 2021-05-20 09:05:41.000000 PaPie-0.4.1/pie/scripts/evaluate.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5604 2021-05-20 09:05:41.000000 PaPie-0.4.1/pie/scripts/group.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      348 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/scripts/inspect_model.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1683 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/scripts/tag.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1782 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/scripts/tag_pipe.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7055 2023-04-27 11:34:03.000000 PaPie-0.4.1/pie/scripts/train.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4554 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/settings.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5987 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/tagger.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     9686 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/torch_utils.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    14611 2023-04-27 09:43:29.000000 PaPie-0.4.1/pie/trainer.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     7136 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/utils.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/pie/webapp/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4644 2021-05-20 08:00:23.000000 PaPie-0.4.1/pie/webapp/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      179 2023-04-27 09:43:29.000000 PaPie-0.4.1/requirements.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-04-27 11:35:16.433087 PaPie-0.4.1/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4634 2023-04-27 11:35:14.000000 PaPie-0.4.1/setup.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/test/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.1/test/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-27 11:35:16.433087 PaPie-0.4.1/test/data/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.1/test/data/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4876 2021-05-20 08:00:23.000000 PaPie-0.4.1/test/data/test_data.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5311 2021-05-20 08:00:23.000000 PaPie-0.4.1/test/data/test_tabreader.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.300379 PaPie-0.4.2/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1075 2021-05-20 08:00:23.000000 PaPie-0.4.2/LICENSE
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       68 2021-05-20 08:00:23.000000 PaPie-0.4.2/MANIFEST.in
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15798 2023-04-28 09:58:06.300379 PaPie-0.4.2/PKG-INFO
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.288378 PaPie-0.4.2/PaPie.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15798 2023-04-28 09:58:06.000000 PaPie-0.4.2/PaPie.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1259 2023-04-28 09:58:06.000000 PaPie-0.4.2/PaPie.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-04-28 09:58:06.000000 PaPie-0.4.2/PaPie.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       51 2023-04-28 09:58:06.000000 PaPie-0.4.2/PaPie.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      180 2023-04-28 09:58:06.000000 PaPie-0.4.2/PaPie.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        9 2023-04-28 09:58:06.000000 PaPie-0.4.2/PaPie.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15050 2021-05-20 08:00:23.000000 PaPie-0.4.2/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.288378 PaPie-0.4.2/pie/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       45 2023-04-27 09:43:29.000000 PaPie-0.4.2/pie/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       18 2023-04-28 09:58:06.000000 PaPie-0.4.2/pie/commit_build.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       92 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/constants.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.292379 PaPie-0.4.2/pie/data/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      181 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3316 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/base_reader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4257 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/conll_reader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    26303 2023-02-04 16:32:10.000000 PaPie-0.4.2/pie/data/dataset.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.292379 PaPie-0.4.2/pie/data/preprocessors/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/preprocessors/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      245 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/preprocessors/edit_tree_tuples.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4940 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/preprocessors/edit_trees.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4272 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/preprocessors/greedy_scripts.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3114 2023-04-27 09:43:29.000000 PaPie-0.4.2/pie/data/reader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5414 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/data/tabreader.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8278 2021-06-08 10:30:41.000000 PaPie-0.4.2/pie/default_settings.json
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2445 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/initialization.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.296379 PaPie-0.4.2/pie/models/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      378 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/models/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6377 2023-04-27 09:43:29.000000 PaPie-0.4.2/pie/models/attention.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     7189 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/models/base_model.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4018 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/models/beam_search.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    20129 2023-04-27 09:43:29.000000 PaPie-0.4.2/pie/models/decoder.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8320 2021-06-08 10:30:37.000000 PaPie-0.4.2/pie/models/embedding.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2356 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/models/encoder.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      970 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/models/highway.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5655 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/models/lstm.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    14659 2023-02-04 16:32:10.000000 PaPie-0.4.2/pie/models/model.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15899 2023-04-28 09:52:07.000000 PaPie-0.4.2/pie/models/scorer.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4661 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/optimize.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    15014 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/pretrain_encoder.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.296379 PaPie-0.4.2/pie/scripts/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/scripts/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4738 2021-05-20 09:05:41.000000 PaPie-0.4.2/pie/scripts/evaluate.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5604 2021-05-20 09:05:41.000000 PaPie-0.4.2/pie/scripts/group.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      348 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/scripts/inspect_model.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1683 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/scripts/tag.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1782 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/scripts/tag_pipe.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     7055 2023-04-27 11:34:03.000000 PaPie-0.4.2/pie/scripts/train.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4554 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/settings.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5987 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/tagger.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     9686 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/torch_utils.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    14611 2023-04-27 09:43:29.000000 PaPie-0.4.2/pie/trainer.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     7136 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/utils.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.296379 PaPie-0.4.2/pie/webapp/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4644 2021-05-20 08:00:23.000000 PaPie-0.4.2/pie/webapp/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      179 2023-04-27 09:43:29.000000 PaPie-0.4.2/requirements.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-04-28 09:58:06.300379 PaPie-0.4.2/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4634 2023-04-28 09:19:41.000000 PaPie-0.4.2/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.296379 PaPie-0.4.2/test/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.2/test/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 09:58:06.296379 PaPie-0.4.2/test/data/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-05-20 08:00:23.000000 PaPie-0.4.2/test/data/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4876 2021-05-20 08:00:23.000000 PaPie-0.4.2/test/data/test_data.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5311 2021-05-20 08:00:23.000000 PaPie-0.4.2/test/data/test_tabreader.py
```

### Comparing `PaPie-0.4.1/LICENSE` & `PaPie-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/PKG-INFO` & `PaPie-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaPie
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Framework for Joint Learning of Sequence Labeling Tasks, forked from Pie
 Home-page: https://github.com/lascivaroma/PaPie
 Author: Enrique Manjavacas; Mike Kestemont; Thibault Clerice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PaPie-0.4.1/PaPie.egg-info/PKG-INFO` & `PaPie-0.4.2/PaPie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaPie
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Framework for Joint Learning of Sequence Labeling Tasks, forked from Pie
 Home-page: https://github.com/lascivaroma/PaPie
 Author: Enrique Manjavacas; Mike Kestemont; Thibault Clerice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PaPie-0.4.1/PaPie.egg-info/SOURCES.txt` & `PaPie-0.4.2/PaPie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/README.md` & `PaPie-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/base_reader.py` & `PaPie-0.4.2/pie/data/base_reader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/conll_reader.py` & `PaPie-0.4.2/pie/data/conll_reader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/dataset.py` & `PaPie-0.4.2/pie/data/dataset.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/preprocessors/edit_trees.py` & `PaPie-0.4.2/pie/data/preprocessors/edit_trees.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/preprocessors/greedy_scripts.py` & `PaPie-0.4.2/pie/data/preprocessors/greedy_scripts.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/reader.py` & `PaPie-0.4.2/pie/data/reader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/data/tabreader.py` & `PaPie-0.4.2/pie/data/tabreader.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/default_settings.json` & `PaPie-0.4.2/pie/default_settings.json`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/initialization.py` & `PaPie-0.4.2/pie/initialization.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/attention.py` & `PaPie-0.4.2/pie/models/attention.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/base_model.py` & `PaPie-0.4.2/pie/models/base_model.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/beam_search.py` & `PaPie-0.4.2/pie/models/beam_search.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/decoder.py` & `PaPie-0.4.2/pie/models/decoder.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/embedding.py` & `PaPie-0.4.2/pie/models/embedding.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/encoder.py` & `PaPie-0.4.2/pie/models/encoder.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/highway.py` & `PaPie-0.4.2/pie/models/highway.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/lstm.py` & `PaPie-0.4.2/pie/models/lstm.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/model.py` & `PaPie-0.4.2/pie/models/model.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/models/scorer.py` & `PaPie-0.4.2/pie/models/scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 import yaml
 import difflib
 from termcolor import colored
 from terminaltables import github_table
 from collections import Counter, defaultdict
 
-from torchmetrics.functional import accuracy, precision, recall, f1_score
+from torchmetrics.functional import accuracy, precision, recall, f1_score, stat_scores
 import numpy as np
 import torch
 from pie import constants
 
 
 def format_score(score):
     return round(float(score), 4)
@@ -24,14 +24,15 @@
             self.toi.index(v)
             for v in array
         ], device="cpu")
 
     def decode(self, idx: int) -> str:
         return self.toi[idx]
 
+
 def precision_recall_fscore_support(
         preds: torch.Tensor,
         trues: torch.Tensor,
         average: Optional[str] = "micro",
         num_classes: int = -1
 ):
     p = precision(preds, trues, task="multiclass", average=average, num_classes=num_classes)
@@ -65,21 +66,25 @@
 
 def compute_scores(trues, preds):
 
     enc = _LocalEncoder(*trues, *preds)
     preds_array = enc.encode(preds)
     trues_array = enc.encode(trues)
     num_classes = len(enc.toi)
-    p, r, f1, s = precision_recall_fscore_support(preds_array, trues_array, num_classes=num_classes)
+
+    if num_classes == 0:
+        return {'accuracy': 1, 'precision': 1, 'recall': 1, 'support': 0, 'balanced-accuracy': 1, 'f1': 1}
+
+    p, r, f1, s = precision_recall_fscore_support(preds_array, trues_array, average="macro", num_classes=num_classes)
     b = format_score(recall(preds_array, trues_array, task="multiclass", average="macro", num_classes=num_classes))
     p = format_score(p)
     r = format_score(r)
     a = format_score(accuracy(preds_array, trues_array, task="multiclass", average="micro", num_classes=num_classes))
 
-    return {'accuracy': a, 'precision': p, 'recall': r, 'support': s,
+    return {'accuracy': a, 'precision': p, 'recall': r, 'support': len(trues),
             'balanced-accuracy': b, 'f1': format_score(f1)}
 
 
 class Scorer(object):
     """
     Accumulate predictions over batches and compute evaluation scores
     """
```

### Comparing `PaPie-0.4.1/pie/optimize.py` & `PaPie-0.4.2/pie/optimize.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/pretrain_encoder.py` & `PaPie-0.4.2/pie/pretrain_encoder.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/scripts/evaluate.py` & `PaPie-0.4.2/pie/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/scripts/group.py` & `PaPie-0.4.2/pie/scripts/group.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/scripts/tag.py` & `PaPie-0.4.2/pie/scripts/tag.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/scripts/tag_pipe.py` & `PaPie-0.4.2/pie/scripts/tag_pipe.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/scripts/train.py` & `PaPie-0.4.2/pie/scripts/train.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/settings.py` & `PaPie-0.4.2/pie/settings.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/tagger.py` & `PaPie-0.4.2/pie/tagger.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/torch_utils.py` & `PaPie-0.4.2/pie/torch_utils.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/trainer.py` & `PaPie-0.4.2/pie/trainer.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/utils.py` & `PaPie-0.4.2/pie/utils.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/pie/webapp/__init__.py` & `PaPie-0.4.2/pie/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/setup.py` & `PaPie-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'PaPie'
 DESCRIPTION = 'A Framework for Joint Learning of Sequence Labeling Tasks, forked from Pie'
 URL = 'https://github.com/lascivaroma/PaPie'
 AUTHOR = 'Enrique Manjavacas; Mike Kestemont; Thibault Clerice'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

### Comparing `PaPie-0.4.1/test/data/test_data.py` & `PaPie-0.4.2/test/data/test_data.py`

 * *Files identical despite different names*

### Comparing `PaPie-0.4.1/test/data/test_tabreader.py` & `PaPie-0.4.2/test/data/test_tabreader.py`

 * *Files identical despite different names*

