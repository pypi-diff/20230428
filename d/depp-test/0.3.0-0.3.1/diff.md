# Comparing `tmp/depp_test-0.3.0.tar.gz` & `tmp/depp_test-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depp_test-0.3.0.tar", last modified: Thu Apr 27 21:38:37 2023, max compression
+gzip compressed data, was "depp_test-0.3.1.tar", last modified: Thu Apr 27 22:18:47 2023, max compression
```

## Comparing `depp_test-0.3.0.tar` & `depp_test-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 21:38:37.732454 depp_test-0.3.0/
--rw-r--r--   0 yueyu      (501) staff       (20)      474 2023-04-27 21:38:37.732217 depp_test-0.3.0/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)       15 2022-12-08 05:14:10.000000 depp_test-0.3.0/README.md
--rw-r--r--   0 yueyu      (501) staff       (20)     1941 2022-12-08 03:54:04.000000 depp_test-0.3.0/agg_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      577 2022-12-08 03:54:04.000000 depp_test-0.3.0/comb_json.py
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 21:38:37.731145 depp_test-0.3.0/depp/
--rw-r--r--   0 yueyu      (501) staff       (20)     5764 2023-02-01 22:01:10.000000 depp_test-0.3.0/depp/Agg_model.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-15 21:40:03.000000 depp_test-0.3.0/depp/Agg_model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     8710 2023-02-01 19:47:27.000000 depp_test-0.3.0/depp/Model_pl.py
--rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-20 17:57:40.000000 depp_test-0.3.0/depp/Model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)        0 2022-12-08 03:54:04.000000 depp_test-0.3.0/depp/__init__.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1605 2022-12-23 18:59:14.000000 depp_test-0.3.0/depp/assign_cluster_by_placement.py
--rw-r--r--   0 yueyu      (501) staff       (20)      526 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/count_gapped_ratio.py
--rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-01-05 06:08:45.000000 depp_test-0.3.0/depp/data.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2431 2022-12-08 03:54:04.000000 depp_test-0.3.0/depp/data.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4009 2022-12-08 04:17:46.000000 depp_test-0.3.0/depp/data_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-01-05 18:39:30.000000 depp_test-0.3.0/depp/default_config.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-19 17:27:35.000000 depp_test-0.3.0/depp/depp_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-19 17:32:01.000000 depp_test-0.3.0/depp/depp_distance_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)      766 2022-12-08 09:41:19.000000 depp_test-0.3.0/depp/filter_by_entropy_gap.sh
--rw-r--r--   0 yueyu      (501) staff       (20)      782 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/get_names_by_entropy_gap.py
--rw-r--r--   0 yueyu      (501) staff       (20)      849 2023-04-27 21:34:13.000000 depp_test-0.3.0/depp/get_tree_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      576 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/grep_jplace.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1008 2022-12-08 09:46:07.000000 depp_test-0.3.0/depp/grep_seq.py
--rw-r--r--   0 yueyu      (501) staff       (20)      885 2023-04-27 21:33:25.000000 depp_test-0.3.0/depp/grep_seq_group.py
--rw-r--r--   0 yueyu      (501) staff       (20)      743 2022-12-23 19:57:48.000000 depp_test-0.3.0/depp/select_placement.py
--rw-------   0 yueyu      (501) staff       (20)      871 2023-04-27 21:32:31.000000 depp_test-0.3.0/depp/select_species_by_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)      342 2023-04-27 18:26:24.000000 depp_test-0.3.0/depp/set_bl_one.py
--rw-r--r--   0 yueyu      (501) staff       (20)     7731 2022-12-08 03:54:04.000000 depp_test-0.3.0/depp/submodule.py
--rw-r--r--   0 yueyu      (501) staff       (20)    32601 2023-04-19 17:28:16.000000 depp_test-0.3.0/depp/utils.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5802 2023-02-03 22:09:45.000000 depp_test-0.3.0/depp-place-rRNA-one-type.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     6477 2023-02-25 20:07:16.000000 depp_test-0.3.0/depp-place-rRNA.sh
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 21:38:37.731965 depp_test-0.3.0/depp_test.egg-info/
--rw-r--r--   0 yueyu      (501) staff       (20)      474 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)      934 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/SOURCES.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/dependency_links.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 21:37:24.000000 depp_test-0.3.0/depp_test.egg-info/not-zip-safe
--rw-r--r--   0 yueyu      (501) staff       (20)      154 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/requires.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        5 2023-04-27 21:38:37.000000 depp_test-0.3.0/depp_test.egg-info/top_level.txt
--rw-r--r--   0 yueyu      (501) staff       (20)     1149 2022-12-08 03:54:04.000000 depp_test-0.3.0/merge_json.py
--rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2022-12-08 03:54:01.000000 depp_test-0.3.0/run_upp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-02-01 07:34:59.000000 depp_test-0.3.0/seq_sep.py
--rw-r--r--   0 yueyu      (501) staff       (20)       38 2023-04-27 21:38:37.732530 depp_test-0.3.0/setup.cfg
--rw-r--r--   0 yueyu      (501) staff       (20)     1994 2023-04-27 21:38:24.000000 depp_test-0.3.0/setup.py
--rw-r--r--   0 yueyu      (501) staff       (20)     6233 2023-04-27 21:35:33.000000 depp_test-0.3.0/train_cluster_depp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-02-01 20:15:45.000000 depp_test-0.3.0/train_depp.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-19 17:48:08.000000 depp_test-0.3.0/train_depp_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5173 2022-12-08 03:54:01.000000 depp_test-0.3.0/wol_placement.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 22:18:47.483978 depp_test-0.3.1/
+-rw-r--r--   0 yueyu      (501) staff       (20)      474 2023-04-27 22:18:47.483796 depp_test-0.3.1/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)       15 2022-12-08 05:14:10.000000 depp_test-0.3.1/README.md
+-rw-r--r--   0 yueyu      (501) staff       (20)     1941 2022-12-08 03:54:04.000000 depp_test-0.3.1/agg_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      577 2022-12-08 03:54:04.000000 depp_test-0.3.1/comb_json.py
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 22:18:47.482264 depp_test-0.3.1/depp/
+-rw-r--r--   0 yueyu      (501) staff       (20)     5764 2023-02-01 22:01:10.000000 depp_test-0.3.1/depp/Agg_model.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-15 21:40:03.000000 depp_test-0.3.1/depp/Agg_model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     8710 2023-02-01 19:47:27.000000 depp_test-0.3.1/depp/Model_pl.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-20 17:57:40.000000 depp_test-0.3.1/depp/Model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)        0 2022-12-08 03:54:04.000000 depp_test-0.3.1/depp/__init__.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1605 2022-12-23 18:59:14.000000 depp_test-0.3.1/depp/assign_cluster_by_placement.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      526 2022-12-08 09:46:07.000000 depp_test-0.3.1/depp/count_gapped_ratio.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-01-05 06:08:45.000000 depp_test-0.3.1/depp/data.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2431 2022-12-08 03:54:04.000000 depp_test-0.3.1/depp/data.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4009 2022-12-08 04:17:46.000000 depp_test-0.3.1/depp/data_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-01-05 18:39:30.000000 depp_test-0.3.1/depp/default_config.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-19 17:27:35.000000 depp_test-0.3.1/depp/depp_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-19 17:32:01.000000 depp_test-0.3.1/depp/depp_distance_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      766 2022-12-08 09:41:19.000000 depp_test-0.3.1/depp/filter_by_entropy_gap.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)      782 2022-12-08 09:46:07.000000 depp_test-0.3.1/depp/get_names_by_entropy_gap.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      873 2023-04-27 22:18:06.000000 depp_test-0.3.1/depp/get_tree_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      576 2022-12-08 09:46:07.000000 depp_test-0.3.1/depp/grep_jplace.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1008 2022-12-08 09:46:07.000000 depp_test-0.3.1/depp/grep_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      909 2023-04-27 22:17:54.000000 depp_test-0.3.1/depp/grep_seq_group.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      743 2022-12-23 19:57:48.000000 depp_test-0.3.1/depp/select_placement.py
+-rw-------   0 yueyu      (501) staff       (20)      895 2023-04-27 22:17:54.000000 depp_test-0.3.1/depp/select_species_by_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      366 2023-04-27 22:17:54.000000 depp_test-0.3.1/depp/set_bl_one.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     7731 2022-12-08 03:54:04.000000 depp_test-0.3.1/depp/submodule.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    32601 2023-04-19 17:28:16.000000 depp_test-0.3.1/depp/utils.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5802 2023-02-03 22:09:45.000000 depp_test-0.3.1/depp-place-rRNA-one-type.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     6477 2023-02-25 20:07:16.000000 depp_test-0.3.1/depp-place-rRNA.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2023-04-27 22:18:47.483572 depp_test-0.3.1/depp_test.egg-info/
+-rw-r--r--   0 yueyu      (501) staff       (20)      474 2023-04-27 22:18:47.000000 depp_test-0.3.1/depp_test.egg-info/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)      934 2023-04-27 22:18:47.000000 depp_test-0.3.1/depp_test.egg-info/SOURCES.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 22:18:47.000000 depp_test-0.3.1/depp_test.egg-info/dependency_links.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2023-04-27 21:37:24.000000 depp_test-0.3.1/depp_test.egg-info/not-zip-safe
+-rw-r--r--   0 yueyu      (501) staff       (20)      154 2023-04-27 22:18:47.000000 depp_test-0.3.1/depp_test.egg-info/requires.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        5 2023-04-27 22:18:47.000000 depp_test-0.3.1/depp_test.egg-info/top_level.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)     1149 2022-12-08 03:54:04.000000 depp_test-0.3.1/merge_json.py
+-rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2022-12-08 03:54:01.000000 depp_test-0.3.1/run_upp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-02-01 07:34:59.000000 depp_test-0.3.1/seq_sep.py
+-rw-r--r--   0 yueyu      (501) staff       (20)       38 2023-04-27 22:18:47.484040 depp_test-0.3.1/setup.cfg
+-rw-r--r--   0 yueyu      (501) staff       (20)     1994 2023-04-27 22:18:33.000000 depp_test-0.3.1/setup.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     6246 2023-04-27 22:17:54.000000 depp_test-0.3.1/train_cluster_depp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-02-01 20:15:45.000000 depp_test-0.3.1/train_depp.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-19 17:48:08.000000 depp_test-0.3.1/train_depp_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5173 2022-12-08 03:54:01.000000 depp_test-0.3.1/wol_placement.sh
```

### Comparing `depp_test-0.3.0/agg_dist.py` & `depp_test-0.3.1/agg_dist.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/comb_json.py` & `depp_test-0.3.1/comb_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/Agg_model.py` & `depp_test-0.3.1/depp/Agg_model.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/Agg_model_recon.py` & `depp_test-0.3.1/depp/Agg_model_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/Model_pl.py` & `depp_test-0.3.1/depp/Model_pl.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/Model_recon.py` & `depp_test-0.3.1/depp/Model_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/assign_cluster_by_placement.py` & `depp_test-0.3.1/depp/assign_cluster_by_placement.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/count_gapped_ratio.py` & `depp_test-0.3.1/depp/count_gapped_ratio.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/data.py` & `depp_test-0.3.1/depp/data.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/data.split.py` & `depp_test-0.3.1/depp/data.split.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/data_recon.py` & `depp_test-0.3.1/depp/data_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/default_config.py` & `depp_test-0.3.1/depp/default_config.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/depp_distance.py` & `depp_test-0.3.1/depp/depp_distance.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/depp_distance_recon.py` & `depp_test-0.3.1/depp/depp_distance_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/filter_by_entropy_gap.sh` & `depp_test-0.3.1/depp/filter_by_entropy_gap.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/get_names_by_entropy_gap.py` & `depp_test-0.3.1/depp/get_names_by_entropy_gap.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/get_tree_dist.py` & `depp_test-0.3.1/depp/get_tree_dist.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import argparse
 import treeswift as ts
 import pandas as pd
 
 parser = argparse.ArgumentParser(description='get the corresponding tree distance matrix of input distance')
 parser.add_argument('--treefile', type=str)
 parser.add_argument('--distfile', type=str, default=None)
```

### Comparing `depp_test-0.3.0/depp/grep_jplace.py` & `depp_test-0.3.1/depp/grep_jplace.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/grep_seq.py` & `depp_test-0.3.1/depp/grep_seq.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/grep_seq_group.py` & `depp_test-0.3.1/depp/grep_seq_group.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import argparse
 import collections
 from Bio import SeqIO
 
 # this is for sequences with multiple copies
 
 parser = argparse.ArgumentParser(description='test')
```

### Comparing `depp_test-0.3.0/depp/select_placement.py` & `depp_test-0.3.1/depp/select_placement.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/select_species_by_distance.py` & `depp_test-0.3.1/depp/select_species_by_distance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import pandas as pd
 import os
 import numpy as np
 import collections
 from Bio import SeqIO
 import argparse
```

### Comparing `depp_test-0.3.0/depp/submodule.py` & `depp_test-0.3.1/depp/submodule.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp/utils.py` & `depp_test-0.3.1/depp/utils.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp-place-rRNA-one-type.sh` & `depp_test-0.3.1/depp-place-rRNA-one-type.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp-place-rRNA.sh` & `depp_test-0.3.1/depp-place-rRNA.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/depp_test.egg-info/SOURCES.txt` & `depp_test-0.3.1/depp_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/merge_json.py` & `depp_test-0.3.1/merge_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/run_upp.sh` & `depp_test-0.3.1/run_upp.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/seq_sep.py` & `depp_test-0.3.1/seq_sep.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/setup.py` & `depp_test-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name='depp_test',    # This is the name of your PyPI-package.
-        version='0.3.0',    # Update the version number for new releases
+        version='0.3.1',    # Update the version number for new releases
         scripts=['train_depp.py',
                  'depp/depp_distance.py',
                  'agg_dist.py',
                  'wol_placement.sh',
                  'run_upp.sh',
                  'merge_json.py',
 		 'train_depp_recon.py',
```

### Comparing `depp_test-0.3.0/train_cluster_depp.sh` & `depp_test-0.3.1/train_cluster_depp.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/bin/bash
+
 # $1 backbone tree
 # $2 backbone sequences
 # $3 outdir
 while getopts t:s:e:g:o: flag
 do
     case "${flag}" in
 	t) backbone_tree=${OPTARG};;
```

### Comparing `depp_test-0.3.0/train_depp.py` & `depp_test-0.3.1/train_depp.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/train_depp_recon.py` & `depp_test-0.3.1/train_depp_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.0/wol_placement.sh` & `depp_test-0.3.1/wol_placement.sh`

 * *Files identical despite different names*

