# Comparing `tmp/chemistry_and_robots-1.5.0.tar.gz` & `tmp/chemistry_and_robots-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemistry_and_robots-1.5.0.tar", last modified: Mon Apr  3 23:23:05 2023, max compression
+gzip compressed data, was "chemistry_and_robots-1.6.0.tar", last modified: Thu Apr 27 16:53:55 2023, max compression
```

## Comparing `chemistry_and_robots-1.5.0.tar` & `chemistry_and_robots-1.6.0.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.126331 chemistry_and_robots-1.5.0/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      727 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/MANIFEST.in
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-04-03 23:23:05.126331 chemistry_and_robots-1.5.0/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8187 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/README.md
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.056331 chemistry_and_robots-1.5.0/chemistry_and_robots/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       78 2023-04-03 23:20:49.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/__init__.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.076331 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      150 2022-09-02 15:03:43.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8002 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/base_ontology.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    24529 2023-04-03 09:38:09.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/iris.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      267 2022-09-02 15:03:43.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontobpr.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    14126 2023-04-03 17:18:49.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontodoe.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     6132 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontohplc.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7925 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontolab.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    36317 2023-04-03 10:33:32.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontoreaction.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    33893 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontovapourtec.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2675 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/unit_conversion.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.076331 chemistry_and_robots-1.5.0/chemistry_and_robots/hardware/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/hardware/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2679 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/hardware/hplc.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.086331 chemistry_and_robots-1.5.0/chemistry_and_robots/kg_operations/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       58 2022-09-04 20:28:19.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/kg_operations/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3261 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/kg_operations/dict_and_list.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)   150019 2023-04-03 09:48:22.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/kg_operations/sparql_client.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.046331 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.086331 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1556 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1521 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1556 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.106331 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5461 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/doe.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5451 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5585 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/doe_template.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    58701 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/dummy_lab.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7234 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3342 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/duplicate_ontorxn.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    24005 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/new_exp_data.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    41226 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      124 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      298 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_incomplete.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      111 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_no_product.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      416 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_unidentified_peaks.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    26112 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    69489 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/rxn_data.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8094 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.126331 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    42961 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/conftest.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4414 2022-09-02 15:03:43.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_base_ontology.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4720 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_dict_and_list.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      663 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_example_triples.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10992 2023-01-20 09:52:31.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_hash_eq.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3610 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_hplc.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1569 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_ontodoe.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    30177 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_single_phase.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    89981 2023-03-31 13:49:03.000000 chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_sparql_client.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-03 23:23:05.066331 chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-04-03 23:23:04.000000 chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2832 2023-04-03 23:23:04.000000 chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/SOURCES.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-04-03 23:23:04.000000 chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/dependency_links.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      157 2023-04-03 23:23:04.000000 chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/requires.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       21 2023-04-03 23:23:04.000000 chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/top_level.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-04-03 23:23:05.126331 chemistry_and_robots-1.5.0/setup.cfg
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      990 2023-04-03 23:20:49.000000 chemistry_and_robots-1.5.0/setup.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.085852 chemistry_and_robots-1.6.0/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      772 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/MANIFEST.in
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-04-27 16:53:55.085852 chemistry_and_robots-1.6.0/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8187 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/README.md
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       78 2023-04-27 16:48:09.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/__init__.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      150 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8002 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/base_ontology.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    24268 2023-04-27 12:30:16.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/iris.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      267 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontobpr.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    14466 2023-04-27 12:45:27.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontodoe.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     6132 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontohplc.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7159 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontolab.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    36143 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontoreaction.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    33784 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontovapourtec.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2675 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/unit_conversion.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots/hardware/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/hardware/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     2679 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/hardware/hplc.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots/kg_operations/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       58 2022-09-04 20:28:19.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/kg_operations/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3261 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/kg_operations/dict_and_list.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)   151217 2023-04-27 14:58:00.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/kg_operations/sparql_client.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      585 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/__init__.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1551 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1516 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1551 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.075852 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    33232 2023-04-27 16:48:42.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/OntoDoE.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    21430 2023-04-27 16:48:58.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/OntoGoal.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    27346 2023-04-27 16:48:51.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/OntoHPLC.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    36783 2023-04-27 16:48:49.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/OntoLab.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    52477 2023-04-27 16:48:46.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/OntoReaction.owl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    62442 2023-04-27 16:48:54.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontology/OntoVapourtec.owl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.075852 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5426 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/doe.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5366 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     5500 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/doe_template.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    57959 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/dummy_lab.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7144 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    23351 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/new_exp_data.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    40339 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      124 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      298 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_incomplete.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      111 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_no_product.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      416 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_unidentified_peaks.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    25600 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    26112 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    67322 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/rxn_data.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8080 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.085852 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    43077 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/conftest.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4414 2022-09-02 15:03:43.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_base_ontology.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4720 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_dict_and_list.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      663 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_example_triples.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10992 2023-01-20 09:52:31.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_hash_eq.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3610 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_hplc.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1569 2023-04-27 12:27:27.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_ontodoe.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    30117 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_single_phase.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    90116 2023-04-27 12:28:53.000000 chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_sparql_client.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 16:53:55.065852 chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8652 2023-04-27 16:53:54.000000 chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     3135 2023-04-27 16:53:54.000000 chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-04-27 16:53:54.000000 chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      157 2023-04-27 16:53:54.000000 chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/requires.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       21 2023-04-27 16:53:54.000000 chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/top_level.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-04-27 16:53:55.085852 chemistry_and_robots-1.6.0/setup.cfg
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      990 2023-04-27 16:48:09.000000 chemistry_and_robots-1.6.0/setup.py
```

### Comparing `chemistry_and_robots-1.5.0/MANIFEST.in` & `chemistry_and_robots-1.6.0/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 recursive-include chemistry_and_robots *.ttl
+recursive-include chemistry_and_robots *.owl
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_txt.txt
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_incomplete.txt
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_unidentified_peaks.txt
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_no_product.txt
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls
 include chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls
```

### Comparing `chemistry_and_robots-1.5.0/PKG-INFO` & `chemistry_and_robots-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemistry_and_robots
-Version: 1.5.0
+Version: 1.6.0
 Summary: chemistryandrobots contains dataclasses and sparql queries for concepts related to chemistry_and_robots as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/utils/chemistry_and_robots
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `chemistry_and_robots-1.5.0/README.md` & `chemistry_and_robots-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/base_ontology.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/base_ontology.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/iris.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/iris.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from pyderivationagent.data_model.iris import *
 
 RDFS_COMMENT = RDFS_BASE_URL + 'comment'
+OWL = 'http://www.w3.org/2002/07/owl#'
+OWL_VERSION = OWL + 'versionInfo'
 
 ###--- Common Base URL ---###
 ONTOCAPE_PHASESYSTEM = 'http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#'
 ONTOCAPE_SUBSTANCE = 'http://www.theworldavatar.com/ontology/ontocape/material/substance/substance.owl#'
 ONTOCAPE_REACTIONMECHANISM = 'http://www.theworldavatar.com/ontology/ontocape/material/substance/reaction_mechanism.owl#'
 ONTOCAPE_MATERIAL = 'http://www.theworldavatar.com/ontology/ontocape/material/material.owl#'
 ONTOCAPE_SYSTEM = 'http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#'
 ONTOCAPE_BEHAVIOR = 'http://www.theworldavatar.com/ontology/ontocape/chemical_process_system/CPS_behavior/behavior.owl#'
 
 ONTODOE = 'https://www.theworldavatar.com/kg/ontodoe/'
 ONTOREACTION = 'https://www.theworldavatar.com/kg/ontoreaction/'
+ONTOGOAL = 'https://www.theworldavatar.com/kg/ontogoal/'
 ONTOKIN = 'http://www.theworldavatar.com/ontology/ontokin/OntoKin.owl#'
 ONTOSPECIES = 'http://www.theworldavatar.com/ontology/ontospecies/OntoSpecies.owl#'
 ONTOLAB = 'https://www.theworldavatar.com/kg/ontolab/'
 ONTOVAPOURTEC = 'https://www.theworldavatar.com/kg/ontovapourtec/'
 ONTOHPLC = 'https://www.theworldavatar.com/kg/ontohplc/'
 ONTOBPR = 'https://www.theworldavatar.com/kg/ontobpr/'
 
@@ -107,15 +110,15 @@
 ONTOCAPE_PHASECOMPONENT = ONTOCAPE_PHASESYSTEM + 'PhaseComponent'
 ONTOCAPE_COMPOSITION = ONTOCAPE_PHASESYSTEM + 'Composition'
 ONTOCAPE_PHASECOMPONENTCONCENTRATION = ONTOCAPE_PHASESYSTEM + 'PhaseComponentConcentration'
 ONTOCAPE_PHYSICALCONTEXT = ONTOCAPE_PHASESYSTEM + 'PhysicalContext'
 ONTOCAPE_VOLUMEBASEDCONCENTRATION = ONTOCAPE_PHASESYSTEM + 'Volume-BasedConcentration'
 ONTOCAPE_MOLARITY = ONTOCAPE_PHASESYSTEM + 'Molarity'
 ONTOCAPE_CHEMICALSPECIES = ONTOCAPE_SUBSTANCE + 'ChemicalSpecies'
-ONTOCAPE_CATALYST = ONTOCAPE_REACTIONMECHANISM + 'hasCatalyst'
+ONTOCAPE_HASCATALYST = ONTOCAPE_REACTIONMECHANISM + 'hasCatalyst'
 ONTOCAPE_REPRESENTSTHERMODYNAMICBEHAVIOROF = ONTOCAPE_MATERIAL + 'representsThermodynamicBehaviorOf'
 ONTOCAPE_THERMODYNAMICBEHAVIOR = ONTOCAPE_MATERIAL + 'thermodynamicBehavior'
 ONTOCAPE_HASSTATEOFAGGREGATION = ONTOCAPE_PHASESYSTEM + 'hasStateOfAggregation'
 ONTOCAPE_ISCOMPOSEDOFSUBSYSTEM = ONTOCAPE_SYSTEM + 'isComposedOfSubsystem'
 ONTOCAPE_HAS_COMPOSITION = ONTOCAPE_PHASESYSTEM + 'has_composition'
 ONTOCAPE_COMPRISESDIRECTLY = ONTOCAPE_SYSTEM + 'comprisesDirectly'
 ONTOCAPE_HAS_PHYSICAL_CONTEXT = ONTOCAPE_PHASESYSTEM + 'has_physical_context'
@@ -163,15 +166,16 @@
 ONTODOE_NEWEXPERIMENT = ONTODOE + 'NewExperiment'
 ONTODOE_USESSTRATEGY = ONTODOE + 'usesStrategy'
 ONTODOE_HASDOMAIN = ONTODOE + 'hasDomain'
 ONTODOE_HASDESIGNVARIABLE = ONTODOE + 'hasDesignVariable'
 ONTODOE_HASSYSTEMRESPONSE = ONTODOE + 'hasSystemResponse'
 ONTODOE_UTILISESHISTORICALDATA = ONTODOE + 'utilisesHistoricalData'
 ONTODOE_PROPOSESNEWEXPERIMENT = ONTODOE + 'proposesNewExperiment'
-ONTODOE_REFERSTO = ONTODOE + 'refersTo'
+ONTODOE_REFERSTOQUANTITY = ONTODOE + 'refersToQuantity'
+ONTODOE_REFERSTOEXPERIMENT = ONTODOE + 'refersToExperiment'
 ONTODOE_HASLEVEL = ONTODOE + 'hasLevel'
 ONTODOE_UPPERLIMIT = ONTODOE + 'upperLimit'
 ONTODOE_LOWERLIMIT = ONTODOE + 'lowerLimit'
 ONTODOE_POSITIONALID = ONTODOE + 'positionalID'
 ONTODOE_MAXIMISE = ONTODOE + 'maximise'
 ONTODOE_NUMOFNEWEXP = ONTODOE + 'numOfNewExp'
 ONTODOE_NRETRIES = ONTODOE + 'nRetries'
@@ -180,14 +184,15 @@
 ONTODOE_POPULATIONSIZE = ONTODOE + 'populationSize'
 ONTODOE_SEED = ONTODOE + 'seed'
 ONTODOE_HASFIXEDPARAMETER = ONTODOE + 'hasFixedParameter'
 ONTODOE_HASDOETEMPLATE = ONTODOE + 'hasDoETemplate'
 ONTODOE_DESIGNSCHEMICALREACTION = ONTODOE + 'designsChemicalReaction'
 
 ###--- IRIs for ONTOREACTION ---###
+ONTOREACTION_CHEMICALREACTION = ONTOREACTION + 'ChemicalReaction'
 ONTOREACTION_REACTIONEXPERIMENT = ONTOREACTION + 'ReactionExperiment'
 ONTOREACTION_REACTIONVARIATION = ONTOREACTION + 'ReactionVariation'
 ONTOREACTION_CATALYST = ONTOREACTION + 'Catalyst'
 ONTOREACTION_SOLVENT = ONTOREACTION + 'Solvent'
 ONTOREACTION_BASE = ONTOREACTION + 'Base'
 ONTOREACTION_TARGETPRODUCT = ONTOREACTION + 'TargetProduct'
 ONTOREACTION_IMPURITY = ONTOREACTION + 'Impurity'
@@ -204,21 +209,19 @@
 ONTOREACTION_REACTIONTEMPERATURE = ONTOREACTION + 'ReactionTemperature'
 ONTOREACTION_REACTIONPRESSURE = ONTOREACTION + 'ReactionPressure'
 ONTOREACTION_STOICHIOMETRYRATIO = ONTOREACTION + 'StoichiometryRatio'
 ONTOREACTION_REACTIONSCALE = ONTOREACTION + 'ReactionScale'
 ONTOREACTION_CHEMICAL = ONTOREACTION + 'Chemical'
 ONTOREACTION_INPUTCHEMICAL = ONTOREACTION + 'InputChemical'
 ONTOREACTION_OUTPUTCHEMICAL = ONTOREACTION + 'OutputChemical'
-ONTOREACTION_HASVARIATION = ONTOREACTION + 'hasVariation'
 ONTOREACTION_ISVARIATIONOF = ONTOREACTION + 'isVariationOf'
 ONTOREACTION_ISASSIGNEDTO = ONTOREACTION + 'isAssignedTo'
-ONTOREACTION_HASEQUIPMENTSETTINGS = ONTOREACTION + 'hasEquipmentSettings'
 ONTOREACTION_ISOCCURENCEOF = ONTOREACTION + 'isOccurenceOf'
-ONTOREACTION_ISREALISEDAS = ONTOREACTION + 'isRealisedAs'
 ONTOREACTION_HASSOLVENT = ONTOREACTION + 'hasSolvent'
+ONTOREACTION_HASCATALYST = ONTOREACTION + 'hasCatalyst'
 ONTOREACTION_HASBASE = ONTOREACTION + 'hasBase'
 ONTOREACTION_HASRXNTYPE = ONTOREACTION + 'hasRxnType'
 ONTOREACTION_HASPERFORMANCEINDICATOR = ONTOREACTION + 'hasPerformanceIndicator'
 ONTOREACTION_HASENVIRONMENTALFACTOR = ONTOREACTION + 'hasEnvironmentalFactor'
 ONTOREACTION_HASYIELD = ONTOREACTION + 'hasYield'
 ONTOREACTION_HASECOSCORE = ONTOREACTION + 'hasEcoScore'
 ONTOREACTION_HASCONVERSION = ONTOREACTION + 'hasConversion'
@@ -242,30 +245,24 @@
 ONTOREACTION_RXNCXSMILES = ONTOREACTION + 'rxnCXSMILES'
 ONTOREACTION_YIELDLIMITINGSPECIES = ONTOREACTION + 'yieldLimitingSpecies'
 
 
 ###--- IRIs for OntoLab ---###
 ONTOLAB_ISMANAGEDBY = ONTOLAB + "isManagedBy"
 ONTOLAB_CONTAINS = ONTOLAB + 'contains'
-ONTOLAB_HASARGUMENT = ONTOLAB + 'hasArgument'
 ONTOLAB_HASHEIGHT = ONTOLAB + 'hasHeight'
 ONTOLAB_HASLENGTH = ONTOLAB + 'hasLength'
 ONTOLAB_HASPOWERSUPPLY = ONTOLAB + 'hasPowerSupply'
 ONTOLAB_HASPRICE = ONTOLAB + 'hasPrice'
 ONTOLAB_HASQUANTITY = ONTOLAB + 'hasQuantity'
 ONTOLAB_HASSETTING = ONTOLAB + 'hasSetting'
 ONTOLAB_HASWEIGHT = ONTOLAB + 'hasWeight'
 ONTOLAB_HASWIDTH = ONTOLAB + 'hasWidth'
-ONTOLAB_ISCONTAINEDIN = ONTOLAB + 'isContainedIn'
 ONTOLAB_ISPREPAREDBY = ONTOLAB + 'isPreparedBy'
-ONTOLAB_ISSPECIFIEDBY = ONTOLAB + 'isSpecifiedBy'
 ONTOLAB_SPECIFIES = ONTOLAB + 'specifies'
-ONTOLAB_HASARGSTR = ONTOLAB + 'hasArgStr'
-ONTOLAB_HASCMDSTR = ONTOLAB + 'hasCmdStr'
-ONTOLAB_ARGUMENT = ONTOLAB + 'Argument'
 ONTOLAB_CHEMICALAMOUNT = ONTOLAB + 'ChemicalAmount'
 ONTOLAB_PREPARATIONMETHOD = ONTOLAB + 'PreparationMethod'
 ONTOLAB_DRIED = ONTOLAB + 'Dried'
 ONTOLAB_DURATIONSETTING = ONTOLAB + 'DurationSetting'
 ONTOLAB_PARAMETERSETTING = ONTOLAB + 'ParameterSetting'
 ONTOLAB_EQUIPMENTSETTINGS = ONTOLAB + 'EquipmentSettings'
 ONTOLAB_LABEQUIPMENT = ONTOLAB + 'LabEquipment'
@@ -280,15 +277,14 @@
 ONTOLAB_SOLARPOWERPACK = ONTOLAB + 'SolarPowerPack'
 ONTOLAB_SPARGED = ONTOLAB + 'Sparged'
 ONTOLAB_SYNTHESISEDINHOUSE = ONTOLAB + 'SynthesisedInHouse'
 ONTOLAB_TEMPERATURESETTING = ONTOLAB + 'TemperatureSetting'
 ONTOLAB_USEDASRECEIVED = ONTOLAB + 'UsedAsReceived'
 ONTOLAB_VOLUMESETTING = ONTOLAB + 'VolumeSetting'
 ONTOLAB_WASGENERATEDFOR = ONTOLAB + 'wasGeneratedFor'
-ONTOLAB_TRANSLATESTOPARAMETERSETTING = ONTOLAB + 'translatesToParameterSetting'
 ONTOLAB_STATELASTUPDATEDAT = ONTOLAB + 'stateLastUpdatedAt'
 ONTOLAB_CHEMICALCONTAINER = ONTOLAB + 'ChemicalContainer'
 ONTOLAB_REAGENTBOTTLE = ONTOLAB + 'ReagentBottle'
 ONTOLAB_WASTEBOTTLE = ONTOLAB + 'WasteBottle'
 ONTOLAB_VIAL = ONTOLAB + 'Vial'
 ONTOLAB_ISFILLEDWITH = ONTOLAB + 'isFilledWith'
 ONTOLAB_HASFILLLEVEL = ONTOLAB + 'hasFillLevel'
@@ -304,15 +300,14 @@
 ONTOVAPOURTEC_HASREACTORMATERIAL = ONTOVAPOURTEC + 'hasReactorMaterial'
 ONTOVAPOURTEC_HASREACTORTEMPERATURESETTING = ONTOVAPOURTEC + 'hasReactorTemperatureSetting'
 ONTOVAPOURTEC_HASREACTORVOLUME = ONTOVAPOURTEC + 'hasReactorVolume'
 ONTOVAPOURTEC_HASRESIDENCETIMESETTING = ONTOVAPOURTEC + 'hasResidenceTimeSetting'
 ONTOVAPOURTEC_HASSAMPLELOOPVOLUMESETTING = ONTOVAPOURTEC + 'hasSampleLoopVolumeSetting'
 ONTOVAPOURTEC_HASSITE = ONTOVAPOURTEC + 'hasSite'
 ONTOVAPOURTEC_HOLDS = ONTOVAPOURTEC + 'holds'
-ONTOVAPOURTEC_ISHELDIN = ONTOVAPOURTEC + 'isHeldIn'
 ONTOVAPOURTEC_PUMPSLIQUIDFROM = ONTOVAPOURTEC + 'pumpsLiquidFrom'
 ONTOVAPOURTEC_AUTOSAMPLER = ONTOVAPOURTEC + 'AutoSampler'
 ONTOVAPOURTEC_AUTOSAMPLERSITE = ONTOVAPOURTEC + 'AutoSamplerSite'
 ONTOVAPOURTEC_AUTOSAMPLERFUNCTION = ONTOVAPOURTEC + 'AutoSamplerFunction'
 ONTOVAPOURTEC_AUTOSAMPLERCOMMAND = ONTOVAPOURTEC + 'AutoSamplerCommand'
 ONTOVAPOURTEC_AUTOSAMPLERTASK = ONTOVAPOURTEC + 'AutoSamplerTask'
 ONTOVAPOURTEC_CLEANREACTOR = ONTOVAPOURTEC + 'CleanReactor'
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontodoe.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontodoe.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 
 class ContinuousVariable(DesignVariable):
     clz: str = ONTODOE_CONTINUOUSVARIABLE
     name: str=None # NOTE this is not part of OntoDoE ontology, but it is used for working with Summit python package
     upperLimit: float
     lowerLimit: float
     positionalID: Optional[str]
-    refersTo: OM_Quantity
+    refersToQuantity: OM_Quantity
 
     def create_instance_for_kg(self, g: Graph):
         g = super().create_instance_for_kg(g)
         g.add((URIRef(self.instance_iri), URIRef(ONTODOE_UPPERLIMIT), Literal(self.upperLimit)))
         g.add((URIRef(self.instance_iri), URIRef(ONTODOE_LOWERLIMIT), Literal(self.lowerLimit)))
         if self.positionalID is not None:
             g.add((URIRef(self.instance_iri), URIRef(ONTODOE_POSITIONALID), Literal(self.positionalID)))
 
-        # <continuous_variable> <OntoDoE:refersTo> <quantity>
+        # <continuous_variable> <OntoDoE:refersToQuantity> <quantity>
         # <quantity> <rdf:type> <QuantityType>
         # <quantity> <OntoDoE:hasUnit> <unit>
-        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTO), URIRef(self.refersTo.instance_iri)))
-        g.add((URIRef(self.refersTo.instance_iri), RDF.type, URIRef(self.refersTo.clz)))
-        g.add((URIRef(self.refersTo.instance_iri), URIRef(OM_HASUNIT), URIRef(self.refersTo.hasUnit)))
+        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTOQUANTITY), URIRef(self.refersToQuantity.instance_iri)))
+        g.add((URIRef(self.refersToQuantity.instance_iri), RDF.type, URIRef(self.refersToQuantity.clz)))
+        g.add((URIRef(self.refersToQuantity.instance_iri), URIRef(OM_HASUNIT), URIRef(self.refersToQuantity.hasUnit)))
 
         return g
 
     @pydantic.root_validator
     @classmethod
     def upper_and_lower_limit(cls, values):
         # validate the upper and lower limit
@@ -89,59 +89,59 @@
                 'ContinuousVariable <%s> has an UpperLimit %s that is smaller then its LowerLimit %s.' 
                 % (values.get('instance_iri'), values.get('upperLimit'), values.get('lowerLimit')))
         return values
 
     @pydantic.root_validator
     @classmethod
     def refers_to_quantity_unit(cls, values):
-        # validate the unit exist for the OM:Quantity that refersTo
-        if values.get('refersTo').hasUnit is None:
-            raise Exception(f"ContinuousVariable {values.get('instance_iri')} refersTo an OM:Quantity {values.get('refersTo').instance_iri} that has no unit.")
+        # validate the unit exist for the OM:Quantity that refersToQuantity
+        if values.get('refersToQuantity').hasUnit is None:
+            raise Exception(f"ContinuousVariable {values.get('instance_iri')} refersToQuantity an OM:Quantity {values.get('refersToQuantity').instance_iri} that has no unit.")
         return values
 
 class FixedParameter(BaseOntology):
     clz: str = ONTODOE_FIXEDPARAMETER
     positionalID: Optional[str]
-    refersTo: OM_Quantity
+    refersToQuantity: OM_Quantity
 
     def create_instance_for_kg(self, g: Graph):
         if self.positionalID is not None:
             g.add((URIRef(self.instance_iri), URIRef(ONTODOE_POSITIONALID), Literal(self.positionalID)))
 
-        # <fixed_parameter> <OntoDoE:refersTo> <quantity>
+        # <fixed_parameter> <OntoDoE:refersToQuantity> <quantity>
         # <quantity> <rdf:type> <QuantityType>
         # <quantity> <OntoDoE:hasUnit> <unit>
-        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTO), URIRef(self.refersTo.instance_iri)))
-        g.add((URIRef(self.refersTo.instance_iri), RDF.type, URIRef(self.refersTo.clz)))
-        g.add((URIRef(self.refersTo.instance_iri), URIRef(OM_HASVALUE), URIRef(self.refersTo.hasValue.instance_iri)))
-        g = self.refersTo.hasValue.create_instance_for_kg(g)
+        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTOQUANTITY), URIRef(self.refersToQuantity.instance_iri)))
+        g.add((URIRef(self.refersToQuantity.instance_iri), RDF.type, URIRef(self.refersToQuantity.clz)))
+        g.add((URIRef(self.refersToQuantity.instance_iri), URIRef(OM_HASVALUE), URIRef(self.refersToQuantity.hasValue.instance_iri)))
+        g = self.refersToQuantity.hasValue.create_instance_for_kg(g)
 
         return g
 
 
 class CategoricalVariable(DesignVariable):
     clz: str = ONTODOE_CATEGORICALVARIABLE
     name: str=None # NOTE this is not part of OntoDoE ontology, but it is used for working with Summit python package
     hasLevel: List[str]
     positionalID: Optional[str]
-    refersTo: OM_Quantity
+    refersToQuantity: OM_Quantity
 
     def create_instance_for_kg(self, g: Graph):
         g = super().create_instance_for_kg(g)
 
         for level in self.hasLevel:
             g.add((URIRef(self.instance_iri), URIRef(ONTODOE_HASLEVEL), Literal(level)))
 
         if self.positionalID is not None:
             g.add((URIRef(self.instance_iri), URIRef(ONTODOE_POSITIONALID), Literal(self.positionalID)))
 
-        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTO), URIRef(self.refersTo.instance_iri)))
-        g.add((URIRef(self.refersTo.instance_iri), RDF.type, URIRef(self.refersTo.clz)))
-        g.add((URIRef(self.refersTo.instance_iri), URIRef(OM_HASVALUE), URIRef(self.refersTo.hasValue.instance_iri)))
-        g = self.refersTo.hasValue.create_instance_for_kg(g)
+        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTOQUANTITY), URIRef(self.refersToQuantity.instance_iri)))
+        g.add((URIRef(self.refersToQuantity.instance_iri), RDF.type, URIRef(self.refersToQuantity.clz)))
+        g.add((URIRef(self.refersToQuantity.instance_iri), URIRef(OM_HASVALUE), URIRef(self.refersToQuantity.hasValue.instance_iri)))
+        g = self.refersToQuantity.hasValue.create_instance_for_kg(g)
 
         return g
 
 
 class Domain(BaseOntology):
     clz: str = ONTODOE_DOMAIN
     hasDesignVariable: List[DesignVariable]
@@ -186,45 +186,45 @@
                 )
                 if _percent_yield < 0 or _percent_yield > 100:
                     _skip = True
 
             # check for the design variables if they are within the range for this doe campaign
             for var in self.hasDesignVariable:
                 if isinstance(var, ContinuousVariable):
-                    _con = rxn_exp.get_reaction_condition(var.refersTo.clz, var.positionalID)
+                    _con = rxn_exp.get_reaction_condition(var.refersToQuantity.clz, var.positionalID)
                     if _con is None:
                         _skip = True
                         break
                     _dq = unit_conv.DimensionalQuantity(
                         hasUnit=_con.hasValue.hasUnit,
                         hasNumericalValue=_con.hasValue.hasNumericalValue,
-                    ).convert_to(var.refersTo.hasUnit)
+                    ).convert_to(var.refersToQuantity.hasUnit)
                     if not (var.lowerLimit <= _dq.hasNumericalValue <= var.upperLimit):
                         # the reaction experiment does not satisfy the domain, so skip it
                         _skip = True
                         break
                 elif isinstance(var, CategoricalVariable):
                     # TODO [next iteration]: implement checks for categorical variables
                     pass
                 else:
                     raise NotImplementedError(f"Design variable type {type(var)} is not implemented yet.")
 
             # check for fixed parameters if the same, only if the reaction experiment is not skipped
             if not _skip and self.hasFixedParameter is not None:
                 # all fixed parameters must be the same
                 for fixed in self.hasFixedParameter:
-                    _con_fixed = rxn_exp.get_reaction_condition(fixed.refersTo.clz, fixed.positionalID)
+                    _con_fixed = rxn_exp.get_reaction_condition(fixed.refersToQuantity.clz, fixed.positionalID)
                     if _con_fixed is None:
                         _skip = True
                         break
                     _dq_fixed = unit_conv.DimensionalQuantity(
                         hasUnit=_con_fixed.hasValue.hasUnit,
                         hasNumericalValue=_con_fixed.hasValue.hasNumericalValue,
-                    ).convert_to(fixed.refersTo.hasValue.hasUnit)
-                    if not _dq_fixed.hasNumericalValue == fixed.refersTo.hasValue.hasNumericalValue:
+                    ).convert_to(fixed.refersToQuantity.hasValue.hasUnit)
+                    if not _dq_fixed.hasNumericalValue == fixed.refersToQuantity.hasValue.hasNumericalValue:
                         # the reaction experiment does not satisfy the domain, so skip it
                         _skip = True
                         break
 
             if not _skip:
                 filtered_rxn_exp_list.append(rxn_exp)
 
@@ -232,53 +232,53 @@
 
 class SystemResponse(BaseOntology):
     clz: str = ONTODOE_SYSTEMRESPONSE
     name: str=None # NOTE this is not part of OntoDoE ontology, but it is used for working with Summit python package
     maximise: bool
     positionalID: Optional[str]
     # instead of the actual class, str is used to host the concept IRI of om:Quantity for simplicity
-    refersTo: str
+    refersToQuantity: str
 
     def create_instance_for_kg(self, g: Graph):
         g.add((URIRef(self.instance_iri), RDF.type, URIRef(self.clz)))
         g.add((URIRef(self.instance_iri), URIRef(ONTODOE_MAXIMISE), Literal(self.maximise)))
         if self.positionalID is not None:
             g.add((URIRef(self.instance_iri), URIRef(ONTODOE_POSITIONALID), Literal(self.positionalID)))
-        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTO), URIRef(self.refersTo)))
+        g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTOQUANTITY), URIRef(self.refersToQuantity)))
         return g
 
 class HistoricalData(BaseOntology):
     clz: str = ONTODOE_HISTORICALDATA
-    refersTo: Optional[List[ReactionExperiment]]
+    refersToExperiment: Optional[List[ReactionExperiment]]
     numOfNewExp: int = 1
 
     def create_instance_for_kg(self, g: Graph):
         # create instance for HistoricalData
         g.add((URIRef(self.instance_iri), RDF.type, URIRef(self.clz)))
 
         # only add connection if previous data is available
-        if bool(self.refersTo): # if not None and not empty list
+        if bool(self.refersToExperiment): # if not None and not empty list
             # add connection to each ReactionExperiment
             # NOTE here we don't collect triples for each ReactionExperiment, we only make the connection
-            for reaction_experiment in self.refersTo:
-                g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTO), URIRef(reaction_experiment.instance_iri)))
+            for reaction_experiment in self.refersToExperiment:
+                g.add((URIRef(self.instance_iri), URIRef(ONTODOE_REFERSTOEXPERIMENT), URIRef(reaction_experiment.instance_iri)))
 
         # add number of new experiments
         g.add((URIRef(self.instance_iri), URIRef(ONTODOE_NUMOFNEWEXP), Literal(self.numOfNewExp)))
 
         return g
 
 class DesignOfExperiment(BaseOntology):
     clz: str = ONTODOE_DESIGNOFEXPERIMENT
     usesStrategy: Strategy
     hasDomain: Domain
     hasSystemResponse: List[SystemResponse]
     utilisesHistoricalData: HistoricalData
     proposesNewExperiment: Optional[ReactionExperiment]
-    designsChemicalReaction: str # NOTE this should be pointing to OntoCAPE:ChemicalReaction instance, here simplified
+    designsChemicalReaction: str # NOTE this should be pointing to OntoReaction:ChemicalReaction instance, here simplified
 
     def create_instance_for_kg(self, g: Graph):
         # create an instance of DesignOfExperiment
         g.add((URIRef(self.instance_iri), RDF.type, URIRef(self.clz)))
 
         # add the strategy
         g.add((URIRef(self.instance_iri), URIRef(ONTODOE_USESSTRATEGY), URIRef(self.usesStrategy.instance_iri)))
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontohplc.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontohplc.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontolab.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontolab.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     def create_instance_for_kg(self, g: Graph) -> Graph:
         # IRI-ise instance iri of hasQuantity
         quantity_iri = URIRef(self.hasQuantity) if isinstance(self.hasQuantity, str) else URIRef(self.hasQuantity.instance_iri)
         # <paramSetting> <rdf:type> <self.clz>
         g.add((URIRef(self.instance_iri), RDF.type, URIRef(self.clz)))
         # <paramSetting> <OntoLab:hasQuantity> <quantity>
         g.add((URIRef(self.instance_iri), URIRef(ONTOLAB_HASQUANTITY), quantity_iri))
-        # <quantity> <OntoLab:translatesToParameterSetting> <paramSetting>
-        g.add((quantity_iri, URIRef(ONTOLAB_TRANSLATESTOPARAMETERSETTING), URIRef(self.instance_iri)))
 
         return g
 
 class TemperatureSetting(ParameterSetting):
     clz: str = ONTOLAB_TEMPERATURESETTING
 
 class DurationSetting(ParameterSetting):
@@ -69,23 +67,19 @@
         if self.wasGeneratedFor == None:
             raise Exception("ReactionExperiment is not provided when writing triples about <%s> to the KG." % self.instance_iri)
 
         # <equip_settings> <rdf:type> <OntoLab:EquipmentSettings>
         g.add((URIRef(self.instance_iri), RDF.type, URIRef(self.clz)))
         # <equip_settings> <OntoLab:wasGeneratedFor> <rxnexp>
         g.add((URIRef(self.instance_iri), URIRef(ONTOLAB_WASGENERATEDFOR), URIRef(self.wasGeneratedFor)))
-        # <reactionExperiment> <OntoReaction:hasEquipmentSettings> <reactorSetting>
-        g.add((URIRef(self.wasGeneratedFor), URIRef(ONTOREACTION_HASEQUIPMENTSETTINGS), URIRef(self.instance_iri)))
 
         # NOTE the links between <equip_settings> and <lab_equipment> are optional depends on if one want to configure the digital twin
         if configure_digital_twin:
             # <equip_settings> <OntoLab:specifies> <lab_equipment>
             g.add((URIRef(self.instance_iri), URIRef(ONTOLAB_SPECIFIES), URIRef(self.specifies.instance_iri)))
-            # <lab_equipment> <OntoLab:isSpecifiedBy> <equip_settings>
-            g.add((URIRef(self.specifies.instance_iri), URIRef(ONTOLAB_ISSPECIFIEDBY), URIRef(self.instance_iri)))
 
         return g
 
 class PowerSupply(BaseOntology):
     pass
 
 class Laboratory(BaseOntology):
@@ -96,18 +90,16 @@
 
 class Saref_State(BaseOntology):
     clz: str = SAREF_STATE
 
 class LabEquipment(Saref_Device):
     clz: str = ONTOLAB_LABEQUIPMENT
     manufacturer: str # it should be pointing to an instance of https://dbpedia.org/ontology/Organisation, but we simplified here
-    isContainedIn: Union[str, Laboratory] # NOTE here str is provided as an optional as it seems impossible to circular reference at instance level
     hasPowerSupply: Union[str, PowerSupply] # NOTE TODO [future work] here str is provided as an optional to simplify the implementation
     consistsOf: Optional[List[LabEquipment]] = None
-    isSpecifiedBy: Optional[EquipmentSettings] = None
     # TODO [future work] add support for hasHeight, hasLength, hasPrice, hasWeight, and hasWidth
     isManagedBy: Optional[str] # NOTE here str is provided, this should refer to the iri of agent service
 
     def consists_of_lab_equipment(self, lab_equipment_iris: List[str]) -> bool:
         return bool([le for le in self.consistsOf if le.instance_iri in lab_equipment_iris])
 
 class PreparationMethod(BaseOntology):
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontoreaction.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontoreaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,16 +304,16 @@
 
 class TargetProduct(OntoKin_Product):
     clz: str = ONTOREACTION_TARGETPRODUCT
 
 class Impurity(OntoKin_Product):
     clz: str = ONTOREACTION_IMPURITY
 
-class OntoCAPE_ChemicalReaction(BaseOntology):
-    clz: str = ONTOCAPE_CHEMICALREACTION
+class ChemicalReaction(BaseOntology):
+    clz: str = ONTOREACTION_CHEMICALREACTION
     hasReactant: List[OntoKin_Species]
     hasProduct: List[OntoKin_Species]
     hasCatalyst: Optional[List[OntoKin_Species]]
     hasSolvent: Optional[List[OntoKin_Species]]
     hasBase: Optional[List[OntoKin_Species]]
     # NOTE here we simplify the implementation by using str instead of the actual OntoDoE:DesignOfExperiment
     # NOTE this is to prevent circular import error
@@ -351,34 +351,34 @@
         return [s.hasUniqueSpecies for s in self.hasBase]
 
 
 class ReactionCondition(BaseOntology):
     objPropWithExp: List[str]
     hasValue: OM_Measure
     positionalID: Optional[str] = None
-    translateToParameterSetting: Optional[str] # NOTE here we put str to simplify the implementation, should be ontolab.ParameterSetting
+    translateToParameterSetting: Optional[str] # NOTE this doesn't belong to ontology, we just put it here for testing purpose
     # instead of the actual class, str is used to host the instance IRI of OntoReaction:InputChemical for simplicity
     # StoichiometryRatio indicatesMultiplicityOf InputChemical
     indicatesMultiplicityOf: Optional[str] = None
     # instead of the actual class, str is used to host the instance IRI of OntoReaction:InputChemical for simplicity
-    # ReactionScale indicateUsageOf InputChemical
-    indicateUsageOf: Optional[str] = None
+    # ReactionScale indicatesUsageOf InputChemical
+    indicatesUsageOf: Optional[str] = None
 
     @pydantic.root_validator
     @classmethod
     def input_chemical_validation(cls, values):
         if values.get('clz') == ONTOREACTION_STOICHIOMETRYRATIO:
             if values.get('indicatesMultiplicityOf') == None:
                 raise Exception(
                     'StoichiometryRatio <%s> is not indicatesMultiplicityOf any InputChemical, received values: %s.' % (values.get('instance_iri'), str(values))
                 )
         elif values.get('clz') == ONTOREACTION_REACTIONSCALE:
-            if values.get('indicateUsageOf') == None:
+            if values.get('indicatesUsageOf') == None:
                 raise Exception(
-                    'ReactionScale <%s> is not indicateUsageOf any InputChemical, received values: %s.' % (values.get('instance_iri'), str(values))
+                    'ReactionScale <%s> is not indicatesUsageOf any InputChemical, received values: %s.' % (values.get('instance_iri'), str(values))
                 )
         return values
 
     def create_instance_for_kg(self, g: Graph) -> Graph:
         # IRI-ise the IRI of ReactionCondition instance to be used by rdflib package
         con_iri = URIRef(self.instance_iri)
 
@@ -394,16 +394,16 @@
 
         # Only add positionalID if it exists
         if self.positionalID is not None:
             g.add((con_iri, URIRef(ONTODOE_POSITIONALID), Literal(self.positionalID)))
         # Also add indicatesMultiplicityOf/indicatesUsageOf if it's a OntoReaction:StoichiometryRatio/OntoReaction:ReactionScale
         if self.indicatesMultiplicityOf is not None:
             g.add((con_iri, URIRef(ONTOREACTION_INDICATESMULTIPLICITYOF), URIRef(self.indicatesMultiplicityOf)))
-        if self.indicateUsageOf is not None:
-            g.add((con_iri, URIRef(ONTOREACTION_INDICATESUSAGEOF), URIRef(self.indicateUsageOf)))
+        if self.indicatesUsageOf is not None:
+            g.add((con_iri, URIRef(ONTOREACTION_INDICATESUSAGEOF), URIRef(self.indicatesUsageOf)))
 
         return g
 
 # TODO [future work] a design choice to be made: are below specific dataclass useful?
 # @dataclass
 # class ResidenceTime(ReactionCondition):
 #     pass
@@ -418,15 +418,15 @@
 
 # @dataclass
 # class StoichiometryRatio(ReactionCondition):
 #     indicatesMultiplicityOf: str # indicatesMultiplicityOf: InputChemical
 
 # @dataclass
 # class ReactionScale(ReactionCondition):
-#     indicateUsageOf: str # indicateUsageOf: InputChemical
+#     indicatesUsageOf: str # indicatesUsageOf: InputChemical
 
 class PerformanceIndicator(BaseOntology):
     rxn_exp_iri: str
     objPropWithExp: List[str]
     hasValue: Optional[OM_Measure]
     positionalID: Optional[int] = None
     yieldLimitingSpecies: Optional[str] = None
@@ -489,15 +489,15 @@
 class ReactionExperiment(BaseOntology):
     hasReactionCondition: Optional[List[ReactionCondition]] = None
     hasPerformanceIndicator: Optional[List[PerformanceIndicator]] = None
     hasInputChemical: Optional[List[InputChemical]] = None
     hasOutputChemical: Optional[List[OutputChemical]] = None
     isAssignedTo: Optional[str] # NOTE here it should be pointing to OntoVapourtec:VapourtecR4Reactor, but we put str to simplify the implementation
     clz: str = ONTOREACTION_REACTIONEXPERIMENT
-    isOccurenceOf: Optional[OntoCAPE_ChemicalReaction] = None
+    isOccurenceOf: Optional[ChemicalReaction] = None
 
     @pydantic.root_validator
     @classmethod
     def if_exp_assigned(cls, values):
         if 'namespace_for_init' not in values: # means we are not creating a new reaction experiment that yet to be uploaded to the KG, i.e. we are pulling existing data from the KG
             if values.get('isAssignedTo') == None and values.get('hasOutputChemical') != None:
                 raise Exception(
@@ -506,15 +506,15 @@
         return values
 
     def get_reference_input_chemical(self) -> Optional[InputChemical]:
         if self.hasInputChemical is None:
             return None
         reaction_scale = self.get_reaction_scale()
         for input_chemical in self.hasInputChemical:
-            if input_chemical.instance_iri == reaction_scale.indicateUsageOf:
+            if input_chemical.instance_iri == reaction_scale.indicatesUsageOf:
                 return input_chemical
         return None
 
     def get_reaction_scale(self, positionalID: str=None) -> Optional[ReactionCondition]:
         if positionalID is None:
             reaction_scale = self.get_reaction_condition(ONTOREACTION_REACTIONSCALE)
             if reaction_scale is None:
@@ -603,15 +603,15 @@
         if self.hasInputChemical is None:
             raise Exception(f"None of InputChemical is set up for {self.instance_iri}")
 
         if self.hasOutputChemical is not None:
             raise Exception(f"OutputChemical is already set for {self.instance_iri}: {self.hasOutputChemical}")
 
         if self.isOccurenceOf is None:
-            raise Exception(f"OntoCAPE:ChemicalReaction is not set up for {self.instance_iri}")
+            raise Exception(f"OntoReaction:ChemicalReaction is not set up for {self.instance_iri}")
 
         if self.isAssignedTo is not None:
             raise Exception(f"OntoVapourtec:VapourtecR4Reactor is already assigned for {self.instance_iri}: {self.isAssignedTo}")
 
         # Add below triples:
         # <reactionExperimentIRI> <rdf:type> <OntoReaction:ReactionExperiment> .
         g.add((URIRef(self.instance_iri), RDF.type, URIRef(ONTOREACTION_REACTIONEXPERIMENT)))
@@ -630,15 +630,15 @@
 
         # <reactionExperimentIRI> <OntoReaction:hasInputChemical> <inputChemicalIRI> .
         # NOTE that the InputChemical instance should exist in KG already before suggesting this experiment
         # NOTE therefore, here we only add the connection between the ReactionExperiment and InputChemical instances
         for input_chemical in self.hasInputChemical:
             g.add((URIRef(self.instance_iri), URIRef(ONTOREACTION_HASINPUTCHEMICAL), URIRef(input_chemical.instance_iri)))
 
-        # <reactionExperimentIRI> <OntoReaction:isOccurenceOf> <OntoCAPE:ChemicalReaction> .
+        # <reactionExperimentIRI> <OntoReaction:isOccurenceOf> <OntoReaction:ChemicalReaction> .
         g.add((URIRef(self.instance_iri), URIRef(ONTOREACTION_ISOCCURENCEOF), URIRef(self.isOccurenceOf.instance_iri)))
 
         return g
 
 class ReactionVariation(ReactionExperiment):
     isVariationOf: Optional[ReactionExperiment] = None
     clz: str = ONTOREACTION_REACTIONVARIATION
@@ -661,19 +661,17 @@
         # IRI-ise the ReactionExperiment instance to be used by rdflib package
         rxn_iri = URIRef(self.isVariationOf.instance_iri)
         rxnvar_iri = URIRef(self.instance_iri)
 
         # Add below triples:
         # <reactionVariationIRI> <rdf:type> <OntoReaction:ReactionVariation> .
         # <reactionVariationIRI> <OntoReaction:isVariationOf> <reactionExperimentIRI> .
-        # <reactionExperimentIRI> <OntoReaction:hasVariation> <reactionVariationIRI> .
         g.add((rxnvar_iri, RDF.type, URIRef(ONTOREACTION_REACTIONVARIATION)))
         g.add((rxnvar_iri, URIRef(ONTOREACTION_ISVARIATIONOF), rxn_iri))
-        g.add((rxn_iri, URIRef(ONTOREACTION_HASVARIATION), rxnvar_iri))
-        
+
         for con in self.hasReactionCondition:
             # Attach the ReactionCondition instance to the OntoReaction:ReactionVariation instance
             # As we are stating the <reactionVariationIRI> <OntoReaction:isVariationOf> <reactionExperimentIRI>
             # we are using the list of the same object properties between the <reactionExperimentIRI> and the instance of ReactionCondition
             for rela in con.objPropWithExp:
                 g.add((rxnvar_iri, URIRef(rela), URIRef(con.instance_iri)))
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/ontovapourtec.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/ontovapourtec.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,14 @@
         if self.pumpsLiquidFrom is not None:
             g.add((URIRef(self.instance_iri), URIRef(ONTOVAPOURTEC_PUMPSLIQUIDFROM), URIRef(self.pumpsLiquidFrom.instance_iri)))
 
         return super().create_instance_for_kg(g, configure_digital_twin)
 
 class Vial(ChemicalContainer):
     clz: str = ONTOLAB_VIAL
-    isHeldIn: str # NOTE here we simplify the implementation to use str instead of the actual AutoSamplerSite
 
 class AutoSamplerSite(BaseOntology):
     clz: str = ONTOVAPOURTEC_AUTOSAMPLERSITE
     holds: Vial
     locationID: str
 
     def get_chemical_given_chemical_species(
@@ -444,15 +443,15 @@
 
         assigned_pumps = []
         assignment = {} # key: input chemical iri, value: pump locationID
         for input_chem in rxn_exp.hasInputChemical:
             autosampler_site = None # initialise autosampler_site as None
 
             # note that if the ReactionScale is specified, then we also need to set the sample volume for the pump
-            if input_chem.instance_iri == reaction_scale.indicateUsageOf:
+            if input_chem.instance_iri == reaction_scale.indicatesUsageOf:
                 # if this is the reference reactant then it also MUST be the reference pump
                 ref_pump_chem_amount = reference_pump.get_reagent_chemical_amount()
                 if ref_pump_chem_amount is not None:
                     # this means the reference_pump is pumping liquid from ReagentBottle
                     # therefore, the chemical in this pump must be the same as the reference chemical
                     if ref_pump_chem_amount.refersToMaterial.thermodynamicBehaviour != input_chem.thermodynamicBehaviour:
                         raise Exception(
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/data_model/unit_conversion.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/data_model/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/hardware/hplc.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/hardware/hplc.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/kg_operations/dict_and_list.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/kg_operations/dict_and_list.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/kg_operations/sparql_client.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/kg_operations/sparql_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,65 @@
 from pyderivationagent.data_model import *
 
 from chemistry_and_robots.data_model import *
 from chemistry_and_robots.hardware import hplc
 
 from chemistry_and_robots.kg_operations import dict_and_list as dal
 
+from chemistry_and_robots.resources import TBOX_PATH_DICT
+from chemistry_and_robots import __version__
+
 from py4jps import agentlogging
 logger = agentlogging.get_logger('dev')
 
 
 class ChemistryAndRobotsSparqlClient(PySparqlClient):
+    def get_ontology_tbox_version(self, tbox_namespace):
+        if not tbox_namespace:
+            raise Exception("No TBox namespace provided.")
+        if TBOX_PATH_DICT.get(tbox_namespace) is None:
+            raise Exception(f"TBox namespace {tbox_namespace} is NOT packaged in chemistry_and_robots=={__version__}.")
+        g = Graph().parse(TBOX_PATH_DICT.get(tbox_namespace), format='xml')
+        results = g.query(f'SELECT ?v WHERE {{ <{tbox_namespace}> <{OWL_VERSION}> ?v. }}')
+        for row in results:
+            return str(row['v'])
+
+    def upload_ontology_tbox(self, tbox_namespace, alternative_url=None):
+        try:
+            query = f'SELECT * WHERE {{ <{tbox_namespace}> <{OWL_VERSION}> ?v. }}'
+            res = self.performQuery(query)
+        except Exception as ex:
+            logger.error("Unable to retrieve TBox version from KG.")
+            raise Exception("Unable to retrieve TBox version from KG.") from ex
+
+        # Upload TBox if not already instantiated
+        if not res:
+            if not alternative_url:
+                # Upload TBox from local file by default
+                self.uploadOntology(TBOX_PATH_DICT.get(tbox_namespace))
+            else:
+                # Upload TBox from alternative URL if provided
+                temp_fp = '_tmp.owl'
+                url_to_upload = alternative_url
+                try:
+                    try:
+                        content = requests.get(url_to_upload)
+                        if content.status_code != 200:
+                            raise Exception(f'HTTP error code for retrieving owl file: {content.status_code}')
+                    except Exception as ex:
+                        raise Exception(f"Unable to retrieve {url_to_upload} from TWA server.") from ex
+                    with open(temp_fp, 'w') as f:
+                        f.write(content.text)
+                        self.uploadOntology(temp_fp)
+                    os.remove(temp_fp)
+                except Exception as ex:
+                    raise Exception(f"Unable to initialise knowledge graph with {tbox_namespace} TBox ({url_to_upload}).") from ex
+
     def get_all_chemical_reaction_iri(self):
-        query = f"""SELECT ?chem_rxn WHERE {{ ?chem_rxn a <{ONTOCAPE_CHEMICALREACTION}>. }}"""
+        query = f"""SELECT ?chem_rxn WHERE {{ ?chem_rxn a <{ONTOREACTION_CHEMICALREACTION}>. }}"""
         response = self.performQuery(query)
         return [list(res.values())[0] for res in response]
 
     def get_all_rxn_exp_given_chem_rxn(self, chem_rxn_iri: str):
         chem_rxn_iri = trimIRI(chem_rxn_iri)
         query = f"""SELECT DISTINCT ?rxn_exp
                     WHERE {{
@@ -91,18 +135,18 @@
                           <{doe_iri}> <{ONTODOE_USESSTRATEGY}> ?strategy;
                                       <{ONTODOE_HASDOMAIN}> ?domain;
                                       <{ONTODOE_UTILISESHISTORICALDATA}> ?hist_data;
                                       <{ONTODOE_DESIGNSCHEMICALREACTION}> ?chem_rxn.
                       }}"""
         response_1 = self.performQuery(query_1)
         if len(response_1) > 1:
-            raise Exception("OntoDoE:DesignOfExperiment instance <%s> is associated with multiple entries of OntoDoE:Strategy/Domain/HistoricalData/OntoCAPE:ChemicalReaction: %s" % (
+            raise Exception("OntoDoE:DesignOfExperiment instance <%s> is associated with multiple entries of OntoDoE:Strategy/Domain/HistoricalData/OntoReaction:ChemicalReaction: %s" % (
                 doe_iri, str(response_1)))
         elif len(response_1) < 1:
-            raise Exception("OntoDoE:DesignOfExperiment instance <%s> is NOT associated with any entries of OntoDoE:Strategy/Domain/HistoricalData/OntoCAPE:ChemicalReaction" % (doe_iri))
+            raise Exception("OntoDoE:DesignOfExperiment instance <%s> is NOT associated with any entries of OntoDoE:Strategy/Domain/HistoricalData/OntoReaction:ChemicalReaction" % (doe_iri))
         else:
             r = response_1[0]
 
         query_2 = f"""SELECT ?sys_res WHERE {{ <{doe_iri}> <{ONTODOE_HASSYSTEMRESPONSE}> ?sys_res. }}"""
         response_2 = self.performQuery(query_2)
 
         doe_instance = DesignOfExperiment(
@@ -133,27 +177,27 @@
         return domain_instance
 
     def get_fixed_parameters(self, domain_iri: str) -> Optional[List[FixedParameter]]:
         domain_iri = trimIRI(domain_iri)
         query = f"""SELECT ?param ?quantity ?clz ?measure ?unit ?value ?id
                     WHERE {{
                         <{domain_iri}> <{ONTODOE_HASFIXEDPARAMETER}> ?param.
-                        ?param <{ONTODOE_REFERSTO}> ?quantity .
+                        ?param <{ONTODOE_REFERSTOQUANTITY}> ?quantity .
                         ?quantity a ?clz; <{OM_HASVALUE}> ?measure.
                         ?measure <{OM_HASUNIT}> ?unit; <{OM_HASNUMERICALVALUE}> ?value.
                         OPTIONAL {{?param <{ONTODOE_POSITIONALID}> ?id . }}
                     }}"""
         response = self.performQuery(query)
 
         list_param = []
         for res in response:
             list_param.append(FixedParameter(
                 instance_iri=res['param'],
                 positionalID=res['id'] if 'id' in res else None,
-                refersTo=OM_Quantity(
+                refersToQuantity=OM_Quantity(
                     instance_iri=res['quantity'],
                     clz=res['clz'],
                     hasValue=OM_Measure(
                         instance_iri=res['measure'],
                         hasUnit=res['unit'],
                         hasNumericalValue=res['value']
                     )
@@ -173,15 +217,15 @@
         domain_iri = trimIRI(domain_iri)
 
         # Prepare query string
         query_continuous = f"""SELECT DISTINCT ?var ?quantity ?clz ?unit ?id ?lower ?upper
                 WHERE {{
                     <{domain_iri}> <{ONTODOE_HASDESIGNVARIABLE}> ?var .
                     ?var a <{ONTODOE_CONTINUOUSVARIABLE}> .
-                    ?var <{ONTODOE_REFERSTO}> ?quantity .
+                    ?var <{ONTODOE_REFERSTOQUANTITY}> ?quantity .
                     ?quantity a ?clz; <{OM_HASUNIT}> ?unit.
                     OPTIONAL {{?var <{ONTODOE_POSITIONALID}> ?id . }}
                     OPTIONAL {{?var <{ONTODOE_LOWERLIMIT}> ?lower . }}
                     OPTIONAL {{?var <{ONTODOE_UPPERLIMIT}> ?upper . }}
                 }}"""
 
         # Perform query
@@ -193,30 +237,30 @@
             list_var.append(
                 ContinuousVariable(
                     instance_iri=res['var'],
                     name=getShortName(res['var']), # NOTE this is not part of OntoDoE ontology, but it is used for working with Summit python package
                     upperLimit=res['upper'],
                     lowerLimit=res['lower'],
                     positionalID=res['id'] if 'id' in res else None,
-                    refersTo=OM_Quantity(
+                    refersToQuantity=OM_Quantity(
                         instance_iri=res['quantity'],
                         clz=res['clz'],
                         hasUnit=res['unit']
                     )
                 )
             )
 
         # Query for categorical variables
         query_categorical = f"""
             SELECT DISTINCT ?var ?cat ?quantity ?clz ?measure ?unit ?value ?id
             WHERE {{
                 <{domain_iri}> <{ONTODOE_HASDESIGNVARIABLE}> ?var .
                 ?var a <{ONTODOE_CATEGORICALVARIABLE}>.
                 ?var <{ONTODOE_HASLEVEL}> ?cat.
-                ?var <{ONTODOE_REFERSTO}> ?quantity .
+                ?var <{ONTODOE_REFERSTOQUANTITY}> ?quantity .
                 ?quantity a ?clz; <{OM_HASVALUE}> ?measure.
                 ?measure <{OM_HASUNIT}> ?unit; <{OM_HASNUMERICALVALUE}> ?value.
                 OPTIONAL {{?var <{ONTODOE_POSITIONALID}> ?id . }}
             }}
             """
         response = self.performQuery(query_categorical)
         _var = dal.get_unique_values_in_list_of_dict(response, 'var')
@@ -224,15 +268,15 @@
             # NOTE we assume that each categorical variable only refers to ONE quantity
             _info_v = dal.get_sublist_in_list_of_dict_matching_key_value(response, 'var', _v) # info for a single categorical variable
             list_var.append(
                 CategoricalVariable(
                     instance_iri=_v,
                     name=getShortName(_v), # NOTE this is not part of OntoDoE ontology, but it is used for working with Summit python package
                     hasLevel=dal.get_unique_values_in_list_of_dict(_info_v, 'cat'),
-                    refersTo=OM_Quantity(
+                    refersToQuantity=OM_Quantity(
                         instance_iri=_info_v[0]['quantity'],
                         clz=_info_v[0]['clz'],
                         hasValue=OM_Measure(
                             instance_iri=_info_v[0]['measure'],
                             hasUnit=_info_v[0]['unit'],
                             hasNumericalValue=_info_v[0]['value']
                         )
@@ -260,24 +304,24 @@
         for sys_ins in systemResponse_iris:
             # Prepare query string
             query = """SELECT DISTINCT ?clz ?id ?maximise \
                     WHERE { \
                     <%s> <%s> ?clz . 
                     OPTIONAL {<%s> <%s> ?id} \
                     OPTIONAL {<%s> <%s> ?maximise} \
-                    }""" % (sys_ins, ONTODOE_REFERSTO, sys_ins, ONTODOE_POSITIONALID, sys_ins, ONTODOE_MAXIMISE)
+                    }""" % (sys_ins, ONTODOE_REFERSTOQUANTITY, sys_ins, ONTODOE_POSITIONALID, sys_ins, ONTODOE_MAXIMISE)
             # Perform query
             response = self.performQuery(query)
             list_sys.append(
                 SystemResponse(
                     instance_iri=sys_ins,
                     name=getShortName(sys_ins), # NOTE this is not part of OntoDoE ontology, but it is used for working with Summit python package
                     maximise=response[0]['maximise'],
                     positionalID=response[0]['id'] if 'id' in response[0] else None,
-                    refersTo=response[0]['clz']
+                    refersToQuantity=response[0]['clz']
                 )
             )
             
         return list_sys
 
     def getDoEHistoricalData(self, historicalData_iri: str) -> HistoricalData:
         """
@@ -287,30 +331,30 @@
                 historicalData_iri - iri of OntoDoE:HistoricalData instance
         """
         # Delete "<" and ">" around the IRI
         historicalData_iri = trimIRI(historicalData_iri)
 
         query = f"""SELECT DISTINCT ?exp ?numOfNewExp
                 WHERE {{
-                    OPTIONAL {{<{historicalData_iri}> <{ONTODOE_REFERSTO}> ?exp .}}
+                    OPTIONAL {{<{historicalData_iri}> <{ONTODOE_REFERSTOEXPERIMENT}> ?exp .}}
                     OPTIONAL {{<{historicalData_iri}> <{ONTODOE_NUMOFNEWEXP}> ?numOfNewExp .}}
                 }}"""
 
         response = self.performQuery(query)
 
         num_ = [res['numOfNewExp'] for res in response if 'numOfNewExp' in res]
         if num_.count(num_[0]) != len(num_):
             raise Exception("There are multiple instances of numOfNewExp associated with OntoDoE:HistoricalData instance <" + historicalData_iri + ">: " + collections.Counter(num_).keys)
 
         rxnexp_iris = [res['exp'] for res in response if 'exp' in res]
 
         historicalData_instance = HistoricalData(
             instance_iri=historicalData_iri,
             numOfNewExp=int(num_[0]) if bool(num_) else HistoricalData.__fields__.get('numOfNewExp').default,
-            refersTo=self.getReactionExperiment(rxnexp_iris) if bool(rxnexp_iris) else None,
+            refersToExperiment=self.getReactionExperiment(rxnexp_iris) if bool(rxnexp_iris) else None,
         )
 
         return historicalData_instance
 
     def getReactionExperiment(self, rxnexp_iris: Union[str, list]) -> List[ReactionExperiment]:
         """
             This method retrieves information given a list of instance iri of OntoReaction:ReactionExperiment.
@@ -386,15 +430,15 @@
                         isAssignedTo=dict_assigned_reactor[rxnexp_iri],
                         isOccurenceOf=dict_chemical_reaction[rxnexp_iri],
                         isVariationOf=dict_exp[dict_variation_of[rxnexp_iri]],
                     )
                 )
         return list_exp
 
-    def get_chemical_reaction(self, rxnexp_iris: Union[str, list]) -> Dict[str, OntoCAPE_ChemicalReaction]:
+    def get_chemical_reaction(self, rxnexp_iris: Union[str, list]) -> Dict[str, ChemicalReaction]:
         if not isinstance(rxnexp_iris, list):
             rxnexp_iris = [rxnexp_iris]
         rxnexp_iris = trimIRI(rxnexp_iris)
         query_mapping = f"""SELECT DISTINCT ?rxn ?chem_rxn
                             WHERE {{
                                 VALUES ?rxn {{ <{'> <'.join(rxnexp_iris)}> }}
                                 ?rxn <{ONTOREACTION_ISVARIATIONOF}>?/<{ONTOREACTION_ISOCCURENCEOF}> ?chem_rxn.
@@ -403,15 +447,15 @@
         dict_rxn_chem_mapping = {}
         for r in response_mapping:
             rxn_iri = r['rxn']
             chem_rxn_iri = r['chem_rxn']
             if rxn_iri not in dict_rxn_chem_mapping:
                 dict_rxn_chem_mapping[rxn_iri] = chem_rxn_iri
             else:
-                raise Exception(f"OntoReaction:ReactionExperiment instance <{rxn_iri}> is found to be occurence of multiple OntoCAPE:ChemicalReaction instance: {dal.get_sublist_in_list_of_dict_matching_key_value(response_mapping, 'rxn', rxn_iri)}")
+                raise Exception(f"OntoReaction:ReactionExperiment instance <{rxn_iri}> is found to be occurence of multiple OntoReaction:ChemicalReaction instance: {dal.get_sublist_in_list_of_dict_matching_key_value(response_mapping, 'rxn', rxn_iri)}")
 
         lst_unique_chem_rxn = dal.get_unique_values_in_list_of_dict(response_mapping, 'chem_rxn')
         query = f"""{PREFIX_RDF}
                     SELECT DISTINCT ?chem_rxn ?reactant ?reac_type ?reac_species ?product ?prod_type ?prod_species
                     ?catalyst ?cata_type ?cata_species ?solvent ?solv_type ?solv_species ?base ?base_type ?base_species
                     ?doe_template
                     WHERE {{
@@ -419,15 +463,15 @@
                         VALUES ?prod_type {{<{ONTOKIN_SPECIES}> <{ONTOKIN_PRODUCT}> <{ONTOREACTION_TARGETPRODUCT}> <{ONTOREACTION_IMPURITY}>}}.
                         VALUES ?chem_rxn {{ <{'> <'.join(lst_unique_chem_rxn)}> }}
                         ?chem_rxn <{ONTOCAPE_HASREACTANT}> ?reactant; <{ONTOCAPE_HASPRODUCT}> ?product.
                         ?reactant rdf:type ?reac_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?reac_species.
                         ?product rdf:type ?prod_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?prod_species.
                         OPTIONAL{{
                             VALUES ?cata_type {{<{ONTOKIN_SPECIES}> <{ONTOREACTION_CATALYST}>}}.
-                            ?chem_rxn <{ONTOCAPE_CATALYST}> ?catalyst.
+                            ?chem_rxn <{ONTOREACTION_HASCATALYST}> ?catalyst.
                             ?catalyst rdf:type ?cata_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?cata_species.
                         }}
                         OPTIONAL{{
                             VALUES ?solv_type {{<{ONTOKIN_SPECIES}> <{ONTOREACTION_SOLVENT}>}}.
                             ?chem_rxn <{ONTOREACTION_HASSOLVENT}> ?solvent.
                             ?solvent rdf:type ?solv_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?solv_species.
                         }}
@@ -435,20 +479,20 @@
                             VALUES ?base_type {{<{ONTOKIN_SPECIES}> <{ONTOREACTION_BASE}>}}.
                             ?chem_rxn <{ONTOREACTION_HASBASE}> ?base.
                             ?base rdf:type ?base_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?base_species.
                         }}
                         OPTIONAL{{?chem_rxn <{ONTODOE_HASDOETEMPLATE}> ?doe_template.}}
                     }}"""
         response_of_all_chem_rxn = self.performQuery(query)
-        dict_chem_rxn = {} # key: chem_rxn_iri, value: OntoCAPE_ChemicalReaction
+        dict_chem_rxn = {} # key: chem_rxn_iri, value: ChemicalReaction
 
         for iri in lst_unique_chem_rxn:
             response = dal.get_sublist_in_list_of_dict_matching_key_value(response_of_all_chem_rxn, 'chem_rxn', iri)
 
-            chem_rxn = OntoCAPE_ChemicalReaction(
+            chem_rxn = ChemicalReaction(
                 instance_iri=iri,
                 hasReactant=self.get_ontokin_species_from_chem_rxn(response, 'reactant', 'reac_type', 'reac_species'),
                 hasProduct=self.get_ontokin_species_from_chem_rxn(response, 'product', 'prod_type', 'prod_species'),
                 hasCatalyst=self.get_ontokin_species_from_chem_rxn(response, 'catalyst', 'cata_type', 'cata_species'),
                 hasSolvent=self.get_ontokin_species_from_chem_rxn(response, 'solvent', 'solv_type', 'solv_species'),
                 hasBase=self.get_ontokin_species_from_chem_rxn(response, 'base', 'base_type', 'base_species'),
                 hasDoETemplate=dal.get_the_unique_value_in_list_of_dict(response, 'doe_template'),
@@ -458,30 +502,30 @@
 
         dict_exp_chem_rxn = {}
         for exp in rxnexp_iris:
             dict_exp_chem_rxn[exp] = dict_chem_rxn[dict_rxn_chem_mapping[exp]]
 
         return dict_exp_chem_rxn
 
-    def get_chemical_reaction_given_iri(self, chem_rxn_iri: str) -> OntoCAPE_ChemicalReaction:
+    def get_chemical_reaction_given_iri(self, chem_rxn_iri: str) -> ChemicalReaction:
         chem_rxn_iri = trimIRI(chem_rxn_iri)
         query = f"""{PREFIX_RDF}
                 SELECT DISTINCT ?chem_rxn ?reactant ?reac_type ?reac_species ?product ?prod_type ?prod_species
                 ?catalyst ?cata_type ?cata_species ?solvent ?solv_type ?solv_species ?base ?base_type ?base_species
                     ?doe_template
                 WHERE {{
                     VALUES ?reac_type {{<{ONTOKIN_SPECIES}> <{ONTOKIN_REACTANT}>}}.
                     VALUES ?prod_type {{<{ONTOKIN_SPECIES}> <{ONTOKIN_PRODUCT}> <{ONTOREACTION_TARGETPRODUCT}> <{ONTOREACTION_IMPURITY}>}}.
                     VALUES ?chem_rxn {{<{chem_rxn_iri}>}}.
                     ?chem_rxn <{ONTOCAPE_HASREACTANT}> ?reactant; <{ONTOCAPE_HASPRODUCT}> ?product.
                     ?reactant rdf:type ?reac_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?reac_species.
                     ?product rdf:type ?prod_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?prod_species.
                     OPTIONAL{{
                         VALUES ?cata_type {{<{ONTOKIN_SPECIES}> <{ONTOREACTION_CATALYST}>}}.
-                        ?chem_rxn <{ONTOCAPE_CATALYST}> ?catalyst.
+                        ?chem_rxn <{ONTOREACTION_HASCATALYST}> ?catalyst.
                         ?catalyst rdf:type ?cata_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?cata_species.
                     }}
                     OPTIONAL{{
                         VALUES ?solv_type {{<{ONTOKIN_SPECIES}> <{ONTOREACTION_SOLVENT}>}}.
                         ?chem_rxn <{ONTOREACTION_HASSOLVENT}> ?solvent.
                         ?solvent rdf:type ?solv_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?solv_species.
                     }}
@@ -490,15 +534,15 @@
                         ?chem_rxn <{ONTOREACTION_HASBASE}> ?base.
                         ?base rdf:type ?base_type; <{ONTOSPECIES_HASUNIQUESPECIES}> ?base_species.
                     }}
                     OPTIONAL{{?chem_rxn <{ONTODOE_HASDOETEMPLATE}> ?doe_template.}}
                 }}"""
         response = self.performQuery(query)
 
-        chem_rxn = OntoCAPE_ChemicalReaction(
+        chem_rxn = ChemicalReaction(
             instance_iri=chem_rxn_iri,
             hasReactant=self.get_ontokin_species_from_chem_rxn(response, 'reactant', 'reac_type', 'reac_species'),
             hasProduct=self.get_ontokin_species_from_chem_rxn(response, 'product', 'prod_type', 'prod_species'),
             hasCatalyst=self.get_ontokin_species_from_chem_rxn(response, 'catalyst', 'cata_type', 'cata_species'),
             hasSolvent=self.get_ontokin_species_from_chem_rxn(response, 'solvent', 'solv_type', 'solv_species'),
             hasBase=self.get_ontokin_species_from_chem_rxn(response, 'base', 'base_type', 'base_species'),
             hasDoETemplate=dal.get_the_unique_value_in_list_of_dict(response, 'doe_template'),
@@ -715,24 +759,23 @@
                 dict_chemical[subject_iri] = lst_chemical
 
         return dict_chemical
 
     def construct_query_for_autosampler(self, given_autosampler_iri: str = None) -> str:
         # TODO this query will return nothing if the autosampler is an empty rack on line "?site <{ONTOVAPOURTEC_HOLDS}> ?vial; <{ONTOVAPOURTEC_LOCATIONID}> ?loc."
         query = f"""{PREFIX_RDF}
-                SELECT ?autosampler ?autosampler_manufacturer ?laboratory ?autosampler_power_supply
+                SELECT ?autosampler ?autosampler_manufacturer ?autosampler_power_supply
                 ?sample_loop_volume ?sample_loop_volume_value ?sample_loop_volume_unit ?sample_loop_volume_num_val
                 ?site ?loc ?vial ?fill_level ?fill_level_om_value ?fill_level_unit ?fill_level_num_val
                 ?warn_level ?warn_level_om_value ?warn_level_unit ?warn_level_num_val
                 ?max_level ?max_level_om_value ?max_level_unit ?max_level_num_val ?chemical_amount ?contains_unidentified_component
                 WHERE {{
                     {'VALUES ?autosampler { <%s> }' % trimIRI(given_autosampler_iri) if given_autosampler_iri is not None else ""}
                     ?autosampler rdf:type <{ONTOVAPOURTEC_AUTOSAMPLER}>;
                                  <{DBPEDIA_MANUFACTURER}> ?autosampler_manufacturer;
-                                 <{ONTOLAB_ISCONTAINEDIN}> ?laboratory;
                                  <{ONTOLAB_HASPOWERSUPPLY}> ?autosampler_power_supply;
                                  <{ONTOVAPOURTEC_SAMPLELOOPVOLUME}> ?sample_loop_volume.
                     ?sample_loop_volume <{OM_HASVALUE}> ?sample_loop_volume_value.
                     ?sample_loop_volume_value <{OM_HASUNIT}> ?sample_loop_volume_unit;
                                               <{OM_HASNUMERICALVALUE}> ?sample_loop_volume_num_val.
                     ?autosampler <{ONTOVAPOURTEC_HASSITE}> ?site.
                     ?site <{ONTOVAPOURTEC_HOLDS}> ?vial; <{ONTOVAPOURTEC_LOCATIONID}> ?loc.
@@ -777,20 +820,14 @@
             try:
                 unique_specific_autosampler_manufacturer_iri = dal.get_the_unique_value_in_list_of_dict(info_of_specific_autosampler, 'autosampler_manufacturer')
             except Exception as e:
                 logger.error(f"dbpedia:manufacturer is not correctly defined for {specific_autosampler}", exc_info=True)
                 raise e
 
             try:
-                unique_specific_autosampler_laboratory_iri = dal.get_the_unique_value_in_list_of_dict(info_of_specific_autosampler, 'laboratory')
-            except Exception as e:
-                logger.error(f"OntoLab:isContainedIn is not correctly defined for {specific_autosampler}", exc_info=True)
-                raise e
-
-            try:
                 unique_specific_autosampler_power_supply_iri = dal.get_the_unique_value_in_list_of_dict(info_of_specific_autosampler, 'autosampler_power_supply')
             except Exception as e:
                 logger.error(f"OntoLab:hasPowerSupply is not correctly defined for {specific_autosampler}", exc_info=True)
                 raise e
 
             try:
                 unique_sample_loop_volume_iri = dal.get_the_unique_value_in_list_of_dict(info_of_specific_autosampler, 'sample_loop_volume')
@@ -863,27 +900,25 @@
                         instance_iri=info_of_specific_site['max_level'],
                         hasValue=OM_Measure(
                             instance_iri=info_of_specific_site['max_level_om_value'],
                             hasUnit=info_of_specific_site['max_level_unit'],
                             hasNumericalValue=info_of_specific_site['max_level_num_val']
                         )
                     ),
-                    isHeldIn=specific_site
                 )
                 autosampler_site = AutoSamplerSite(
                     instance_iri=specific_site,
                     holds=vial,
                     locationID=info_of_specific_site['loc']
                 )
                 list_autosampler_site.append(autosampler_site)
 
             autosampler = AutoSampler(
                 instance_iri=specific_autosampler,
                 manufacturer=unique_specific_autosampler_manufacturer_iri,
-                isContainedIn=unique_specific_autosampler_laboratory_iri,
                 hasPowerSupply=unique_specific_autosampler_power_supply_iri,
                 hasSite=list_autosampler_site,
                 sampleLoopVolume=OM_Volume(
                     instance_iri=unique_sample_loop_volume_iri,
                     hasValue=OM_Measure(
                         instance_iri=unique_sample_loop_volume_value_iri,
                         hasUnit=unique_sample_loop_volume_unit,
@@ -913,15 +948,15 @@
         query = f"""{PREFIX_RDFS} {PREFIX_RDF} {PREFIX_XSD} {PREFIX_OWL}
                 SELECT DISTINCT ?rxn ?condition ?subo ?clz ?measure ?val ?unit ?parameter_setting ?id ?multi ?usage
                 WHERE {{
                     VALUES ?rxn {{ <{'> <'.join(rxnexp_iris)}> }}
                     ?subo rdfs:subPropertyOf* <{ONTOREACTION_HASREACTIONCONDITION}> . ?rxn ?subo ?condition .
                     ?condition rdf:type ?clz . FILTER(?clz != owl:Thing && ?clz != owl:NamedIndividual && ?clz != <{ONTOREACTION_REACTIONCONDITION}>) .
                     ?condition <{OM_HASVALUE}> ?measure . ?measure <{OM_HASUNIT}> ?unit; <{OM_HASNUMERICALVALUE}> ?val .
-                    OPTIONAL {{ ?condition <{ONTOLAB_TRANSLATESTOPARAMETERSETTING}> ?parameter_setting . }} .
+                    OPTIONAL {{ ?parameter_setting <{ONTOLAB_HASQUANTITY}> ?condition . }} .
                     OPTIONAL {{ ?condition <{ONTODOE_POSITIONALID}> ?id . }} .
                     OPTIONAL {{ ?condition <{ONTOREACTION_INDICATESMULTIPLICITYOF}> ?multi . }} .
                     OPTIONAL {{ ?condition <{ONTOREACTION_INDICATESUSAGEOF}> ?usage . }} .
                 }}"""
 
         # Perform SPARQL query
         response_of_all_rxn = self.performQuery(query)
@@ -959,15 +994,15 @@
                     instance_iri=rc,
                     clz=_clz,
                     objPropWithExp=_subo,
                     hasValue=OM_Measure(instance_iri=_measure[0],hasUnit=_unit[0],hasNumericalValue=_val[0]) if len(_measure) == 1 else None,
                     positionalID=_id[0] if len(_id) == 1 else None,
                     translateToParameterSetting=_parameter_setting[0] if len(_parameter_setting) == 1 else None,
                     indicatesMultiplicityOf=_multi[0] if len(_multi) == 1 else None,
-                    indicateUsageOf=_usage[0] if len(_usage) == 1 else None
+                    indicatesUsageOf=_usage[0] if len(_usage) == 1 else None
                 )
                 list_con.append(rxn_condition)
 
             dict_rxn_condition[rxn_iri] = list_con
 
         return dict_rxn_condition
 
@@ -1185,23 +1220,23 @@
     def get_vapourtec_rs400(
         self,
         list_vapourtec_rs400_iri: Union[str, list]=None,
         list_of_labs_as_constraint: list=None
     ) -> List[VapourtecRS400]:
         list_vapourtec_rs400_iri = trimIRI([list_vapourtec_rs400_iri] if not isinstance(list_vapourtec_rs400_iri, list) else list_vapourtec_rs400_iri) if list_vapourtec_rs400_iri is not None else None
         list_of_labs_as_constraint = trimIRI(list_of_labs_as_constraint) if list_of_labs_as_constraint is not None else None
-        query = f"""SELECT ?rs400 ?rs400_manufacturer ?laboratory ?rs400_power_supply ?state
+        query = f"""SELECT ?rs400 ?rs400_manufacturer ?rs400_power_supply ?state
                            ?state_type ?last_update ?autosampler ?is_managed_by
                            ?collection_method ?collection_method_type ?waste_receptacle
                            ?recommended_reaction_scale ?recommended_reaction_scale_measure ?recommended_reaction_scale_unit ?recommended_reaction_scale_val
                 WHERE {{
                     {"VALUES ?rs400 { <%s> } ." % '> <'.join(list_vapourtec_rs400_iri) if list_vapourtec_rs400_iri is not None else ""}
                     {"VALUES ?laboratory { <%s> } ." % '> <'.join(list_of_labs_as_constraint) if list_of_labs_as_constraint is not None else ""}
-                    ?rs400 <{ONTOLAB_ISCONTAINEDIN}> ?laboratory;
-                           <{SAREF_CONSISTSOF}> ?autosampler;
+                    ?laboratory <{ONTOLAB_CONTAINS}> ?rs400.
+                    ?rs400 <{SAREF_CONSISTSOF}> ?autosampler;
                            <{DBPEDIA_MANUFACTURER}> ?rs400_manufacturer;
                            <{ONTOLAB_HASPOWERSUPPLY}> ?rs400_power_supply;
                            <{SAREF_HASSTATE}> ?state.
                     ?state a ?state_type; <{ONTOLAB_STATELASTUPDATEDAT}> ?last_update.
                     ?autosampler a <{ONTOVAPOURTEC_AUTOSAMPLER}>.
                     ?rs400 <{ONTOVAPOURTEC_HASCOLLECTIONMETHOD}> ?collection_method.
                     ?collection_method a ?collection_method_type.
@@ -1232,47 +1267,45 @@
             list_vapourtec_reactor_and_pump.append(self.get_autosampler(res['autosampler']))
             list_vapourtec_reactor_and_pump += self.get_r4_reactor_given_vapourtec_rs400(rs400_iri)
             list_vapourtec_reactor_and_pump += self.get_r2_pump_given_vapourtec_rs400(rs400_iri)
 
             vapourtec_rs400 = VapourtecRS400(
                 instance_iri=rs400_iri,
                 manufacturer=res['rs400_manufacturer'],
-                isContainedIn=res['laboratory'],
                 hasPowerSupply=res['rs400_power_supply'],
                 isManagedBy=res['is_managed_by'] if 'is_managed_by' in res else None,
                 consistsOf=list_vapourtec_reactor_and_pump,
                 hasState=VapourtecState(
                     instance_iri=res['state'],
                     clz=res['state_type'],
                     stateLastUpdatedAt=res['last_update']
                 ),
                 hasCollectionMethod=CollectionMethod(
                     instance_iri=res['collection_method'],
                     clz=res['collection_method_type'],
-                    toReceptacle=res['waste_receptacle'],
+                    toReceptacle=res.get('waste_receptacle'),
                 ),
                 recommendedReactionScale=OM_Volume(
                     instance_iri=res['recommended_reaction_scale'],
                     hasValue=OM_Measure(instance_iri=res['recommended_reaction_scale_measure'],hasUnit=res['recommended_reaction_scale_unit'],hasNumericalValue=res['recommended_reaction_scale_val'])
                 ) if 'recommended_reaction_scale' in res else None,
             )
             list_vapourtec_rs400_instance.append(vapourtec_rs400)
 
         return list_vapourtec_rs400_instance
 
     def get_vapourtec_rs400_given_autosampler(self, autosampler: AutoSampler) -> VapourtecRS400:
         query = f"""{PREFIX_RDF}
-                SELECT ?rs400 ?rs400_manufacturer ?laboratory ?rs400_power_supply ?state ?state_type ?last_update ?is_managed_by
+                SELECT ?rs400 ?rs400_manufacturer ?rs400_power_supply ?state ?state_type ?last_update ?is_managed_by
                 ?collection_method ?collection_method_type ?waste_receptacle
                 ?recommended_reaction_scale ?recommended_reaction_scale_measure ?recommended_reaction_scale_unit ?recommended_reaction_scale_val
                 WHERE {{
                     ?rs400 <{SAREF_CONSISTSOF}> <{autosampler.instance_iri}>;
                             rdf:type <{ONTOVAPOURTEC_VAPOURTECRS400}>;
                             <{DBPEDIA_MANUFACTURER}> ?rs400_manufacturer;
-                            <{ONTOLAB_ISCONTAINEDIN}> ?laboratory;
                             <{ONTOLAB_HASPOWERSUPPLY}> ?rs400_power_supply;
                             <{SAREF_HASSTATE}> ?state.
                     ?state a ?state_type; <{ONTOLAB_STATELASTUPDATEDAT}> ?last_update.
                     ?rs400 <{ONTOVAPOURTEC_HASCOLLECTIONMETHOD}> ?collection_method.
                     ?collection_method a ?collection_method_type.
                     OPTIONAL{{?collection_method <{ONTOVAPOURTEC_TORECEPTACLE}> ?waste_receptacle.}}
                     OPTIONAL{{?rs400 <{ONTOLAB_ISMANAGEDBY}> ?is_managed_by.}}
@@ -1297,27 +1330,26 @@
         list_vapourtec_reactor_and_pump.append(autosampler)
         list_vapourtec_reactor_and_pump += self.get_r4_reactor_given_vapourtec_rs400(res['rs400'])
         list_vapourtec_reactor_and_pump += self.get_r2_pump_given_vapourtec_rs400(res['rs400'])
 
         vapourtec_rs400 = VapourtecRS400(
             instance_iri=res['rs400'],
             manufacturer=res['rs400_manufacturer'],
-            isContainedIn=res['laboratory'],
             hasPowerSupply=res['rs400_power_supply'],
             isManagedBy=res['is_managed_by'] if 'is_managed_by' in res else None,
             consistsOf=list_vapourtec_reactor_and_pump,
             hasState=VapourtecState(
                 instance_iri=res['state'],
                 clz=res['state_type'],
                 stateLastUpdatedAt=res['last_update']
             ),
             hasCollectionMethod=CollectionMethod(
                 instance_iri=res['collection_method'],
                 clz=res['collection_method_type'],
-                toReceptacle=res['waste_receptacle'],
+                toReceptacle=res.get('waste_receptacle'),
             ),
             recommendedReactionScale=OM_Volume(
                 instance_iri=res['recommended_reaction_scale'],
                 hasValue=OM_Measure(instance_iri=res['recommended_reaction_scale_measure'],hasUnit=res['recommended_reaction_scale_unit'],hasNumericalValue=res['recommended_reaction_scale_val'])
             ) if 'recommended_reaction_scale' in res else None,
         )
 
@@ -1358,33 +1390,33 @@
             dict_reactor[iri] = r4_reactor_iri[0] if len(r4_reactor_iri) == 1 else None
         return dict_reactor
 
     def get_r4_reactor_given_vapourtec_rs400(self, vapourtec_rs400_iri: str) -> List[VapourtecR4Reactor]:
         vapourtec_rs400_iri = trimIRI(vapourtec_rs400_iri)
         query = PREFIX_RDF + \
                 """
-                SELECT ?r4_reactor ?r4_reactor_manufacturer ?laboratory ?r4_reactor_power_supply ?loc ?r4_reactor_material
+                SELECT ?r4_reactor ?r4_reactor_manufacturer ?r4_reactor_power_supply ?loc ?r4_reactor_material
                 ?r4_reactor_internal_diameter ?r4_reactor_internal_diameter_measure ?r4_reactor_internal_diameter_unit ?r4_reactor_internal_diameter_val
                 ?r4_reactor_length ?r4_reactor_length_measure ?r4_reactor_length_unit ?r4_reactor_length_val
                 ?r4_reactor_volume ?r4_reactor_volume_measure ?r4_reactor_volume_unit ?r4_reactor_volume_val
                 ?r4_reactor_temp_lower ?r4_reactor_temp_lower_measure ?r4_reactor_temp_lower_unit ?r4_reactor_temp_lower_val
                 ?r4_reactor_temp_upper ?r4_reactor_temp_upper_measure ?r4_reactor_temp_upper_unit ?r4_reactor_temp_upper_val
                 WHERE {
                     <%s> <%s> ?r4_reactor .
-                    ?r4_reactor rdf:type <%s>; <%s> ?r4_reactor_manufacturer; <%s> ?laboratory; <%s> ?r4_reactor_power_supply; <%s> ?loc;
+                    ?r4_reactor rdf:type <%s>; <%s> ?r4_reactor_manufacturer; <%s> ?r4_reactor_power_supply; <%s> ?loc;
                     <%s> ?r4_reactor_material; <%s> ?r4_reactor_internal_diameter; <%s> ?r4_reactor_length;
                     <%s> ?r4_reactor_volume; <%s> ?r4_reactor_temp_lower; <%s> ?r4_reactor_temp_upper.
                     ?r4_reactor_internal_diameter <%s> ?r4_reactor_internal_diameter_measure. ?r4_reactor_internal_diameter_measure <%s> ?r4_reactor_internal_diameter_unit; <%s> ?r4_reactor_internal_diameter_val.
                     ?r4_reactor_length <%s> ?r4_reactor_length_measure. ?r4_reactor_length_measure <%s> ?r4_reactor_length_unit; <%s> ?r4_reactor_length_val.
                     ?r4_reactor_volume <%s> ?r4_reactor_volume_measure. ?r4_reactor_volume_measure <%s> ?r4_reactor_volume_unit; <%s> ?r4_reactor_volume_val.
                     ?r4_reactor_temp_lower <%s> ?r4_reactor_temp_lower_measure. ?r4_reactor_temp_lower_measure <%s> ?r4_reactor_temp_lower_unit; <%s> ?r4_reactor_temp_lower_val.
                     ?r4_reactor_temp_upper <%s> ?r4_reactor_temp_upper_measure. ?r4_reactor_temp_upper_measure <%s> ?r4_reactor_temp_upper_unit; <%s> ?r4_reactor_temp_upper_val.
                 }
                 """ % (
-                    vapourtec_rs400_iri, SAREF_CONSISTSOF, ONTOVAPOURTEC_VAPOURTECR4REACTOR, DBPEDIA_MANUFACTURER, ONTOLAB_ISCONTAINEDIN, ONTOLAB_HASPOWERSUPPLY, ONTOVAPOURTEC_LOCATIONID,
+                    vapourtec_rs400_iri, SAREF_CONSISTSOF, ONTOVAPOURTEC_VAPOURTECR4REACTOR, DBPEDIA_MANUFACTURER, ONTOLAB_HASPOWERSUPPLY, ONTOVAPOURTEC_LOCATIONID,
                     ONTOVAPOURTEC_HASREACTORMATERIAL, ONTOVAPOURTEC_HASINTERNALDIAMETER, ONTOVAPOURTEC_HASREACTORLENGTH,
                     ONTOVAPOURTEC_HASREACTORVOLUME, ONTOVAPOURTEC_HASREACTORTEMPERATURELOWERLIMIT, ONTOVAPOURTEC_HASREACTORTEMPERATUREUPPERLIMIT,
                     OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE,
                     OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE,
                     OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE,
                     OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE,
                     OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE
@@ -1402,15 +1434,14 @@
                 raise Exception("No record of OntoVapourtec:VapourtecR4Reactor <%s> are identified." % (specific_r4_reactor))
             else:
                 info_ = info_of_specific_r4_reactor[0]
 
             r4_reactor = VapourtecR4Reactor(
                 instance_iri=info_['r4_reactor'],
                 manufacturer=info_['r4_reactor_manufacturer'],
-                isContainedIn=info_['laboratory'],
                 hasPowerSupply=info_['r4_reactor_power_supply'],
                 locationID=info_['loc'],
                 hasReactorMaterial=info_['r4_reactor_material'],
                 hasInternalDiameter=OM_Diameter(
                     instance_iri=info_['r4_reactor_internal_diameter'],
                     hasValue=OM_Measure(instance_iri=info_['r4_reactor_internal_diameter_measure'],hasUnit=info_['r4_reactor_internal_diameter_unit'],hasNumericalValue=info_['r4_reactor_internal_diameter_val'])
                 ),
@@ -1433,20 +1464,19 @@
             )
             list_r4_reactor.append(r4_reactor)
 
         return list_r4_reactor
 
     def get_r2_pump_given_vapourtec_rs400(self, vapourtec_rs400_iri: str) -> List[VapourtecR2Pump]:
         vapourtec_rs400_iri = trimIRI(vapourtec_rs400_iri)
-        query = f"""SELECT ?r2_pump ?r2_pump_manufacturer ?laboratory ?r2_pump_power_supply ?loc ?reagent_bottle
+        query = f"""SELECT ?r2_pump ?r2_pump_manufacturer ?r2_pump_power_supply ?loc ?reagent_bottle
                 WHERE {{
                     <{vapourtec_rs400_iri}> <{SAREF_CONSISTSOF}> ?r2_pump .
                     ?r2_pump a <{ONTOVAPOURTEC_VAPOURTECR2PUMP}>;
                              <{DBPEDIA_MANUFACTURER}> ?r2_pump_manufacturer;
-                             <{ONTOLAB_ISCONTAINEDIN}> ?laboratory;
                              <{ONTOLAB_HASPOWERSUPPLY}> ?r2_pump_power_supply;
                              <{ONTOVAPOURTEC_LOCATIONID}> ?loc.
                     OPTIONAL{{?r2_pump <{ONTOVAPOURTEC_HASREAGENTSOURCE}> ?reagent_bottle.}}
                 }}"""
 
         response = self.performQuery(query)
         unique_r2_pump_list = dal.get_unique_values_in_list_of_dict(response, 'r2_pump')
@@ -1461,15 +1491,14 @@
                 raise Exception("No record of OntoVapourtec:VapourtecR4Reactor <%s> are identified." % (specific_r2_pump))
             else:
                 info_ = info_of_specific_r2_pump[0]
 
             r2_pump = VapourtecR2Pump(
                 instance_iri=info_['r2_pump'],
                 manufacturer=info_['r2_pump_manufacturer'],
-                isContainedIn=info_['laboratory'],
                 hasPowerSupply=info_['r2_pump_power_supply'],
                 locationID=info_['loc'],
                 hasReagentSource=self.get_reagent_bottle(info_['reagent_bottle']) if 'reagent_bottle' in info_ else None,
             )
             list_r2_pump.append(r2_pump)
 
         return list_r2_pump
@@ -1660,16 +1689,16 @@
         update = """INSERT { %s } WHERE { FILTER NOT EXISTS { %s } }""" % (
             g.serialize(format='nt'), g.serialize(format='nt')
         )
         self.performUpdate(update)
 
     def identify_rxn_exp_when_uploading_hplc_report(self, hplc_digital_twin: str, hplc_remote_file_path: str) -> str:
         hplc_digital_twin = trimIRI(hplc_digital_twin)
-        query = """SELECT DISTINCT ?rxn_exp WHERE {<%s> ^<%s>/<%s>+/<%s>/<%s> ?rxn_exp.}""" % (
-            hplc_digital_twin, SAREF_CONSISTSOF, SAREF_CONSISTSOF, ONTOLAB_ISSPECIFIEDBY, ONTOLAB_WASGENERATEDFOR)
+        query = """SELECT DISTINCT ?rxn_exp WHERE {<%s> ^<%s>/<%s>+/^<%s>/<%s> ?rxn_exp.}""" % (
+            hplc_digital_twin, SAREF_CONSISTSOF, SAREF_CONSISTSOF, ONTOLAB_SPECIFIES, ONTOLAB_WASGENERATEDFOR)
         response = self.performQuery(query)
         rxn_exp = [list(res.values())[0] for res in response]
         if len(rxn_exp) > 1:
             raise Exception("Multiple instances of ReactionExperiment is identified to be associated with HPLC <%s> when uploading HPLCReport <%s>: %s" % (
                 hplc_digital_twin, hplc_remote_file_path, str(response)))
         elif len(rxn_exp) < 1:
             raise Exception("No instance of ReactionExperiment is identified to be associated with HPLC <%s> when uploading HPLCReport <%s>" % (
@@ -1823,43 +1852,43 @@
                 return float(response[0]['value'])
             else:
                 raise NotImplementedError("Record of MolecularWeight in unit of <%s> is NOT yet supported for OntoSpecies:Species <%s>" % (
                     response[0]['unit'], species_iri))
 
     # TODO replace this with the proper representation of the species density - at given temperature, what's the density of the given species
     def get_species_density(self, species_iri: str) -> Tuple[float, str]:
-        PLACEHOLDER_HASDENSITY = 'http://www.theworldavatar.com/kg/_for_species/hasDensity'
+        PLACEHOLDER_HASDENSITY = 'https://www.theworldavatar.com/kg/_for_species/hasDensity'
         species_iri = trimIRI(species_iri)
         query = """SELECT ?value ?unit WHERE { <%s> <%s>/<%s> ?density. ?density <%s> ?unit; <%s> ?value. }""" % (
             species_iri, PLACEHOLDER_HASDENSITY, OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE)
         response = self.performQuery(query)
         if len(response) > 1:
             raise Exception("Multiple records of Density were identified for OntoSpecies:Species <%s>: %s" % (species_iri, str(response)))
         elif len(response) < 1:
             raise Exception("No record of Density was identified for OntoSpecies:Species <%s>" % (species_iri))
         else:
             return float(response[0]['value']), response[0]['unit']
 
     # TODO replace this with the proper representation of the material cost - with the given vendor, what's the cost of the given chemical
     def get_species_material_cost(self, species_iri: str) -> Tuple[float, str]:
-        PLACEHOLDER_HASMATERIALCOST = 'http://www.theworldavatar.com/kg/_for_species/hasMaterialCost'
+        PLACEHOLDER_HASMATERIALCOST = 'https://www.theworldavatar.com/kg/_for_species/hasMaterialCost'
         species_iri = trimIRI(species_iri)
         query = """SELECT ?value ?unit WHERE { <%s> <%s>/<%s> ?cost. ?cost <%s> ?unit; <%s> ?value. }""" % (
             species_iri, PLACEHOLDER_HASMATERIALCOST, OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE)
         response = self.performQuery(query)
         if len(response) > 1:
             raise Exception("Multiple records of MaterialCost were identified for OntoSpecies:Species <%s>: %s" % (species_iri, str(response)))
         elif len(response) < 1:
             raise Exception("No record of MaterialCost was identified for OntoSpecies:Species <%s>" % (species_iri))
         else:
             return float(response[0]['value']), response[0]['unit']
 
     # TODO replace this with the proper representation of the eco score - not sure if this is an "intrinsic" property of a given chemical
     def get_species_eco_score(self, species_iri: str) -> Tuple[float, str]:
-        PLACEHOLDER_HASECOSCORE = 'http://www.theworldavatar.com/kg/_for_species/hasEcoScore'
+        PLACEHOLDER_HASECOSCORE = 'https://www.theworldavatar.com/kg/_for_species/hasEcoScore'
         species_iri = trimIRI(species_iri)
         query = """SELECT ?value ?unit WHERE { <%s> <%s>/<%s> ?ecoscore. ?ecoscore <%s> ?unit; <%s> ?value. }""" % (
             species_iri, PLACEHOLDER_HASECOSCORE, OM_HASVALUE, OM_HASUNIT, OM_HASNUMERICALVALUE)
         response = self.performQuery(query)
         if len(response) > 1:
             raise Exception("Multiple records of EcoScore were identified for OntoSpecies:Species <%s>: %s" % (species_iri, str(response)))
         elif len(response) < 1:
@@ -2381,16 +2410,16 @@
         self.update_waste_bottle_liquid_level_millilitre(
             {waste_bottle_iri:amount_of_chemical_amount}, for_consumption=False
         )
         return g
 
     def release_vapourtec_rs400_settings(self, vapourtec_rs400_iri: str):
         vapourtec_rs400_iri = trimIRI(vapourtec_rs400_iri)
-        update = """DELETE {?hardware <%s> ?settings. ?settings <%s> ?hardware.} WHERE {<%s> <%s>* ?hardware. ?hardware <%s> ?settings.}""" % (
-                ONTOLAB_ISSPECIFIEDBY, ONTOLAB_SPECIFIES, vapourtec_rs400_iri, SAREF_CONSISTSOF, ONTOLAB_ISSPECIFIEDBY
+        update = """DELETE {?settings <%s> ?hardware.} WHERE {<%s> <%s>* ?hardware. ?settings <%s> ?hardware.}""" % (
+                ONTOLAB_SPECIFIES, vapourtec_rs400_iri, SAREF_CONSISTSOF, ONTOLAB_SPECIFIES
             )
         self.performUpdate(update)
 
     def upload_vapourtec_input_file_to_kg(self, vapourtec_digital_twin, local_file_path: str, remote_file_subdir: str):
         # replace windows path separators with unix path separators
         _remote_file_subdir = remote_file_subdir.replace(':', '').replace('\\', '/') if remote_file_subdir is not None else None
         try:
@@ -2428,32 +2457,31 @@
 
         vapourtec_input_file = VapourtecInputFile(instance_iri=vapourtec_input_file_iri, **response[0])
         return vapourtec_input_file
 
     def get_hplc_given_vapourtec_rs400(self, vapourtec_rs400_iri: str) -> HPLC:
         vapourtec_rs400_iri = trimIRI(vapourtec_rs400_iri)
         query = """SELECT ?hplc ?hplc_manufacturer ?lab ?hplc_power_supply ?is_managed_by ?report_extension
-                WHERE {<%s> ^<%s>/<%s> ?hplc. ?hplc a <%s>; <%s> ?hplc_manufacturer; <%s> ?lab; <%s> ?hplc_power_supply; <%s> ?report_extension.
+                WHERE {<%s> ^<%s>/<%s> ?hplc. ?hplc a <%s>; <%s> ?hplc_manufacturer; <%s> ?hplc_power_supply; <%s> ?report_extension.
                 OPTIONAL{?hplc <%s> ?is_managed_by}}""" % (
-            vapourtec_rs400_iri, SAREF_CONSISTSOF, SAREF_CONSISTSOF, ONTOHPLC_HIGHPERFORMANCELIQUIDCHROMATOGRAPHY, DBPEDIA_MANUFACTURER, ONTOLAB_ISCONTAINEDIN, ONTOLAB_HASPOWERSUPPLY,
+            vapourtec_rs400_iri, SAREF_CONSISTSOF, SAREF_CONSISTSOF, ONTOHPLC_HIGHPERFORMANCELIQUIDCHROMATOGRAPHY, DBPEDIA_MANUFACTURER, ONTOLAB_HASPOWERSUPPLY,
             ONTOHPLC_REPORTEXTENSION, ONTOLAB_ISMANAGEDBY
         )
         response = self.performQuery(query)
         if (len(response) > 1):
             # NOTE here we assume one HPLC module has only ONE manufacturer, locates in only ONE laboratory, also has only ONE type of power supply
             # NOTE this might not hold universally, but we will simplify for the moment
             raise NotImplementedError("Not yet supported - VapourtecRS400 <%s> is associated with multiple HPLC: %s" % (vapourtec_rs400_iri, str(response)))
         elif (len(response) < 1):
             raise Exception("No HPLC is identified connected with VapourtecRS400 <%s> when querying: %s" % (vapourtec_rs400_iri, query))
 
         res = response[0]
         hplc = HPLC(
             instance_iri=res['hplc'],
             manufacturer=res['hplc_manufacturer'],
-            isContainedIn=res['lab'],
             hasPowerSupply=res['hplc_power_supply'],
             isManagedBy=res['is_managed_by'] if 'is_managed_by' in res else None,
             reportExtension=res['report_extension'],
             # hasJob=, # TODO [future work] add support
             # hasPastReport=, # TODO [future work] add support
         )
         return hplc
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/Service__DoE.ttl`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 @prefix ontoagent:           <http://www.theworldavatar.com/ontology/ontoagent/MSM.owl#> .
 @prefix ontodoe:             <https://www.theworldavatar.com/kg/ontodoe/> .
 @prefix ontorxn:             <https://www.theworldavatar.com/kg/ontoreaction/> .
 @prefix rdf:                 <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix xsd:                 <http://www.w3.org/2001/XMLSchema#> .
-@prefix :                    <http://www.theworldavatar.com/resource/agents/Service__DoE#> .
+@prefix :                    <https://www.theworldavatar.com/kg/agents/Service__DoE/> .
 
 :Service
     rdf:type ontoagent:Service;
     ontoagent:hasOperation :Operation;
 .
 
 :Operation
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 @prefix ontoagent:           <http://www.theworldavatar.com/ontology/ontoagent/MSM.owl#> .
 @prefix ontorxn:             <https://www.theworldavatar.com/kg/ontoreaction/> .
 @prefix ontolab:             <https://www.theworldavatar.com/kg/ontolab/> .
 @prefix ontohplc:            <https://www.theworldavatar.com/kg/ontohplc/> .
 @prefix rdf:                 <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix xsd:                 <http://www.w3.org/2001/XMLSchema#> .
-@prefix :                    <http://www.theworldavatar.com/resource/agents/Service__Execution#> .
+@prefix :                    <https://www.theworldavatar.com/kg/agents/Service__PostProc/> .
 
 :Service
     rdf:type ontoagent:Service;
     ontoagent:hasOperation :Operation;
 .
 
 :Operation
     rdf:type ontoagent:Operation;
     ontoagent:hasInput :MessageContent_input;
     ontoagent:hasOutput :MessageContent_output;
-    ontoagent:hasHttpUrl "http://localhost:7000/execution/placeholder"^^xsd:string;
+    ontoagent:hasHttpUrl "http://localhost:7000/postprocessing/placeholder"^^xsd:string;
 .
 
 :MessageContent_input
     rdf:type ontoagent:MessageContent;
-    ontoagent:hasMandatoryPart :MessagePart_rxnexp;
+    ontoagent:hasMandatoryPart :MessagePart_hplcreport;
 .
 
 :MessageContent_output
     rdf:type ontoagent:MessageContent;
-    ontoagent:hasMandatoryPart :MessagePart_hplcreport;
-.
-
-:MessagePart_rxnexp
-    rdf:type ontoagent:MessagePart;
-    ontoagent:isArray "false"^^xsd:boolean;
-    ontoagent:hasType ontorxn:ReactionExperiment;
-    ontoagent:hasName "reactionExperiment"^^xsd:string;
+    ontoagent:hasMandatoryPart :MessagePart_performanceindicator;
 .
 
 :MessagePart_hplcreport
     rdf:type ontoagent:MessagePart;
     ontoagent:isArray "false"^^xsd:boolean;
     ontoagent:hasType ontohplc:HPLCReport;
     ontoagent:hasName "hplcReport"^^xsd:string;
 .
+
+:MessagePart_performanceindicator
+    rdf:type ontoagent:MessagePart;
+    ontoagent:isArray "true"^^xsd:boolean;
+    ontoagent:hasType ontorxn:PerformanceIndicator;
+    ontoagent:hasName "performanceIndicator"^^xsd:string;
+.
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/ontoagent/Service__Execution.ttl`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 @prefix ontoagent:           <http://www.theworldavatar.com/ontology/ontoagent/MSM.owl#> .
 @prefix ontorxn:             <https://www.theworldavatar.com/kg/ontoreaction/> .
 @prefix ontolab:             <https://www.theworldavatar.com/kg/ontolab/> .
 @prefix ontohplc:            <https://www.theworldavatar.com/kg/ontohplc/> .
 @prefix rdf:                 <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix xsd:                 <http://www.w3.org/2001/XMLSchema#> .
-@prefix :                    <http://www.theworldavatar.com/resource/agents/Service__PostProc#> .
+@prefix :                    <https://www.theworldavatar.com/kg/agents/Service__Execution/> .
 
 :Service
     rdf:type ontoagent:Service;
     ontoagent:hasOperation :Operation;
 .
 
 :Operation
     rdf:type ontoagent:Operation;
     ontoagent:hasInput :MessageContent_input;
     ontoagent:hasOutput :MessageContent_output;
-    ontoagent:hasHttpUrl "http://localhost:7000/postprocessing/placeholder"^^xsd:string;
+    ontoagent:hasHttpUrl "http://localhost:7000/execution/placeholder"^^xsd:string;
 .
 
 :MessageContent_input
     rdf:type ontoagent:MessageContent;
-    ontoagent:hasMandatoryPart :MessagePart_hplcreport;
+    ontoagent:hasMandatoryPart :MessagePart_rxnexp;
 .
 
 :MessageContent_output
     rdf:type ontoagent:MessageContent;
-    ontoagent:hasMandatoryPart :MessagePart_performanceindicator;
+    ontoagent:hasMandatoryPart :MessagePart_hplcreport;
 .
 
-:MessagePart_hplcreport
+:MessagePart_rxnexp
     rdf:type ontoagent:MessagePart;
     ontoagent:isArray "false"^^xsd:boolean;
-    ontoagent:hasType ontohplc:HPLCReport;
-    ontoagent:hasName "hplcReport"^^xsd:string;
+    ontoagent:hasType ontorxn:ReactionExperiment;
+    ontoagent:hasName "reactionExperiment"^^xsd:string;
 .
 
-:MessagePart_performanceindicator
+:MessagePart_hplcreport
     rdf:type ontoagent:MessagePart;
-    ontoagent:isArray "true"^^xsd:boolean;
-    ontoagent:hasType ontorxn:PerformanceIndicator;
-    ontoagent:hasName "performanceIndicator"^^xsd:string;
+    ontoagent:isArray "false"^^xsd:boolean;
+    ontoagent:hasType ontohplc:HPLCReport;
+    ontoagent:hasName "hplcReport"^^xsd:string;
 .
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/doe.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl`

 * *Files 6% similar despite different names*

```diff
@@ -6,107 +6,105 @@
 @prefix exp4:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_4/> .
 @prefix exp5:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_5/> .
 @prefix exp6:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_6/> .
 @prefix om:             <http://www.ontology-of-units-of-measure.org/resource/om-2/> .
 @prefix rdf:			<http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs:           <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix xsd:            <http://www.w3.org/2001/XMLSchema#> .
-@prefix :			    <https://www.example.com/triplestore/ontodoe/DoE_1/> .
+@prefix :			    <https://www.example.com/triplestore/ontodoe/DoE_no_prior_data/> .
 
 @prefix ChemRxn:        <https://www.example.com/triplestore/ontorxn/ChemRxn_1/> .
 
-####################################
-## Design of Experiment instances ##
-####################################
+###################################
+## Design of Experiment instance ##
+## NOTE no prior experiment data ##
+###################################
 :DoE_1
     rdf:type OntoDoE:DesignOfExperiment;
     OntoDoE:usesStrategy :Strategy_1;
     OntoDoE:hasDomain :Domain_1;
     OntoDoE:hasSystemResponse :SystemResponse_1;
     OntoDoE:hasSystemResponse :SystemResponse_2;
     OntoDoE:utilisesHistoricalData :HistoricalData_1;
     OntoDoE:designsChemicalReaction ChemRxn:ChemRxn_1;
 .
 
+# strategy
 :Strategy_1
     rdf:type OntoDoE:TSEMO;
     OntoDoE:nRetries "10"^^xsd:integer;
     OntoDoE:nSpectralPoints "30"^^xsd:integer;
     OntoDoE:nGenerations "20"^^xsd:integer;
     OntoDoE:populationSize "20"^^xsd:integer;
 .
 
-# This statement is actually part of OntoDoE TBox
-# just added here to enable query by property paths
-OntoDoE:TSEMO
-    rdfs:subClassOf OntoDoE:Strategy;
-.
-
+# domain
 :Domain_1
     rdf:type OntoDoE:Domain;
     OntoDoE:hasDesignVariable :ContinuousVariable_1;
     OntoDoE:hasDesignVariable :ContinuousVariable_2;
     OntoDoE:hasDesignVariable :ContinuousVariable_3;
     OntoDoE:hasDesignVariable :ContinuousVariable_4;
-    # below fixed parameters are added to reflect the latest design of DoEAgent
+    # NOTE as there's no prior experiment data, below fixed parameters are required for DoEAgent to read the default settings
     OntoDoE:hasFixedParameter :FixedParameter_1;
     OntoDoE:hasFixedParameter :FixedParameter_2;
     OntoDoE:hasFixedParameter :FixedParameter_3;
 .
 
+# continuous variables
 :ContinuousVariable_1
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :StoiRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:refersToQuantity :StoiRatio;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     OntoDoE:upperLimit "10"^^xsd:double;
     OntoDoE:lowerLimit "1"^^xsd:double;
 .
 
 :ContinuousVariable_2
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :StoiRatio;
+    OntoDoE:refersToQuantity :StoiRatio;
     OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202"^^xsd:string;
     OntoDoE:upperLimit "0.2"^^xsd:double;
     OntoDoE:lowerLimit "0.02"^^xsd:double;
 .
 
 :StoiRatio
     rdf:type OntoRxn:StoichiometryRatio;
     om:hasUnit om:one;
 .
 
 :ContinuousVariable_3
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :ResTime;
+    OntoDoE:refersToQuantity :ResTime;
     OntoDoE:upperLimit "15"^^xsd:double;
     OntoDoE:lowerLimit "5"^^xsd:double;
 .
 
 :ResTime
     rdf:type OntoRxn:ResidenceTime;
     om:hasUnit om:minute-Time;
 .
 
 :ContinuousVariable_4
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :RxnTemp;
+    OntoDoE:refersToQuantity :RxnTemp;
     OntoDoE:upperLimit "70"^^xsd:double;
     OntoDoE:lowerLimit "30"^^xsd:double;
 .
 
 :RxnTemp
     rdf:type OntoRxn:ReactionTemperature;
     om:hasUnit om:degreeCelsius;
 .
 
 # fixed parameters
 :FixedParameter_1
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :StoiRatio_1;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:refersToQuantity :StoiRatio_1;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
 .
 
 :StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
     om:hasValue :StoiRatio_1_Measure_1;
 .
 
@@ -114,16 +112,16 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 :FixedParameter_2
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :RxnScale_1;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:refersToQuantity :RxnScale_1;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
 .
 
 :RxnScale_1
     rdf:type OntoRxn:ReactionScale;
     om:hasValue :RxnScale_1_Measure_1;
 .
 
@@ -131,42 +129,39 @@
     rdf:type om:Measure;
     om:hasUnit om:millilitre;
     om:hasNumericalValue "5"^^xsd:double;
 .
 
 :FixedParameter_3
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :RxnPressure_1;
+    OntoDoE:refersToQuantity :RxnPressure_1;
 .
 
 :RxnPressure_1
     rdf:type OntoRxn:ReactionPressure;
     om:hasValue :RxnPressure_1_Measure_1;
 .
 
 :RxnPressure_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:bar;
     om:hasNumericalValue "6"^^xsd:double;
 .
 
+# system response
 :SystemResponse_1
     rdf:type OntoDoE:SystemResponse;
-    OntoDoE:refersTo OntoRxn:Yield;
+    OntoDoE:refersToQuantity OntoRxn:Yield;
     OntoDoE:maximise "true"^^xsd:boolean;
 .
 
 :SystemResponse_2
     rdf:type OntoDoE:SystemResponse;
-    OntoDoE:refersTo OntoRxn:RunMaterialCost;
+    OntoDoE:refersToQuantity OntoRxn:RunMaterialCost;
     OntoDoE:maximise "false"^^xsd:boolean;
 .
 
+# historical data
 :HistoricalData_1
     rdf:type OntoDoE:HistoricalData;
-    OntoDoE:refersTo exp1:RxnExp_1;
-    OntoDoE:refersTo exp2:RxnExp_1;
-    OntoDoE:refersTo exp3:RxnExp_1;
-    OntoDoE:refersTo exp4:RxnExp_1;
-    OntoDoE:refersTo exp5:RxnExp_1;
     OntoDoE:numOfNewExp "1"^^xsd:integer; # the numOfNewExp is set to be 1 for the DoE design of this iteration
 .
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/doe.ttl`

 * *Files 4% similar despite different names*

```diff
@@ -6,111 +6,101 @@
 @prefix exp4:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_4/> .
 @prefix exp5:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_5/> .
 @prefix exp6:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_6/> .
 @prefix om:             <http://www.ontology-of-units-of-measure.org/resource/om-2/> .
 @prefix rdf:			<http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs:           <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix xsd:            <http://www.w3.org/2001/XMLSchema#> .
-@prefix :			    <https://www.example.com/triplestore/ontodoe/DoE_no_prior_data/> .
+@prefix :			    <https://www.example.com/triplestore/ontodoe/DoE_1/> .
 
 @prefix ChemRxn:        <https://www.example.com/triplestore/ontorxn/ChemRxn_1/> .
 
-###################################
-## Design of Experiment instance ##
-## NOTE no prior experiment data ##
-###################################
+####################################
+## Design of Experiment instances ##
+####################################
 :DoE_1
     rdf:type OntoDoE:DesignOfExperiment;
     OntoDoE:usesStrategy :Strategy_1;
     OntoDoE:hasDomain :Domain_1;
     OntoDoE:hasSystemResponse :SystemResponse_1;
     OntoDoE:hasSystemResponse :SystemResponse_2;
     OntoDoE:utilisesHistoricalData :HistoricalData_1;
     OntoDoE:designsChemicalReaction ChemRxn:ChemRxn_1;
 .
 
-# strategy
 :Strategy_1
     rdf:type OntoDoE:TSEMO;
     OntoDoE:nRetries "10"^^xsd:integer;
     OntoDoE:nSpectralPoints "30"^^xsd:integer;
     OntoDoE:nGenerations "20"^^xsd:integer;
     OntoDoE:populationSize "20"^^xsd:integer;
 .
 
-# This statement is actually part of OntoDoE TBox
-# just added here to enable query by property paths
-OntoDoE:TSEMO
-    rdfs:subClassOf OntoDoE:Strategy;
-.
-
-# domain
 :Domain_1
     rdf:type OntoDoE:Domain;
     OntoDoE:hasDesignVariable :ContinuousVariable_1;
     OntoDoE:hasDesignVariable :ContinuousVariable_2;
     OntoDoE:hasDesignVariable :ContinuousVariable_3;
     OntoDoE:hasDesignVariable :ContinuousVariable_4;
-    # NOTE as there's no prior experiment data, below fixed parameters are required for DoEAgent to read the default settings
+    # below fixed parameters are added to reflect the latest design of DoEAgent
     OntoDoE:hasFixedParameter :FixedParameter_1;
     OntoDoE:hasFixedParameter :FixedParameter_2;
     OntoDoE:hasFixedParameter :FixedParameter_3;
 .
 
-# continuous variables
 :ContinuousVariable_1
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :StoiRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:refersToQuantity :StoiRatio;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     OntoDoE:upperLimit "10"^^xsd:double;
     OntoDoE:lowerLimit "1"^^xsd:double;
 .
 
 :ContinuousVariable_2
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :StoiRatio;
+    OntoDoE:refersToQuantity :StoiRatio;
     OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202"^^xsd:string;
     OntoDoE:upperLimit "0.2"^^xsd:double;
     OntoDoE:lowerLimit "0.02"^^xsd:double;
 .
 
 :StoiRatio
     rdf:type OntoRxn:StoichiometryRatio;
     om:hasUnit om:one;
 .
 
 :ContinuousVariable_3
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :ResTime;
+    OntoDoE:refersToQuantity :ResTime;
     OntoDoE:upperLimit "15"^^xsd:double;
     OntoDoE:lowerLimit "5"^^xsd:double;
 .
 
 :ResTime
     rdf:type OntoRxn:ResidenceTime;
     om:hasUnit om:minute-Time;
 .
 
 :ContinuousVariable_4
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :RxnTemp;
+    OntoDoE:refersToQuantity :RxnTemp;
     OntoDoE:upperLimit "70"^^xsd:double;
     OntoDoE:lowerLimit "30"^^xsd:double;
 .
 
 :RxnTemp
     rdf:type OntoRxn:ReactionTemperature;
     om:hasUnit om:degreeCelsius;
 .
 
 # fixed parameters
 :FixedParameter_1
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :StoiRatio_1;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:refersToQuantity :StoiRatio_1;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
 .
 
 :StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
     om:hasValue :StoiRatio_1_Measure_1;
 .
 
@@ -118,16 +108,16 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 :FixedParameter_2
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :RxnScale_1;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:refersToQuantity :RxnScale_1;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
 .
 
 :RxnScale_1
     rdf:type OntoRxn:ReactionScale;
     om:hasValue :RxnScale_1_Measure_1;
 .
 
@@ -135,39 +125,42 @@
     rdf:type om:Measure;
     om:hasUnit om:millilitre;
     om:hasNumericalValue "5"^^xsd:double;
 .
 
 :FixedParameter_3
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :RxnPressure_1;
+    OntoDoE:refersToQuantity :RxnPressure_1;
 .
 
 :RxnPressure_1
     rdf:type OntoRxn:ReactionPressure;
     om:hasValue :RxnPressure_1_Measure_1;
 .
 
 :RxnPressure_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:bar;
     om:hasNumericalValue "6"^^xsd:double;
 .
 
-# system response
 :SystemResponse_1
     rdf:type OntoDoE:SystemResponse;
-    OntoDoE:refersTo OntoRxn:Yield;
+    OntoDoE:refersToQuantity OntoRxn:Yield;
     OntoDoE:maximise "true"^^xsd:boolean;
 .
 
 :SystemResponse_2
     rdf:type OntoDoE:SystemResponse;
-    OntoDoE:refersTo OntoRxn:RunMaterialCost;
+    OntoDoE:refersToQuantity OntoRxn:RunMaterialCost;
     OntoDoE:maximise "false"^^xsd:boolean;
 .
 
-# historical data
 :HistoricalData_1
     rdf:type OntoDoE:HistoricalData;
+    OntoDoE:refersToExperiment exp1:RxnExp_1;
+    OntoDoE:refersToExperiment exp2:RxnExp_1;
+    OntoDoE:refersToExperiment exp3:RxnExp_1;
+    OntoDoE:refersToExperiment exp4:RxnExp_1;
+    OntoDoE:refersToExperiment exp5:RxnExp_1;
     OntoDoE:numOfNewExp "1"^^xsd:integer; # the numOfNewExp is set to be 1 for the DoE design of this iteration
 .
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/doe_template.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/doe_template.ttl`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,14 @@
     rdf:type OntoDoE:TSEMO;
     OntoDoE:nRetries "10"^^xsd:integer;
     OntoDoE:nSpectralPoints "30"^^xsd:integer;
     OntoDoE:nGenerations "20"^^xsd:integer;
     OntoDoE:populationSize "20"^^xsd:integer;
 .
 
-# This statement is actually part of OntoDoE TBox
-# just added here to enable query by property paths
-OntoDoE:TSEMO
-    rdfs:subClassOf OntoDoE:Strategy;
-.
-
 # domain
 :Domain_1
     rdf:type OntoDoE:Domain;
     OntoDoE:hasDesignVariable :ContinuousVariable_1;
     OntoDoE:hasDesignVariable :ContinuousVariable_2;
     OntoDoE:hasDesignVariable :ContinuousVariable_3;
     OntoDoE:hasDesignVariable :ContinuousVariable_4;
@@ -60,62 +54,62 @@
     OntoDoE:hasFixedParameter :FixedParameter_2;
     OntoDoE:hasFixedParameter :FixedParameter_3;
 .
 
 # continuous variables
 :ContinuousVariable_1
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :StoiRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:refersToQuantity :StoiRatio;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     OntoDoE:upperLimit "10"^^xsd:double;
     OntoDoE:lowerLimit "1"^^xsd:double;
 .
 
 :ContinuousVariable_2
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :StoiRatio;
+    OntoDoE:refersToQuantity :StoiRatio;
     OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202"^^xsd:string;
     OntoDoE:upperLimit "0.2"^^xsd:double;
     OntoDoE:lowerLimit "0.02"^^xsd:double;
 .
 
 :StoiRatio
     rdf:type OntoRxn:StoichiometryRatio;
     om:hasUnit om:one;
 .
 
 :ContinuousVariable_3
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :ResTime;
+    OntoDoE:refersToQuantity :ResTime;
     OntoDoE:upperLimit "15"^^xsd:double;
     OntoDoE:lowerLimit "5"^^xsd:double;
 .
 
 :ResTime
     rdf:type OntoRxn:ResidenceTime;
     om:hasUnit om:minute-Time;
 .
 
 :ContinuousVariable_4
     rdf:type OntoDoE:ContinuousVariable;
-    OntoDoE:refersTo :RxnTemp;
+    OntoDoE:refersToQuantity :RxnTemp;
     OntoDoE:upperLimit "70"^^xsd:double;
     OntoDoE:lowerLimit "30"^^xsd:double;
 .
 
 :RxnTemp
     rdf:type OntoRxn:ReactionTemperature;
     om:hasUnit om:degreeCelsius;
 .
 
 # fixed parameters
 :FixedParameter_1
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :StoiRatio_1;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:refersToQuantity :StoiRatio_1;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
 .
 
 :StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
     om:hasValue :StoiRatio_1_Measure_1;
 .
 
@@ -123,16 +117,16 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 :FixedParameter_2
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :RxnScale_1;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:refersToQuantity :RxnScale_1;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
 .
 
 :RxnScale_1
     rdf:type OntoRxn:ReactionScale;
     om:hasValue :RxnScale_1_Measure_1;
 .
 
@@ -140,15 +134,15 @@
     rdf:type om:Measure;
     om:hasUnit om:millilitre;
     om:hasNumericalValue "5"^^xsd:double;
 .
 
 :FixedParameter_3
     rdf:type OntoDoE:FixedParameter;
-    OntoDoE:refersTo :RxnPressure_1;
+    OntoDoE:refersToQuantity :RxnPressure_1;
 .
 
 :RxnPressure_1
     rdf:type OntoRxn:ReactionPressure;
     om:hasValue :RxnPressure_1_Measure_1;
 .
 
@@ -157,21 +151,21 @@
     om:hasUnit om:bar;
     om:hasNumericalValue "6"^^xsd:double;
 .
 
 # # system response
 # :SystemResponse_1
 #     rdf:type OntoDoE:SystemResponse;
-#     OntoDoE:refersTo OntoRxn:Yield;
+#     OntoDoE:refersToQuantity OntoRxn:Yield;
 #     OntoDoE:maximise "true"^^xsd:boolean;
 # .
 
 # :SystemResponse_2
 #     rdf:type OntoDoE:SystemResponse;
-#     OntoDoE:refersTo OntoRxn:RunMaterialCost;
+#     OntoDoE:refersToQuantity OntoRxn:RunMaterialCost;
 #     OntoDoE:maximise "false"^^xsd:boolean;
 # .
 
 # historical data
 :HistoricalData_1
     rdf:type OntoDoE:HistoricalData;
     OntoDoE:numOfNewExp "1"^^xsd:integer; # the numOfNewExp is set to be 1 for the DoE template of this chemrxn
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/dummy_lab.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/dummy_lab.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @prefix OntoCAPEPha:    <http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#> .
 @prefix OntoCAPEUpp:    <http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#> .
 @prefix ontospecies:    <http://www.theworldavatar.com/ontology/ontospecies/OntoSpecies.owl#> .
 @prefix OntoVapourtec:    <https://www.theworldavatar.com/kg/ontovapourtec/> .
 @prefix ontohplc:        <https://www.theworldavatar.com/kg/ontohplc/> .
 @prefix ontobpr:        <https://www.theworldavatar.com/kg/ontobpr/> .
 @prefix OntoLab:        <https://www.theworldavatar.com/kg/ontolab/> .
-@prefix :                <http://example.com/blazegraph/namespace/testlab/dummy_lab/> .
+@prefix :                <https://example.com/blazegraph/namespace/testlab/dummy_lab/> .
 
 @prefix exp1:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/> .
 @prefix exp2:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_2/> .
 @prefix exp3:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_3/> .
 @prefix exp4:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_4/> .
 @prefix exp5:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_5/> .
 @prefix ontorxn:        <https://www.theworldavatar.com/kg/ontoreaction/> .
@@ -55,27 +55,25 @@
 .
 
 ##################################################
 ## Automated reaction platform in the Dummy lab ##
 ##################################################
 :AutomatedRxnPlatform_Dummy 
     a OntoLab:LabEquipment;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     saref:consistsOf :VapourtecRS400_Dummy;
     saref:consistsOf :HPLC_Dummy;
     saref:consistsOf :BPR_Dummy;
 .
 
 ##################
 ## HPLC - Dummy ##
 ##################
 :HPLC_Dummy
     a ontohplc:HighPerformanceLiquidChromatography;
     dbo:manufacturer :HPLC_Manufacturer;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :HPLC_Dummy_PowerSupply;
     ontohplc:localReportDirectory "/home/user/CHEM32/**/"^^xsd:string; # NOTE "\**\" or "/**/" depends on whether its windows or linux machine
     ontohplc:reportExtension <http://dbpedia.org/resource/Microsoft_Excel>;
     ontohplc:hasJob :HPLCJob_Dummy;
     ontohplc:hasPastReport :HPLCReport_Dummy;
 .
 
@@ -160,15 +158,15 @@
     rdf:type OntoCAPEUpp:ScalarValue;
     OntoCAPEUpp:hasUnitOfMeasure om:molePerLitre;
     OntoCAPEUpp:numericalValue "0.0"^^xsd:double; # TODO this value is only put as placeholder for testing purpose
 .
 
 :PhaseComponent_IS_oc
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     OntoCAPEUpp:hasProperty :PhaseComponent_IS_oc_Property_1;
 .
 
 :PhaseComponent_IS_oc_Property_1
     rdf:type OntoCAPEPha:Molarity;
     OntoCAPEUpp:hasValue :PhaseComponent_IS_oc_Property_1_ScalarValue_1;
 .
@@ -444,15 +442,15 @@
     ontohplc:usesInternalStandard SinglePhase:PhaseComponent_InternalStandard;
     ontohplc:retentionTimeMatchThreshold "0.15"^^xsd:double;
     rdfs:comment "HPLCMethod records the operation details of an HPLC job, e.g. HPLC analysis was performed using a XXX system equipped with a XXX pump, XXX column and XXX variable wavelength detector (VWD)... https://doi.org/10.1002/cmtd.202000044"^^xsd:string;
 .
 
 SinglePhase:PhaseComponent_InternalStandard
     rdf:type ontohplc:InternalStandard;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_InternalStandard_Property_1;
 .
 
 SinglePhase:PhaseComponent_InternalStandard_Property_1
     rdf:type OntoCAPEPha:Molarity;
     OntoCAPEUpp:hasValue SinglePhase:PhaseComponent_InternalStandard_Property_1_ScalarValue_1;
 .
@@ -463,27 +461,27 @@
     OntoCAPEUpp:numericalValue "0.05"^^xsd:double;
 .
 
 # reactant benzaldehyde
 # NOTE the response factor is commented out to minic the situation if we don't have this information
 # :ResponseFactor_1
 #     a ontohplc:ResponseFactor;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
 #     om:hasValue :ResponseFactor_1_value;
 # .
 
 # :ResponseFactor_1_value
 #     a om:Measure;
 #     om:hasUnit om:one;
 #     om:hasNumericalValue "10"^^xsd:double;
 # .
 
 :RetentionTime_1
     a ontohplc:RetentionTime;
-    ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
+    ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
     om:hasValue :RetentionTime_1_value;
 .
 
 :RetentionTime_1_value
     a om:Measure;
     om:hasUnit om:minute-Time;
     om:hasNumericalValue "0.55"^^xsd:double;
@@ -511,27 +509,27 @@
     a om:Measure;
     om:hasUnit om:minute-Time;
     om:hasNumericalValue "1.55"^^xsd:double;
 .
 
 :ResponseFactor_4 # internal standard
     a ontohplc:ResponseFactor;
-    ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     om:hasValue :ResponseFactor_4_value;
 .
 
 :ResponseFactor_4_value
     a om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1"^^xsd:double;
 .
 
 :RetentionTime_4
     a ontohplc:RetentionTime;
-    ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     om:hasValue :RetentionTime_4_value;
 .
 
 :RetentionTime_4_value
     a om:Measure;
     om:hasUnit om:minute-Time;
     om:hasNumericalValue "3.62"^^xsd:double;
@@ -564,27 +562,27 @@
 .
 
 ########################################################################################################
 ## NOTE below response factor and retention time are removed as it is not visible in the chromatogram ##
 ########################################################################################################
 # :ResponseFactor_3 # reactant acetone
 #     a ontohplc:ResponseFactor;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
 #     om:hasValue :ResponseFactor_3_value;
 # .
 
 # :ResponseFactor_3_value
 #     a om:Measure;
 #     om:hasUnit om:one;
 #     om:hasNumericalValue "25"^^xsd:double;
 # .
 
 # :RetentionTime_3
 #     a ontohplc:RetentionTime;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
 #     om:hasValue :RetentionTime_3_value;
 # .
 
 # :RetentionTime_3_value
 #     a om:Measure;
 #     om:hasUnit om:minute-Time;
 #     om:hasNumericalValue "2.56"^^xsd:double;
@@ -612,51 +610,51 @@
 #     a om:Measure;
 #     om:hasUnit om:minute-Time;
 #     om:hasNumericalValue "5.60"^^xsd:double;
 # .
 
 # :ResponseFactor_7 # solvent acetonitrile
 #     a ontohplc:ResponseFactor;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
 #     om:hasValue :ResponseFactor_7_value;
 # .
 
 # :ResponseFactor_7_value
 #     a om:Measure;
 #     om:hasUnit om:one;
 #     om:hasNumericalValue "30"^^xsd:double;
 # .
 
 # :RetentionTime_7
 #     a ontohplc:RetentionTime;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
 #     om:hasValue :RetentionTime_7_value;
 # .
 
 # :RetentionTime_7_value
 #     a om:Measure;
 #     om:hasUnit om:minute-Time;
 #     om:hasNumericalValue "6.49"^^xsd:double;
 # .
 
 # :ResponseFactor_8 # solvent ethanol
 #     a ontohplc:ResponseFactor;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
 #     om:hasValue :ResponseFactor_8_value;
 # .
 
 # :ResponseFactor_8_value
 #     a om:Measure;
 #     om:hasUnit om:one;
 #     om:hasNumericalValue "20"^^xsd:double;
 # .
 
 # :RetentionTime_8
 #     a ontohplc:RetentionTime;
-#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
+#     ontohplc:refersToSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
 #     om:hasValue :RetentionTime_8_value;
 # .
 
 # :RetentionTime_8_value
 #     a om:Measure;
 #     om:hasUnit om:minute-Time;
 #     om:hasNumericalValue "7.5"^^xsd:double;
@@ -672,15 +670,14 @@
 # :BPR_Dummy # TODO
 
 #############################
 ## Vapourtec RS400 - Dummy ##
 #############################
 :VapourtecRS400_Dummy
     a OntoVapourtec:VapourtecRS400;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     # Basic information
     OntoLab:hasPrice :VapRS400_Price;
     OntoLab:hasWeight :VapRS400_Weight; # TODO
     OntoLab:hasHeight :VapRS400_Height; # TODO
     OntoLab:hasWidth :VapRS400_Width; # TODO
     OntoLab:hasLength :VapRS400_Length; # TODO
     OntoLab:hasPowerSupply :VapRS400_PowerSupply; # TODO
@@ -784,15 +781,14 @@
 .
 
 ##################################
 ## Vapourtec R4 Reactor - Dummy ##
 ##################################
 :VapourtecR4_Dummy
     a OntoVapourtec:VapourtecR4Reactor;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :VapR4_PowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:locationID "4"^^xsd:string;
     OntoVapourtec:hasReactorMaterial :VapourtecR4_Dummy_ReactorMaterial; #TODO to be added
     OntoVapourtec:hasInternalDiameter :VapourtecR4_Dummy_ReactorDiameter;
     OntoVapourtec:hasReactorLength :VapourtecR4_Dummy_ReactorLength;
     OntoVapourtec:hasReactorVolume :VapourtecR4_Dummy_ReactorVolume;
@@ -856,15 +852,14 @@
 .
 
 ##########################################
 ## Vapourtec R4 Reactor - Another_Dummy ##
 ##########################################
 :VapourtecR4_Another_Dummy
     a OntoVapourtec:VapourtecR4Reactor;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :VapR4_Another_DummyPowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:locationID "1"^^xsd:string; # NOTE this is different from the locationID of :VapourtecR4_Dummy
     OntoVapourtec:hasReactorMaterial :VapourtecR4_Another_Dummy_ReactorMaterial; #TODO to be added
     OntoVapourtec:hasInternalDiameter :VapourtecR4_Another_Dummy_ReactorDiameter;
     OntoVapourtec:hasReactorLength :VapourtecR4_Another_Dummy_ReactorLength;
     OntoVapourtec:hasReactorVolume :VapourtecR4_Another_Dummy_ReactorVolume;
@@ -928,15 +923,14 @@
 .
 
 #################################
 ## Vapourtec R2 Pump - 1_Dummy ##
 #################################
 :VapourtecR2_1_Dummy
     a OntoVapourtec:VapourtecR2Pump;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :VapR2_1_PowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:locationID "A"^^xsd:string;
     # NOTE this pump is set to have a ReagentBottle to test the mixed sourcing of input chemicals
     OntoVapourtec:hasReagentSource :ReagentBottle_1_Dummy;
 .
 
@@ -982,48 +976,44 @@
 .
 
 #################################
 ## Vapourtec R2 Pump - 2_Dummy ##
 #################################
 :VapourtecR2_2_Dummy
     a OntoVapourtec:VapourtecR2Pump;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :VapR2_2_PowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:locationID "B"^^xsd:string;
 .
 
 #################################
 ## Vapourtec R2 Pump - 3_Dummy ##
 #################################
 :VapourtecR2_3_Dummy
     a OntoVapourtec:VapourtecR2Pump;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :VapR2_3_PowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:locationID "C"^^xsd:string;
 .
 
 #################################
 ## Vapourtec R2 Pump - 4_Dummy ##
 #################################
 :VapourtecR2_4_Dummy
     a OntoVapourtec:VapourtecR2Pump;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :VapR2_4_PowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:locationID "D"^^xsd:string;
 .
 
 #########################
 ## AutoSampler - Dummy ##
 #########################
 :AutoSampler_Dummy
     a OntoVapourtec:AutoSampler;
-    OntoLab:isContainedIn :Laboratory_Dummy;
     OntoLab:hasPowerSupply :AutoSampler_PowerSupply; # TODO
     dbo:manufacturer :VapourtecLtd;
     OntoVapourtec:sampleLoopVolume :AutoSampler_Dummy_SampleLoopVolume;
     OntoVapourtec:hasSite :Site_1;
     OntoVapourtec:hasSite :Site_2;
     OntoVapourtec:hasSite :Site_3;
     OntoVapourtec:hasSite :Site_4;
@@ -1260,15 +1250,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "1"^^xsd:string;
     OntoVapourtec:holds :Vial_1;
 .
 
 :Vial_1
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_1;
     OntoLab:isFilledWith :ChemicalAmount_1;
     OntoLab:hasMaxLevel :Vial_1_level_max;
     OntoLab:hasWarningLevel :Vial_1_level_warning;
     OntoLab:hasFillLevel :Vial_1_level_fill;
 .
 
 :Vial_1_level_max
@@ -1308,15 +1297,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "2"^^xsd:string;
     OntoVapourtec:holds :Vial_2;
 .
 
 :Vial_2
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_2;
     OntoLab:isFilledWith :ChemicalAmount_2;
     OntoLab:hasMaxLevel :Vial_2_level_max;
     OntoLab:hasWarningLevel :Vial_2_level_warning;
     OntoLab:hasFillLevel :Vial_2_level_fill;
 .
 
 :Vial_2_level_max
@@ -1356,15 +1344,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "3"^^xsd:string;
     OntoVapourtec:holds :Vial_3;
 .
 
 :Vial_3
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_3;
     OntoLab:isFilledWith :ChemicalAmount_3;
     OntoLab:hasMaxLevel :Vial_3_level_max;
     OntoLab:hasWarningLevel :Vial_3_level_warning;
     OntoLab:hasFillLevel :Vial_3_level_fill;
 .
 
 :Vial_3_level_max
@@ -1404,15 +1391,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "4"^^xsd:string;
     OntoVapourtec:holds :Vial_4;
 .
 
 :Vial_4
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_4;
     OntoLab:isFilledWith :ChemicalAmount_4;
     OntoLab:hasMaxLevel :Vial_4_level_max;
     OntoLab:hasWarningLevel :Vial_4_level_warning;
     OntoLab:hasFillLevel :Vial_4_level_fill;
 .
 
 :Vial_4_level_max
@@ -1452,15 +1438,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "5"^^xsd:string;
     OntoVapourtec:holds :Vial_5;
 .
 
 :Vial_5
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_5;
     OntoLab:isFilledWith :ChemicalAmount_For_Dummy_OutputChemical;
     OntoLab:hasMaxLevel :Vial_5_level_max;
     OntoLab:hasWarningLevel :Vial_5_level_warning;
     OntoLab:hasFillLevel :Vial_5_level_fill;
 .
 
 :Vial_5_level_max
@@ -1501,15 +1486,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "56"^^xsd:string;
     OntoVapourtec:holds :Vial_56;
 .
 
 :Vial_56
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_56;
     OntoLab:hasMaxLevel :Vial_56_level_max;
     OntoLab:hasWarningLevel :Vial_56_level_warning;
     OntoLab:hasFillLevel :Vial_56_level_fill;
 .
 
 :Vial_56_level_max
     a om:Volume;
@@ -1549,15 +1533,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "153"^^xsd:string;
     OntoVapourtec:holds :Vial_153;
 .
 
 :Vial_153
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_153;
     OntoLab:hasMaxLevel :Vial_153_level_max;
     OntoLab:hasWarningLevel :Vial_153_level_warning;
     OntoLab:hasFillLevel :Vial_153_level_fill;
 .
 
 :Vial_153_level_max
     a om:Volume;
@@ -1597,15 +1580,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "216"^^xsd:string;
     OntoVapourtec:holds :Vial_216;
 .
 
 :Vial_216
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_216;
     OntoLab:hasMaxLevel :Vial_216_level_max;
     OntoLab:hasWarningLevel :Vial_216_level_warning;
     OntoLab:hasFillLevel :Vial_216_level_fill;
 .
 
 :Vial_216_level_max
     a om:Volume;
@@ -1749,27 +1731,27 @@
     OntoCAPEUpp:comprisesDirectly :PhaseComponent_3_Property_1;
     OntoCAPEUpp:comprisesDirectly :PhaseComponent_4_Property_1;
 .
 
 
 :PhaseComponent_1
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
     OntoCAPEUpp:hasProperty :PhaseComponent_1_Property_1;
 .
 
 :PhaseComponent_2
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
     OntoCAPEUpp:hasProperty :PhaseComponent_2_Property_1;
 .
 
 :PhaseComponent_IS_Input
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     OntoCAPEUpp:hasProperty :PhaseComponent_IS_Input_Property_1;
 .
 
 :PhaseComponent_3
     rdf:type OntoCAPEPha:PhaseComponent;
     OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2>;
     OntoCAPEUpp:hasProperty :PhaseComponent_3_Property_1;
@@ -1785,27 +1767,27 @@
     rdf:type OntoCAPEPha:PhaseComponent;
     OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202>;
     OntoCAPEUpp:hasProperty :PhaseComponent_5_Property_1;
 .
 
 :PhaseComponent_6
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
     OntoCAPEUpp:hasProperty :PhaseComponent_6_Property_1;
 .
 
 :PhaseComponent_6_2
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
     OntoCAPEUpp:hasProperty :PhaseComponent_6_Property_2;
 .
 
 :PhaseComponent_7
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
     OntoCAPEUpp:hasProperty :PhaseComponent_7_Property_1;
 .
 
 :PhaseComponent_1_Property_1
     rdf:type OntoCAPEPha:Molarity;
     OntoCAPEUpp:hasValue :PhaseComponent_1_Property_1_ScalarValue_1;
 .
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 @prefix OntoCAPEPha:    <http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#> .
 @prefix OntoCAPEUpp:    <http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#> .
 @prefix ontospecies:    <http://www.theworldavatar.com/ontology/ontospecies/OntoSpecies.owl#> .
 @prefix OntoVapourtec:    <https://www.theworldavatar.com/kg/ontovapourtec/> .
 @prefix ontohplc:        <https://www.theworldavatar.com/kg/ontohplc/> .
 @prefix ontobpr:        <https://www.theworldavatar.com/kg/ontobpr/> .
 @prefix OntoLab:        <https://www.theworldavatar.com/kg/ontolab/> .
-@prefix :                <http://example.com/blazegraph/namespace/testlab/dummy_lab_for_post_proc/> .
-@prefix dummylab:       <http://example.com/blazegraph/namespace/testlab/dummy_lab/> .
+@prefix :                <https://example.com/blazegraph/namespace/testlab/dummy_lab_for_post_proc/> .
+@prefix dummylab:       <https://example.com/blazegraph/namespace/testlab/dummy_lab/> .
 
 @prefix exp1:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/> .
 @prefix exp2:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_2/> .
 @prefix exp3:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_3/> .
 @prefix exp4:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_4/> .
 @prefix exp5:            <https://www.example.com/triplestore/ontorxn/ReactionExperiment_5/> .
 @prefix ontorxn:        <https://www.theworldavatar.com/kg/ontoreaction/> .
@@ -74,15 +74,14 @@
     saref:consistsOf :AutoSampler_1;
     saref:hasState OntoVapourtec:RunningReaction;
 .
 
 :VapourtecR4_1
     a OntoVapourtec:VapourtecR4Reactor;
     OntoVapourtec:hasReactorVolume :VapourtecR4_1_ReactorVolume;
-    OntoLab:isSpecifiedBy :ReactorSettings_1;
 .
 
 :VapourtecR4_1_ReactorVolume
     a om:Volume;
     om:hasValue :VapR4_1_ReactorVolume_Value;
 .
 
@@ -91,14 +90,15 @@
     om:hasUnit om:millilitre;
     om:hasNumericalValue "10"^^xsd:double;
 .
 
 :ReactorSettings_1
     a OntoVapourtec:ReactorSettings;
     OntoLab:wasGeneratedFor <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70>;
+    OntoLab:specifies :VapourtecR4_1;
 .
 
 :AutoSampler_1
     a OntoVapourtec:AutoSampler;
     OntoVapourtec:hasSite :Site_1_1;
 .
 
@@ -106,15 +106,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "1"^^xsd:string;
     OntoVapourtec:holds :Vial_1_1;
 .
 
 :Vial_1_1
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_1_1;
     OntoLab:isFilledWith :ChemicalAmount_1_1;
 .
 
 :ChemicalAmount_1_1
     a OntoLab:ChemicalAmount;
     # OntoLab:containsUnidentifiedComponent is not specified for this chemical as it is not post processed yet
 .
@@ -140,15 +139,14 @@
     saref:consistsOf :AutoSampler_2;
     saref:hasState OntoVapourtec:RunningReaction;
 .
 
 :VapourtecR4_2
     a OntoVapourtec:VapourtecR4Reactor;
     OntoVapourtec:hasReactorVolume :VapourtecR4_2_ReactorVolume;
-    OntoLab:isSpecifiedBy :ReactorSettings_2;
 .
 
 :VapourtecR4_2_ReactorVolume
     a om:Volume;
     om:hasValue :VapR4_2_ReactorVolume_Value;
 .
 
@@ -157,14 +155,15 @@
     om:hasUnit om:millilitre;
     om:hasNumericalValue "10"^^xsd:double;
 .
 
 :ReactorSettings_2
     a OntoVapourtec:ReactorSettings;
     OntoLab:wasGeneratedFor <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8>;
+    OntoLab:specifies :VapourtecR4_2;
 .
 
 :AutoSampler_2
     a OntoVapourtec:AutoSampler;
     OntoVapourtec:hasSite :Site_2_1;
 .
 
@@ -172,15 +171,14 @@
     a OntoVapourtec:AutoSamplerSite;
     OntoVapourtec:locationID "1"^^xsd:string;
     OntoVapourtec:holds :Vial_2_1;
 .
 
 :Vial_2_1
     a OntoLab:Vial;
-    OntoVapourtec:isHeldIn :Site_2_1;
     OntoLab:isFilledWith :ChemicalAmount_2_1;
 .
 
 :ChemicalAmount_2_1
     a OntoLab:ChemicalAmount;
     # OntoLab:containsUnidentifiedComponent is not specified for this chemical as it is not post processed yet
 .
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/new_exp_data.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/new_exp_data.ttl`

 * *Files 4% similar despite different names*

```diff
@@ -34,37 +34,35 @@
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionPressure_a75c05d9-e6c5-4710-8618-cfada4d27ad3> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_db866035-fa8c-405e-9cd3-f7fe542a2eb3> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionScale_12f103bd-5831-4538-80f1-e9f1b67ccf3b> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_596b84d2-03d7-4715-9f00-56c45017cd19> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionTemperature_ccb93a20-fea9-4179-a3c2-067e31989adf> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_dce31f1f-6891-4b81-9a41-09163060eb6e> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ResidenceTime_f228988f-7b01-4776-84c0-8cf41bb57176> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_07d73e67-a930-42df-a475-2d1c3ac2d19f> .
 
-<https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/RxnExp_1> ns2:hasVariation <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> .
-
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_866bfdf2-0d32-40da-8fcb-f89669cf1d31> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_740fa259-0149-4f49-99e7-95fbcff8c7e7> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_8ae63d49-d3e5-469c-a85a-e7799ddf1807> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_02c2c471-cf86-4b6c-b41a-aa8cde84b457> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_c242fa46-e60c-481c-8dc2-741f69386f25> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_a7974834-3f69-4004-9831-15bf4c559b5e> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> .
@@ -120,43 +118,41 @@
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionPressure_06f24390-c46f-4a82-b998-d52f6b03701d> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_eace1d6e-3405-4584-907e-4bd0c3a37e48> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionScale_340aac69-106c-4894-94b9-a7c489b5c597> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_b8517bf9-6de4-4312-804e-90f6fa9ffd93> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionTemperature_9809328d-1e34-4b5f-87aa-67e4accb75bd> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_2e95d17c-48a9-4cf4-98a8-820e4cdeb674> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ResidenceTime_e8c453af-4dca-4e0b-8137-a073e1ab0d82> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_37d9d2de-f8b6-419a-8ca0-890cb41fbc6c> .
 
-<https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/RxnExp_1> ns2:hasVariation <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> .
-
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_4f55a3ff-3a06-4749-8775-52d7673497c7> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_90891b5e-2a35-4847-a39d-fbec6064c2d5> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_58691e29-9d69-41ad-ab5f-8fd9b35f5e0c> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_f2fbbd93-35b7-47d3-8bd6-446bac0b470b> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_6a845185-032d-41d8-86ff-6a9952418063> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_3d89e7e7-f7a4-45ff-b4aa-6c982ff28cf7> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> a ns2:ReactionVariation ;
     ns2:hasInputChemical <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1>,
         <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2>,
         <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> ;
     ns2:hasReactionCondition <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionPressure_06f24390-c46f-4a82-b998-d52f6b03701d>,
@@ -206,43 +202,41 @@
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionPressure_b57d5d10-70bc-43c5-9424-f493aeda7967> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_03a6b288-6bbc-4f4d-bb9c-2eecc2ad19da> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionScale_2845e69e-1441-4758-9803-f038744cea8a> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_9054ddbe-c176-493a-b5f1-149e8a2068b1> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionTemperature_867f1bd9-0c7b-41d1-adc6-44738631a568> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_ba9b84eb-0605-4d4e-83eb-74c3a706bc6f> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ResidenceTime_6e59352a-5296-4d13-8df9-2839b1f66eef> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_9479bc7e-a5f1-474d-bbd2-0c9d65bb24c3> .
 
-<https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/RxnExp_1> ns2:hasVariation <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> .
-
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_3712c062-8b67-4a82-82d9-166ff34909ba> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_c89f50e2-1909-4e9c-a456-83c894af387f> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_9968472e-74b9-4925-b5cc-63220f4be1a9> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_04daf6e1-2fe9-48cc-8096-ec383adf2bf3> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/StoichiometryRatio_fb5fecbb-3de2-4d98-b96c-38a3d033ca2d> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/Measure_686ffd08-02bb-4c8f-86bc-72433bd6ce1a> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2> .
 
 <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> a ns2:ReactionVariation ;
     ns2:hasInputChemical <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1>,
         <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2>,
         <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> ;
     ns2:hasReactionCondition <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/ReactionPressure_b57d5d10-70bc-43c5-9424-f493aeda7967>,
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl`

 * *Files 5% similar despite different names*

```diff
@@ -47,48 +47,46 @@
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionPressure_a75c05d9-e6c5-4710-8618-cfada4d27ad3> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_db866035-fa8c-405e-9cd3-f7fe542a2eb3> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionScale_12f103bd-5831-4538-80f1-e9f1b67ccf3b> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_596b84d2-03d7-4715-9f00-56c45017cd19> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionTemperature_ccb93a20-fea9-4179-a3c2-067e31989adf> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_dce31f1f-6891-4b81-9a41-09163060eb6e> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ResidenceTime_f228988f-7b01-4776-84c0-8cf41bb57176> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_07d73e67-a930-42df-a475-2d1c3ac2d19f> .
 
-<https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/RxnExp_1> ns2:hasVariation <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> .
-
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_866bfdf2-0d32-40da-8fcb-f89669cf1d31> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_740fa259-0149-4f49-99e7-95fbcff8c7e7> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_8ae63d49-d3e5-469c-a85a-e7799ddf1807> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_02c2c471-cf86-4b6c-b41a-aa8cde84b457> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_c242fa46-e60c-481c-8dc2-741f69386f25> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_a7974834-3f69-4004-9831-15bf4c559b5e> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70/Yield> a ns2:Yield ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70/Yield/Measure> ;
-    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
+    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70/Yield/Measure> a ns1:Measure ;
     ns1:hasNumericalValue "50"^^xsd:double ;
     ns1:hasUnit ns1:percent .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70> a ns2:ReactionVariation ;
     ns2:hasYield <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70/Yield> ;
@@ -148,48 +146,46 @@
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionPressure_06f24390-c46f-4a82-b998-d52f6b03701d> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_eace1d6e-3405-4584-907e-4bd0c3a37e48> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionScale_340aac69-106c-4894-94b9-a7c489b5c597> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_b8517bf9-6de4-4312-804e-90f6fa9ffd93> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionTemperature_9809328d-1e34-4b5f-87aa-67e4accb75bd> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_2e95d17c-48a9-4cf4-98a8-820e4cdeb674> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ResidenceTime_e8c453af-4dca-4e0b-8137-a073e1ab0d82> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_37d9d2de-f8b6-419a-8ca0-890cb41fbc6c> .
 
-<https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/RxnExp_1> ns2:hasVariation <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> .
-
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_4f55a3ff-3a06-4749-8775-52d7673497c7> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_90891b5e-2a35-4847-a39d-fbec6064c2d5> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_58691e29-9d69-41ad-ab5f-8fd9b35f5e0c> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_f2fbbd93-35b7-47d3-8bd6-446bac0b470b> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_6a845185-032d-41d8-86ff-6a9952418063> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_3d89e7e7-f7a4-45ff-b4aa-6c982ff28cf7> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8/Yield> a ns2:Yield ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8/Yield/Measure> ;
-    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
+    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8/Yield/Measure> a ns1:Measure ;
     ns1:hasNumericalValue "50"^^xsd:double ;
     ns1:hasUnit ns1:percent .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8> a ns2:ReactionVariation ;
     ns2:hasYield <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8/Yield> ;
@@ -250,49 +246,47 @@
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionPressure_b57d5d10-70bc-43c5-9424-f493aeda7967> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_03a6b288-6bbc-4f4d-bb9c-2eecc2ad19da> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionScale_2845e69e-1441-4758-9803-f038744cea8a> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_9054ddbe-c176-493a-b5f1-149e8a2068b1> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionTemperature_867f1bd9-0c7b-41d1-adc6-44738631a568> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_ba9b84eb-0605-4d4e-83eb-74c3a706bc6f> .
 
 # Commented out to minic missing condition
 # <https://intentionally_created_ReactionExperiment_out_of_range/ResidenceTime_6e59352a-5296-4d13-8df9-2839b1f66eef> a ns2:ResidenceTime ;
 #     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
 #     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_9479bc7e-a5f1-474d-bbd2-0c9d65bb24c3> .
 
-<https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/RxnExp_1> ns2:hasVariation <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> .
-
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_3712c062-8b67-4a82-82d9-166ff34909ba> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_c89f50e2-1909-4e9c-a456-83c894af387f> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_9968472e-74b9-4925-b5cc-63220f4be1a9> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_04daf6e1-2fe9-48cc-8096-ec383adf2bf3> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_1> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/StoichiometryRatio_fb5fecbb-3de2-4d98-b96c-38a3d033ca2d> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/Measure_686ffd08-02bb-4c8f-86bc-72433bd6ce1a> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_2> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf/Yield> a ns2:Yield ;
     ns1:hasValue <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf/Yield/Measure> ;
-    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
+    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf/Yield/Measure> a ns1:Measure ;
     ns1:hasNumericalValue "50"^^xsd:double ;
     ns1:hasUnit ns1:percent .
 
 <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf> a ns2:ReactionVariation ;
     ns2:hasYield <https://intentionally_created_ReactionExperiment_out_of_range/ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf/Yield> ;
@@ -352,48 +346,46 @@
 <https://yield_out_of_range/ReactionPressure_a75c05d9-e6c5-4710-8618-cfada4d27ad3> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_db866035-fa8c-405e-9cd3-f7fe542a2eb3> .
 
 <https://yield_out_of_range/ReactionScale_12f103bd-5831-4538-80f1-e9f1b67ccf3b> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_596b84d2-03d7-4715-9f00-56c45017cd19> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://yield_out_of_range/InputChemical_1> .
 
 <https://yield_out_of_range/ReactionTemperature_ccb93a20-fea9-4179-a3c2-067e31989adf> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_dce31f1f-6891-4b81-9a41-09163060eb6e> .
 
 <https://yield_out_of_range/ResidenceTime_f228988f-7b01-4776-84c0-8cf41bb57176> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_07d73e67-a930-42df-a475-2d1c3ac2d19f> .
 
-<https://yield_out_of_range/RxnExp_1> ns2:hasVariation <https://yield_out_of_range/ReactionExperiment_negative_yield> .
-
 <https://yield_out_of_range/StoichiometryRatio_866bfdf2-0d32-40da-8fcb-f89669cf1d31> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_740fa259-0149-4f49-99e7-95fbcff8c7e7> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://yield_out_of_range/InputChemical_2> .
 
 <https://yield_out_of_range/StoichiometryRatio_8ae63d49-d3e5-469c-a85a-e7799ddf1807> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_02c2c471-cf86-4b6c-b41a-aa8cde84b457> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://yield_out_of_range/InputChemical_1> .
 
 <https://yield_out_of_range/StoichiometryRatio_c242fa46-e60c-481c-8dc2-741f69386f25> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_negative_yield> ;
     ns1:hasValue <https://yield_out_of_range/Measure_a7974834-3f69-4004-9831-15bf4c559b5e> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://yield_out_of_range/InputChemical_3> .
 
 <https://yield_out_of_range/ReactionExperiment_negative_yield/Yield> a ns2:Yield ;
     ns1:hasValue <https://yield_out_of_range/ReactionExperiment_negative_yield/Yield/Measure> ;
-    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
+    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
 
 <https://yield_out_of_range/ReactionExperiment_negative_yield/Yield/Measure> a ns1:Measure ;
     ns1:hasNumericalValue "-5"^^xsd:double ;
     ns1:hasUnit ns1:percent .
 
 <https://yield_out_of_range/ReactionExperiment_negative_yield> a ns2:ReactionVariation ;
     ns2:hasYield <https://yield_out_of_range/ReactionExperiment_negative_yield/Yield> ;
@@ -453,48 +445,46 @@
 <https://yield_out_of_range/ReactionPressure_06f24390-c46f-4a82-b998-d52f6b03701d> a ns2:ReactionPressure ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_eace1d6e-3405-4584-907e-4bd0c3a37e48> .
 
 <https://yield_out_of_range/ReactionScale_340aac69-106c-4894-94b9-a7c489b5c597> a ns2:ReactionScale ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_b8517bf9-6de4-4312-804e-90f6fa9ffd93> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesUsageOf <https://yield_out_of_range/InputChemical_1> .
 
 <https://yield_out_of_range/ReactionTemperature_9809328d-1e34-4b5f-87aa-67e4accb75bd> a ns2:ReactionTemperature ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_2e95d17c-48a9-4cf4-98a8-820e4cdeb674> .
 
 <https://yield_out_of_range/ResidenceTime_e8c453af-4dca-4e0b-8137-a073e1ab0d82> a ns2:ResidenceTime ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_37d9d2de-f8b6-419a-8ca0-890cb41fbc6c> .
 
-<https://yield_out_of_range/RxnExp_1> ns2:hasVariation <https://yield_out_of_range/ReactionExperiment_yield_too_high> .
-
 <https://yield_out_of_range/StoichiometryRatio_4f55a3ff-3a06-4749-8775-52d7673497c7> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_90891b5e-2a35-4847-a39d-fbec6064c2d5> ;
     ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202" ;
     ns2:indicatesMultiplicityOf <https://yield_out_of_range/InputChemical_3> .
 
 <https://yield_out_of_range/StoichiometryRatio_58691e29-9d69-41ad-ab5f-8fd9b35f5e0c> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_f2fbbd93-35b7-47d3-8bd6-446bac0b470b> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b" ;
     ns2:indicatesMultiplicityOf <https://yield_out_of_range/InputChemical_1> .
 
 <https://yield_out_of_range/StoichiometryRatio_6a845185-032d-41d8-86ff-6a9952418063> a ns2:StoichiometryRatio ;
     ns1:hasPhenomenon <https://yield_out_of_range/ReactionExperiment_yield_too_high> ;
     ns1:hasValue <https://yield_out_of_range/Measure_3d89e7e7-f7a4-45ff-b4aa-6c982ff28cf7> ;
-    ns3:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
+    ns3:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3" ;
     ns2:indicatesMultiplicityOf <https://yield_out_of_range/InputChemical_2> .
 
 <https://yield_out_of_range/ReactionExperiment_yield_too_high/Yield> a ns2:Yield ;
     ns1:hasValue <https://yield_out_of_range/ReactionExperiment_yield_too_high/Yield/Measure> ;
-    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
+    ns2:yieldLimitingSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> .
 
 <https://yield_out_of_range/ReactionExperiment_yield_too_high/Yield/Measure> a ns1:Measure ;
     ns1:hasNumericalValue "110"^^xsd:double ;
     ns1:hasUnit ns1:percent .
 
 <https://yield_out_of_range/ReactionExperiment_yield_too_high> a ns2:ReactionVariation ;
     ns2:hasYield <https://yield_out_of_range/ReactionExperiment_yield_too_high/Yield> ;
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_incomplete.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_no_product.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/raw_hplc_report_xls_unidentified_peaks.xls`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/rxn_data.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/rxn_data.ttl`

 * *Files 3% similar despite different names*

```diff
@@ -15,60 +15,29 @@
 @prefix exp5:		    <https://www.example.com/triplestore/ontorxn/ReactionExperiment_5/> .
 @prefix SinglePhase:    <https://www.example.com/triplestore/ontorxn/SinglePhase/> .
 @prefix ChemRxn:        <https://www.example.com/triplestore/ontorxn/ChemRxn_1/> .
 @prefix doe_instance:   <https://www.example.com/triplestore/ontodoe/DoE_1/> .
 @prefix rdf:	    	<http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix xsd:            <http://www.w3.org/2001/XMLSchema#> .
 @prefix rdfs:		    <http://www.w3.org/2000/01/rdf-schema#> .
-@prefix placeholder:	<http://www.theworldavatar.com/kg/_for_species/> .
+@prefix placeholder:	<https://www.theworldavatar.com/kg/_for_species/> .
 
 
-##############################################################
-## Part of OntoRxn ontology for /subPropertyOf relationship ##
-##############################################################
-OntoRxn:ResidenceTime rdfs:subClassOf OntoRxn:ReactionCondition .
-OntoRxn:ReactionTemperature rdfs:subClassOf OntoRxn:ReactionCondition .
-OntoRxn:ReactionPressure rdfs:subClassOf OntoRxn:ReactionCondition .
-OntoRxn:StoichiometryRatio rdfs:subClassOf OntoRxn:ReactionCondition .
-OntoRxn:ReactionScale rdfs:subClassOf OntoRxn:ReactionCondition .
-
-OntoRxn:EnvironmentalFactor rdfs:subClassOf OntoRxn:PerformanceIndicator .
-OntoRxn:Yield rdfs:subClassOf OntoRxn:PerformanceIndicator .
-OntoRxn:EcoScore rdfs:subClassOf OntoRxn:PerformanceIndicator .
-OntoRxn:Conversion rdfs:subClassOf OntoRxn:PerformanceIndicator .
-OntoRxn:SpaceTimeYield rdfs:subClassOf OntoRxn:PerformanceIndicator .
-OntoRxn:RunMaterialCost rdfs:subClassOf OntoRxn:PerformanceIndicator .
-OntoRxn:RunMaterialCostPerKilogramProduct rdfs:subClassOf OntoRxn:PerformanceIndicator .
-
-OntoRxn:hasResTime rdfs:subPropertyOf OntoRxn:hasReactionCondition .
-OntoRxn:hasRxnTemperature rdfs:subPropertyOf OntoRxn:hasReactionCondition .
-OntoRxn:hasRxnPressure rdfs:subPropertyOf OntoRxn:hasReactionCondition .
-OntoRxn:hasStoichiometryRatio rdfs:subPropertyOf OntoRxn:hasReactionCondition .
-OntoRxn:hasRxnScale rdfs:subPropertyOf OntoRxn:hasReactionCondition .
-
-OntoRxn:hasEnvironmentalFactor rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-OntoRxn:hasYield rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-OntoRxn:hasEcoScore rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-OntoRxn:hasConversion rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-OntoRxn:hasSpaceTimeYield rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-OntoRxn:hasRunMaterialCost rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-OntoRxn:hasRunMaterialCostPerKilogramProduct rdfs:subPropertyOf OntoRxn:hasPerformanceIndicator .
-
 ##############################################################################
 ## Placeholder Density data -- TODO to find a proper way of representing it ##
 ##############################################################################
 # NOTE all the values are taken as its Specific Gravity at a temperature of 4 C if not otherwise noted
 
 # https://pubchem.ncbi.nlm.nih.gov/compound/240#section=Density&fullscreen=true
-<http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> placeholder:hasDensity placeholder:Density_Species_240.
+<http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> placeholder:hasDensity placeholder:Density_Species_240.
 placeholder:Density_Species_240 a om:Density; om:hasValue placeholder:D_S_240_V;.
 placeholder:D_S_240_V a om:Measure; om:hasUnit om:kilogramPerLitre; om:hasNumericalValue "1.04"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 # https://pubchem.ncbi.nlm.nih.gov/compound/180#section=Density&fullscreen=true
-<http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3> placeholder:hasDensity placeholder:Density_Species_180.
+<http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3> placeholder:hasDensity placeholder:Density_Species_180.
 placeholder:Density_Species_180 a om:Density; om:hasValue placeholder:D_S_180_V;.
 placeholder:D_S_180_V a om:Measure; om:hasUnit om:kilogramPerLitre; om:hasNumericalValue "0.784"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 # NO experimental data available at https://pubchem.ncbi.nlm.nih.gov/compound/637759
 # Data (mean value) from "Predicted - ACD/Labs" at http://www.chemspider.com/Chemical-Structure.21106584.html
 <http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2> placeholder:hasDensity placeholder:Density_Species_637759.
 placeholder:Density_Species_637759 a om:Density; om:hasValue placeholder:D_S_637759_V;.
@@ -82,37 +51,37 @@
 
 # Value taken as the solid density of NaOH at 68 F (20 C) in https://pubchem.ncbi.nlm.nih.gov/compound/14798#section=Density&fullscreen=true
 <http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202> placeholder:hasDensity placeholder:Density_Species_14798.
 placeholder:Density_Species_14798 a om:Density; om:hasValue placeholder:D_S_14798_V;.
 placeholder:D_S_14798_V a om:Measure; om:hasUnit om:kilogramPerLitre; om:hasNumericalValue "2.13"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 # https://pubchem.ncbi.nlm.nih.gov/compound/6342#section=Density&fullscreen=true
-<http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb> placeholder:hasDensity placeholder:Density_Species_6342.
+<http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb> placeholder:hasDensity placeholder:Density_Species_6342.
 placeholder:Density_Species_6342 a om:Density; om:hasValue placeholder:D_S_6342_V;.
 placeholder:D_S_6342_V a om:Measure; om:hasUnit om:kilogramPerLitre; om:hasNumericalValue "0.786"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 # https://pubchem.ncbi.nlm.nih.gov/compound/702#section=Density&fullscreen=true
-<http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983> placeholder:hasDensity placeholder:Density_Species_702.
+<http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983> placeholder:hasDensity placeholder:Density_Species_702.
 placeholder:Density_Species_702 a om:Density; om:hasValue placeholder:D_S_702_V;.
 placeholder:D_S_702_V a om:Measure; om:hasUnit om:kilogramPerLitre; om:hasNumericalValue "0.789"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 # https://pubchem.ncbi.nlm.nih.gov/compound/931#section=Density&fullscreen=true
-<http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340> placeholder:hasDensity placeholder:Density_Species_931.
+<http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340> placeholder:hasDensity placeholder:Density_Species_931.
 placeholder:Density_Species_931 a om:Density; om:hasValue placeholder:D_S_931_V;.
 placeholder:D_S_931_V a om:Measure; om:hasUnit om:kilogramPerLitre; om:hasNumericalValue "1.14"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 ####################################################################################
 ## Placeholder Material Cost data -- TODO to find a proper way of representing it ##
 ####################################################################################
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> placeholder:hasMaterialCost placeholder:MaterialCost_Species_240.
+<http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> placeholder:hasMaterialCost placeholder:MaterialCost_Species_240.
 placeholder:MaterialCost_Species_240 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_240_V;.
 placeholder:M_C_S_240_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "18.0024"^^xsd:double;. # calculated from https://doi.org/10.1002/cmtd.202000044
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3> placeholder:hasMaterialCost placeholder:MaterialCost_Species_180.
+<http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3> placeholder:hasMaterialCost placeholder:MaterialCost_Species_180.
 placeholder:MaterialCost_Species_180 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_180_V;.
 placeholder:M_C_S_180_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "6.38176"^^xsd:double;. # calculated from https://doi.org/10.1002/cmtd.202000044
 
 # dummy data
 <http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2> placeholder:hasMaterialCost placeholder:MaterialCost_Species_637759.
 placeholder:MaterialCost_Species_637759 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_637759_V;.
 placeholder:M_C_S_637759_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "500"^^xsd:double;.
@@ -122,37 +91,37 @@
 placeholder:MaterialCost_Species_640180 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_640180_V;.
 placeholder:M_C_S_640180_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "10"^^xsd:double;.
 
 <http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202> placeholder:hasMaterialCost placeholder:MaterialCost_Species_14798.
 placeholder:MaterialCost_Species_14798 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_14798_V;.
 placeholder:M_C_S_14798_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "58.575"^^xsd:double;. # calculated from https://doi.org/10.1002/cmtd.202000044
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb> placeholder:hasMaterialCost placeholder:MaterialCost_Species_6342.
+<http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb> placeholder:hasMaterialCost placeholder:MaterialCost_Species_6342.
 placeholder:MaterialCost_Species_6342 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_6342_V;.
 placeholder:M_C_S_6342_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "8.83"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983> placeholder:hasMaterialCost placeholder:MaterialCost_Species_702.
+<http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983> placeholder:hasMaterialCost placeholder:MaterialCost_Species_702.
 placeholder:MaterialCost_Species_702 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_702_V;.
 placeholder:M_C_S_702_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "8.83"^^xsd:double;. # from https://doi.org/10.1002/cmtd.202000044
 
 # dummy data
-<http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340> placeholder:hasMaterialCost placeholder:MaterialCost_Species_931.
+<http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340> placeholder:hasMaterialCost placeholder:MaterialCost_Species_931.
 placeholder:MaterialCost_Species_931 a om:SpecificAmountOfMoney; om:hasValue placeholder:M_C_S_931_V;.
 placeholder:M_C_S_931_V a om:Measure; om:hasUnit om:poundSterlingPerLitre; om:hasNumericalValue "400"^^xsd:double;.
 
 ###############################################################################
 ## Placeholder EcoScore data -- TODO to find a proper way of representing it ##
 ###############################################################################
 # NOTE all below eco-score data are dummy data
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> placeholder:hasEcoScore placeholder:EcoScore_Species_240.
+<http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b> placeholder:hasEcoScore placeholder:EcoScore_Species_240.
 placeholder:EcoScore_Species_240 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_240_V;.
 placeholder:E_S_S_240_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "20"^^xsd:double;.
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3> placeholder:hasEcoScore placeholder:EcoScore_Species_180.
+<http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3> placeholder:hasEcoScore placeholder:EcoScore_Species_180.
 placeholder:EcoScore_Species_180 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_180_V;.
 placeholder:E_S_S_180_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "70"^^xsd:double;.
 
 <http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2> placeholder:hasEcoScore placeholder:EcoScore_Species_637759.
 placeholder:EcoScore_Species_637759 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_637759_V;.
 placeholder:E_S_S_637759_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "50"^^xsd:double;.
 
@@ -160,23 +129,23 @@
 placeholder:EcoScore_Species_640180 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_640180_V;.
 placeholder:E_S_S_640180_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "10"^^xsd:double;.
 
 <http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202> placeholder:hasEcoScore placeholder:EcoScore_Species_14798.
 placeholder:EcoScore_Species_14798 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_14798_V;.
 placeholder:E_S_S_14798_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "20"^^xsd:double;.
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb> placeholder:hasEcoScore placeholder:EcoScore_Species_6342.
+<http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb> placeholder:hasEcoScore placeholder:EcoScore_Species_6342.
 placeholder:EcoScore_Species_6342 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_6342_V;.
 placeholder:E_S_S_6342_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "60"^^xsd:double;.
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983> placeholder:hasEcoScore placeholder:EcoScore_Species_702.
+<http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983> placeholder:hasEcoScore placeholder:EcoScore_Species_702.
 placeholder:EcoScore_Species_702 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_702_V;.
 placeholder:E_S_S_702_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "30"^^xsd:double;.
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340> placeholder:hasEcoScore placeholder:EcoScore_Species_931.
+<http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340> placeholder:hasEcoScore placeholder:EcoScore_Species_931.
 placeholder:EcoScore_Species_931 a om:QuantityOfDimensionOne; om:hasValue placeholder:E_S_S_931_V;.
 placeholder:E_S_S_931_V a om:Measure; om:hasUnit om:one; om:hasNumericalValue "40"^^xsd:double;.
 
 ################################
 ## Reaction experiment data 1 ##
 ################################
 exp1:RxnExp_1
@@ -275,29 +244,29 @@
 exp1:OutputChemical_4
     rdf:type OntoRxn:OutputChemical;
     OntoCAPEMat:thermodynamicBehavior SinglePhase:Phase_OutputChemical_exp1;
 .
 
 exp1:StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp1:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp1:InputChemical_1;
     om:hasValue exp1:StoiRatio_1_Measure_1;
 .
 
 exp1:StoiRatio_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 exp1:StoiRatio_2
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     om:hasPhenomenon exp1:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp1:InputChemical_2;
     om:hasValue exp1:StoiRatio_2_Measure_1;
 .
 
 exp1:StoiRatio_2_Measure_1
     rdf:type om:Measure;
@@ -317,15 +286,15 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "0.17"^^xsd:double;
 .
 
 exp1:RxnScale_1
     rdf:type OntoRxn:ReactionScale;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp1:RxnExp_1;
     OntoRxn:indicatesUsageOf exp1:InputChemical_1;
     om:hasValue exp1:RxnScale_1_Measure_1;
 .
 
 exp1:RxnScale_1_Measure_1
     rdf:type om:Measure;
@@ -432,29 +401,29 @@
 exp2:OutputChemical_4
     rdf:type OntoRxn:OutputChemical;
     OntoCAPEMat:thermodynamicBehavior SinglePhase:Phase_OutputChemical_exp2;
 .
 
 exp2:StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp2:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp2:InputChemical_1;
     om:hasValue exp2:StoiRatio_1_Measure_1;
 .
 
 exp2:StoiRatio_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 exp2:StoiRatio_2
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     om:hasPhenomenon exp2:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp2:InputChemical_2;
     om:hasValue exp2:StoiRatio_2_Measure_1;
 .
 
 exp2:StoiRatio_2_Measure_1
     rdf:type om:Measure;
@@ -474,15 +443,15 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "0.04"^^xsd:double;
 .
 
 exp2:RxnScale_1
     rdf:type OntoRxn:ReactionScale;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp2:RxnExp_1;
     OntoRxn:indicatesUsageOf exp2:InputChemical_1;
     om:hasValue exp2:RxnScale_1_Measure_1;
 .
 
 exp2:RxnScale_1_Measure_1
     rdf:type om:Measure;
@@ -589,29 +558,29 @@
 exp3:OutputChemical_4
     rdf:type OntoRxn:OutputChemical;
     OntoCAPEMat:thermodynamicBehavior SinglePhase:Phase_OutputChemical_exp3;
 .
 
 exp3:StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp3:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp3:InputChemical_1;
     om:hasValue exp3:StoiRatio_1_Measure_1;
 .
 
 exp3:StoiRatio_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 exp3:StoiRatio_2
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     om:hasPhenomenon exp3:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp3:InputChemical_2;
     om:hasValue exp3:StoiRatio_2_Measure_1;
 .
 
 exp3:StoiRatio_2_Measure_1
     rdf:type om:Measure;
@@ -631,15 +600,15 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "0.16"^^xsd:double;
 .
 
 exp3:RxnScale_1
     rdf:type OntoRxn:ReactionScale;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp3:RxnExp_1;
     OntoRxn:indicatesUsageOf exp3:InputChemical_1;
     om:hasValue exp3:RxnScale_1_Measure_1;
 .
 
 exp3:RxnScale_1_Measure_1
     rdf:type om:Measure;
@@ -746,29 +715,29 @@
 exp4:OutputChemical_4
     rdf:type OntoRxn:OutputChemical;
     OntoCAPEMat:thermodynamicBehavior SinglePhase:Phase_OutputChemical_exp4;
 .
 
 exp4:StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp4:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp4:InputChemical_1;
     om:hasValue exp4:StoiRatio_1_Measure_1;
 .
 
 exp4:StoiRatio_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 exp4:StoiRatio_2
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     om:hasPhenomenon exp4:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp4:InputChemical_2;
     om:hasValue exp4:StoiRatio_2_Measure_1;
 .
 
 exp4:StoiRatio_2_Measure_1
     rdf:type om:Measure;
@@ -788,15 +757,15 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "0.07"^^xsd:double;
 .
 
 exp4:RxnScale_1
     rdf:type OntoRxn:ReactionScale;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp4:RxnExp_1;
     OntoRxn:indicatesUsageOf exp4:InputChemical_1;
     om:hasValue exp4:RxnScale_1_Measure_1;
 .
 
 exp4:RxnScale_1_Measure_1
     rdf:type om:Measure;
@@ -903,29 +872,29 @@
 exp5:OutputChemical_4
     rdf:type OntoRxn:OutputChemical;
     OntoCAPEMat:thermodynamicBehavior SinglePhase:Phase_OutputChemical_exp5;
 .
 
 exp5:StoiRatio_1
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp5:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp5:InputChemical_1;
     om:hasValue exp5:StoiRatio_1_Measure_1;
 .
 
 exp5:StoiRatio_1_Measure_1
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "1.0"^^xsd:double;
 .
 
 exp5:StoiRatio_2
     rdf:type OntoRxn:StoichiometryRatio;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3"^^xsd:string;
     om:hasPhenomenon exp5:RxnExp_1;
     OntoRxn:indicatesMultiplicityOf exp5:InputChemical_2;
     om:hasValue exp5:StoiRatio_2_Measure_1;
 .
 
 exp5:StoiRatio_2_Measure_1
     rdf:type om:Measure;
@@ -945,15 +914,15 @@
     rdf:type om:Measure;
     om:hasUnit om:one;
     om:hasNumericalValue "0.10"^^xsd:double;
 .
 
 exp5:RxnScale_1
     rdf:type OntoRxn:ReactionScale;
-    OntoDoE:positionalID "http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
+    OntoDoE:positionalID "http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b"^^xsd:string;
     om:hasPhenomenon exp5:RxnExp_1;
     OntoRxn:indicatesUsageOf exp5:InputChemical_1;
     om:hasValue exp5:RxnScale_1_Measure_1;
 .
 
 exp5:RxnScale_1_Measure_1
     rdf:type om:Measure;
@@ -961,58 +930,53 @@
     om:hasNumericalValue "5"^^xsd:double;
 .
 
 #################################
 ## Chemical reaction instances ##
 #################################
 ChemRxn:ChemRxn_1
-    rdf:type OntoCAPERxn:ChemicalReaction;
-    OntoRxn:isRealisedAs exp1:RxnExp_1;
-    OntoRxn:isRealisedAs exp2:RxnExp_1;
-    OntoRxn:isRealisedAs exp3:RxnExp_1;
-    OntoRxn:isRealisedAs exp4:RxnExp_1;
-    OntoRxn:isRealisedAs exp5:RxnExp_1;
+    rdf:type OntoRxn:ChemicalReaction;
     OntoKin:hasEquation "C6H5CHO + CH3COCH3 = C10H10O"^^xsd:string;
     OntoCAPERxn:hasReactant ChemRxn:Species_1;
     OntoCAPERxn:hasReactant ChemRxn:Species_2;
     OntoCAPERxn:hasProduct ChemRxn:Species_3;
     OntoCAPERxn:hasProduct ChemRxn:Species_4;
-    OntoCAPERxn:hasCatalyst ChemRxn:Species_5;
+    OntoRxn:hasCatalyst ChemRxn:Species_5;
     OntoRxn:hasSolvent ChemRxn:Species_6;
     OntoRxn:hasSolvent ChemRxn:Species_7;
 .
 
 ChemRxn:Species_1
     rdf:type OntoKin:Reactant;
-    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
+    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
 .
 
 # NOTE we hardcode the OntoSpecies instance IRIs here to simplify the implementation for the purpose of testing
 # NOTE for the production operations, one need to provide access to a real triple store of OntoSpecies
 # NOTE where the instance IRI of a real OntoSpecies:Species will be obtained/identified based on specific identifiers
 # NOTE i.e. OntoSpecies:inChI, OntoSpecies:pubChemCID, etc.
-<http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>
+<http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>
     # OntoSpecies:pubChemCID "240"^^xsd:string;
     rdfs:label "C7H6O"^^xsd:string;
     skos:altLabel "benzaldehyde"^^xsd:string;
     OntoSpecies:hasMolecularWeight <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
 .
 
 <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>
     a OntoSpecies:MolecularWeight;
     OntoSpecies:units <http://www.theworldavatar.com/kg/ontospecies/Unit_a501ff0e-7cbc-4e3c-ba2e-211da22cac2b>;
     OntoSpecies:value "106.12"^^xsd:decimal;
 .
 
 ChemRxn:Species_2
     rdf:type OntoKin:Reactant;
-    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
+    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
 .
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>
+<http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>
     # OntoSpecies:pubChemCID "180"^^xsd:string;
     rdfs:label "C3H6O"^^xsd:string;
     skos:altLabel "acetone"^^xsd:string;
     OntoSpecies:hasMolecularWeight <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
 .
 
 <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_353d4667-e25d-476a-bd74-5c34723c8ea3>
@@ -1073,62 +1037,62 @@
     a OntoSpecies:MolecularWeight;
     OntoSpecies:units <http://www.theworldavatar.com/kg/ontospecies/Unit_a501ff0e-7cbc-4e3c-ba2e-211da22cac2b>;
     OntoSpecies:value "39.997"^^xsd:decimal;
 .
 
 ChemRxn:Species_6
     rdf:type OntoRxn:Solvent;
-    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
 .
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>
+<http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>
     # OntoSpecies:pubChemCID "6342"^^xsd:string;
     rdfs:label "CH3CN"^^xsd:string;
     skos:altLabel "acetonitrile"^^xsd:string;
     OntoSpecies:hasMolecularWeight <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
 .
 
 <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>
     a OntoSpecies:MolecularWeight;
     OntoSpecies:units <http://www.theworldavatar.com/kg/ontospecies/Unit_a501ff0e-7cbc-4e3c-ba2e-211da22cac2b>;
     OntoSpecies:value "41.05"^^xsd:decimal;
 .
 
 ChemRxn:Species_7
     rdf:type OntoRxn:Solvent;
-    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
+    OntoSpecies:hasUniqueSpecies <http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
 .
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>
+<http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>
     # OntoSpecies:pubChemCID "702"^^xsd:string;
     rdfs:label "C2H6O"^^xsd:string;
     skos:altLabel "ethanol"^^xsd:string;
     OntoSpecies:hasMolecularWeight <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
 .
 
 <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_63fefc5a-d49d-4841-a946-2cdb5f356983>
     a OntoSpecies:MolecularWeight;
     OntoSpecies:units <http://www.theworldavatar.com/kg/ontospecies/Unit_a501ff0e-7cbc-4e3c-ba2e-211da22cac2b>;
     OntoSpecies:value "46.07"^^xsd:decimal;
 .
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>
+<http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>
     # OntoSpecies:pubChemCID "931"^^xsd:string;
     rdfs:label "C10H8"^^xsd:string;
     skos:altLabel "naphthalene"^^xsd:string;
     OntoSpecies:hasMolecularWeight <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
 .
 
 <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>
     a OntoSpecies:MolecularWeight;
     OntoSpecies:units <http://www.theworldavatar.com/kg/ontospecies/Unit_a501ff0e-7cbc-4e3c-ba2e-211da22cac2b>;
     OntoSpecies:value "128.17"^^xsd:decimal;
 .
 
-<http://www.theworldavatar.com/kb/ontospecies/Species_471ce681-98f3-4245-be7d-3f38dfb6dd22>
+<http://www.theworldavatar.com/kg/ontospecies/Species_471ce681-98f3-4245-be7d-3f38dfb6dd22>
     # OntoSpecies:pubChemCID "7095"^^xsd:string;
     rdfs:label "C12H10"^^xsd:string;
     skos:altLabel "biphenyl"^^xsd:string;
     OntoSpecies:hasMolecularWeight <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_471ce681-98f3-4245-be7d-3f38dfb6dd22>;
 .
 
 <http://www.theworldavatar.com/kg/ontospecies/MolecularWeight_1_Species_471ce681-98f3-4245-be7d-3f38dfb6dd22>
@@ -1143,51 +1107,51 @@
 .
 
 ##############################
 ## Chemical phase instances ##
 ##############################
 SinglePhase:PhaseComponent_1
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_1_Property_1;
 .
 
 SinglePhase:PhaseComponent_2
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_2_Property_1;
 .
 
 SinglePhase:PhaseComponent_5
     rdf:type OntoCAPEPha:PhaseComponent;
     OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_5_Property_1;
 .
 
 SinglePhase:PhaseComponent_6
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_6_Property_1;
 .
 
 SinglePhase:PhaseComponent_6_2
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_6_Property_2;
 .
 
 SinglePhase:PhaseComponent_7
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_7_Property_1;
 .
 
 SinglePhase:PhaseComponent_IS_Input
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_IS_Input_Property_1;
 .
 
 SinglePhase:PhaseComponent_1_Property_1
     rdf:type OntoCAPEPha:Molarity;
     OntoCAPEUpp:hasValue SinglePhase:PhaseComponent_1_Property_1_ScalarValue_1;
 .
@@ -1350,21 +1314,21 @@
     OntoCAPEUpp:comprisesDirectly SinglePhase:PhaseComponent_6_exp1_oc_Property_1;
     OntoCAPEUpp:comprisesDirectly SinglePhase:PhaseComponent_7_exp1_oc_Property_1;
     OntoCAPEUpp:comprisesDirectly SinglePhase:PhaseComponent_InternalStandard_exp1_Property_1;
 .
 
 SinglePhase:PhaseComponent_1_exp1_oc
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_1_exp1_oc_Property_1;
 .
 
 SinglePhase:PhaseComponent_2_exp1_oc
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_2_exp1_oc_Property_1;
 .
 
 SinglePhase:PhaseComponent_3_exp1_oc
     rdf:type OntoCAPEPha:PhaseComponent;
     OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_3_exp1_oc_Property_1;
@@ -1380,27 +1344,27 @@
     rdf:type OntoCAPEPha:PhaseComponent;
     OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_5_exp1_oc_Property_1;
 .
 
 SinglePhase:PhaseComponent_6_exp1_oc
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_6_exp1_oc_Property_1;
 .
 
 SinglePhase:PhaseComponent_7_exp1_oc
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_7_exp1_oc_Property_1;
 .
 
 SinglePhase:PhaseComponent_IS_exp1_oc
     rdf:type OntoCAPEPha:PhaseComponent;
-    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
+    OntoCAPEPha:representsOccurenceOf <http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340>;
     OntoCAPEUpp:hasProperty SinglePhase:PhaseComponent_InternalStandard_exp1_Property_1;
 .
 
 SinglePhase:PhaseComponent_1_exp1_oc_Property_1
     rdf:type OntoCAPEPha:Molarity;
     OntoCAPEUpp:hasValue SinglePhase:PhaseComponent_1_exp1_oc_Property_1_ScalarValue_1;
 .
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl` & `chemistry_and_robots-1.6.0/chemistry_and_robots/resources/sample_data/rxn_queue_test.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 @prefix ontodoe:		<https://www.theworldavatar.com/kg/ontodoe/> .
 @prefix ontorxn:		<https://www.theworldavatar.com/kg/ontoreaction/> .
 @prefix ontoderivation: <https://www.theworldavatar.com/kg/ontoderivation/> .
-@prefix : <http://example.com/blazegraph/namespace/test_temp/> .
-@prefix doeagent: <http://www.theworldavatar.com/resource/agents/Service__DoE#> .
-@prefix exeagent: <http://www.theworldavatar.com/resource/agents/Service__Execution#> .
-@prefix postprocagent: <http://www.theworldavatar.com/resource/agents/Service__PostProc#> .
+@prefix : <https://example.com/blazegraph/namespace/test_temp/> .
+@prefix doeagent: <https://www.theworldavatar.com/kg/agents/Service__DoE/> .
+@prefix exeagent: <https://www.theworldavatar.com/kg/agents/Service__Execution/> .
+@prefix postprocagent: <https://www.theworldavatar.com/kg/agents/Service__PostProc/> .
 @prefix time: <http://www.w3.org/2006/time#> .
 
 :postproc_derivation_6 ontoderivation:isDerivedFrom :exe_6 ;
 	ontoderivation:isDerivedUsing postprocagent:Service ;
 	a ontoderivation:DerivationAsyn .
 
 :postproc_derivation_7 ontoderivation:isDerivedFrom :exe_7 ;
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/conftest.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,17 @@
     # Upload the example triples for testing
     pathlist = Path(RESOURCE_DIR).glob('**/*.ttl')
     for path in pathlist:
         g = Graph()
         g.parse(str(path), format='turtle')
         sparql_client.uploadGraph(g)
 
+    sparql_client.upload_ontology_tbox(onto.ONTODOE)
+    sparql_client.upload_ontology_tbox(onto.ONTOREACTION)
+
     # Create folder for downloaded files
     if not os.path.exists(DOWNLOADED_DIR):
         os.mkdir(DOWNLOADED_DIR)
 
     yield sparql_client
 
     # Clear all triples
@@ -166,16 +169,16 @@
     for logger in loggers:
         handlers = getattr(logger, 'handlers', [])
         for handler in handlers:
             logger.removeHandler(handler)
 
 class TargetIRIs(Enum):
     CHEMICAL_REACTION_BASE_IRI = 'https://www.example.com/triplestore/ontorxn/ChemRxn_1/'
-    DUMMY_VAPOURTEC_EXECUTION_AGENT_SERVICE_IRI = 'http://www.theworldavatar.com/resource/agents/Service__Execution#Service' # same as in rxn_queue_test.ttl
-    DUMMY_LAB_BASE_IRI = 'http://example.com/blazegraph/namespace/testlab/dummy_lab/'
+    DUMMY_VAPOURTEC_EXECUTION_AGENT_SERVICE_IRI = 'https://www.theworldavatar.com/kg/agents/Service__Execution/Service' # same as in rxn_queue_test.ttl
+    DUMMY_LAB_BASE_IRI = 'https://example.com/blazegraph/namespace/testlab/dummy_lab/'
     DUMMY_LAB_IRI = DUMMY_LAB_BASE_IRI + 'Laboratory_Dummy'
     AUTOMATEDRXNPLATFORM_DUMMY_IRI = DUMMY_LAB_BASE_IRI + 'AutomatedRxnPlatform_Dummy'
     VAPOURTECRS400_DUMMY_IRI = DUMMY_LAB_BASE_IRI + 'VapourtecRS400_Dummy'
     VAPOURTEC_LTD = DUMMY_LAB_BASE_IRI + 'VapourtecLtd'
     VAPOURTECRS400_POWERSUPPLY = DUMMY_LAB_BASE_IRI + 'VapRS400_PowerSupply'
     VAPOURTECRS400_DUMMY_COLLECTION_METHOD_IRI = DUMMY_LAB_BASE_IRI + 'CollectionMethod_VapourtecRS400_Dummy'
     VAPOURTECRS400_DUMMY_COLLECTION_METHOD_TO_RECEPTACLE_IRI = DUMMY_LAB_BASE_IRI + 'WasteReceptacle_Dummy'
@@ -204,22 +207,22 @@
         DUMMY_LAB_BASE_IRI + 'Site_4': 7.0,
         DUMMY_LAB_BASE_IRI + 'Site_216': 0.0,
         DUMMY_LAB_BASE_IRI + 'Site_5': 3.0}
     AUTOSAMPLER_LIQUID_COMPONENT_DICT = {
         DUMMY_LAB_BASE_IRI + 'Site_4': ['http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2',
             'http://www.theworldavatar.com/kg/ontospecies/Species_8765d201-0da9-4112-b653-3455002f535b'],
         DUMMY_LAB_BASE_IRI + 'Site_5': ['http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2',
-            'http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340'],
+            'http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340'],
         DUMMY_LAB_BASE_IRI + 'Site_3': ['http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202',
-            'http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983'],
-        DUMMY_LAB_BASE_IRI + 'Site_1': ['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-            'http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',
-            'http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340'],
-        DUMMY_LAB_BASE_IRI + 'Site_2': ['http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
-            'http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb']
+            'http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983'],
+        DUMMY_LAB_BASE_IRI + 'Site_1': ['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+            'http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',
+            'http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340'],
+        DUMMY_LAB_BASE_IRI + 'Site_2': ['http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+            'http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb']
     }
     AUTOSAMPLER_LIQUID_CONTAINS_UNIDENTIFIED_COMPONENT_DICT = {
         DUMMY_LAB_BASE_IRI + 'Site_4': False,
         DUMMY_LAB_BASE_IRI + 'Site_5': True,
         DUMMY_LAB_BASE_IRI + 'Site_3': False,
         DUMMY_LAB_BASE_IRI + 'Site_1': False,
         DUMMY_LAB_BASE_IRI + 'Site_2': False,
@@ -297,79 +300,79 @@
         EXP_1_BASE_IRI+'StoichiometryRatio_3712c062-8b67-4a82-82d9-166ff34909ba',
         EXP_1_BASE_IRI+'StoichiometryRatio_9968472e-74b9-4925-b5cc-63220f4be1a9',
         EXP_1_BASE_IRI+'StoichiometryRatio_fb5fecbb-3de2-4d98-b96c-38a3d033ca2d']
     NEW_RXN_EXP_1_PERFORMANCE_INDICATOR_IRI_LIST = None
     NEW_RXN_EXP_2_PERFORMANCE_INDICATOR_IRI_LIST = None
     NEW_RXN_EXP_3_PERFORMANCE_INDICATOR_IRI_LIST = None
     RXN_EXP_REACTION_CONDITION_CLZ_POSITIONAL_ID_DICT = {EXAMPLE_RXN_EXP_1_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         EXAMPLE_RXN_EXP_2_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         EXAMPLE_RXN_EXP_3_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         EXAMPLE_RXN_EXP_4_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         EXAMPLE_RXN_EXP_5_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         NEW_RXN_EXP_1_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         NEW_RXN_EXP_2_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']},
         NEW_RXN_EXP_3_IRI:{onto.ONTOREACTION_RESIDENCETIME:[None], onto.ONTOREACTION_REACTIONPRESSURE:[None],
-        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
-        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-        'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        onto.ONTOREACTION_REACTIONSCALE:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'],
+        onto.ONTOREACTION_REACTIONTEMPERATURE:[None], onto.ONTOREACTION_STOICHIOMETRYRATIO:['http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+        'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
         'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202']}}
     RXN_EXP_REACTION_CONDITION_POSITIONAL_ID_DICT = {
-        EXAMPLE_RXN_EXP_1_IRI:{EXP_1_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        EXAMPLE_RXN_EXP_1_IRI:{EXP_1_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                                EXP_1_BASE_IRI+'StoiRatio_3':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        EXAMPLE_RXN_EXP_2_IRI:{EXP_2_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        EXAMPLE_RXN_EXP_2_IRI:{EXP_2_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                                EXP_2_BASE_IRI+'StoiRatio_3':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        EXAMPLE_RXN_EXP_3_IRI:{EXP_3_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        EXAMPLE_RXN_EXP_3_IRI:{EXP_3_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                                EXP_3_BASE_IRI+'StoiRatio_3':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        EXAMPLE_RXN_EXP_4_IRI:{EXP_4_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        EXAMPLE_RXN_EXP_4_IRI:{EXP_4_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                                EXP_4_BASE_IRI+'StoiRatio_3':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        EXAMPLE_RXN_EXP_5_IRI:{EXP_5_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        EXAMPLE_RXN_EXP_5_IRI:{EXP_5_BASE_IRI+'StoiRatio_2':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                                EXP_5_BASE_IRI+'StoiRatio_3':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        NEW_RXN_EXP_1_IRI:{EXP_1_BASE_IRI+'StoichiometryRatio_866bfdf2-0d32-40da-8fcb-f89669cf1d31':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        NEW_RXN_EXP_1_IRI:{EXP_1_BASE_IRI+'StoichiometryRatio_866bfdf2-0d32-40da-8fcb-f89669cf1d31':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                            EXP_1_BASE_IRI+'StoichiometryRatio_c242fa46-e60c-481c-8dc2-741f69386f25':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        NEW_RXN_EXP_2_IRI:{EXP_1_BASE_IRI+'StoichiometryRatio_6a845185-032d-41d8-86ff-6a9952418063':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        NEW_RXN_EXP_2_IRI:{EXP_1_BASE_IRI+'StoichiometryRatio_6a845185-032d-41d8-86ff-6a9952418063':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                            EXP_1_BASE_IRI+'StoichiometryRatio_4f55a3ff-3a06-4749-8775-52d7673497c7':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'},
-        NEW_RXN_EXP_3_IRI:{EXP_1_BASE_IRI+'StoichiometryRatio_fb5fecbb-3de2-4d98-b96c-38a3d033ca2d':'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
+        NEW_RXN_EXP_3_IRI:{EXP_1_BASE_IRI+'StoichiometryRatio_fb5fecbb-3de2-4d98-b96c-38a3d033ca2d':'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',
                            EXP_1_BASE_IRI+'StoichiometryRatio_3712c062-8b67-4a82-82d9-166ff34909ba':'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'}}
 
     CHEMICAL_REACTION_IRI = CHEMICAL_REACTION_BASE_IRI + 'ChemRxn_1'
-    REACTANT_SPECIES_DICTIONARY = {CHEMICAL_REACTION_BASE_IRI + 'Species_1': 'http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
-    CHEMICAL_REACTION_BASE_IRI + 'Species_2': 'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3'}
+    REACTANT_SPECIES_DICTIONARY = {CHEMICAL_REACTION_BASE_IRI + 'Species_1': 'http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',
+    CHEMICAL_REACTION_BASE_IRI + 'Species_2': 'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3'}
     PRODUCT_SPECIES_DICTIONARY = {CHEMICAL_REACTION_BASE_IRI + 'Species_3': 'http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2',
     CHEMICAL_REACTION_BASE_IRI + 'Species_4': 'http://www.theworldavatar.com/kg/ontospecies/Species_8765d201-0da9-4112-b653-3455002f535b'}
     CATALYST_SPECIES_DICTIONARY = {CHEMICAL_REACTION_BASE_IRI + 'Species_5': 'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202'}
-    SOLVENT_SPECIES_DICTIONARY = {CHEMICAL_REACTION_BASE_IRI + 'Species_6': 'http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',
-    CHEMICAL_REACTION_BASE_IRI + 'Species_7': 'http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983'}
+    SOLVENT_SPECIES_DICTIONARY = {CHEMICAL_REACTION_BASE_IRI + 'Species_6': 'http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',
+    CHEMICAL_REACTION_BASE_IRI + 'Species_7': 'http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983'}
     EXP_1_INPUT_CHEMICAL_1_IRI = EXP_1_BASE_IRI + 'InputChemical_1'
     EXP_1_INPUT_CHEMICAL_2_IRI = EXP_1_BASE_IRI + 'InputChemical_2'
     EXP_1_INPUT_CHEMICAL_3_IRI = EXP_1_BASE_IRI + 'InputChemical_3'
     EXP_2_INPUT_CHEMICAL_1_IRI = EXP_2_BASE_IRI + 'InputChemical_1'
     EXP_2_INPUT_CHEMICAL_2_IRI = EXP_2_BASE_IRI + 'InputChemical_2'
     EXP_2_INPUT_CHEMICAL_3_IRI = EXP_2_BASE_IRI + 'InputChemical_3'
     EXP_3_INPUT_CHEMICAL_1_IRI = EXP_3_BASE_IRI + 'InputChemical_1'
@@ -405,22 +408,22 @@
 
     AUTOSAMPLER_SITE_CHEMICAL_MAPPING_DICT = {
         DUMMY_LAB_BASE_IRI + 'Site_3': EXP_1_INPUT_CHEMICAL_3_IRI,
         DUMMY_LAB_BASE_IRI + 'Site_1': EXP_1_INPUT_CHEMICAL_1_IRI,
         DUMMY_LAB_BASE_IRI + 'Site_2': EXP_1_INPUT_CHEMICAL_2_IRI
     }
 
-    SPECIES_MOLAR_MASS_DICT = {"http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b": 106.12/1000,
-        "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3": 58.08/1000,
+    SPECIES_MOLAR_MASS_DICT = {"http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b": 106.12/1000,
+        "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3": 58.08/1000,
         'http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2': 146.19/1000,
         'http://www.theworldavatar.com/kg/ontospecies/Species_8765d201-0da9-4112-b653-3455002f535b': 234.29/1000,
         "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202": 39.997/1000,
-        "http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb": 41.05/1000,
-        "http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983": 46.07/1000,
-        "http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340": 128.17/1000}
+        "http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb": 41.05/1000,
+        "http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983": 46.07/1000,
+        "http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340": 128.17/1000}
 
     RXNEXP_TYPE_DICT = {EXAMPLE_RXN_EXP_1_IRI:onto.ONTOREACTION_REACTIONEXPERIMENT,EXAMPLE_RXN_EXP_2_IRI:onto.ONTOREACTION_REACTIONEXPERIMENT,
         EXAMPLE_RXN_EXP_3_IRI:onto.ONTOREACTION_REACTIONEXPERIMENT,EXAMPLE_RXN_EXP_4_IRI:onto.ONTOREACTION_REACTIONEXPERIMENT,
         EXAMPLE_RXN_EXP_5_IRI:onto.ONTOREACTION_REACTIONEXPERIMENT,NEW_RXN_EXP_1_IRI:onto.ONTOREACTION_REACTIONVARIATION,
         NEW_RXN_EXP_2_IRI:onto.ONTOREACTION_REACTIONVARIATION,NEW_RXN_EXP_3_IRI:onto.ONTOREACTION_REACTIONVARIATION}
     RXNEXP_REACTION_CONDITION_DICT = {EXAMPLE_RXN_EXP_1_IRI:EXAMPLE_RXN_EXP_1_REACTION_CONDITION_IRI_LIST,EXAMPLE_RXN_EXP_2_IRI:EXAMPLE_RXN_EXP_2_REACTION_CONDITION_IRI_LIST,
         EXAMPLE_RXN_EXP_3_IRI:EXAMPLE_RXN_EXP_3_REACTION_CONDITION_IRI_LIST,EXAMPLE_RXN_EXP_4_IRI:EXAMPLE_RXN_EXP_4_REACTION_CONDITION_IRI_LIST,
@@ -447,31 +450,31 @@
     LIST_NEW_RXN_EXP = [NEW_RXN_EXP_1_IRI, NEW_RXN_EXP_2_IRI, NEW_RXN_EXP_3_IRI]
     LIST_RXN_EXP_ASSIGNEDTO_VAPR4_DUMMY = [EXAMPLE_RXN_EXP_1_IRI, EXAMPLE_RXN_EXP_2_IRI]
     # LIST_VAPR4_DUMMY_CONDUCTED_RXN_EXP = [EXAMPLE_RXN_EXP_1_IRI, EXAMPLE_RXN_EXP_2_IRI]
     LIST_RXN_EXP_ASSIGNEDTO_VAPR4_ANOTHER_DUMMY = [EXAMPLE_RXN_EXP_3_IRI, EXAMPLE_RXN_EXP_4_IRI, EXAMPLE_RXN_EXP_5_IRI]
     # LIST_VAPR4_ANOTHER_DUMMY_CONDUCTED_RXN_EXP = [EXAMPLE_RXN_EXP_3_IRI, EXAMPLE_RXN_EXP_4_IRI, EXAMPLE_RXN_EXP_5_IRI]
     LIST_DUMMY_R2PUMPS = [VAPOURTECR2PUMP_1_DUMMY_IRI, VAPOURTECR2PUMP_2_DUMMY_IRI, VAPOURTECR2PUMP_3_DUMMY_IRI, VAPOURTECR2PUMP_4_DUMMY_IRI]
     LIST_DUMMY_R4REACTORS = [VAPOURTECR4REACTOR_DUMMY_IRI, VAPOURTECR4REACTOR_ANOTHER_DUMMY_IRI]
-    RXN_EXP_QUEUE_1 = 'http://example.com/blazegraph/namespace/test_temp/exp_1'
-    RXN_EXP_QUEUE_2 = 'http://example.com/blazegraph/namespace/test_temp/exp_2'
-    RXN_EXP_QUEUE_3 = 'http://example.com/blazegraph/namespace/test_temp/exp_3'
-    RXN_EXP_QUEUE_4 = 'http://example.com/blazegraph/namespace/test_temp/exp_4'
-    RXN_EXP_QUEUE_5 = 'http://example.com/blazegraph/namespace/test_temp/exp_5'
-    RXN_EXP_QUEUE_6 = 'http://example.com/blazegraph/namespace/test_temp/exp_6'
-    RXN_EXP_QUEUE_7 = 'http://example.com/blazegraph/namespace/test_temp/exp_7'
+    RXN_EXP_QUEUE_1 = 'https://example.com/blazegraph/namespace/test_temp/exp_1'
+    RXN_EXP_QUEUE_2 = 'https://example.com/blazegraph/namespace/test_temp/exp_2'
+    RXN_EXP_QUEUE_3 = 'https://example.com/blazegraph/namespace/test_temp/exp_3'
+    RXN_EXP_QUEUE_4 = 'https://example.com/blazegraph/namespace/test_temp/exp_4'
+    RXN_EXP_QUEUE_5 = 'https://example.com/blazegraph/namespace/test_temp/exp_5'
+    RXN_EXP_QUEUE_6 = 'https://example.com/blazegraph/namespace/test_temp/exp_6'
+    RXN_EXP_QUEUE_7 = 'https://example.com/blazegraph/namespace/test_temp/exp_7'
     RXN_EXP_1_PRIOR = []
     RXN_EXP_2_PRIOR = [RXN_EXP_QUEUE_1]
     RXN_EXP_3_PRIOR = [RXN_EXP_QUEUE_1, RXN_EXP_QUEUE_2]
     RXN_EXP_4_PRIOR = [RXN_EXP_QUEUE_1, RXN_EXP_QUEUE_2, RXN_EXP_QUEUE_3]
     RXN_EXP_5_PRIOR = [RXN_EXP_QUEUE_1, RXN_EXP_QUEUE_2, RXN_EXP_QUEUE_3, RXN_EXP_QUEUE_4]
     RXN_EXP_6_PRIOR = [RXN_EXP_QUEUE_1, RXN_EXP_QUEUE_2, RXN_EXP_QUEUE_3, RXN_EXP_QUEUE_4]
     RXN_EXP_7_PRIOR = [RXN_EXP_QUEUE_1, RXN_EXP_QUEUE_2, RXN_EXP_QUEUE_3, RXN_EXP_QUEUE_4]
     HPLCMETHOD_DUMMY_IRI = DUMMY_LAB_BASE_IRI + 'HPLCMethod_Dummy'
     PHASECOMPONENT_INTERNAL_STANDARD_IRI = 'https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_InternalStandard'
-    ONTOSPECIES_INTERNAL_STANDARD_IRI = 'http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340'
+    ONTOSPECIES_INTERNAL_STANDARD_IRI = 'http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340'
     MOLARITY_INTERNAL_STANDARD = 0.05
     HPLCREPORT_DUMMY_IRI = DUMMY_LAB_BASE_IRI + 'HPLCReport_Dummy'
     HPLCJOB_DUMMY_IRI = DUMMY_LAB_BASE_IRI + 'HPLCJob_Dummy'
     HPLC_LOCAL_FOLDER_PATH = '/home/jb2197/CHEM32/**/'
     HPLCREPORT_DUMMY_REMOTE_PATH = 'http://placeholder_path'
     HPLCREPORT_DUMMY_LOCAL_PATH = 'placeholder_file_name'
     CHEMICAL_AMOUNT_FOR_DUMMY_OUTPUTCHEMICAL_IRI = DUMMY_LAB_BASE_IRI + 'ChemicalAmount_For_Dummy_OutputChemical'
@@ -519,43 +522,43 @@
     DOE_NO_PRIOR_DATA_FIXED_PARAM_3_IRIR = DOE_NO_PRIOR_DATA_BASE_IRI + 'FixedParameter_3'
     DOE_NO_PRIOR_DATA_FIXED_PARAM_IRI_LIST = [DOE_NO_PRIOR_DATA_FIXED_PARAM_1_IRIR, DOE_NO_PRIOR_DATA_FIXED_PARAM_2_IRIR, DOE_NO_PRIOR_DATA_FIXED_PARAM_3_IRIR]
 
     DOE_TEMPLATE_BASE_IRI = 'https://www.example.com/triplestore/ontodoe/DoE_Template/'
     DOE_TEMPLATE_IRI = DOE_TEMPLATE_BASE_IRI + 'DoE_1'
     DOE_TEMPLATE_DOMAIN_IRI = DOE_TEMPLATE_BASE_IRI + 'Domain_1'
 
-    DUMMY_LAB_FOR_POST_PROC_BASE_IRI = 'http://example.com/blazegraph/namespace/testlab/dummy_lab_for_post_proc/'
+    DUMMY_LAB_FOR_POST_PROC_BASE_IRI = 'https://example.com/blazegraph/namespace/testlab/dummy_lab_for_post_proc/'
     HPLC_1_POST_PROC_IRI = DUMMY_LAB_FOR_POST_PROC_BASE_IRI + 'HPLC_1'
     HPLC_2_POST_PROC_IRI = DUMMY_LAB_FOR_POST_PROC_BASE_IRI + 'HPLC_2'
     CHEMICAL_AMOUNT_1_POST_PROC_IRI = DUMMY_LAB_FOR_POST_PROC_BASE_IRI + 'ChemicalAmount_1_1'
     CHEMICAL_AMOUNT_2_POST_PROC_IRI = DUMMY_LAB_FOR_POST_PROC_BASE_IRI + 'ChemicalAmount_2_1'
     VAPOURTECR4_1_POST_PROC_IRI = DUMMY_LAB_FOR_POST_PROC_BASE_IRI + 'VapourtecR4_1'
     VAPOURTECR4_2_POST_PROC_IRI = DUMMY_LAB_FOR_POST_PROC_BASE_IRI + 'VapourtecR4_2'
 
     # NOTE some of the information below are commented out following the changes made to HPLCMETHOD_DUMMY_IRI in dummy_lab.ttl
     # this is to mimic the situation where either the species is not visible in the chromatogram or some information are not available/presented in the HPLC method
     HPLC_DUMMAY_REPORT_FILE_SPECIES_RETENTION_TIME_IDENTIFY = {
-        'http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b': 0.55,
-        # "http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3": 2.55,
+        'http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b': 0.55,
+        # "http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3": 2.55,
         'http://www.theworldavatar.com/kg/ontospecies/Species_f999de28-55dc-477e-8afc-e8802064e0d2': 1.55,
         'http://www.theworldavatar.com/kg/ontospecies/Species_8765d201-0da9-4112-b653-3455002f535b': 4.55,
         # "http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202": 5.55,
-        # "http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb": 6.55,
-        # "http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983": 7.55,
-        "http://www.theworldavatar.com/kb/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340": 3.55
+        # "http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb": 6.55,
+        # "http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983": 7.55,
+        "http://www.theworldavatar.com/kg/ontospecies/Species_4fa4fdea-ed3d-4b0a-aee5-1f4e97dd2340": 3.55
     }
 
     RXNEXP_REACTOR_ASSIGNED_DICT = {EXAMPLE_RXN_EXP_1_IRI:VAPOURTECR4REACTOR_DUMMY_IRI,EXAMPLE_RXN_EXP_2_IRI:VAPOURTECR4REACTOR_DUMMY_IRI,
         EXAMPLE_RXN_EXP_3_IRI:VAPOURTECR4REACTOR_ANOTHER_DUMMY_IRI,EXAMPLE_RXN_EXP_4_IRI:VAPOURTECR4REACTOR_ANOTHER_DUMMY_IRI,
         EXAMPLE_RXN_EXP_5_IRI:VAPOURTECR4REACTOR_ANOTHER_DUMMY_IRI,NEW_RXN_EXP_1_IRI:VAPOURTECR4_1_POST_PROC_IRI,NEW_RXN_EXP_2_IRI:VAPOURTECR4_2_POST_PROC_IRI,NEW_RXN_EXP_3_IRI:None}
 
-    INTENTIONALLY_OUT_OF_RANGE_BAES_IRI = 'https://intentionally_created_ReactionExperiment_out_of_range/'
-    OUT_OF_RANGE_RXN_EXP_1_IRI = INTENTIONALLY_OUT_OF_RANGE_BAES_IRI + 'ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70'
-    OUT_OF_RANGE_RXN_EXP_2_IRI = INTENTIONALLY_OUT_OF_RANGE_BAES_IRI + 'ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8'
-    OUT_OF_RANGE_RXN_EXP_3_IRI = INTENTIONALLY_OUT_OF_RANGE_BAES_IRI + 'ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf'
-    YIELD_INTENTIONALLY_OUT_OF_RANGE_BAES_IRI = 'https://yield_out_of_range/'
-    YIELD_OUT_OF_RANGE_RXN_EXP_1_IRI = YIELD_INTENTIONALLY_OUT_OF_RANGE_BAES_IRI + 'ReactionExperiment_negative_yield'
-    YIELD_OUT_OF_RANGE_RXN_EXP_2_IRI = YIELD_INTENTIONALLY_OUT_OF_RANGE_BAES_IRI + 'ReactionExperiment_yield_too_high'
+    INTENTIONALLY_OUT_OF_RANGE_BASE_IRI = 'https://intentionally_created_ReactionExperiment_out_of_range/'
+    OUT_OF_RANGE_RXN_EXP_1_IRI = INTENTIONALLY_OUT_OF_RANGE_BASE_IRI + 'ReactionVariation_fac53bb1-3ae0-4941-9f5b-38738b07ab70'
+    OUT_OF_RANGE_RXN_EXP_2_IRI = INTENTIONALLY_OUT_OF_RANGE_BASE_IRI + 'ReactionVariation_3bd3166d-f782-4cdc-a6a8-75336afd71a8'
+    OUT_OF_RANGE_RXN_EXP_3_IRI = INTENTIONALLY_OUT_OF_RANGE_BASE_IRI + 'ReactionVariation_c4b175d9-e53c-4d7e-b053-3a81f7ca0ddf'
+    YIELD_INTENTIONALLY_OUT_OF_RANGE_BASE_IRI = 'https://yield_out_of_range/'
+    YIELD_OUT_OF_RANGE_RXN_EXP_1_IRI = YIELD_INTENTIONALLY_OUT_OF_RANGE_BASE_IRI + 'ReactionExperiment_negative_yield'
+    YIELD_OUT_OF_RANGE_RXN_EXP_2_IRI = YIELD_INTENTIONALLY_OUT_OF_RANGE_BASE_IRI + 'ReactionExperiment_yield_too_high'
     LIST_INTENTIONALLY_OUT_OF_RANGE_RXN_EXP = [
         OUT_OF_RANGE_RXN_EXP_1_IRI, OUT_OF_RANGE_RXN_EXP_2_IRI, OUT_OF_RANGE_RXN_EXP_3_IRI,
         YIELD_OUT_OF_RANGE_RXN_EXP_1_IRI, YIELD_OUT_OF_RANGE_RXN_EXP_2_IRI
     ]
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_base_ontology.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_base_ontology.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_dict_and_list.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_dict_and_list.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_example_triples.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_example_triples.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_hash_eq.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_hash_eq.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_hplc.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_hplc.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_ontodoe.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_ontodoe.py`

 * *Files identical despite different names*

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_single_phase.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_single_phase.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                         instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_1_Property_1_ScalarValue_1',
                         clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                         namespace_for_init=None,
                         hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                         numericalValue=0.5
                     )
                 ),
-                representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'
+                representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'
             ),
             OntoCAPE_PhaseComponent(
                 instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_6',
                 clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#PhaseComponent',
                 namespace_for_init=None,
                 hasProperty=OntoCAPE_Molarity(
                     instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_6_Property_1',
@@ -46,15 +46,15 @@
                         instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_6_Property_1_ScalarValue_1',
                         clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                         namespace_for_init=None,
                         hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                         numericalValue=18.1
                     )
                 ),
-                representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb'
+                representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb'
             )
         ],
         has_composition=OntoCAPE_Composition(
             instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/Composition_1',
             clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Composition',
             namespace_for_init=None,
             comprisesDirectly=[
@@ -109,15 +109,15 @@
                     namespace_for_init=None, hasValue=OntoCAPE_ScalarValue(
                         instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_2_Property_1_ScalarValue_1',
                         clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                         namespace_for_init=None,
                         hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre', numericalValue=6.73
                     )
                 ),
-                representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3'
+                representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3'
             ), OntoCAPE_PhaseComponent(
                 instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_6_2',
                 clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#PhaseComponent',
                 namespace_for_init=None,
                 hasProperty=OntoCAPE_Molarity(
                     instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_6_Property_2',
                     clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Molarity',
@@ -126,15 +126,15 @@
                         instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_6_Property_2_ScalarValue_1',
                         clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                         namespace_for_init=None,
                         hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                         numericalValue=9.6
                     )
                 ),
-                representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb'
+                representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb'
             )
         ],
         has_composition=OntoCAPE_Composition(
             instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/Composition_2',
             clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Composition',
             namespace_for_init=None,
             comprisesDirectly=[
@@ -210,15 +210,15 @@
                         instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/PhaseComponent_7_Property_1_ScalarValue_1',
                         clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                         namespace_for_init=None,
                         hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                         numericalValue=17.1
                     )
                 ),
-                representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983'
+                representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983'
             )
         ], has_composition=OntoCAPE_Composition(
             instance_iri='https://www.example.com/triplestore/ontorxn/SinglePhase/Composition_3',
             clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Composition',
             namespace_for_init=None,
             comprisesDirectly=[
                          OntoCAPE_Molarity(
@@ -247,149 +247,148 @@
                          )
             ]
         ),
         representsThermodynamicBehaviorOf='https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/InputChemical_3'
     )
 )
 AUTOSAMPLERSITE_1 = AutoSamplerSite(
-    instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Site_1',
+    instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Site_1',
     clz='https://www.theworldavatar.com/kg/ontovapourtec/AutoSamplerSite',
     namespace_for_init=None,
     holds=Vial(
-        instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1',
+        instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1',
         clz='https://www.theworldavatar.com/kg/ontovapourtec/Vial',
         namespace_for_init=None,
         isFilledWith=ChemicalAmount(
-            instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/ChemicalAmount_1',
+            instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/ChemicalAmount_1',
             clz='https://www.theworldavatar.com/kg/ontolab/ChemicalAmount',
             namespace_for_init=None,
             refersToMaterial=Chemical(
-                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Material_1',
+                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Material_1',
                 clz='http://www.theworldavatar.com/ontology/ontocape/material/material.owl#Material',
                 namespace_for_init=None,
                 thermodynamicBehaviour=OntoCAPE_SinglePhase(
-                    instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Phase_1',
+                    instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Phase_1',
                     clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#SinglePhase',
                     namespace_for_init=None,
                     hasStateOfAggregation=OntoCAPE_StateOfAggregation(
                         instance_iri='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#liquid',
                         clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#StateOfAggregation',
                         namespace_for_init=None
                     ),
                     isComposedOfSubsystem=[
                         OntoCAPE_PhaseComponent(
-                            instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1',
+                            instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1',
                             clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#PhaseComponent',
                             namespace_for_init=None,
                             hasProperty=OntoCAPE_Molarity(
-                                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1',
+                                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1',
                                 clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Molarity',
                                 namespace_for_init=None,
                                 hasValue=OntoCAPE_ScalarValue(
-                                    instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1_ScalarValue_1',
+                                    instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1_ScalarValue_1',
                                     clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                                     namespace_for_init=None,
                                     hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                                     numericalValue=0.5
                                 )
                             ),
-                            representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'),
+                            representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b'),
                         OntoCAPE_PhaseComponent(
-                            instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6',
+                            instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6',
                             clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#PhaseComponent',
                             namespace_for_init=None,
                             hasProperty=OntoCAPE_Molarity(
-                                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1',
+                                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1',
                                 clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Molarity',
                                 namespace_for_init=None,
                                 hasValue=OntoCAPE_ScalarValue(
-                                    instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1_ScalarValue_1',
+                                    instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1_ScalarValue_1',
                                     clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                                     namespace_for_init=None,
                                     hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                                     numericalValue=18.1
                                 )
                             ),
-                            representsOccurenceOf='http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb'
+                            representsOccurenceOf='http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb'
                         )
                     ],
                     has_composition=OntoCAPE_Composition(
-                        instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Composition_1',
+                        instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Composition_1',
                         clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Composition',
                         namespace_for_init=None,
                         comprisesDirectly=[
                             OntoCAPE_Molarity(
-                                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1',
+                                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1',
                                 clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Molarity',
                                 namespace_for_init=None,
                                 hasValue=OntoCAPE_ScalarValue(
-                                    instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1_ScalarValue_1',
+                                    instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_1_Property_1_ScalarValue_1',
                                     clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                                     namespace_for_init=None,
                                     hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                                     numericalValue=0.5
                                 )
                             ),
                             OntoCAPE_Molarity(
-                                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1',
+                                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1',
                                 clz='http://www.theworldavatar.com/ontology/ontocape/material/phase_system/phase_system.owl#Molarity',
                                 namespace_for_init=None,
                                 hasValue=OntoCAPE_ScalarValue(
-                                    instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1_ScalarValue_1',
+                                    instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/PhaseComponent_6_Property_1_ScalarValue_1',
                                     clz='http://www.theworldavatar.com/ontology/ontocape/upper_level/system.owl#ScalarValue',
                                     namespace_for_init=None,
                                     hasUnitOfMeasure='http://www.ontology-of-units-of-measure.org/resource/om-2/molePerLitre',
                                     numericalValue=18.1
                                 )
                             )
                         ]
                     ),
-                    representsThermodynamicBehaviorOf='http://example.com/blazegraph/namespace/testlab/dummy_lab/Material_1'
+                    representsThermodynamicBehaviorOf='https://example.com/blazegraph/namespace/testlab/dummy_lab/Material_1'
                 )
             ),
-            fills='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1',
+            fills='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1',
             isPreparedBy=None
         ),
         hasFillLevel=OM_Volume(
-            instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_fill',
+            instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_fill',
             clz='http://www.ontology-of-units-of-measure.org/resource/om-2/Volume',
             namespace_for_init=None,
             hasValue=OM_Measure(
-                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_fill_value',
+                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_fill_value',
                 clz='http://www.ontology-of-units-of-measure.org/resource/om-2/Measure',
                 namespace_for_init=None,
                 hasUnit='http://www.ontology-of-units-of-measure.org/resource/om-2/millilitre',
                 hasNumericalValue=5.0
             )
         ),
         hasWarningLevel=OM_Volume(
-            instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_warning',
+            instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_warning',
             clz='http://www.ontology-of-units-of-measure.org/resource/om-2/Volume',
             namespace_for_init=None,
             hasValue=OM_Measure(
-                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_warning_value',
+                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_warning_value',
                 clz='http://www.ontology-of-units-of-measure.org/resource/om-2/Measure',
                 namespace_for_init=None,
                 hasUnit='http://www.ontology-of-units-of-measure.org/resource/om-2/millilitre',
                 hasNumericalValue=3.0
             ),
         ),
         hasMaxLevel=OM_Volume(
-            instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_max',
+            instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_max',
             clz='http://www.ontology-of-units-of-measure.org/resource/om-2/Volume',
             namespace_for_init=None,
             hasValue=OM_Measure(
-                instance_iri='http://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_max_value',
+                instance_iri='https://example.com/blazegraph/namespace/testlab/dummy_lab/Vial_1_level_max_value',
                 clz='http://www.ontology-of-units-of-measure.org/resource/om-2/Measure',
                 namespace_for_init=None,
                 hasUnit='http://www.ontology-of-units-of-measure.org/resource/om-2/millilitre',
                 hasNumericalValue=10.0
             )
         ),
-        isHeldIn='http://example.com/blazegraph/namespace/testlab/dummy_lab/Site_1'
     ),
     locationID='1'
 )
 
 @pytest.mark.parametrize(
     "input_chemical,autosamplersite,desired_result",
     [
@@ -400,26 +399,26 @@
 )
 def test_equal_single_phase(input_chemical, autosamplersite, desired_result):
     assert (input_chemical.thermodynamicBehaviour == autosamplersite.holds.isFilledWith.refersToMaterial.thermodynamicBehaviour) == desired_result
 
 @pytest.mark.parametrize(
     "chemical,chemical_species,desired_result",
     [
-        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',True),
-        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',True),
-        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',False),
+        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',True),
+        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',True),
+        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',False),
         (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202',False),
-        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983',False),
-        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',False),
-        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',True),
-        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',True),
+        (INPUTCHEMICAL_1,'http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983',False),
+        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',False),
+        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',True),
+        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',True),
         (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202',False),
-        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983',False),
-        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kb/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',False),
-        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kb/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',False),
-        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kb/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',False),
+        (INPUTCHEMICAL_2,'http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983',False),
+        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kg/ontospecies/Species_54d8b46b-17bc-4bbd-a3cc-3b3a16d6ae4b',False),
+        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kg/ontospecies/Species_0401f93b-b62d-488e-ba1f-7d5c37e365cb',False),
+        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kg/ontospecies/Species_353d4667-e25d-476a-bd74-5c34723c8ea3',False),
         (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kg/ontospecies/Species_eab77458-560d-4ce9-9b5e-96650fc3e202',True),
-        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kb/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983',True),
+        (INPUTCHEMICAL_3,'http://www.theworldavatar.com/kg/ontospecies/Species_63fefc5a-d49d-4841-a946-2cdb5f356983',True),
     ],
 )
 def test_contains_chemical_species(chemical, chemical_species, desired_result):
     assert chemical.contains_chemical_species(chemical_species) == desired_result
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots/tests/test_sparql_client.py` & `chemistry_and_robots-1.6.0/chemistry_and_robots/tests/test_sparql_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,45 +21,51 @@
 
 # ----------------------------------------------------------------------------------
 # Test cases for sparql_client
 # ----------------------------------------------------------------------------------
 # collect_triples_for_equip_settings and collect_triples_for_new_experiment are
 # tested in integration test of agents
 
+def test_get_ontology_tbox_version(initialise_triples):
+    sparql_client = initialise_triples
+    assert sparql_client.get_ontology_tbox_version(onto.ONTODOE) is not None
+    with pytest.raises(Exception):
+        sparql_client.get_ontology_tbox_version(f'http://fake_ontology/{str(uuid.uuid4())}/')
+
 def test_amount_of_triples_none_zero(initialise_triples):
     sparql_client = initialise_triples
     assert sparql_client.getAmountOfTriples() != 0
 
 def test_getDesignVariables(initialise_triples):
     sparql_client = initialise_triples
     design_var_list = sparql_client.getDesignVariables(TargetIRIs.DOE_DOMAIN_IRI.value)
     design_var_iri_list = [var.instance_iri for var in design_var_list]
     assert len(design_var_iri_list) == len(TargetIRIs.DOE_CONT_VAR_IRI_LIST.value)
     assert all(iri in design_var_iri_list for iri in TargetIRIs.DOE_CONT_VAR_IRI_LIST.value)
     assert all(all([isinstance(var, onto.ContinuousVariable),
-                    var.refersTo is not None,
-                    var.refersTo.hasUnit is not None,
+                    var.refersToQuantity is not None,
+                    var.refersToQuantity.hasUnit is not None,
                     var.upperLimit > var.lowerLimit]) for var in design_var_list)
 
 def test_get_fixed_parameters(initialise_triples):
     sparql_client = initialise_triples
     param_list = sparql_client.get_fixed_parameters(TargetIRIs.DOE_NO_PRIOR_DATA_DOMAIN_IRI.value)
     param_iri_list = [param.instance_iri for param in param_list]
     assert dal.check_if_two_lists_equal(
         param_iri_list,
         TargetIRIs.DOE_NO_PRIOR_DATA_FIXED_PARAM_IRI_LIST.value
     )
     assert all(
         all(
             [
                 isinstance(param, onto.FixedParameter),
-                param.refersTo is not None,
-                param.refersTo.hasValue is not None,
-                param.refersTo.hasValue.hasUnit is not None,
-                param.refersTo.hasValue.hasNumericalValue is not None
+                param.refersToQuantity is not None,
+                param.refersToQuantity.hasValue is not None,
+                param.refersToQuantity.hasValue.hasUnit is not None,
+                param.refersToQuantity.hasValue.hasNumericalValue is not None
             ]
         ) for param in param_list
     )
 
 @pytest.mark.parametrize(
     "sys_res_iri,maximise",
     [# here we are testing that the function should work wether the passed in iri is already a list or not
@@ -71,15 +77,15 @@
     ],
 )
 def test_getSystemResponses(initialise_triples, sys_res_iri, maximise):
     sparql_client = initialise_triples
     sys_res_list = sparql_client.getSystemResponses(sys_res_iri)
     length = len(sys_res_iri) if isinstance(sys_res_iri, list) else 1
     assert length == len(sys_res_list)
-    assert all(all([isinstance(r, onto.SystemResponse), r.refersTo is not None]) for r in sys_res_list)
+    assert all(all([isinstance(r, onto.SystemResponse), r.refersToQuantity is not None]) for r in sys_res_list)
     dct_m = {s.instance_iri:s.maximise for s in sys_res_list}
     if isinstance(sys_res_iri, list):
         assert all(m == dct_m.get(s) for s, m in zip(sys_res_iri, maximise))
 
 def test_getTSEMOSettings(initialise_triples):
     sparql_client = initialise_triples
     tsemo = sparql_client.getTSEMOSettings(TargetIRIs.DOE_TSEMO_STRATEGY_IRI.value)
@@ -104,16 +110,16 @@
     sparql_client = initialise_triples
     doe_domain_instance = sparql_client.getDoEDomain(TargetIRIs.DOE_DOMAIN_IRI.value)
     assert doe_domain_instance.instance_iri == TargetIRIs.DOE_DOMAIN_IRI.value
     lst_var = [v.instance_iri for v in doe_domain_instance.hasDesignVariable]
     assert len(lst_var) == len(TargetIRIs.DOE_CONT_VAR_IRI_LIST.value)
     assert all(var in lst_var for var in TargetIRIs.DOE_CONT_VAR_IRI_LIST.value)
     assert all(all([isinstance(var, onto.ContinuousVariable),
-                    var.refersTo is not None,
-                    var.refersTo.hasUnit is not None,
+                    var.refersToQuantity is not None,
+                    var.refersToQuantity.hasUnit is not None,
                     var.upperLimit > var.lowerLimit]) for var in doe_domain_instance.hasDesignVariable)
 
 @pytest.mark.parametrize(
     "rxnexp_iri,rxnexp_condition_iri",
     [# here we are testing that the function should work wether the passed in iri is already a list or not
         (TargetIRIs.EXAMPLE_RXN_EXP_1_IRI.value, TargetIRIs.EXAMPLE_RXN_EXP_1_REACTION_CONDITION_IRI_LIST.value),
         (TargetIRIs.NEW_RXN_EXP_1_IRI.value, TargetIRIs.NEW_RXN_EXP_1_REACTION_CONDITION_IRI_LIST.value),
@@ -147,15 +153,15 @@
         assert len(rxnexp_condition_iri[i]) == len(rxn_condition_list)
         for con in rxn_condition_list:
             assert all([isinstance(con, onto.ReactionCondition), con.clz is not None, isinstance(con.objPropWithExp, list),
                 con.hasValue.hasUnit is not None, con.hasValue.hasNumericalValue is not None, con.instance_iri in rxnexp_condition_iri[i]])
             if con.clz == onto.ONTOREACTION_STOICHIOMETRYRATIO:
                 assert con.indicatesMultiplicityOf is not None
             elif con.clz == onto.ONTOREACTION_REACTIONSCALE:
-                assert con.indicateUsageOf is not None
+                assert con.indicatesUsageOf is not None
 
 @pytest.mark.parametrize(
     "rxnexp_iri,rxnexp_pref_indicator_iri,rxn_type",
     [# here we are testing that the function should work wether the passed in iri is already a list or not
         (TargetIRIs.EXAMPLE_RXN_EXP_1_IRI.value, TargetIRIs.EXAMPLE_RXN_EXP_1_PERFORMANCE_INDICATOR_IRI_LIST.value, onto.ONTOREACTION_REACTIONEXPERIMENT),
         (TargetIRIs.NEW_RXN_EXP_1_IRI.value, TargetIRIs.NEW_RXN_EXP_1_PERFORMANCE_INDICATOR_IRI_LIST.value, onto.ONTOREACTION_REACTIONVARIATION),
         (
@@ -289,31 +295,31 @@
     new_exp_iri = sparql_client.getNewExperimentFromDoE(TargetIRIs.DOE_IRI.value)
     assert new_exp_iri is None
 
 def test_getDoEHistoricalData(initialise_triples):
     sparql_client = initialise_triples
     hist_data_instance = sparql_client.getDoEHistoricalData(TargetIRIs.DOE_HIST_DATA_IRI.value)
     assert isinstance(hist_data_instance, onto.HistoricalData)
-    assert len(hist_data_instance.refersTo) == len(TargetIRIs.DOE_HIST_DATE_REFERTO_IRI.value)
-    assert all(iri in [h.instance_iri for h in hist_data_instance.refersTo] for iri in TargetIRIs.DOE_HIST_DATE_REFERTO_IRI.value)
+    assert len(hist_data_instance.refersToExperiment) == len(TargetIRIs.DOE_HIST_DATE_REFERTO_IRI.value)
+    assert all(iri in [h.instance_iri for h in hist_data_instance.refersToExperiment] for iri in TargetIRIs.DOE_HIST_DATE_REFERTO_IRI.value)
 
 def test_get_doe_instance(initialise_triples):
     sparql_client = initialise_triples
     doe_instance = sparql_client.get_doe_instance(TargetIRIs.DOE_IRI.value)
     # Check Domain
     assert doe_instance.hasDomain.instance_iri == TargetIRIs.DOE_DOMAIN_IRI.value
     lst_var = [v.instance_iri for v in doe_instance.hasDomain.hasDesignVariable]
     assert len(lst_var) == len(TargetIRIs.DOE_CONT_VAR_IRI_LIST.value)
     assert all(var in lst_var for var in TargetIRIs.DOE_CONT_VAR_IRI_LIST.value)
     assert all(all([isinstance(var, onto.ContinuousVariable),
-                    var.refersTo is not None,
-                    var.refersTo.hasUnit is not None,
+                    var.refersToQuantity is not None,
+                    var.refersToQuantity.hasUnit is not None,
                     var.upperLimit > var.lowerLimit]) for var in doe_instance.hasDomain.hasDesignVariable)
     # Check SystemResponse
-    assert all(all([isinstance(r, onto.SystemResponse), r.refersTo is not None]) for r in doe_instance.hasSystemResponse)
+    assert all(all([isinstance(r, onto.SystemResponse), r.refersToQuantity is not None]) for r in doe_instance.hasSystemResponse)
     dct_m = {s.instance_iri:s.maximise for s in doe_instance.hasSystemResponse}
     assert all([int(TargetIRIs.DOE_SYS_RES_MAXIMISE_DICT.value[s]) == int(dct_m.get(s)) for s in TargetIRIs.DOE_SYS_RES_MAXIMISE_DICT.value])
     # Check Strategy
     strategy = doe_instance.usesStrategy
     assert strategy.instance_iri == TargetIRIs.DOE_STRATEGY_IRI.value
     assert isinstance(strategy, onto.TSEMO)
     assert strategy.nRetries is not None
@@ -815,15 +821,14 @@
     vapourtec_rs400_list = sparql_client.get_vapourtec_rs400(
         list_vapourtec_rs400_iri=[TargetIRIs.VAPOURTECRS400_DUMMY_IRI.value]
     )
     assert len(vapourtec_rs400_list) == 1
     vapourtec_rs400 = vapourtec_rs400_list[0]
     assert vapourtec_rs400.instance_iri == TargetIRIs.VAPOURTECRS400_DUMMY_IRI.value
     assert vapourtec_rs400.manufacturer == TargetIRIs.VAPOURTEC_LTD.value
-    assert vapourtec_rs400.isContainedIn == TargetIRIs.DUMMY_LAB_IRI.value
     assert vapourtec_rs400.isManagedBy is None
     assert vapourtec_rs400.consistsOf is not None
     assert dal.check_if_two_lists_equal(TargetIRIs.VAPOURTECRS400_DUMMY_CONSISTS_OF_LIST.value,
         [r.instance_iri for r in vapourtec_rs400.consistsOf])
     assert vapourtec_rs400.hasState.clz == onto.ONTOVAPOURTEC_IDLE
     assert vapourtec_rs400.hasState.stateLastUpdatedAt == 0
     assert vapourtec_rs400.hasCollectionMethod is not None
@@ -924,15 +929,14 @@
 
     assert uploaded_hplc_report == detected_hplc_report
 
 def test_get_autosampler(initialise_triples):
     sparql_client = initialise_triples
     autosampler = sparql_client.get_autosampler(TargetIRIs.AUTOSAMPLER_DUMMY_IRI.value)
     assert autosampler.instance_iri == TargetIRIs.AUTOSAMPLER_DUMMY_IRI.value
-    assert autosampler.isContainedIn == TargetIRIs.DUMMY_LAB_IRI.value
 
     # Check autosampler sampleLoopVolume is correctly parsed
     assert autosampler.sampleLoopVolume.instance_iri == TargetIRIs.AUTOSAMPLER_SAMPLE_LOOP_VOLUME_IRI.value
     assert autosampler.sampleLoopVolume.hasValue.instance_iri == TargetIRIs.AUTOSAMPLER_SAMPLE_LOOP_VOLUME_MEASURE_IRI.value
     assert autosampler.sampleLoopVolume.hasValue.hasUnit == TargetIRIs.AUTOSAMPLER_SAMPLE_LOOP_VOLUME_MEASURE_UNIT.value
     assert autosampler.sampleLoopVolume.hasValue.hasNumericalValue == TargetIRIs.AUTOSAMPLER_SAMPLE_LOOP_VOLUME_MEASURE_NUM_VAL.value
 
@@ -1017,28 +1021,28 @@
     assert dct_site_loop_volume[empty_site] == amount_of_chemical_amount
     assert dct_site_chemical_amount[empty_site] == chemical_amount_iri.toPython()
 
 def test_release_vapourtec_rs400_settings(initialise_triples):
     sparql_client = initialise_triples
 
     vapourtec_rs400_iri = TargetIRIs.VAPOURTECRS400_DUMMY_IRI.value
-    assert not sparql_client.performQuery("""ASK {<%s> <%s>* ?hardware. ?hardware <%s> ?settings.}""" % (
-        vapourtec_rs400_iri, onto.SAREF_CONSISTSOF, onto.ONTOLAB_ISSPECIFIEDBY))[0]['ASK']
+    assert not sparql_client.performQuery("""ASK {<%s> <%s>* ?hardware. ?settings <%s> ?hardware.}""" % (
+        vapourtec_rs400_iri, onto.SAREF_CONSISTSOF, onto.ONTOLAB_SPECIFIES))[0]['ASK']
 
     setting_iri = "http://"+str(uuid.uuid4())
     sparql_client.performUpdate("""
-        INSERT {?hardware <%s> <%s>. <%s> <%s> ?hardware.} WHERE {<%s> <%s>* ?hardware.}""" % (
-            onto.ONTOLAB_ISSPECIFIEDBY, setting_iri, setting_iri, onto.ONTOLAB_SPECIFIES,
+        INSERT {<%s> <%s> ?hardware.} WHERE {<%s> <%s>* ?hardware.}""" % (
+            setting_iri, onto.ONTOLAB_SPECIFIES,
             vapourtec_rs400_iri, onto.SAREF_CONSISTSOF))
-    assert sparql_client.performQuery("""ASK {<%s> <%s>* ?hardware. ?hardware <%s> ?settings.}""" % (
-        vapourtec_rs400_iri, onto.SAREF_CONSISTSOF, onto.ONTOLAB_ISSPECIFIEDBY))[0]['ASK']
+    assert sparql_client.performQuery("""ASK {<%s> <%s>* ?hardware. ?settings <%s> ?hardware.}""" % (
+        vapourtec_rs400_iri, onto.SAREF_CONSISTSOF, onto.ONTOLAB_SPECIFIES))[0]['ASK']
 
     sparql_client.release_vapourtec_rs400_settings(vapourtec_rs400_iri=vapourtec_rs400_iri)
-    assert not sparql_client.performQuery("""ASK {<%s> <%s>* ?hardware. ?hardware <%s> ?settings.}""" % (
-        vapourtec_rs400_iri, onto.SAREF_CONSISTSOF, onto.ONTOLAB_ISSPECIFIEDBY))[0]['ASK']
+    assert not sparql_client.performQuery("""ASK {<%s> <%s>* ?hardware. ?settings <%s> ?hardware.}""" % (
+        vapourtec_rs400_iri, onto.SAREF_CONSISTSOF, onto.ONTOLAB_SPECIFIES))[0]['ASK']
 
 def test_upload_and_get_vapourtec_input_file(initialise_triples, generate_random_download_path):
     """Integration test for upload_vapourtec_input_file_to_kg and test_get_vapourtec_input_file."""
     sparql_client = initialise_triples
 
     local_file_path = conftest.VAPOURTEC_INPUT_FILE
     timestamp_last_modified = os.path.getmtime(local_file_path)
@@ -1065,15 +1069,14 @@
     assert filecmp.cmp(local_file_path,full_downloaded_path)
 
 def test_get_hplc_given_vapourtec_rs400(initialise_triples):
     sparql_client = initialise_triples
     hplc = sparql_client.get_hplc_given_vapourtec_rs400(vapourtec_rs400_iri=TargetIRIs.VAPOURTECRS400_DUMMY_IRI.value)
     assert hplc.instance_iri == TargetIRIs.HPLC_DUMMY_IRI.value
     assert hplc.manufacturer == TargetIRIs.HPLC_DUMMY_MANUFACTURER_IRI.value
-    assert hplc.isContainedIn == TargetIRIs.DUMMY_LAB_IRI.value
     assert hplc.isManagedBy is None
 
     # Register agent with hplc
     agent_iri = "http://"+str(uuid.uuid4())
     sparql_client.register_agent_with_hardware(agent_iri=agent_iri, hardware_digital_twin=TargetIRIs.HPLC_DUMMY_IRI.value)
     hplc = sparql_client.get_hplc_given_vapourtec_rs400(vapourtec_rs400_iri=TargetIRIs.VAPOURTECRS400_DUMMY_IRI.value)
     assert hplc.isManagedBy == agent_iri
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/PKG-INFO` & `chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemistry-and-robots
-Version: 1.5.0
+Version: 1.6.0
 Summary: chemistryandrobots contains dataclasses and sparql queries for concepts related to chemistry_and_robots as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/utils/chemistry_and_robots
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `chemistry_and_robots-1.5.0/chemistry_and_robots.egg-info/SOURCES.txt` & `chemistry_and_robots-1.6.0/chemistry_and_robots.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,29 @@
 chemistry_and_robots/data_model/ontovapourtec.py
 chemistry_and_robots/data_model/unit_conversion.py
 chemistry_and_robots/hardware/__init__.py
 chemistry_and_robots/hardware/hplc.py
 chemistry_and_robots/kg_operations/__init__.py
 chemistry_and_robots/kg_operations/dict_and_list.py
 chemistry_and_robots/kg_operations/sparql_client.py
+chemistry_and_robots/resources/__init__.py
 chemistry_and_robots/resources/ontoagent/Service__DoE.ttl
 chemistry_and_robots/resources/ontoagent/Service__Execution.ttl
 chemistry_and_robots/resources/ontoagent/Service__PostProc.ttl
+chemistry_and_robots/resources/ontology/OntoDoE.owl
+chemistry_and_robots/resources/ontology/OntoGoal.owl
+chemistry_and_robots/resources/ontology/OntoHPLC.owl
+chemistry_and_robots/resources/ontology/OntoLab.owl
+chemistry_and_robots/resources/ontology/OntoReaction.owl
+chemistry_and_robots/resources/ontology/OntoVapourtec.owl
 chemistry_and_robots/resources/sample_data/doe.ttl
 chemistry_and_robots/resources/sample_data/doe_no_prior_data.ttl
 chemistry_and_robots/resources/sample_data/doe_template.ttl
 chemistry_and_robots/resources/sample_data/dummy_lab.ttl
 chemistry_and_robots/resources/sample_data/dummy_post_proc.ttl
-chemistry_and_robots/resources/sample_data/duplicate_ontorxn.ttl
 chemistry_and_robots/resources/sample_data/new_exp_data.ttl
 chemistry_and_robots/resources/sample_data/new_exp_data_out_of_range.ttl
 chemistry_and_robots/resources/sample_data/raw_hplc_report_txt.txt
 chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_incomplete.txt
 chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_no_product.txt
 chemistry_and_robots/resources/sample_data/raw_hplc_report_txt_unidentified_peaks.txt
 chemistry_and_robots/resources/sample_data/raw_hplc_report_xls.xls
```

### Comparing `chemistry_and_robots-1.5.0/setup.py` & `chemistry_and_robots-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='chemistry_and_robots',
-    version='1.5.0',
+    version='1.6.0',
     author='Jiaru Bai',
     author_email='jb2197@cam.ac.uk',
     license='MIT',
     python_requires='>=3.8',
     description="chemistryandrobots contains dataclasses and sparql queries for concepts related to chemistry_and_robots as part of The World Avatar project.",
     url="https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/utils/chemistry_and_robots",
     long_description=open('README.md').read(),
```

