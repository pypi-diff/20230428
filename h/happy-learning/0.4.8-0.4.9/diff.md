# Comparing `tmp/happy_learning-0.4.8.tar.gz` & `tmp/happy_learning-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_learning-0.4.8.tar", last modified: Wed Apr 26 21:03:42 2023, max compression
+gzip compressed data, was "happy_learning-0.4.9.tar", last modified: Thu Apr 27 22:39:28 2023, max compression
```

## Comparing `happy_learning-0.4.8.tar` & `happy_learning-0.4.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.137548 happy_learning-0.4.8/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.4.8/LICENSE
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-26 21:03:42.137920 happy_learning-0.4.8/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.4.8/README.md
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.088538 happy_learning-0.4.8/happy_learning/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/__init__.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/arbitrary_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    26360 2023-04-16 23:16:10.000000 happy_learning-0.4.8/happy_learning/environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   350467 2023-04-24 16:52:19.000000 happy_learning-0.4.8/happy_learning/feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    47861 2023-04-26 16:11:34.000000 happy_learning-0.4.8/happy_learning/feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   137255 2023-04-25 10:59:35.000000 happy_learning-0.4.8/happy_learning/genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    74495 2023-04-16 17:16:09.000000 happy_learning-0.4.8/happy_learning/neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 17:16:33.000000 happy_learning-0.4.8/happy_learning/neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/self_taught_short_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   136214 2023-04-25 13:55:53.000000 happy_learning-0.4.8/happy_learning/swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    29520 2023-04-16 11:52:14.000000 happy_learning-0.4.8/happy_learning/text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/utils.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.096675 happy_learning-0.4.8/happy_learning.egg-info/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1745 2023-04-26 21:03:42.000000 happy_learning-0.4.8/happy_learning.egg-info/SOURCES.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/dependency_links.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      356 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/requires.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/top_level.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-04-26 21:03:42.139332 happy_learning-0.4.8/setup.cfg
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3650 2023-04-26 17:15:04.000000 happy_learning-0.4.8/setup.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.136320 happy_learning-0.4.8/test/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4869 2023-04-24 23:30:40.000000 happy_learning-0.4.8/test/test_data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    21152 2023-04-17 16:30:20.000000 happy_learning-0.4.8/test/test_deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3788 2023-04-17 00:38:08.000000 happy_learning-0.4.8/test/test_environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     5483 2023-04-17 00:42:31.000000 happy_learning-0.4.8/test/test_evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    39531 2023-04-24 17:12:05.000000 happy_learning-0.4.8/test/test_feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    17611 2023-04-17 21:02:23.000000 happy_learning-0.4.8/test/test_feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4758 2023-04-26 17:10:24.000000 happy_learning-0.4.8/test/test_feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34272 2023-04-24 23:19:19.000000 happy_learning-0.4.8/test/test_genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.4.8/test/test_neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.4.8/test/test_neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_self_taught_short_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34193 2023-04-26 17:28:30.000000 happy_learning-0.4.8/test/test_swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.230883 happy_learning-0.4.9/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.4.9/LICENSE
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-27 22:39:28.231241 happy_learning-0.4.9/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.4.9/README.md
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.121143 happy_learning-0.4.9/happy_learning/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/__init__.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/arbitrary_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    26360 2023-04-16 23:16:10.000000 happy_learning-0.4.9/happy_learning/environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   350467 2023-04-24 16:52:19.000000 happy_learning-0.4.9/happy_learning/feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    46706 2023-04-27 22:21:13.000000 happy_learning-0.4.9/happy_learning/feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   137255 2023-04-25 10:59:35.000000 happy_learning-0.4.9/happy_learning/genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    74495 2023-04-16 17:16:09.000000 happy_learning-0.4.9/happy_learning/neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 17:16:33.000000 happy_learning-0.4.9/happy_learning/neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/self_taught_short_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   136214 2023-04-25 13:55:53.000000 happy_learning-0.4.9/happy_learning/swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    29520 2023-04-16 11:52:14.000000 happy_learning-0.4.9/happy_learning/text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.128091 happy_learning-0.4.9/happy_learning.egg-info/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1745 2023-04-27 22:39:28.000000 happy_learning-0.4.9/happy_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      356 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/requires.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/top_level.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-04-27 22:39:28.232520 happy_learning-0.4.9/setup.cfg
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3650 2023-04-27 12:48:30.000000 happy_learning-0.4.9/setup.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.229786 happy_learning-0.4.9/test/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4869 2023-04-24 23:30:40.000000 happy_learning-0.4.9/test/test_data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    21152 2023-04-17 16:30:20.000000 happy_learning-0.4.9/test/test_deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3788 2023-04-17 00:38:08.000000 happy_learning-0.4.9/test/test_environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     5483 2023-04-17 00:42:31.000000 happy_learning-0.4.9/test/test_evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    39531 2023-04-24 17:12:05.000000 happy_learning-0.4.9/test/test_feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    17611 2023-04-17 21:02:23.000000 happy_learning-0.4.9/test/test_feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4739 2023-04-27 22:24:30.000000 happy_learning-0.4.9/test/test_feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34272 2023-04-24 23:19:19.000000 happy_learning-0.4.9/test/test_genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.4.9/test/test_neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.4.9/test/test_neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_self_taught_short_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34193 2023-04-26 17:28:30.000000 happy_learning-0.4.9/test/test_swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_utils.py
```

### Comparing `happy_learning-0.4.8/LICENSE` & `happy_learning-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/PKG-INFO` & `happy_learning-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_learning
-Version: 0.4.8
+Version: 0.4.9
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `happy_learning-0.4.8/README.md` & `happy_learning-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/arbitrary_modeling.py` & `happy_learning-0.4.9/happy_learning/arbitrary_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/chaid_decision_tree.py` & `happy_learning-0.4.9/happy_learning/chaid_decision_tree.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/data_miner.py` & `happy_learning-0.4.9/happy_learning/data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/deep_q_learning.py` & `happy_learning-0.4.9/happy_learning/deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/environment_modeling.py` & `happy_learning-0.4.9/happy_learning/environment_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/evaluate_machine_learning.py` & `happy_learning-0.4.9/happy_learning/evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/feature_engineer.py` & `happy_learning-0.4.9/happy_learning/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/feature_learning.py` & `happy_learning-0.4.9/happy_learning/feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/feature_selector.py` & `happy_learning-0.4.9/happy_learning/feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,23 @@
     """
     def __init__(self,
                  df: pd.DataFrame,
                  features: List[str],
                  target: str,
                  force_target_type: str = None,
                  model_name: str = 'cat',
+                 use_standard_params: bool = True,
+                 evolutionary_algorithm: str = 'ga',
                  init_pairs: int = 3,
                  init_games: int = 5,
                  increasing_pair_size_factor: float = 0.5,
                  games: int = 3,
                  penalty_factor: float = 0.1,
                  max_iter: int = 50,
                  max_players: int = -1,
-                 evolutionary_algorithm: str = 'ga',
-                 use_standard_params: bool = True,
-                 aggregate_feature_imp: Dict[str, dict] = None,
-                 visualize_all_scores: bool = True,
-                 visualize_variant_scores: bool = True,
-                 visualize_core_feature_scores: bool = True,
                  path: str = None,
                  mlflow_log: bool = True,
                  multi_threading: bool = False,
                  **kwargs
                  ):
         """
         :param df: Pandas or dask DataFrame
@@ -78,14 +74,22 @@
             Force specific target type
                 -> clf_multi: Multi-Classification
                 -> reg: Regression
 
         :param model_name: str
             Name of the model
 
+        :param use_standard_params: bool
+            Use standard model hyperparameter or evolve proper hyperparameter using an evolutionary algorithm
+
+        :param evolutionary_algorithm: str
+            Name of the reinforced evolutionary algorithm
+                -> ga: Genetic Algorithm
+                -> si: Swarm Intelligence
+
         :param init_pairs: int
             Number of players in each starting game of the tournament
 
         :param init_games: int
             Number of penalty games to qualify players for the tournament
 
         :param increasing_pair_size_factor: float
@@ -99,33 +103,14 @@
 
         :param max_iter: int
             Maximum number of steps of the tournament
 
         :param max_players: int
             Maximum number of features used for training machine learning model
 
-        :param evolutionary_algorithm: str
-            Name of the reinforced evolutionary algorithm
-                -> ga: Genetic Algorithm
-                -> si: Swarm Intelligence
-
-        :param aggregate_feature_imp: Dict[str, dict]
-            Name of the aggregation method and the feature names to aggregate
-                -> core: Aggregate feature importance score by each core (original) feature
-                -> level: Aggregate feature importance score by the processing level of each feature
-
-        :param visualize_all_scores: bool
-            Whether to visualize all feature importance scores or not
-
-        :param visualize_variant_scores: bool
-            Whether to visualize all variants of feature processing importance scores separately or not
-
-        :param visualize_core_feature_scores: bool
-            Whether to visualize summarized core feature importance scores or not
-
         :param path: str
             Path or directory to export visualization to
 
         :param mlflow_log: bool
             Track experiment results using mlflow
 
         :param multi_threading: bool
@@ -135,14 +120,16 @@
             Key-word arguments
         """
         self.df: pd.DataFrame = df
         self.target: str = target
         self.features: List[str] = features
         if self.target in self.features:
             del self.features[self.features.index(self.target)]
+        if len(self.features) < 2:
+            raise FeatureSelectorException(f'Number of features ({len(self.features)}) are too small')
         self.df = self.df[self.features + [self.target]]
         self.n_cases: int = self.df.shape[0]
         self.n_features: int = len(self.features)
         self.force_target_type: str = force_target_type
         if self.force_target_type is None:
             self.ml_type: str = HappyLearningUtils().get_ml_type(values=self.df[self.target].values) if kwargs.get('ml_type') is None else kwargs.get('ml_type')
         else:
@@ -176,18 +163,14 @@
         self.multi_threading: bool = multi_threading
         self.tournament: bool = False
         self.shapley_additive_explanation: dict = dict(sum={}, game={}, tournament={})
         self.model_name: str = model_name
         self.evolutionary_algorithm: str = evolutionary_algorithm
         self.imp_score: Dict[str, float] = {}
         self.use_standard_params: bool = use_standard_params
-        self.aggregate_feature_imp: Dict[str, dict] = aggregate_feature_imp
-        self.visualize_all_scores: bool = visualize_all_scores
-        self.visualize_variant_scores: bool = visualize_variant_scores
-        self.visualize_core_features_scores: bool = visualize_core_feature_scores
         self.path: str = path
         if self.path is not None:
             self.path = self.path.replace('\\', '/')
             if os.path.isfile(self.path):
                 self.path = self.path.replace(self.path.split('/')[-1], '')
             else:
                 if self.path.split('/')[-1] != '':
@@ -475,37 +458,55 @@
                 self.shapley_additive_explanation.update({'total': _shapley_values})
             if self.n_features <= (self.pair_size_factor * _permutation_space):
                 if i + 1 == self.max_iter:
                     break
 
     def select(self,
                imp_threshold: float = 0.01,
-               redundant_threshold: float = 0.02,
+               redundant_threshold: float = 0.01,
+               aggregate_feature_imp: Dict[str, dict] = None,
+               visualize_feature_importance: bool = True,
+               visualize_variant_scores: bool = True,
+               visualize_core_feature_scores: bool = True,
                visualize_game_stats: bool = True,
                plot_type: str = 'bar'
                ) -> dict:
         """
         Select most important features based on shapley values
 
         :param imp_threshold: float
-            Threshold of importance score
+            Threshold of importance score to exclude features during initial games of the feature tournament
 
         :param redundant_threshold: float
-            Threshold for defining redundant features in percent
+            Threshold for defining metric reduction to define redundant features
+
+        :param aggregate_feature_imp: Dict[str, dict]
+            Name of the aggregation method and the feature names to aggregate
+                -> core: Aggregate feature importance score by each core (original) feature
+                -> level: Aggregate feature importance score by the processing level of each feature
+
+        :param visualize_feature_importance: bool
+            Whether to visualize feature importance scores or not
+
+        :param visualize_variant_scores: bool
+            Whether to visualize all variants of feature processing importance scores separately or not
+
+        :param visualize_core_feature_scores: bool
+            Whether to visualize summarized core feature importance scores or not
 
         :param visualize_game_stats: bool
             Whether to visualize game statistics or not
 
         :param plot_type: str
             Name of the plot type
                 -> pie: Pie Chart
                 -> bar: Bar Chart
 
         :return dict
-            Redundant features, important features and reduction scores
+            Results of feature tournament like shapley values, redundant features, important features, reduction scores and evaluated metrics
         """
         self._play_tournament()
         _imp_plot: dict = {}
         _core_features: List[str] = []
         _processed_features: List[str] = []
         _imp_threshold: float = imp_threshold if (imp_threshold >= 0) and (imp_threshold <= 1) else 0.7
         _df: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation.get('total'), index=['score']).transpose()
@@ -526,124 +527,128 @@
                     _rank.append(r + 1)
         _df['rank'] = _rank
         _game_df: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation.get('game'))
         # _game_df['game'] = _game_df.index.values
         _tournament_df: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation.get('tournament'))
         # _tournament_df['game'] = _tournament_df.index.values
         _file_paths: List[str] = []
-        if self.visualize_all_scores:
-            if visualize_game_stats:
-                _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_stats.html'))
-                _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_size.html'))
-                _game_plot: dict = {'Feature Tournament Game Stats (Shapley Scores)': dict(data=_game_df,
-                                                                                           features=list(
-                                                                                               _game_df.columns),
-                                                                                           plot_type='violin',
-                                                                                           melt=True,
-                                                                                           render=True,
-                                                                                           file_path=_file_paths[
-                                                                                               0] if self.path is not None else None
-                                                                                           ),
-                                    'Feature Tournament Stats (Game Size)': dict(data=_tournament_df,
-                                                                                 features=list(_tournament_df.columns),
-                                                                                 plot_type='heat',
-                                                                                 render=True,
-                                                                                 file_path=_file_paths[
-                                                                                     1] if self.path is not None else None
-                                                                                 )
-                                    }
-                DataVisualizer(subplots=_game_plot,
-                               height=500,
-                               width=500
-                               ).run()
-            _file_paths.append(os.path.join(str(self.path), 'feature_importance_shapley.html'))
+        if visualize_game_stats:
+            _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_stats.html'))
+            DataVisualizer(df=_game_df,
+                           title='Feature Tournament Game Stats (Shapley Scores)',
+                           features=_game_df.columns.tolist(),
+                           melt=True,
+                           plot_type='violin',
+                           file_path=_file_paths[0] if self.path is not None else None
+                           ).run()
+            _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_size.html'))
+            DataVisualizer(df=_tournament_df,
+                           title='Feature Tournament Stats (Game Size)',
+                           features=_tournament_df.columns.tolist(),
+                           plot_type='heat',
+                           file_path=_file_paths[1] if self.path is not None else None
+                           ).run()
+        _file_paths.append(os.path.join(str(self.path), 'feature_importance_shapley.html'))
+        if visualize_feature_importance:
             _imp_plot: dict = {'Feature Importance (Shapley Scores)': dict(df=_df,
                                                                            plot_type=plot_type,
                                                                            render=True if self.path is None else False,
-                                                                           file_path=_file_paths[
-                                                                               -1] if self.path is not None else None,
+                                                                           file_path=_file_paths[-1] if self.path is not None else None,
                                                                            kwargs=dict(layout={},
                                                                                        y=_df['score'].values,
                                                                                        x=_df.index.values.tolist(),
                                                                                        marker=dict(color=_df['score'],
                                                                                                    colorscale='rdylgn',
                                                                                                    autocolorscale=True
                                                                                                    )
                                                                                        )
                                                                            )
                                }
+            DataVisualizer(subplots=_imp_plot,
+                           height=500,
+                           width=500
+                           ).run()
         if self.mlflow_log:
             self._mlflow_tracking(stats={'Feature Score (Feature Tournament)': _df,
                                          'Game Size (Feature Tournament)': _tournament_df,
                                          'Game Score (Feature Tournament)': _game_df
                                          },
                                   file_paths=_file_paths)
-        if self.aggregate_feature_imp is not None:
+        if aggregate_feature_imp is not None:
             _aggre_score: dict = {}
-            for core_feature in self.aggregate_feature_imp.keys():
+            for core_feature in aggregate_feature_imp.keys():
                 _feature_scores: dict = {}
                 _aggre_score.update({core_feature: 0.0 if self.imp_score.get(core_feature) is None else self.imp_score.get(core_feature)})
                 if self.imp_score.get(core_feature) is not None:
                     _feature_scores.update({core_feature: self.imp_score.get(core_feature)})
-                for proc_feature in self.aggregate_feature_imp[core_feature]:
+                for proc_feature in aggregate_feature_imp[core_feature]:
                     _feature_scores.update({proc_feature: 0.0 if self.imp_score.get(proc_feature) is None else self.imp_score.get(proc_feature)})
                     if self.imp_score.get(proc_feature) is not None:
                         _aggre_score[core_feature] += self.imp_score.get(proc_feature)
-                if len(self.aggregate_feature_imp[core_feature]) < 2:
+                if len(aggregate_feature_imp[core_feature]) < 2:
                     continue
-                _aggre_score[core_feature] = _aggre_score[core_feature] / len(self.aggregate_feature_imp[core_feature])
+                _aggre_score[core_feature] = _aggre_score[core_feature] / len(aggregate_feature_imp[core_feature])
                 _processed_feature_matrix: pd.DataFrame = pd.DataFrame(data=_feature_scores, index=['score']).transpose()
                 _processed_feature_matrix.sort_values(by='score', axis=0, ascending=False, inplace=True)
                 _processed_features.append(_processed_feature_matrix.index.values.tolist()[0])
-                if self.visualize_variant_scores:
-                    _imp_plot.update(
-                        {'Feature Importance (Preprocessing Variants {})'.format(core_feature): dict(data=_processed_feature_matrix,
-                                                                                                     plot_type=plot_type,
-                                                                                                     melt=True,
-                                                                                                     render=True if self.path is None else False,
-                                                                                                     file_path='{}feature_importance_processing_variants.html'.format(self.path) if self.path is not None else None,
-                                                                                                     kwargs=dict(layout={},
-                                                                                                                 y=_processed_feature_matrix['score'].values,
-                                                                                                                 x=_processed_feature_matrix.index.values,
-                                                                                                                 marker=dict(color=_processed_feature_matrix['score'],
-                                                                                                                             colorscale='rdylgn',
-                                                                                                                             autocolorscale=True
-                                                                                                                             )
-                                                                                                                 )
-                                                                                                     )
-                         })
+                if visualize_variant_scores:
+                    _variant_scores = {'Feature Importance (Preprocessing Variants {})'.format(core_feature): dict(
+                            data=_processed_feature_matrix,
+                            plot_type=plot_type,
+                            melt=True,
+                            render=True if self.path is None else False,
+                            file_path='{}feature_importance_processing_variants.html'.format(
+                                self.path) if self.path is not None else None,
+                            kwargs=dict(layout={},
+                                        y=_processed_feature_matrix['score'].values,
+                                        x=_processed_feature_matrix.index.values,
+                                        marker=dict(color=_processed_feature_matrix['score'],
+                                                    colorscale='rdylgn',
+                                                    autocolorscale=True
+                                                    )
+                                        )
+                            )
+                         }
+                    DataVisualizer(subplots=_variant_scores,
+                                   height=500,
+                                   width=500
+                                   ).run()
             _core_imp_matrix: pd.DataFrame = pd.DataFrame(data=_aggre_score, index=['abs_score']).transpose()
             _core_imp_matrix['rel_score'] = _core_imp_matrix['abs_score'] / sum(_core_imp_matrix['abs_score'])
             _core_imp_matrix.sort_values(by='abs_score', axis=0, ascending=False, inplace=True)
             _raw_core_features: List[str] = _core_imp_matrix.loc[_core_imp_matrix['rel_score'] >= _imp_threshold, :].index.values.tolist()
             for core in _raw_core_features:
-                _core_features.extend(self.aggregate_feature_imp[core])
+                _core_features.extend(aggregate_feature_imp[core])
                 _core_features = list(set(_core_features))
-            if self.visualize_core_features_scores:
-                _imp_plot.update({'Feature Importance (Core Feature Aggregation)': dict(data=_core_imp_matrix,
+            if visualize_core_feature_scores:
+                _core_feature_scores_plot: dict = {'Feature Importance (Core Feature Aggregation)': dict(data=_core_imp_matrix,
                                                                                         plot_type=plot_type,
                                                                                         melt=False,
                                                                                         render=True if self.path is None else False,
-                                                                                        file_path='{}feature_importance_core_aggregation.html'.format(self.path) if self.path is not None else None,
+                                                                                        file_path='{}feature_importance_core_aggregation.html'.format(
+                                                                                            self.path) if self.path is not None else None,
                                                                                         kwargs=dict(layout={},
-                                                                                                    y=_core_imp_matrix['abs_score'].values,
-                                                                                                    x=_core_imp_matrix['abs_score'].index.values,
+                                                                                                    y=_core_imp_matrix[
+                                                                                                        'abs_score'].values,
+                                                                                                    x=_core_imp_matrix[
+                                                                                                        'abs_score'].index.values,
                                                                                                     marker=dict(
-                                                                                                        color=_core_imp_matrix['abs_score'],
+                                                                                                        color=
+                                                                                                        _core_imp_matrix[
+                                                                                                            'abs_score'],
                                                                                                         colorscale='rdylgn',
                                                                                                         autocolorscale=True
-                                                                                                        )
+                                                                                                    )
                                                                                                     )
                                                                                         )
-                                  })
-        if self.visualize_all_scores or self.visualize_variant_scores or self.visualize_core_features_scores:
-            DataVisualizer(subplots=_imp_plot,
-                           height=500,
-                           width=500
-                           ).run()
+                                  }
+                DataVisualizer(subplots=_core_feature_scores_plot,
+                               height=500,
+                               width=500
+                               ).run()
         if self.ml_type == 'reg':
             _model_generator: ModelGeneratorReg = ModelGeneratorReg(model_name=self.feature_tournament_ai.get('model_name'),
                                                                     reg_params=self.feature_tournament_ai.get('param')
                                                                     )
         else:
             _model_generator: ModelGeneratorClf = ModelGeneratorClf(model_name=self.feature_tournament_ai.get('model_name'),
                                                                     clf_params=self.feature_tournament_ai.get('param')
@@ -657,51 +662,51 @@
         _pred = _model_generator.predict(x=_train_test_split.get('x_test').values)
         _model_generator.eval(obs=_train_test_split.get('y_test').values, pred=_pred)
         _model_test_score: float = _model_generator.fitness['test'].get(self.ml_metric)
         if self.ml_type == 'reg':
             _threshold: float = _model_test_score * (1 + redundant_threshold)
         else:
             _threshold: float = _model_test_score * (1 - redundant_threshold)
-        print('Metric', _model_test_score)
-        print('Threshold', _threshold)
         _features: List[str] = copy.deepcopy(_imp_features)
-        print(_features)
-        _result: dict = dict(redundant=[], important=[], reduction={})
+        _result: dict = dict(redundant=[], important=[], reduction={}, model_metric=[])
         for i in range(len(_imp_features) - 1, 0, -1):
-            print(_imp_features[i])
+            del _features[i]
             if len(_features) == 1:
                 _result['important'] = _features
                 break
-            del _features[i]
             _model_generator.train(x=_train_test_split.get('x_train')[_features].values, y=_train_test_split.get('y_train').values)
             _pred = _model_generator.predict(x=_train_test_split.get('x_test')[_features].values)
             _model_generator.eval(obs=_train_test_split.get('y_test').values, pred=_pred)
             _new_model_test_score: float = _model_generator.fitness['test'].get(self.ml_metric)
-            print('New model score', _new_model_test_score)
             if self.ml_type == 'reg':
                 if _threshold <= _new_model_test_score:
                     _features.append(_imp_features[i])
                     _result['important'] = _features
                     break
                 else:
                     _result['redundant'].append(_imp_features[i])
+                    _result['model_metric'].append(_model_test_score)
                     _result['reduction'].update({_imp_features[i]: _model_test_score - _new_model_test_score})
             else:
                 if _threshold >= _new_model_test_score:
                     _features.append(_imp_features[i])
                     _result['important'] = _features
                     break
                 else:
                     _result['redundant'].append(_imp_features[i])
+                    _result['model_metric'].append(_model_test_score)
                     _result['reduction'].update({_imp_features[i]: _model_test_score - _new_model_test_score})
         Log(write=False,
             level='info'
             ).log(msg=f'Number of redundant features: {len(_result["redundant"])}\nNumber of important features: {len(_result["important"])}')
         return dict(imp_features=_imp_features,
                     imp_score=self.imp_score,
                     imp_threshold=imp_threshold,
                     imp_core_features=_core_features,
                     imp_processed_features=_processed_features,
                     redundant=_result['redundant'],
                     important=_result['important'],
-                    reduction=_result['reduction']
+                    reduction=_result['reduction'],
+                    model_metric=_result['model_metric'],
+                    base_metric=_model_test_score,
+                    threshold=_threshold
                     )
```

### Comparing `happy_learning-0.4.8/happy_learning/genetic_algorithm.py` & `happy_learning-0.4.9/happy_learning/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/missing_data_analysis.py` & `happy_learning-0.4.9/happy_learning/missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/multiple_imputation.py` & `happy_learning-0.4.9/happy_learning/multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/neural_network_generator_torch.py` & `happy_learning-0.4.9/happy_learning/neural_network_generator_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/neural_network_torch.py` & `happy_learning-0.4.9/happy_learning/neural_network_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/sampler.py` & `happy_learning-0.4.9/happy_learning/sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/self_taught_short_text_clustering.py` & `happy_learning-0.4.9/happy_learning/self_taught_short_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/supervised_machine_learning.py` & `happy_learning-0.4.9/happy_learning/supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/swarm_intelligence.py` & `happy_learning-0.4.9/happy_learning/swarm_intelligence.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/text_clustering.py` & `happy_learning-0.4.9/happy_learning/text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/text_clustering_generator.py` & `happy_learning-0.4.9/happy_learning/text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/text_miner.py` & `happy_learning-0.4.9/happy_learning/text_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning/utils.py` & `happy_learning-0.4.9/happy_learning/utils.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/happy_learning.egg-info/PKG-INFO` & `happy_learning-0.4.9/happy_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy-learning
-Version: 0.4.8
+Version: 0.4.9
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `happy_learning-0.4.8/happy_learning.egg-info/SOURCES.txt` & `happy_learning-0.4.9/happy_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/setup.py` & `happy_learning-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open('requirements.txt', 'r') as _requirements:
     requires = _requirements.read()
 
 requires = [r.strip() for r in requires.split('\n') if ((r.strip()[0] != "#") and (len(r.strip()) > 3) and "-e git://" not in r)]
 
 setuptools.setup(
     name='happy_learning',
-    version='0.4.8',
+    version='0.4.9',
     author='Gianni Francesco Balistreri',
     author_email='gbalistreri@gmx.de',
     description='Toolbox for reinforced developing of machine learning models (as proof-of-concept)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch',
     license='GNU',
```

### Comparing `happy_learning-0.4.8/test/test_data_miner.py` & `happy_learning-0.4.9/test/test_data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_deep_q_learning.py` & `happy_learning-0.4.9/test/test_deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_environment_modeling.py` & `happy_learning-0.4.9/test/test_environment_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_evaluate_machine_learning.py` & `happy_learning-0.4.9/test/test_evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_feature_engineer.py` & `happy_learning-0.4.9/test/test_feature_engineer.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_feature_learning.py` & `happy_learning-0.4.9/test/test_feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_feature_selector.py` & `happy_learning-0.4.9/test/test_feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
                                                              increasing_pair_size_factor=0.5,
                                                              games=3,
                                                              penalty_factor=0.1,
                                                              max_iter=50,
                                                              max_players=-1,
                                                              evolutionary_algorithm='ga',
                                                              use_standard_params=True,
-                                                             aggregate_feature_imp=None,
-                                                             visualize_all_scores=False,
-                                                             visualize_variant_scores=False,
-                                                             visualize_core_feature_scores=False,
                                                              path='data/',
                                                              mlflow_log=True,
                                                              multi_threading=False
                                                              )
         _eval_result: dict = _feature_selector.select(imp_threshold=0.01,
-                                                      redundant_threshold=0.02,
-                                                      visualize_game_stats=True,
+                                                      redundant_threshold=0.01,
+                                                      aggregate_feature_imp=None,
+                                                      visualize_feature_importance=False,
+                                                      visualize_variant_scores=False,
+                                                      visualize_core_feature_scores=False,
+                                                      visualize_game_stats=False,
                                                       plot_type='bar'
                                                       )
         _imp_features: List[str] = _eval_result.get('important')
         _train_test_split: dict = MLSampler(df=DATA_SET,
                                             target='AveragePrice',
                                             features=_features,
                                             train_size=0.8,
```

### Comparing `happy_learning-0.4.8/test/test_genetic_algorithm.py` & `happy_learning-0.4.9/test/test_genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_missing_data_analysis.py` & `happy_learning-0.4.9/test/test_missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_multiple_imputation.py` & `happy_learning-0.4.9/test/test_multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_neural_network_generator_torch.py` & `happy_learning-0.4.9/test/test_neural_network_generator_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_neural_network_torch.py` & `happy_learning-0.4.9/test/test_neural_network_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_sampler.py` & `happy_learning-0.4.9/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_supervised_machine_learning.py` & `happy_learning-0.4.9/test/test_supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_swarm_intelligence.py` & `happy_learning-0.4.9/test/test_swarm_intelligence.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_text_clustering.py` & `happy_learning-0.4.9/test/test_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_text_clustering_generator.py` & `happy_learning-0.4.9/test/test_text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.8/test/test_text_miner.py` & `happy_learning-0.4.9/test/test_text_miner.py`

 * *Files identical despite different names*

