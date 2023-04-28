# Comparing `tmp/aspring-1.2.0.tar.gz` & `tmp/aspring-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspring-1.2.0.tar", last modified: Thu Feb 23 16:16:57 2023, max compression
+gzip compressed data, was "aspring-1.3.0.tar", last modified: Fri Apr 28 09:20:29 2023, max compression
```

## Comparing `aspring-1.2.0.tar` & `aspring-1.3.0.tar`

### file list

```diff
@@ -1,293 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.757365 aspring-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-23 16:16:43.000000 aspring-1.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.721364 aspring-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.725364 aspring-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-02-23 16:16:43.000000 aspring-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-23 16:16:43.000000 aspring-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-23 16:16:43.000000 aspring-1.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-23 16:16:43.000000 aspring-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-23 16:16:43.000000 aspring-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 16:16:43.000000 aspring-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-02-23 16:16:43.000000 aspring-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-23 16:16:43.000000 aspring-1.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-23 16:16:43.000000 aspring-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-23 16:16:43.000000 aspring-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-02-23 16:16:57.757365 aspring-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-02-23 16:16:43.000000 aspring-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/_static/nomenclature_example.png
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/docs/programs/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/programs/aspring.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/programs/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/programs/programs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-23 16:16:43.000000 aspring-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-23 16:16:43.000000 aspring-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-23 16:16:57.761365 aspring-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-23 16:16:43.000000 aspring-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.725364 aspring-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/src/aspring/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/src/aspring/R_script/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/R_script/.Rprofile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/src/aspring/R_script/renv/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/R_script/renv/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    27179 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/R_script/renv/activate.R
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/R_script/renv/settings.dcf
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/R_script/renv.lock
--rw-r--r--   0 runner    (1001) docker     (123)    24689 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/R_script/step_06_getStats.R
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_01_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_02_hmm_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_03_hmm_aligner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_04_gettable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_05_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_06_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_07_reformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    35879 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_08_ASRUs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-23 16:16:43.000000 aspring-1.2.0/src/aspring/step_09_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/src/aspring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 16:16:57.000000 aspring-1.2.0/src/aspring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.729364 aspring-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.725364 aspring-1.2.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.725364 aspring-1.2.0/tests/data/ENSG00000007866/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.733364 aspring-1.2.0/tests/data/ENSG00000007866/ASPRING_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_ASRUs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_duplication_pairs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_eventsDup_withCols.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_instances_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.733364 aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/ensembl_version.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50389 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/exonstable.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    73011 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/sequences.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    31669 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/tree.nh
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/tsl.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.733364 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.749364 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_10.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_11.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_12.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_13.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_14.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_15.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_16.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_17.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_18.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_19.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_20.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_21.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_23.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_24.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_25.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_26.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_27.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_28.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_30.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_4.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_6.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_7.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_8.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_9.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_12.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_13.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_14.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_16.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_17.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_18.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_19.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_20.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_21.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_23.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_24.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_25.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_26.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_27.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_28.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_30.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_12.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_13.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_14.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_15.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_16.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_17.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_18.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_19.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_20.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_21.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_23.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_24.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_25.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_26.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_27.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_28.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_30.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)   180874 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_10.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_11.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_12.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_13.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_14.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_15.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_16.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_17.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_18.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_19.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_20.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_21.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_23.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_24.csv
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_25.csv
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_26.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_27.csv
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_30.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_6.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_7.csv
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_8.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_9.csv
--rw-r--r--   0 runner    (1001) docker     (123)   175139 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/transcript_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/ases_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.757365 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_2.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_3.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_11_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_11_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_19_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_19_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_1_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_1_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_20_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_20_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_21_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_21_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_24_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_24_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_25_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_25_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_26_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_26_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_27_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_27_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_28_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_28_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_2.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_30_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_30_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_4_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_4_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_2.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_6_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_6_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_1.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_2.hhm
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_8_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_8_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.hhm
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/path_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:16:57.757365 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/s_exons.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    30757 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.pir
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/tree.nh
--rw-r--r--   0 runner    (1001) docker     (123)   213036 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/s_exon_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)    65982 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/splice_graph.gml
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-02-23 16:16:43.000000 aspring-1.2.0/tests/test_aspring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-02-23 16:16:43.000000 aspring-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.141781 aspring-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 09:20:16.000000 aspring-1.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.109780 aspring-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.109780 aspring-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-28 09:20:16.000000 aspring-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:20:16.000000 aspring-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 09:20:16.000000 aspring-1.3.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 09:20:16.000000 aspring-1.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 09:20:16.000000 aspring-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 09:20:16.000000 aspring-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-28 09:20:16.000000 aspring-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 09:20:16.000000 aspring-1.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 09:20:16.000000 aspring-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-28 09:20:16.000000 aspring-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-04-28 09:20:29.141781 aspring-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-04-28 09:20:16.000000 aspring-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.113780 aspring-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.113780 aspring-1.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/_static/nomenclature_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   116320 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/_static/pymol.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.113780 aspring-1.3.0/docs/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/programs/aspring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/programs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/programs/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 09:20:16.000000 aspring-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 09:20:16.000000 aspring-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-28 09:20:29.141781 aspring-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 09:20:16.000000 aspring-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.109780 aspring-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.113780 aspring-1.3.0/src/aspring/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.113780 aspring-1.3.0/src/aspring/R_script/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/R_script/.Rprofile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.117780 aspring-1.3.0/src/aspring/R_script/renv/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/R_script/renv/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    27179 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/R_script/renv/activate.R
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/R_script/renv/settings.dcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/R_script/renv.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    24689 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/R_script/step_06_getStats.R
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_01_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_02_hmm_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_03_hmm_aligner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_04_gettable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_05_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_06_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_07_reformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35879 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_08_ASRUs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_09_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-28 09:20:16.000000 aspring-1.3.0/src/aspring/step_10_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.113780 aspring-1.3.0/src/aspring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-04-28 09:20:29.000000 aspring-1.3.0/src/aspring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-28 09:20:29.000000 aspring-1.3.0/src/aspring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:20:29.000000 aspring-1.3.0/src/aspring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 09:20:29.000000 aspring-1.3.0/src/aspring.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:20:28.000000 aspring-1.3.0/src/aspring.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-28 09:20:29.000000 aspring-1.3.0/src/aspring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 09:20:29.000000 aspring-1.3.0/src/aspring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.117780 aspring-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.109780 aspring-1.3.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.109780 aspring-1.3.0/tests/data/ENSG00000007866/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.117780 aspring-1.3.0/tests/data/ENSG00000007866/ASPRING_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_ASRUs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_duplication_pairs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_eventsDup_withCols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_instances_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.117780 aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/ensembl_version.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50389 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/exonstable.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    73011 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/sequences.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    31669 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/tree.nh
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/tsl.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.117780 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.129781 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_10.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_11.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_12.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_13.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_14.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_15.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_16.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_17.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_18.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_19.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_20.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_21.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_23.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_24.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_25.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_26.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_27.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_28.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_30.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_4.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_6.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_7.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_8.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_9.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_12.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_13.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_14.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_16.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_18.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_19.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_20.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_21.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_23.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_24.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_25.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_26.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_27.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_28.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/gene_ids_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_12.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_13.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_14.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_16.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_18.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_19.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_20.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_21.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_23.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_24.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_25.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_26.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_27.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_28.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   180874 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_12.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_14.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_15.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_16.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_18.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_30.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   175139 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/transcript_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/ases_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.141781 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_2.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_3.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_11_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_11_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_19_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_19_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_1_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_1_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_20_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_20_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_21_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_21_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_24_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_24_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_25_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_25_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_26_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_26_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_27_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_27_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_28_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_28_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_2.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_30_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_30_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_4_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_4_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_2.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_6_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_6_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_1.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_2.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_8_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_8_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.hhm
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/path_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:20:29.141781 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/s_exons.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    30757 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.pir
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/tree.nh
+-rw-r--r--   0 runner    (1001) docker     (123)   213036 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/s_exon_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    65982 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/splice_graph.gml
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-28 09:20:16.000000 aspring-1.3.0/tests/test_aspring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-28 09:20:16.000000 aspring-1.3.0/tox.ini
```

### Comparing `aspring-1.2.0/.coveragerc` & `aspring-1.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/.github/workflows/ci.yml` & `aspring-1.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/.gitignore` & `aspring-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/.readthedocs.yml` & `aspring-1.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/CONTRIBUTING.rst` & `aspring-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/Dockerfile` & `aspring-1.3.0/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 FROM continuumio/miniconda3:4.9.2
 
 # Install hhsuite, r-base=4.2.2, and aspring==1.0.0
 RUN conda install -y -c conda-forge -c bioconda hhsuite && \
     conda install -y -c conda-forge r-base=4.2.2 && \
-    pip install aspring==1.2.0
+    pip install aspring==1.3.0
 
 # Install renv package for R and restore renv environment for aspring R script
 RUN Rscript -e 'options(repos = c(CRAN = "https://cran.rstudio.com/")); install.packages("renv")' && \
     Rscript -e 'renv::restore(project="/opt/conda/lib/python3.8/site-packages/aspring/R_script")'
 
 ENV HHSUITE_SCRIPTS /opt/conda/scripts
```

### Comparing `aspring-1.2.0/LICENSE.txt` & `aspring-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/MANIFEST.in` & `aspring-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/PKG-INFO` & `aspring-1.3.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: aspring
-Version: 1.2.0
-Summary: Alternatively Spliced Pseudo Repeat IN-Gene
-Home-page: https://github.com/PhyloSofS-Team/aspring
-Author: Antoine Szatkownik, Diego Javier Zea, Hugues Richard & Elodie Laine
-Author-email: diegozea@gmail.com
-License: MIT
-Project-URL: Documentation, https://aspring.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/PhyloSofS-Team/aspring
-Project-URL: Changelog, https://github.com/PhyloSofS-Team/aspring/changelog.html
-Project-URL: Tracker, https://github.com/PhyloSofS-Team/aspring/issues
-Platform: Linux
-Platform: Mac
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE.txt
-
 .. image:: https://readthedocs.org/projects/aspring/badge/?version=latest
     :alt: ReadTheDocs
     :target: https://aspring.readthedocs.io/en/stable/
 .. image:: https://img.shields.io/coveralls/github/PhyloSofS-Team/aspring/main.svg
     :alt: Coveralls
     :target: https://coveralls.io/r/PhyloSofS-Team/aspring
 .. image:: https://img.shields.io/pypi/v/aspring.svg
@@ -51,23 +26,22 @@
 **ASPRING** is a computational tool for detecting Alternative Splicing Repetitive Units
 (ASRUs) on a gene. It analyzes the outputs of ThorAxe, which provides Multiple Sequence
 Alignments of exonic regions and generates information about their use on alternative
 isoforms. You can run aspring through the command line to find duplication events of such
 exonic regions. This tool will provide information on the duplicated regions through a
 couple of tables.
 
-.. note:: 
-
-    **ASPRING** requires **ThorAxe outputs** for a single query gene to run. If you don't
+.. note::  **ASPRING** requires **ThorAxe outputs** for a single query gene to run. If you don't
     have ThorAxe outputs, you can visit the `ThorAxe documentation`_ to learn how to install
     and run ThorAxe on your data. ThorAxe can also be run using the `Ases web server`_,
     which provides a user-friendly interface for running ThorAxe online. Note that you can
     skip the PhyloSofS step of Ases to obtain results more quickly for use with ``aspring``.
     Once you have ThorAxe outputs, you can use ``aspring`` to identify ASRUs for your query
     gene.
+.. 
 
 
 
 Requirements
 ============
 
 **ASPRING** is a Python package that can be installed from PyPI using the pip package
@@ -98,33 +72,31 @@
 
 Nomenclature
 ============
 
 .. image:: https://raw.githubusercontent.com/PhyloSofS-Team/aspring/main/docs/_static/nomenclature_example.png
   :alt: ASPRING nomenclature explained using a ThorAxe Evolutionary Splicing Graph (ESG). The image shows an ASRU composed by two ASPRs, one of them composed by multiple s-exons.
 
-The figure shows an example of an **Alternative Splicing Repetitive Unit** (**ASRU**)
-composed by two **Alternatively Spliced Pseudo Repeats** (**ASPRs**), one of them composed
-by multiple **s-exons**.
+The figure shows an example of an **Alternatively Spliced Repetitive Unit** (**ASRU**)
+composed by two **spliced-repeats** (**s-repeats**), one of them defined by a single s-exon and the other one comprising multiple **s-exons**.
 
-The nodes are the s-exons. The opaque red boxes are the ASPRs, and the transparent red box
+The nodes are the s-exons. The opaque red boxes are the s-repeats, and the transparent red box
 is the ASRU.
 
-The **ASPRs** are repetitive units identified by ASPRING that consist of one or more s-exons
-alternatively spliced in different isoforms. Note that ASPRs are called **instances** on the
+The **s-repeats** are repetitive units identified by ASPRING consisting of one or more s-exons
+alternatively included or excluded in different isoforms. Note that s-repeats are called **instances** on the
 output tables.
 
 How to use aspring
 ==================
 
 ``aspring`` is a Python-based command-line tool that helps identify Alternative Splicing
 Repetitive Units (ASRUs) from Thoraxe outputs for a single query gene. The tool executes
 several steps that involve converting data, creating HMM profiles, aligning profiles,
-parsing and filtering alignments, and generating ASRUs and Alternatively Spliced Pseudo
-Repeats (ASPRs) tables for the query gene.
+parsing and filtering alignments, and generating ASRUs and spliced-repeats (s-repeats) tables for the query gene.
 
 Here is how to run the script after installing the package:
 
 1. Open your terminal.
 2. Run the script with the following command:
 
    ::
@@ -140,15 +112,15 @@
    path to the ``reformat.pl`` script directory. Replace ``PATH_TO_THORAXE_OUTPUTS``
    with the path to the ThorAxe outputs directory for the gene of  interest.
 
    Optional arguments are available to customize the behavior of the script. Run the command
    ``aspring --help`` to see the full list of options.
 
 The script will execute several steps and generate output files containing ASRU and
-ASPR tables for the query gene.
+s-repeats tables for the query gene.
 
 
 Docker
 ------
 
 To ease the use and installation of ASPRING, we have created a Docker image that
 you can easily download and run. The aspring Docker image is available on
@@ -201,14 +173,15 @@
    coverage, p-value and number of species in the MSAs.
 6. ``step_06_stats``: Generates statistics on the filtered duplicated regions.
 7. ``step_07_reformat``: Reformat the previous outputs to add the information about the
    duplicated regions.
 8. ``step_08_ASRUs``: Identifies the Alternative Splicing Repetitive Units (ASRUs) on the
    gene.
 9. ``step_09_clean``: Removes the intermediate files generated during the pipeline.
+10. ``step_10_struct``: Maps s-exons and ASRUs to the protein structures obtained from AlphaFold DB.
 
 Note that the main script ``aspring`` **runs the entire pipeline** automatically. However,
 the user can also execute the scripts of each pipeline step individually for more control
 over the pipeline.
 
 
 Outputs
@@ -217,48 +190,50 @@
 For a given ``gene`` (Ensembl Gene ID), ASPRING returns:
 
 - ``{gene}_ASRUs_table.csv``
 - ``{gene}_instances_table.csv``
 - ``{gene}_duplication_pairs.csv``
 - ``{gene}_eventsDup_withCols.txt``
 - ``DupRaw/{gene}`` folder containing the ``s-exon_A.s-exon_B.hhr`` files (HMM-HMM alignments) 
+- ``structures`` folder containing the isoform structures obtained from 
+  `AlphaFold DB`_ (``.pdb`` files) and a set of `PyMol`_ scripts (``.pml`` files) with the 
+  s-exons and ASRUs selected and colored in the structure.
 
 {gene}_ASRUs_table.csv
 ----------------------
 
 This table provides information on the Alternatively Spliced Repeat Units (ASRUs) detected
 for the given ``gene``. Each row corresponds to a distinct ASRU and provides the following
 information:
 
 - ``gene``: The Ensembl Gene ID for the given gene.
-- ``ASRU``: The set of duplicated s-exons, a.k.a Alternatively Spliced Pseudo Repeats (ASPRs)
-  that belong to the ASRU.
+- ``ASRU``: The set s-repeats belonging to the ASRU.
 - ``Nbinstances``: The number of Alternatively Spliced Pseudo Repeats of the ASRU that were
   found in the exonic regions of the gene.
-- ``max``: The length of the longest ASPR instance of the ASRU, in residues.
-- ``min``: The length of the shortest ASPR instance of the ASRU, in residues.
+- ``max``: The length of the longest s-repeat of the ASRU, in residues.
+- ``min``: The length of the shortest s-repeat of the ASRU, in residues.
 - ``moy``: The mean length of the instances of the ASRU, in amino acid residues.
 - ``median``: The median length of the instances of the ASRU, in residues.
 - ``std``: The standard deviation of the lengths of the instances of the ASRU, in amino acid
   residues.
 - ``eventsRank``: The rank/position of the alternative splicing events involving the ASRU in
   the ``ases.csv`` output table from ThorAxe — from the most to the least conserved/frequent.
 
 {gene}_instances_table.csv
 --------------------------
 
 This table provides information on the instances of ASRUs detected for the given ``gene``.
 Each row corresponds to a distinct instance and provides the following information:
 
-- ``instance``: The sequence of the ASPR instance, in the form of a string of amino acid
+- ``instance``: The sequence of the s-repeat, in the form of a string of amino acid
   residues.
-- ``size``: The length of the ASPR instance, in amino acid residues.
-- ``NbSex``: The number of exonic regions where the ASPR instance was detected.
-- ``ASRU``: The set of homologous/duplicated s-exons that belong to the ASRU to which the ASPR
-  instance belongs.
+- ``size``: The length of the s-repeat, in amino acid residues.
+- ``NbSex``: The number of exonic regions where the s-repeat was detected.
+- ``ASRU``: The set of homologous/duplicated s-exons that belong to the ASRU to which the s-repeat
+   belongs.
 - ``gene``: The Ensembl Gene ID for the given gene.
  
 {gene}_duplication_pairs.csv
 ----------------------------
 
 This table provides information on the pairs of exonic regions that were involved in the
 duplication events. Each row corresponds to a distinct pair of s-exons and provides the
@@ -311,14 +286,38 @@
 - ``typePair``: The type of the alternative splicing event.
 - ``ColA``: The alignment columns corresponding to the first s-exon, in the format
   "start-end".
 - ``ColB``: The alignment columns corresponding to the second s-exon, in the format
   "start-end".
 
 
+structures
+----------
+
+This directory contains the isoform structures predicted by AlphaFold 2 that were obtained
+from `AlphaFold DB`_. These are the files with the ``.pdb`` extension. The folder also contains
+a PyMol script for each transcript whose isoform has a known downloaded structure. Those
+scripts have a name composed of the Ensembl gene name, followed by the transcript name, and ending with
+the file name of the AlphaFold structure and the ``.pml`` extension. For example,
+``ENSG00000007866_ENST00000338863_AF-Q99594-F1-model_v4.pml`` is the PyMol script for the isoform
+corresponding to the transcript ``ENST00000338863`` of the gene ``ENSG00000007866``. 
+When you run that script using `PyMol`_ as:
+
+.. code-block:: bash
+
+  pymol ENSG00000007866_ENST00000338863_AF-Q99594-F1-model_v4.pml
+  
+You will see the AlphaFold predicted structure of the isoform with the s-exon colored in 
+alternating light blue and yellow, and the ASRUs in red and green. For example, the 
+following image shows the PyMOL session for the ``ENST00000338863`` transcript:
+
+.. image:: https://raw.githubusercontent.com/PhyloSofS-Team/aspring/main/docs/_static/pymol.png
+  :alt: Screen capture of the PyMOL session for the ``ENST00000338863`` transcript showing the s-exons alternating in light blue and yellow, and the ARSU in red.
+
+
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage information on
 PyScaffold see https://pyscaffold.org/.
@@ -326,7 +325,9 @@
 
 .. _miniconda: https://docs.conda.io/en/latest/miniconda.html
 .. _renv: https://rstudio.github.io/renv/articles/renv.html
 .. _ThorAxe documentation: https://phylosofs-team.github.io/thoraxe/
 .. _Ases web server: http://www.lcqb.upmc.fr/Ases
 .. _Docker Hub: https://hub.docker.com/r/diegozea/aspring
 .. _official website: https://www.docker.com/
+.. _AlphaFold DB: https://alphafold.ebi.ac.uk/
+.. _PyMol: https://pymol.org/
```

### Comparing `aspring-1.2.0/README.rst` & `aspring-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: aspring
+Version: 1.3.0
+Summary: Alternatively Spliced Pseudo Repeat IN-Gene
+Home-page: https://github.com/PhyloSofS-Team/aspring
+Author: Antoine Szatkownik, Diego Javier Zea, Hugues Richard & Elodie Laine
+Author-email: diegozea@gmail.com
+License: MIT
+Project-URL: Documentation, https://aspring.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/PhyloSofS-Team/aspring
+Project-URL: Changelog, https://github.com/PhyloSofS-Team/aspring/changelog.html
+Project-URL: Tracker, https://github.com/PhyloSofS-Team/aspring/issues
+Platform: Linux
+Platform: Mac
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE.txt
+
 .. image:: https://readthedocs.org/projects/aspring/badge/?version=latest
     :alt: ReadTheDocs
     :target: https://aspring.readthedocs.io/en/stable/
 .. image:: https://img.shields.io/coveralls/github/PhyloSofS-Team/aspring/main.svg
     :alt: Coveralls
     :target: https://coveralls.io/r/PhyloSofS-Team/aspring
 .. image:: https://img.shields.io/pypi/v/aspring.svg
@@ -26,23 +51,22 @@
 **ASPRING** is a computational tool for detecting Alternative Splicing Repetitive Units
 (ASRUs) on a gene. It analyzes the outputs of ThorAxe, which provides Multiple Sequence
 Alignments of exonic regions and generates information about their use on alternative
 isoforms. You can run aspring through the command line to find duplication events of such
 exonic regions. This tool will provide information on the duplicated regions through a
 couple of tables.
 
-.. note:: 
-
-    **ASPRING** requires **ThorAxe outputs** for a single query gene to run. If you don't
+.. note::  **ASPRING** requires **ThorAxe outputs** for a single query gene to run. If you don't
     have ThorAxe outputs, you can visit the `ThorAxe documentation`_ to learn how to install
     and run ThorAxe on your data. ThorAxe can also be run using the `Ases web server`_,
     which provides a user-friendly interface for running ThorAxe online. Note that you can
     skip the PhyloSofS step of Ases to obtain results more quickly for use with ``aspring``.
     Once you have ThorAxe outputs, you can use ``aspring`` to identify ASRUs for your query
     gene.
+.. 
 
 
 
 Requirements
 ============
 
 **ASPRING** is a Python package that can be installed from PyPI using the pip package
@@ -73,33 +97,31 @@
 
 Nomenclature
 ============
 
 .. image:: https://raw.githubusercontent.com/PhyloSofS-Team/aspring/main/docs/_static/nomenclature_example.png
   :alt: ASPRING nomenclature explained using a ThorAxe Evolutionary Splicing Graph (ESG). The image shows an ASRU composed by two ASPRs, one of them composed by multiple s-exons.
 
-The figure shows an example of an **Alternative Splicing Repetitive Unit** (**ASRU**)
-composed by two **Alternatively Spliced Pseudo Repeats** (**ASPRs**), one of them composed
-by multiple **s-exons**.
+The figure shows an example of an **Alternatively Spliced Repetitive Unit** (**ASRU**)
+composed by two **spliced-repeats** (**s-repeats**), one of them defined by a single s-exon and the other one comprising multiple **s-exons**.
 
-The nodes are the s-exons. The opaque red boxes are the ASPRs, and the transparent red box
+The nodes are the s-exons. The opaque red boxes are the s-repeats, and the transparent red box
 is the ASRU.
 
-The **ASPRs** are repetitive units identified by ASPRING that consist of one or more s-exons
-alternatively spliced in different isoforms. Note that ASPRs are called **instances** on the
+The **s-repeats** are repetitive units identified by ASPRING consisting of one or more s-exons
+alternatively included or excluded in different isoforms. Note that s-repeats are called **instances** on the
 output tables.
 
 How to use aspring
 ==================
 
 ``aspring`` is a Python-based command-line tool that helps identify Alternative Splicing
 Repetitive Units (ASRUs) from Thoraxe outputs for a single query gene. The tool executes
 several steps that involve converting data, creating HMM profiles, aligning profiles,
-parsing and filtering alignments, and generating ASRUs and Alternatively Spliced Pseudo
-Repeats (ASPRs) tables for the query gene.
+parsing and filtering alignments, and generating ASRUs and spliced-repeats (s-repeats) tables for the query gene.
 
 Here is how to run the script after installing the package:
 
 1. Open your terminal.
 2. Run the script with the following command:
 
    ::
@@ -115,15 +137,15 @@
    path to the ``reformat.pl`` script directory. Replace ``PATH_TO_THORAXE_OUTPUTS``
    with the path to the ThorAxe outputs directory for the gene of  interest.
 
    Optional arguments are available to customize the behavior of the script. Run the command
    ``aspring --help`` to see the full list of options.
 
 The script will execute several steps and generate output files containing ASRU and
-ASPR tables for the query gene.
+s-repeats tables for the query gene.
 
 
 Docker
 ------
 
 To ease the use and installation of ASPRING, we have created a Docker image that
 you can easily download and run. The aspring Docker image is available on
@@ -176,14 +198,15 @@
    coverage, p-value and number of species in the MSAs.
 6. ``step_06_stats``: Generates statistics on the filtered duplicated regions.
 7. ``step_07_reformat``: Reformat the previous outputs to add the information about the
    duplicated regions.
 8. ``step_08_ASRUs``: Identifies the Alternative Splicing Repetitive Units (ASRUs) on the
    gene.
 9. ``step_09_clean``: Removes the intermediate files generated during the pipeline.
+10. ``step_10_struct``: Maps s-exons and ASRUs to the protein structures obtained from AlphaFold DB.
 
 Note that the main script ``aspring`` **runs the entire pipeline** automatically. However,
 the user can also execute the scripts of each pipeline step individually for more control
 over the pipeline.
 
 
 Outputs
@@ -192,48 +215,50 @@
 For a given ``gene`` (Ensembl Gene ID), ASPRING returns:
 
 - ``{gene}_ASRUs_table.csv``
 - ``{gene}_instances_table.csv``
 - ``{gene}_duplication_pairs.csv``
 - ``{gene}_eventsDup_withCols.txt``
 - ``DupRaw/{gene}`` folder containing the ``s-exon_A.s-exon_B.hhr`` files (HMM-HMM alignments) 
+- ``structures`` folder containing the isoform structures obtained from 
+  `AlphaFold DB`_ (``.pdb`` files) and a set of `PyMol`_ scripts (``.pml`` files) with the 
+  s-exons and ASRUs selected and colored in the structure.
 
 {gene}_ASRUs_table.csv
 ----------------------
 
 This table provides information on the Alternatively Spliced Repeat Units (ASRUs) detected
 for the given ``gene``. Each row corresponds to a distinct ASRU and provides the following
 information:
 
 - ``gene``: The Ensembl Gene ID for the given gene.
-- ``ASRU``: The set of duplicated s-exons, a.k.a Alternatively Spliced Pseudo Repeats (ASPRs)
-  that belong to the ASRU.
+- ``ASRU``: The set s-repeats belonging to the ASRU.
 - ``Nbinstances``: The number of Alternatively Spliced Pseudo Repeats of the ASRU that were
   found in the exonic regions of the gene.
-- ``max``: The length of the longest ASPR instance of the ASRU, in residues.
-- ``min``: The length of the shortest ASPR instance of the ASRU, in residues.
+- ``max``: The length of the longest s-repeat of the ASRU, in residues.
+- ``min``: The length of the shortest s-repeat of the ASRU, in residues.
 - ``moy``: The mean length of the instances of the ASRU, in amino acid residues.
 - ``median``: The median length of the instances of the ASRU, in residues.
 - ``std``: The standard deviation of the lengths of the instances of the ASRU, in amino acid
   residues.
 - ``eventsRank``: The rank/position of the alternative splicing events involving the ASRU in
   the ``ases.csv`` output table from ThorAxe — from the most to the least conserved/frequent.
 
 {gene}_instances_table.csv
 --------------------------
 
 This table provides information on the instances of ASRUs detected for the given ``gene``.
 Each row corresponds to a distinct instance and provides the following information:
 
-- ``instance``: The sequence of the ASPR instance, in the form of a string of amino acid
+- ``instance``: The sequence of the s-repeat, in the form of a string of amino acid
   residues.
-- ``size``: The length of the ASPR instance, in amino acid residues.
-- ``NbSex``: The number of exonic regions where the ASPR instance was detected.
-- ``ASRU``: The set of homologous/duplicated s-exons that belong to the ASRU to which the ASPR
-  instance belongs.
+- ``size``: The length of the s-repeat, in amino acid residues.
+- ``NbSex``: The number of exonic regions where the s-repeat was detected.
+- ``ASRU``: The set of homologous/duplicated s-exons that belong to the ASRU to which the s-repeat
+   belongs.
 - ``gene``: The Ensembl Gene ID for the given gene.
  
 {gene}_duplication_pairs.csv
 ----------------------------
 
 This table provides information on the pairs of exonic regions that were involved in the
 duplication events. Each row corresponds to a distinct pair of s-exons and provides the
@@ -286,14 +311,38 @@
 - ``typePair``: The type of the alternative splicing event.
 - ``ColA``: The alignment columns corresponding to the first s-exon, in the format
   "start-end".
 - ``ColB``: The alignment columns corresponding to the second s-exon, in the format
   "start-end".
 
 
+structures
+----------
+
+This directory contains the isoform structures predicted by AlphaFold 2 that were obtained
+from `AlphaFold DB`_. These are the files with the ``.pdb`` extension. The folder also contains
+a PyMol script for each transcript whose isoform has a known downloaded structure. Those
+scripts have a name composed of the Ensembl gene name, followed by the transcript name, and ending with
+the file name of the AlphaFold structure and the ``.pml`` extension. For example,
+``ENSG00000007866_ENST00000338863_AF-Q99594-F1-model_v4.pml`` is the PyMol script for the isoform
+corresponding to the transcript ``ENST00000338863`` of the gene ``ENSG00000007866``. 
+When you run that script using `PyMol`_ as:
+
+.. code-block:: bash
+
+  pymol ENSG00000007866_ENST00000338863_AF-Q99594-F1-model_v4.pml
+  
+You will see the AlphaFold predicted structure of the isoform with the s-exon colored in 
+alternating light blue and yellow, and the ASRUs in red and green. For example, the 
+following image shows the PyMOL session for the ``ENST00000338863`` transcript:
+
+.. image:: https://raw.githubusercontent.com/PhyloSofS-Team/aspring/main/docs/_static/pymol.png
+  :alt: Screen capture of the PyMOL session for the ``ENST00000338863`` transcript showing the s-exons alternating in light blue and yellow, and the ARSU in red.
+
+
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage information on
 PyScaffold see https://pyscaffold.org/.
@@ -301,7 +350,9 @@
 
 .. _miniconda: https://docs.conda.io/en/latest/miniconda.html
 .. _renv: https://rstudio.github.io/renv/articles/renv.html
 .. _ThorAxe documentation: https://phylosofs-team.github.io/thoraxe/
 .. _Ases web server: http://www.lcqb.upmc.fr/Ases
 .. _Docker Hub: https://hub.docker.com/r/diegozea/aspring
 .. _official website: https://www.docker.com/
+.. _AlphaFold DB: https://alphafold.ebi.ac.uk/
+.. _PyMol: https://pymol.org/
```

### Comparing `aspring-1.2.0/docs/Makefile` & `aspring-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/docs/_static/nomenclature_example.png` & `aspring-1.3.0/docs/_static/nomenclature_example.png`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/docs/conf.py` & `aspring-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/docs/programs/pipeline.rst` & `aspring-1.3.0/docs/programs/pipeline.rst`

 * *Files 10% similar despite different names*

```diff
@@ -63,8 +63,15 @@
     :prog: step_08_ASRUs
 
 step_09_clean
 -------------
 
 .. argparse::
     :ref: aspring.step_09_clean.get_arg_parser
-    :prog: step_09_clean
+    :prog: step_09_clean
+
+step_10_struct
+--------------
+
+.. argparse::
+    :ref: aspring.step_10_struct.get_arg_parser
+    :prog: step_10_struct
```

### Comparing `aspring-1.2.0/setup.cfg` & `aspring-1.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 	=src
 python_requires = >=3.7,<3.12
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numpy>=1.12.0,<1.30
 	pandas>=0.21.0,<1.6
 	networkx>=2.3.0,<2.9
+	requests>=2.25,<2.27
+	biomart>=0.9.2,<0.10
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
@@ -55,14 +57,15 @@
 	step_03_hmm_aligner = aspring.step_03_hmm_aligner:run
 	step_04_gettable = aspring.step_04_gettable:run
 	step_05_filter = aspring.step_05_filter:run
 	step_06_stats = aspring.step_06_stats:run
 	step_07_reformat = aspring.step_07_reformat:run
 	step_08_ASRUs = aspring.step_08_ASRUs:run
 	step_09_clean = aspring.step_09_clean:run
+	step_10_struct = aspring.step_10_struct:run
 
 [tool:pytest]
 addopts = 
 	--cov aspring --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `aspring-1.2.0/setup.py` & `aspring-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/R_script/renv/activate.R` & `aspring-1.3.0/src/aspring/R_script/renv/activate.R`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/R_script/renv.lock` & `aspring-1.3.0/src/aspring/R_script/renv.lock`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/R_script/step_06_getStats.R` & `aspring-1.3.0/src/aspring/R_script/step_06_getStats.R`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/__init__.py` & `aspring-1.3.0/src/aspring/__init__.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/main.py` & `aspring-1.3.0/src/aspring/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,21 @@
     print("END STEP 7")
 
     print("START STEP 8 : create ASRUs and instances tables for query gene")
     bashCommand = f"step_08_ASRUs --gene {gene} --dataPATH {path_data}"
     subprocess.run(bashCommand.split(), stdout=subprocess.PIPE)
     print("END STEP 8")
 
-    print("START FINAL STEP : remove temporary files")
+    print("START STEP 9 : remove temporary files")
     bashCommand = f"step_09_clean --gene {gene} --path_data {path_data}"
     subprocess.run(bashCommand.split(), stdout=subprocess.PIPE)
+
+    print("START FINAL STEP : map s-exons and ASRUs to the AlphaFold protein structures")
+    bashCommand = f"step_10_struct --gene {gene} --dataPATH {path_data}"
+    subprocess.run(bashCommand.split(), stdout=subprocess.PIPE)
     print("END")
 
 
 def run():
     args = parse_args(sys.argv[1:])
 
     gene = args.geneName
```

### Comparing `aspring-1.2.0/src/aspring/step_01_preprocess.py` & `aspring-1.3.0/src/aspring/step_01_preprocess.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_02_hmm_maker.py` & `aspring-1.3.0/src/aspring/step_02_hmm_maker.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_03_hmm_aligner.py` & `aspring-1.3.0/src/aspring/step_03_hmm_aligner.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_04_gettable.py` & `aspring-1.3.0/src/aspring/step_04_gettable.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_05_filter.py` & `aspring-1.3.0/src/aspring/step_05_filter.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_06_stats.py` & `aspring-1.3.0/src/aspring/step_06_stats.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_07_reformat.py` & `aspring-1.3.0/src/aspring/step_07_reformat.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_08_ASRUs.py` & `aspring-1.3.0/src/aspring/step_08_ASRUs.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring/step_09_clean.py` & `aspring-1.3.0/src/aspring/step_09_clean.py`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/src/aspring.egg-info/PKG-INFO` & `aspring-1.3.0/src/aspring.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspring
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alternatively Spliced Pseudo Repeat IN-Gene
 Home-page: https://github.com/PhyloSofS-Team/aspring
 Author: Antoine Szatkownik, Diego Javier Zea, Hugues Richard & Elodie Laine
 Author-email: diegozea@gmail.com
 License: MIT
 Project-URL: Documentation, https://aspring.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/PhyloSofS-Team/aspring
@@ -51,23 +51,22 @@
 **ASPRING** is a computational tool for detecting Alternative Splicing Repetitive Units
 (ASRUs) on a gene. It analyzes the outputs of ThorAxe, which provides Multiple Sequence
 Alignments of exonic regions and generates information about their use on alternative
 isoforms. You can run aspring through the command line to find duplication events of such
 exonic regions. This tool will provide information on the duplicated regions through a
 couple of tables.
 
-.. note:: 
-
-    **ASPRING** requires **ThorAxe outputs** for a single query gene to run. If you don't
+.. note::  **ASPRING** requires **ThorAxe outputs** for a single query gene to run. If you don't
     have ThorAxe outputs, you can visit the `ThorAxe documentation`_ to learn how to install
     and run ThorAxe on your data. ThorAxe can also be run using the `Ases web server`_,
     which provides a user-friendly interface for running ThorAxe online. Note that you can
     skip the PhyloSofS step of Ases to obtain results more quickly for use with ``aspring``.
     Once you have ThorAxe outputs, you can use ``aspring`` to identify ASRUs for your query
     gene.
+.. 
 
 
 
 Requirements
 ============
 
 **ASPRING** is a Python package that can be installed from PyPI using the pip package
@@ -98,33 +97,31 @@
 
 Nomenclature
 ============
 
 .. image:: https://raw.githubusercontent.com/PhyloSofS-Team/aspring/main/docs/_static/nomenclature_example.png
   :alt: ASPRING nomenclature explained using a ThorAxe Evolutionary Splicing Graph (ESG). The image shows an ASRU composed by two ASPRs, one of them composed by multiple s-exons.
 
-The figure shows an example of an **Alternative Splicing Repetitive Unit** (**ASRU**)
-composed by two **Alternatively Spliced Pseudo Repeats** (**ASPRs**), one of them composed
-by multiple **s-exons**.
+The figure shows an example of an **Alternatively Spliced Repetitive Unit** (**ASRU**)
+composed by two **spliced-repeats** (**s-repeats**), one of them defined by a single s-exon and the other one comprising multiple **s-exons**.
 
-The nodes are the s-exons. The opaque red boxes are the ASPRs, and the transparent red box
+The nodes are the s-exons. The opaque red boxes are the s-repeats, and the transparent red box
 is the ASRU.
 
-The **ASPRs** are repetitive units identified by ASPRING that consist of one or more s-exons
-alternatively spliced in different isoforms. Note that ASPRs are called **instances** on the
+The **s-repeats** are repetitive units identified by ASPRING consisting of one or more s-exons
+alternatively included or excluded in different isoforms. Note that s-repeats are called **instances** on the
 output tables.
 
 How to use aspring
 ==================
 
 ``aspring`` is a Python-based command-line tool that helps identify Alternative Splicing
 Repetitive Units (ASRUs) from Thoraxe outputs for a single query gene. The tool executes
 several steps that involve converting data, creating HMM profiles, aligning profiles,
-parsing and filtering alignments, and generating ASRUs and Alternatively Spliced Pseudo
-Repeats (ASPRs) tables for the query gene.
+parsing and filtering alignments, and generating ASRUs and spliced-repeats (s-repeats) tables for the query gene.
 
 Here is how to run the script after installing the package:
 
 1. Open your terminal.
 2. Run the script with the following command:
 
    ::
@@ -140,15 +137,15 @@
    path to the ``reformat.pl`` script directory. Replace ``PATH_TO_THORAXE_OUTPUTS``
    with the path to the ThorAxe outputs directory for the gene of  interest.
 
    Optional arguments are available to customize the behavior of the script. Run the command
    ``aspring --help`` to see the full list of options.
 
 The script will execute several steps and generate output files containing ASRU and
-ASPR tables for the query gene.
+s-repeats tables for the query gene.
 
 
 Docker
 ------
 
 To ease the use and installation of ASPRING, we have created a Docker image that
 you can easily download and run. The aspring Docker image is available on
@@ -201,14 +198,15 @@
    coverage, p-value and number of species in the MSAs.
 6. ``step_06_stats``: Generates statistics on the filtered duplicated regions.
 7. ``step_07_reformat``: Reformat the previous outputs to add the information about the
    duplicated regions.
 8. ``step_08_ASRUs``: Identifies the Alternative Splicing Repetitive Units (ASRUs) on the
    gene.
 9. ``step_09_clean``: Removes the intermediate files generated during the pipeline.
+10. ``step_10_struct``: Maps s-exons and ASRUs to the protein structures obtained from AlphaFold DB.
 
 Note that the main script ``aspring`` **runs the entire pipeline** automatically. However,
 the user can also execute the scripts of each pipeline step individually for more control
 over the pipeline.
 
 
 Outputs
@@ -217,48 +215,50 @@
 For a given ``gene`` (Ensembl Gene ID), ASPRING returns:
 
 - ``{gene}_ASRUs_table.csv``
 - ``{gene}_instances_table.csv``
 - ``{gene}_duplication_pairs.csv``
 - ``{gene}_eventsDup_withCols.txt``
 - ``DupRaw/{gene}`` folder containing the ``s-exon_A.s-exon_B.hhr`` files (HMM-HMM alignments) 
+- ``structures`` folder containing the isoform structures obtained from 
+  `AlphaFold DB`_ (``.pdb`` files) and a set of `PyMol`_ scripts (``.pml`` files) with the 
+  s-exons and ASRUs selected and colored in the structure.
 
 {gene}_ASRUs_table.csv
 ----------------------
 
 This table provides information on the Alternatively Spliced Repeat Units (ASRUs) detected
 for the given ``gene``. Each row corresponds to a distinct ASRU and provides the following
 information:
 
 - ``gene``: The Ensembl Gene ID for the given gene.
-- ``ASRU``: The set of duplicated s-exons, a.k.a Alternatively Spliced Pseudo Repeats (ASPRs)
-  that belong to the ASRU.
+- ``ASRU``: The set s-repeats belonging to the ASRU.
 - ``Nbinstances``: The number of Alternatively Spliced Pseudo Repeats of the ASRU that were
   found in the exonic regions of the gene.
-- ``max``: The length of the longest ASPR instance of the ASRU, in residues.
-- ``min``: The length of the shortest ASPR instance of the ASRU, in residues.
+- ``max``: The length of the longest s-repeat of the ASRU, in residues.
+- ``min``: The length of the shortest s-repeat of the ASRU, in residues.
 - ``moy``: The mean length of the instances of the ASRU, in amino acid residues.
 - ``median``: The median length of the instances of the ASRU, in residues.
 - ``std``: The standard deviation of the lengths of the instances of the ASRU, in amino acid
   residues.
 - ``eventsRank``: The rank/position of the alternative splicing events involving the ASRU in
   the ``ases.csv`` output table from ThorAxe — from the most to the least conserved/frequent.
 
 {gene}_instances_table.csv
 --------------------------
 
 This table provides information on the instances of ASRUs detected for the given ``gene``.
 Each row corresponds to a distinct instance and provides the following information:
 
-- ``instance``: The sequence of the ASPR instance, in the form of a string of amino acid
+- ``instance``: The sequence of the s-repeat, in the form of a string of amino acid
   residues.
-- ``size``: The length of the ASPR instance, in amino acid residues.
-- ``NbSex``: The number of exonic regions where the ASPR instance was detected.
-- ``ASRU``: The set of homologous/duplicated s-exons that belong to the ASRU to which the ASPR
-  instance belongs.
+- ``size``: The length of the s-repeat, in amino acid residues.
+- ``NbSex``: The number of exonic regions where the s-repeat was detected.
+- ``ASRU``: The set of homologous/duplicated s-exons that belong to the ASRU to which the s-repeat
+   belongs.
 - ``gene``: The Ensembl Gene ID for the given gene.
  
 {gene}_duplication_pairs.csv
 ----------------------------
 
 This table provides information on the pairs of exonic regions that were involved in the
 duplication events. Each row corresponds to a distinct pair of s-exons and provides the
@@ -311,14 +311,38 @@
 - ``typePair``: The type of the alternative splicing event.
 - ``ColA``: The alignment columns corresponding to the first s-exon, in the format
   "start-end".
 - ``ColB``: The alignment columns corresponding to the second s-exon, in the format
   "start-end".
 
 
+structures
+----------
+
+This directory contains the isoform structures predicted by AlphaFold 2 that were obtained
+from `AlphaFold DB`_. These are the files with the ``.pdb`` extension. The folder also contains
+a PyMol script for each transcript whose isoform has a known downloaded structure. Those
+scripts have a name composed of the Ensembl gene name, followed by the transcript name, and ending with
+the file name of the AlphaFold structure and the ``.pml`` extension. For example,
+``ENSG00000007866_ENST00000338863_AF-Q99594-F1-model_v4.pml`` is the PyMol script for the isoform
+corresponding to the transcript ``ENST00000338863`` of the gene ``ENSG00000007866``. 
+When you run that script using `PyMol`_ as:
+
+.. code-block:: bash
+
+  pymol ENSG00000007866_ENST00000338863_AF-Q99594-F1-model_v4.pml
+  
+You will see the AlphaFold predicted structure of the isoform with the s-exon colored in 
+alternating light blue and yellow, and the ASRUs in red and green. For example, the 
+following image shows the PyMOL session for the ``ENST00000338863`` transcript:
+
+.. image:: https://raw.githubusercontent.com/PhyloSofS-Team/aspring/main/docs/_static/pymol.png
+  :alt: Screen capture of the PyMOL session for the ``ENST00000338863`` transcript showing the s-exons alternating in light blue and yellow, and the ARSU in red.
+
+
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage information on
 PyScaffold see https://pyscaffold.org/.
@@ -326,7 +350,9 @@
 
 .. _miniconda: https://docs.conda.io/en/latest/miniconda.html
 .. _renv: https://rstudio.github.io/renv/articles/renv.html
 .. _ThorAxe documentation: https://phylosofs-team.github.io/thoraxe/
 .. _Ases web server: http://www.lcqb.upmc.fr/Ases
 .. _Docker Hub: https://hub.docker.com/r/diegozea/aspring
 .. _official website: https://www.docker.com/
+.. _AlphaFold DB: https://alphafold.ebi.ac.uk/
+.. _PyMol: https://pymol.org/
```

### Comparing `aspring-1.2.0/src/aspring.egg-info/SOURCES.txt` & `aspring-1.3.0/src/aspring.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,30 @@
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 docs/_static/nomenclature_example.png
+docs/_static/pymol.png
 docs/programs/aspring.rst
 docs/programs/pipeline.rst
 docs/programs/programs.rst
 src/aspring/__init__.py
 src/aspring/main.py
 src/aspring/step_01_preprocess.py
 src/aspring/step_02_hmm_maker.py
 src/aspring/step_03_hmm_aligner.py
 src/aspring/step_04_gettable.py
 src/aspring/step_05_filter.py
 src/aspring/step_06_stats.py
 src/aspring/step_07_reformat.py
 src/aspring/step_08_ASRUs.py
 src/aspring/step_09_clean.py
+src/aspring/step_10_struct.py
 src/aspring.egg-info/PKG-INFO
 src/aspring.egg-info/SOURCES.txt
 src/aspring.egg-info/dependency_links.txt
 src/aspring.egg-info/entry_points.txt
 src/aspring.egg-info/not-zip-safe
 src/aspring.egg-info/requires.txt
 src/aspring.egg-info/top_level.txt
```

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_duplication_pairs.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/ASPRING_reference/ENSG00000007866_duplication_pairs.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/exonstable.tsv` & `aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/exonstable.tsv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/sequences.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/sequences.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/tree.nh` & `aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/tree.nh`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/Ensembl/tsl.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/Ensembl/tsl.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_10.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_10.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_12.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_12.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_13.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_13.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_14.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_14.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_16.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_16.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_3.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_3.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_5.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_5.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_9.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/chimeric_alignment_9.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_10.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_10.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_12.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_12.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_13.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_13.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_14.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_14.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_16.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_16.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_20.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_20.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_21.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_21.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_3.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_3.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_30.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_30.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_5.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_5.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_9.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/msa_matrix_9.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_1.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_1.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_10.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_10.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_11.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_11.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_12.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_12.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_13.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_13.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_14.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_14.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_15.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_15.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_16.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_16.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_17.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_17.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_18.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_18.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_19.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_19.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_2.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_2.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_20.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_20.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_21.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_21.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_23.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_23.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_24.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_24.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_25.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_25.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_26.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_26.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_27.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_27.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_28.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_28.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_3.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_3.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_30.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_30.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_4.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_4.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_5.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_5.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_6.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_6.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_7.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_7.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_8.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_8.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_9.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/subexon_table_9.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/_intermediate/transcript_table.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/_intermediate/transcript_table.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/ases_table.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/ases_table.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_2.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_2.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_3.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_10_3.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_11_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_11_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_12_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_13_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_14_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_15_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_16_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_17_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_18_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_19_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_19_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_1_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_1_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_20_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_20_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_21_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_21_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_23_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_24_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_24_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_25_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_25_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_26_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_26_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_27_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_27_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_28_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_28_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_2.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_2_2.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_3_3.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_4_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_4_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_2.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_5_2.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_6_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_6_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_1.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_1.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_2.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_7_2.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_8_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_8_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.fasta` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.fasta`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.hhm` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/msa/msa_s_exon_9_0.hhm`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/path_table.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/path_table.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.pir` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.pir`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.txt` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/phylosofs/transcripts.txt`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/s_exon_table.csv` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/s_exon_table.csv`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tests/data/ENSG00000007866/thoraxe/splice_graph.gml` & `aspring-1.3.0/tests/data/ENSG00000007866/thoraxe/splice_graph.gml`

 * *Files identical despite different names*

### Comparing `aspring-1.2.0/tox.ini` & `aspring-1.3.0/tox.ini`

 * *Files identical despite different names*

