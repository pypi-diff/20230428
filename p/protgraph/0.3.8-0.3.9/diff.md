# Comparing `tmp/protgraph-0.3.8.tar.gz` & `tmp/protgraph-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ProtGraph/ProtGraph/dist/tmpr99arvpf/protgraph-0.3.8.tar", last modified: Wed Oct 26 19:46:38 2022, max compression
+gzip compressed data, was "protgraph-0.3.9.tar", last modified: Fri Apr 28 17:57:57 2023, max compression
```

## Comparing `protgraph-0.3.8.tar` & `protgraph-0.3.9.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph/ft_execution/
--rw-r--r--   0 runner    (1001) docker     (121)     9939 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/ft_execution/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/ft_execution/signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/ft_execution/init_met.py
--rw-r--r--   0 runner    (1001) docker     (121)     8680 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/ft_execution/var_seq.py
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/ft_execution/generic_cleaved_peptide.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/ft_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/aa_replacer.py
--rw-r--r--   0 runner    (1001) docker     (121)    33762 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/unexpected_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/read_embl.py
--rw-r--r--   0 runner    (1001) docker     (121)     7242 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/digestion.py
--rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/graph_collapse_edges.py
--rw-r--r--   0 runner    (1001) docker     (121)    11862 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/protgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph/export/
--rw-r--r--   0 runner    (1001) docker     (121)     7559 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph/export/peptides/
--rw-r--r--   0 runner    (1001) docker     (121)     8043 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/pep_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)    11599 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/pep_mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/abstract_peptide_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12742 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/pep_postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/pep_trie.py
--rw-r--r--   0 runner    (1001) docker     (121)     7211 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/pep_fasta.py
--rw-r--r--   0 runner    (1001) docker     (121)     7280 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/pep_citus.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/peptides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/binary_pcsr.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/gml.py
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (121)     7461 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/generic_file_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/abstract_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/large_binary_pcsr.py
--rw-r--r--   0 runner    (1001) docker     (121)     9924 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/pcsr.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/dot.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/graphml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/large_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/gremlin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/redisgraph.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/large_pcsr.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/aa_masses_annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/verify_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8439 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/graph_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13557 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/annotate_ptms.py
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/graph_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/scripts/pepsqlite_to_fasta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/scripts/print_sums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/scripts/compact_fasta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/scripts/replace_fasta_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/scripts/generate_fasta_decoys.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12573 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/merge_aminoacids.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-26 19:46:26.000000 protgraph-0.3.8/protgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-10-26 19:46:26.000000 protgraph-0.3.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-10-26 19:46:26.000000 protgraph-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 19:46:38.000000 protgraph-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    21010 2022-10-26 19:46:26.000000 protgraph-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-26 19:46:26.000000 protgraph-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2022-10-26 19:46:26.000000 protgraph-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21649 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-26 19:46:38.000000 protgraph-0.3.8/protgraph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21649 2022-10-26 19:46:38.000000 protgraph-0.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.363413 protgraph-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-28 17:57:47.000000 protgraph-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 17:57:47.000000 protgraph-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-04-28 17:57:57.363413 protgraph-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-04-28 17:57:47.000000 protgraph-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.351413 protgraph-0.3.9/protgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/aa_masses_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/aa_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/annotate_ptms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33762 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/digestion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.359413 protgraph-0.3.9/protgraph/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/abstract_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/binary_pcsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/generic_file_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/gml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/graphml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/gremlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/large_binary_pcsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/large_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/large_pcsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/pcsr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.359413 protgraph-0.3.9/protgraph/export/peptides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/abstract_peptide_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/pep_citus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/pep_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/pep_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/pep_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/pep_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/peptides/pep_trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/export/redisgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.363413 protgraph-0.3.9/protgraph/ft_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/ft_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/ft_execution/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/ft_execution/generic_cleaved_peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/ft_execution/init_met.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/ft_execution/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/ft_execution/var_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/graph_collapse_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/graph_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/graph_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/merge_aminoacids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/protgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/read_embl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.363413 protgraph-0.3.9/protgraph/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/compact_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/convert_fasta_to_sp_embl_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/generate_fasta_decoys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/pepsqlite_to_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/print_sums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/scripts/replace_fasta_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/unexpected_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 17:57:48.000000 protgraph-0.3.9/protgraph/verify_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:57:57.351413 protgraph-0.3.9/protgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-04-28 17:57:57.000000 protgraph-0.3.9/protgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-28 17:57:57.000000 protgraph-0.3.9/protgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:57:57.000000 protgraph-0.3.9/protgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-28 17:57:57.000000 protgraph-0.3.9/protgraph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-28 17:57:57.000000 protgraph-0.3.9/protgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 17:57:57.000000 protgraph-0.3.9/protgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 17:57:48.000000 protgraph-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:57:57.363413 protgraph-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-28 17:57:48.000000 protgraph-0.3.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `protgraph-0.3.8/protgraph/ft_execution/generic.py` & `protgraph-0.3.9/protgraph/ft_execution/generic.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/ft_execution/signal.py` & `protgraph-0.3.9/protgraph/ft_execution/signal.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/ft_execution/init_met.py` & `protgraph-0.3.9/protgraph/ft_execution/init_met.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/ft_execution/var_seq.py` & `protgraph-0.3.9/protgraph/ft_execution/var_seq.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/ft_execution/generic_cleaved_peptide.py` & `protgraph-0.3.9/protgraph/ft_execution/generic_cleaved_peptide.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/ft_execution/__init__.py` & `protgraph-0.3.9/protgraph/ft_execution/__init__.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/aa_replacer.py` & `protgraph-0.3.9/protgraph/aa_replacer.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/cli.py` & `protgraph-0.3.9/protgraph/cli.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/unexpected_exception.py` & `protgraph-0.3.9/protgraph/unexpected_exception.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/read_embl.py` & `protgraph-0.3.9/protgraph/read_embl.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/digestion.py` & `protgraph-0.3.9/protgraph/digestion.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/graph_collapse_edges.py` & `protgraph-0.3.9/protgraph/graph_collapse_edges.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/protgraph.py` & `protgraph-0.3.9/protgraph/protgraph.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/postgres.py` & `protgraph-0.3.9/protgraph/export/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 import psycopg
-from Bio.SwissProt import FeatureLocation, FeatureTable
+from Bio.SeqFeature import FeatureLocation
+from Bio.SwissProt import FeatureTable
 
 from protgraph.export.abstract_exporter import AExporter
 from protgraph.graph_collapse_edges import Or
 
 
 class Postgres(AExporter):
     """
```

### Comparing `protgraph-0.3.8/protgraph/export/exporters.py` & `protgraph-0.3.9/protgraph/export/exporters.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/peptides/pep_sqlite.py` & `protgraph-0.3.9/protgraph/export/peptides/pep_sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                     meta {B});""".format(B="BLOB" if self.use_blob else "TEXT"))
             else:
                 cur.execute("""
                 CREATE TABLE if not exists peptide_meta (
                     peptide {B},
                     meta {B});""".format(B="BLOB" if self.use_blob else "TEXT"))
         except Exception as e:
-            print("Warning: Failed creating table 'peptides_meta' (Reason: {})".format(str(e)))
+            print("Warning: Failed creating table 'peptide_meta' (Reason: {})".format(str(e)))
         finally:
             # self.conn.commit()
             cur.close()
 
         if self.use_blob:
             self.set_upsert_query = \
                 """
@@ -191,15 +191,15 @@
                 self.set_upsert_query,
                 zip(compressed_peptides, compressed_metas, compressed_metas)
             )
         else:
             self._retry_query_many(
                 cur,
                 """
-                INSERT INTO peptides_meta (peptide, meta)
+                INSERT INTO peptide_meta (peptide, meta)
                 VALUES (?, ?);
                 """,
                 zip(compressed_peptides, compressed_metas)
             )
         cur.execute('COMMIT')
 
         # self.conn.commit()
```

### Comparing `protgraph-0.3.8/protgraph/export/peptides/pep_mysql.py` & `protgraph-0.3.9/protgraph/export/peptides/pep_mysql.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/peptides/abstract_peptide_exporter.py` & `protgraph-0.3.9/protgraph/export/peptides/abstract_peptide_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         l_path = []
         l_edge_ids = []
         l_aas = []
         l_cleaved = []
         # Iterate over all peptides
         for path in self._get_peps(prot_graph, __start_node__, __stop_node__):
 
-
             # Get the actual peptide (concatenated aminoacids)
             aas = "".join(prot_graph.vs[path[1:-1]]["aminoacid"])
 
             # Get the edge ids from a path
-            edge_ids = prot_graph.get_eids(path=path)
+            pairs = [(a, b) for a, b in zip(path, path[1:])]
+            edge_ids = prot_graph.get_eids(pairs=pairs)
 
             # Skip Peptides, which contain an X
             if self.skip_x and "X" in aas:
                 continue
 
             # Filter by peptide length
             if len(aas) < self.peptide_min_length:
```

### Comparing `protgraph-0.3.8/protgraph/export/peptides/pep_postgres.py` & `protgraph-0.3.9/protgraph/export/peptides/pep_postgres.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/peptides/pep_trie.py` & `protgraph-0.3.9/protgraph/export/peptides/pep_trie.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/peptides/pep_fasta.py` & `protgraph-0.3.9/protgraph/export/peptides/pep_fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Bio.SwissProt import UnknownPosition
+from Bio.SeqFeature import UnknownPosition
 
 from protgraph.export.peptides.abstract_peptide_exporter import \
     APeptideExporter
 from protgraph.graph_collapse_edges import Or
 
 
 class PepFasta(APeptideExporter):
```

### Comparing `protgraph-0.3.8/protgraph/export/peptides/pep_citus.py` & `protgraph-0.3.9/protgraph/export/peptides/pep_citus.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/binary_pcsr.py` & `protgraph-0.3.9/protgraph/export/binary_pcsr.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/cassandra.py` & `protgraph-0.3.9/protgraph/export/cassandra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 # import cassandra
-from Bio.SwissProt import FeatureLocation, FeatureTable
+from Bio.SeqFeature import FeatureLocation
+from Bio.SwissProt import FeatureTable
 # from cassandra.query import BatchStatement
 from cassandra import InvalidRequest
 from cassandra.cluster import Cluster
 
 from protgraph.export.abstract_exporter import AExporter
 # import cassandra.concurrent
 from protgraph.graph_collapse_edges import Or
```

### Comparing `protgraph-0.3.8/protgraph/export/mysql.py` & `protgraph-0.3.9/protgraph/export/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 import mysql.connector
-from Bio.SwissProt import FeatureLocation, FeatureTable
+from Bio.SeqFeature import FeatureLocation
+from Bio.SwissProt import FeatureTable
 
 from protgraph.export.abstract_exporter import AExporter
 from protgraph.graph_collapse_edges import Or
 
 
 class MySQL(AExporter):
     """
```

### Comparing `protgraph-0.3.8/protgraph/export/generic_file_exporter.py` & `protgraph-0.3.9/protgraph/export/generic_file_exporter.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/abstract_exporter.py` & `protgraph-0.3.9/protgraph/export/abstract_exporter.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/large_binary_pcsr.py` & `protgraph-0.3.9/protgraph/export/large_binary_pcsr.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/pcsr.py` & `protgraph-0.3.9/protgraph/export/pcsr.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/large_csv.py` & `protgraph-0.3.9/protgraph/export/large_csv.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/gremlin.py` & `protgraph-0.3.9/protgraph/export/gremlin.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/csv.py` & `protgraph-0.3.9/protgraph/export/csv.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/export/redisgraph.py` & `protgraph-0.3.9/protgraph/export/redisgraph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import redis
-from Bio.SwissProt import FeatureLocation, FeatureTable
+from Bio.SeqFeature import FeatureLocation
+from Bio.SwissProt import FeatureTable
 from redisgraph import Edge, Graph, Node
 
 from protgraph.export.abstract_exporter import AExporter
 from protgraph.graph_collapse_edges import Or
 
 
 class RedisGraph(AExporter):
```

### Comparing `protgraph-0.3.8/protgraph/export/large_pcsr.py` & `protgraph-0.3.9/protgraph/export/large_pcsr.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/aa_masses_annotation.py` & `protgraph-0.3.9/protgraph/aa_masses_annotation.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/verify_graphs.py` & `protgraph-0.3.9/protgraph/verify_graphs.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/graph_generator.py` & `protgraph-0.3.9/protgraph/graph_generator.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/annotate_ptms.py` & `protgraph-0.3.9/protgraph/annotate_ptms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from Bio.SwissProt import FeatureLocation, FeatureTable, UnknownPosition
+from Bio.SeqFeature import FeatureLocation, UnknownPosition
+from Bio.SwissProt import FeatureTable
 
 
 def annotate_ptms(graph_entry, var_mods: list, fix_mods: list, mass_factor: int):
     """
     Annotates a delta_mass which should be considered during the generation of weights
 
     E.G: var_mods contains [("M",  "+15.994915")] (via CLI "-vb 'M:+15.994915'")
```

### Comparing `protgraph-0.3.8/protgraph/graph_statistics.py` & `protgraph-0.3.9/protgraph/graph_statistics.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/scripts/pepsqlite_to_fasta.py` & `protgraph-0.3.9/protgraph/scripts/pepsqlite_to_fasta.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/scripts/print_sums.py` & `protgraph-0.3.9/protgraph/scripts/print_sums.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/scripts/compact_fasta.py` & `protgraph-0.3.9/protgraph/scripts/compact_fasta.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/scripts/replace_fasta_header.py` & `protgraph-0.3.9/protgraph/scripts/replace_fasta_header.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/scripts/generate_fasta_decoys.py` & `protgraph-0.3.9/protgraph/scripts/generate_fasta_decoys.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/protgraph/merge_aminoacids.py` & `protgraph-0.3.9/protgraph/merge_aminoacids.py`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/LICENSE` & `protgraph-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/README.md` & `protgraph-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `protgraph-0.3.8/setup.py` & `protgraph-0.3.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,43 @@
 from setuptools import find_packages, setup
 
-# Get Packages from Pipfile by parsing them
-lines = []
-with open("Pipfile", "r") as pipfile:
-    lines = pipfile.readlines()
-c = [idx for idx, x in enumerate(lines) if x[0] == "["]
-
-# packages index range
-packages_sec = [x for x in c if "[packages]" in lines[x]][0]
-if c.index(packages_sec) + 1 == len(c):
-    packages_end = len(lines)
-else:
-    packages_end = c[c.index(packages_sec)+1]
-
-# retrieve the packages (except itself)
+# Get Packages from requirements.txt by parsing them
 packages = []
-for i in range(packages_sec+1, packages_end):
-    if lines[i] == "\n":
-        continue
-    package = lines[i].split("=")[0].strip()
-    if package != "protgraph":
-        packages.append(package)
+with open("requirements.txt", "r") as reqs:
+    packages = reqs.readlines()
 
 # read README.md
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
+with open("README.md", "r", encoding="utf-8") as long_desc:
+    long_description = long_desc.read()
 
 setup(
     name='protgraph',
-    version='0.3.8',
+    version='0.3.9',
     author="Dominik Lux",
     description="ProtGraph, a graph generator for proteins.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mpc-bioinformatics/ProtGraph",
     project_urls={
         "Bugs": "https://github.com/mpc-bioinformatics/ProtGraph/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: BSD License',
     ],
     license="BSD",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     entry_points=dict(console_scripts=[
         'protgraph = protgraph.protgraph:main',
         'protgraph_pepsqlite_to_fasta = protgraph.scripts.pepsqlite_to_fasta:main [sqlite]',
         'protgraph_replace_fasta_header = protgraph.scripts.replace_fasta_header:main',
         'protgraph_generate_fasta_decoys = protgraph.scripts.generate_fasta_decoys:main',
         'protgraph_compact_fasta = protgraph.scripts.compact_fasta:main',
-        'protgraph_print_sums = protgraph.scripts.print_sums:main'
+        'protgraph_print_sums = protgraph.scripts.print_sums:main',
+        'protgraph_convert_fasta_to_sp_embl_txt = protgraph.scripts.convert_fasta_to_sp_embl_txt:main'
     ]),
     packages=find_packages(),
     include_package_data=True,
     install_requires=packages,
     extras_require={
         "postgres": ["psycopg>=3.0"],
         "mysql": ["mysql"],
```

### Comparing `protgraph-0.3.8/protgraph.egg-info/SOURCES.txt` & `protgraph-0.3.9/protgraph.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
-Pipfile
 README.md
+requirements.txt
 setup.py
 protgraph/__init__.py
 protgraph/__main__.py
 protgraph/aa_masses_annotation.py
 protgraph/aa_replacer.py
 protgraph/annotate_ptms.py
 protgraph/cli.py
@@ -55,11 +55,12 @@
 protgraph/ft_execution/generic.py
 protgraph/ft_execution/generic_cleaved_peptide.py
 protgraph/ft_execution/init_met.py
 protgraph/ft_execution/signal.py
 protgraph/ft_execution/var_seq.py
 protgraph/scripts/__init__.py
 protgraph/scripts/compact_fasta.py
+protgraph/scripts/convert_fasta_to_sp_embl_txt.py
 protgraph/scripts/generate_fasta_decoys.py
 protgraph/scripts/pepsqlite_to_fasta.py
 protgraph/scripts/print_sums.py
 protgraph/scripts/replace_fasta_header.py
```

### Comparing `protgraph-0.3.8/protgraph.egg-info/PKG-INFO` & `protgraph-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: protgraph
-Version: 0.3.8
+Version: 0.3.9
 Summary: ProtGraph, a graph generator for proteins.
 Home-page: https://github.com/mpc-bioinformatics/ProtGraph
 Author: Dominik Lux
 License: BSD
 Project-URL: Bugs, https://github.com/mpc-bioinformatics/ProtGraph/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: postgres
 Provides-Extra: mysql
 Provides-Extra: sqlite
 Provides-Extra: cassandra
 Provides-Extra: gremlin
 Provides-Extra: redis
@@ -390,9 +389,7 @@
 ```
 
 Instead of directly generating a FASTA-file we first create a database, summarizing same sequences and headers. As a post-processing step, the database-entries are exported into FASTA. The generated FASTA has unique sequence as entries and offers some additionally insights. From the first entries we see peptides shared by exactly 2 proteins. Looking at the difference between the compact and
 non-compact FASTA, we see that ~244 000 entries could be summarized into already included entries in the FASTA. This generated FASTA-file can be used for identification.
 
 **NOTE:** Protein-Graphs can contain large amounts of peptides/proteins. Do a dry run with the flags `-cnp`, `-cnpm` or `cnph` (or all of them) WITHOUT the export functionality first and examine the statistics output if it is feasible to generate a FASTA-file. Without a dry run it may happen that a protein like P04637 (P53 Human) with all possible peptides and variants is exported, which will
 very likely take up all your disk space.
-
-
```

### Comparing `protgraph-0.3.8/PKG-INFO` & `protgraph-0.3.9/protgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: protgraph
-Version: 0.3.8
+Version: 0.3.9
 Summary: ProtGraph, a graph generator for proteins.
 Home-page: https://github.com/mpc-bioinformatics/ProtGraph
 Author: Dominik Lux
 License: BSD
 Project-URL: Bugs, https://github.com/mpc-bioinformatics/ProtGraph/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: postgres
 Provides-Extra: mysql
 Provides-Extra: sqlite
 Provides-Extra: cassandra
 Provides-Extra: gremlin
 Provides-Extra: redis
@@ -390,9 +389,7 @@
 ```
 
 Instead of directly generating a FASTA-file we first create a database, summarizing same sequences and headers. As a post-processing step, the database-entries are exported into FASTA. The generated FASTA has unique sequence as entries and offers some additionally insights. From the first entries we see peptides shared by exactly 2 proteins. Looking at the difference between the compact and
 non-compact FASTA, we see that ~244 000 entries could be summarized into already included entries in the FASTA. This generated FASTA-file can be used for identification.
 
 **NOTE:** Protein-Graphs can contain large amounts of peptides/proteins. Do a dry run with the flags `-cnp`, `-cnpm` or `cnph` (or all of them) WITHOUT the export functionality first and examine the statistics output if it is feasible to generate a FASTA-file. Without a dry run it may happen that a protein like P04637 (P53 Human) with all possible peptides and variants is exported, which will
 very likely take up all your disk space.
-
-
```

