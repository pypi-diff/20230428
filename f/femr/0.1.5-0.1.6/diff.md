# Comparing `tmp/femr-0.1.5.tar.gz` & `tmp/femr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femr-0.1.5.tar", last modified: Wed Apr 26 20:59:35 2023, max compression
+gzip compressed data, was "femr-0.1.6.tar", last modified: Fri Apr 28 02:31:49 2023, max compression
```

## Comparing `femr-0.1.5.tar` & `femr-0.1.6.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.878107 femr-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-26 20:59:24.000000 femr-0.1.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.842105 femr-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.850106 femr-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 20:59:24.000000 femr-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 20:59:24.000000 femr-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.850106 femr-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-26 20:59:24.000000 femr-0.1.5/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-26 20:59:24.000000 femr-0.1.5/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 20:59:24.000000 femr-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-26 20:59:24.000000 femr-0.1.5/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-26 20:59:24.000000 femr-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-26 20:59:24.000000 femr-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-26 20:59:35.878107 femr-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-26 20:59:24.000000 femr-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 20:59:24.000000 femr-0.1.5/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.862106 femr-0.1.5/native/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 20:59:24.000000 femr-0.1.5/native/.bazelrc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 20:59:24.000000 femr-0.1.5/native/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 20:59:24.000000 femr-0.1.5/native/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-26 20:59:24.000000 femr-0.1.5/native/BUILD
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-26 20:59:24.000000 femr-0.1.5/native/WORKSPACE
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-26 20:59:24.000000 femr-0.1.5/native/backupbazelrc
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-26 20:59:24.000000 femr-0.1.5/native/civil_day_caster.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 20:59:24.000000 femr-0.1.5/native/clmbr_dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 20:59:24.000000 femr-0.1.5/native/compute_statistics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-26 20:59:24.000000 femr-0.1.5/native/constdb.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-26 20:59:24.000000 femr-0.1.5/native/constdb.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-26 20:59:24.000000 femr-0.1.5/native/convert_dictionary_formats.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-26 20:59:24.000000 femr-0.1.5/native/count_codes_and_values.cc
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-26 20:59:24.000000 femr-0.1.5/native/count_codes_and_values.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 20:59:24.000000 femr-0.1.5/native/count_codes_and_values_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 20:59:24.000000 femr-0.1.5/native/cpu_jax_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-04-26 20:59:24.000000 femr-0.1.5/native/create_dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 20:59:24.000000 femr-0.1.5/native/create_dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-04-26 20:59:24.000000 femr-0.1.5/native/create_survival_dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 20:59:24.000000 femr-0.1.5/native/create_survival_dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-26 20:59:24.000000 femr-0.1.5/native/csv.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-26 20:59:24.000000 femr-0.1.5/native/csv.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-26 20:59:24.000000 femr-0.1.5/native/csv_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    44062 2023-04-26 20:59:24.000000 femr-0.1.5/native/database.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-04-26 20:59:24.000000 femr-0.1.5/native/database.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-26 20:59:24.000000 femr-0.1.5/native/database_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-26 20:59:24.000000 femr-0.1.5/native/database_test_helper.cc
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 20:59:24.000000 femr-0.1.5/native/database_test_helper.hh
--rw-r--r--   0 runner    (1001) docker     (123)    49731 2023-04-26 20:59:24.000000 femr-0.1.5/native/dataloader_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 20:59:24.000000 femr-0.1.5/native/dataloader_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-04-26 20:59:24.000000 femr-0.1.5/native/datasets_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 20:59:24.000000 femr-0.1.5/native/datasets_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-26 20:59:24.000000 femr-0.1.5/native/dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-26 20:59:24.000000 femr-0.1.5/native/dictionary.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-26 20:59:24.000000 femr-0.1.5/native/dictionary_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-26 20:59:24.000000 femr-0.1.5/native/embedding_dot.cu
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-26 20:59:24.000000 femr-0.1.5/native/embedding_dot.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-26 20:59:24.000000 femr-0.1.5/native/exp_mean.cu
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-26 20:59:24.000000 femr-0.1.5/native/exp_mean.hh
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-26 20:59:24.000000 femr-0.1.5/native/extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-26 20:59:24.000000 femr-0.1.5/native/extension_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-26 20:59:24.000000 femr-0.1.5/native/filesystem_caster.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-26 20:59:24.000000 femr-0.1.5/native/flatmap.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-26 20:59:24.000000 femr-0.1.5/native/gather_scatter.cu
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 20:59:24.000000 femr-0.1.5/native/gather_scatter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-26 20:59:24.000000 femr-0.1.5/native/jax_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 20:59:24.000000 femr-0.1.5/native/jax_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-26 20:59:24.000000 femr-0.1.5/native/join_csvs.cc
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 20:59:24.000000 femr-0.1.5/native/join_csvs.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-26 20:59:24.000000 femr-0.1.5/native/join_csvs_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-04-26 20:59:24.000000 femr-0.1.5/native/local_attention.cu
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 20:59:24.000000 femr-0.1.5/native/local_attention.hh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 20:59:24.000000 femr-0.1.5/native/malloc_trim.hh
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-26 20:59:24.000000 femr-0.1.5/native/metrics_extension.cc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 20:59:24.000000 femr-0.1.5/native/metrics_extension.hh
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-26 20:59:24.000000 femr-0.1.5/native/npy.hh
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 20:59:24.000000 femr-0.1.5/native/parse_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 20:59:24.000000 femr-0.1.5/native/parse_utils.hh
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 20:59:24.000000 femr-0.1.5/native/prepare_all.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-26 20:59:24.000000 femr-0.1.5/native/prepare_notes_for_tokenization.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-26 20:59:24.000000 femr-0.1.5/native/register_iterable.hh
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 20:59:24.000000 femr-0.1.5/native/simple_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-26 20:59:24.000000 femr-0.1.5/native/stat_utils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-26 20:59:24.000000 femr-0.1.5/native/survival.hh
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-04-26 20:59:24.000000 femr-0.1.5/native/survival_metrics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 20:59:24.000000 femr-0.1.5/native/survival_metrics.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-26 20:59:24.000000 femr-0.1.5/native/survival_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-26 20:59:24.000000 femr-0.1.5/native/thread_utils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-26 20:59:24.000000 femr-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:59:35.878107 femr-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-26 20:59:24.000000 femr-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.846106 femr-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.862106 femr-0.1.5/src/femr/
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.866107 femr-0.1.5/src/femr/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/datasets/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/datasets/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.866107 femr-0.1.5/src/femr/etl_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/etl_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/etl_pipelines/omop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/etl_pipelines/sickkids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/etl_pipelines/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/etl_pipelines/stanford.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.866107 femr-0.1.5/src/femr/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/extension/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/extension/datasets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/extension/jax.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.866107 femr-0.1.5/src/femr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/extractors/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/extractors/omop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.870107 femr-0.1.5/src/femr/featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/featurizers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/featurizers/featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/featurizers/featurizers_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.870107 femr-0.1.5/src/femr/labelers/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/labelers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/labelers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24599 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/labelers/omop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/labelers/omop_inpatient_admissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/labelers/omop_lab_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.870107 femr-0.1.5/src/femr/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.870107 femr-0.1.5/src/femr/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/models/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/models/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/models/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.870107 femr-0.1.5/src/femr/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/transforms/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/transforms/sickkids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-26 20:59:24.000000 femr-0.1.5/src/femr/transforms/stanford.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.866107 femr-0.1.5/src/femr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 20:59:35.000000 femr-0.1.5/src/femr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.874107 femr-0.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.874107 femr-0.1.5/tests/featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-26 20:59:24.000000 femr-0.1.5/tests/featurizers/test_OnlineStatistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-04-26 20:59:24.000000 femr-0.1.5/tests/featurizers/test_featurizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.874107 femr-0.1.5/tests/labelers/
--rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_CodeLabelers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_InpatientAdmissionLabelers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_LabValueLabelers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_LabeledPatients.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_NLabelerPerPatient.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_OpioidOverdoseLabeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-26 20:59:24.000000 femr-0.1.5/tests/labelers/test_TimeHorizonEventLabeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-26 20:59:24.000000 femr-0.1.5/tests/test_csvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-26 20:59:24.000000 femr-0.1.5/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-26 20:59:24.000000 femr-0.1.5/tests/test_jax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 20:59:24.000000 femr-0.1.5/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-26 20:59:24.000000 femr-0.1.5/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-26 20:59:24.000000 femr-0.1.5/tests/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.846106 femr-0.1.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.874107 femr-0.1.5/tools/omop/
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-26 20:59:24.000000 femr-0.1.5/tools/omop/normalize_visit_detail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.874107 femr-0.1.5/tools/stanford/
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-26 20:59:24.000000 femr-0.1.5/tools/stanford/download_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-26 20:59:24.000000 femr-0.1.5/tools/stanford/flowsheet_cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:59:35.878107 femr-0.1.5/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/1_run_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/2_train_baseline_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/3_run_text_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/4_train_clmbr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/Simple FEMR Format.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-26 20:59:24.000000 femr-0.1.5/tutorials/mimic_etl_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.653302 femr-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 02:31:38.000000 femr-0.1.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.617301 femr-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.625301 femr-0.1.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 02:31:38.000000 femr-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 02:31:38.000000 femr-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.625301 femr-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-28 02:31:38.000000 femr-0.1.6/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-28 02:31:38.000000 femr-0.1.6/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 02:31:38.000000 femr-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 02:31:38.000000 femr-0.1.6/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 02:31:38.000000 femr-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-28 02:31:38.000000 femr-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-28 02:31:49.653302 femr-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-28 02:31:38.000000 femr-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 02:31:38.000000 femr-0.1.6/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.637301 femr-0.1.6/native/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-28 02:31:38.000000 femr-0.1.6/native/.bazelrc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 02:31:38.000000 femr-0.1.6/native/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 02:31:38.000000 femr-0.1.6/native/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-28 02:31:38.000000 femr-0.1.6/native/BUILD
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-28 02:31:38.000000 femr-0.1.6/native/WORKSPACE
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-28 02:31:38.000000 femr-0.1.6/native/backupbazelrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-28 02:31:38.000000 femr-0.1.6/native/civil_day_caster.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-28 02:31:38.000000 femr-0.1.6/native/clmbr_dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 02:31:38.000000 femr-0.1.6/native/compute_statistics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-28 02:31:38.000000 femr-0.1.6/native/constdb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 02:31:38.000000 femr-0.1.6/native/constdb.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-28 02:31:38.000000 femr-0.1.6/native/convert_dictionary_formats.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-28 02:31:38.000000 femr-0.1.6/native/count_codes_and_values.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 02:31:38.000000 femr-0.1.6/native/count_codes_and_values.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-28 02:31:38.000000 femr-0.1.6/native/count_codes_and_values_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-28 02:31:38.000000 femr-0.1.6/native/cpu_jax_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-04-28 02:31:38.000000 femr-0.1.6/native/create_dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-28 02:31:38.000000 femr-0.1.6/native/create_dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-04-28 02:31:38.000000 femr-0.1.6/native/create_survival_dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 02:31:38.000000 femr-0.1.6/native/create_survival_dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-28 02:31:38.000000 femr-0.1.6/native/csv.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-28 02:31:38.000000 femr-0.1.6/native/csv.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-28 02:31:38.000000 femr-0.1.6/native/csv_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    44062 2023-04-28 02:31:38.000000 femr-0.1.6/native/database.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-04-28 02:31:38.000000 femr-0.1.6/native/database.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-28 02:31:38.000000 femr-0.1.6/native/database_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-28 02:31:38.000000 femr-0.1.6/native/database_test_helper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-28 02:31:38.000000 femr-0.1.6/native/database_test_helper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    49731 2023-04-28 02:31:38.000000 femr-0.1.6/native/dataloader_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 02:31:38.000000 femr-0.1.6/native/dataloader_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-04-28 02:31:38.000000 femr-0.1.6/native/datasets_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 02:31:38.000000 femr-0.1.6/native/datasets_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-28 02:31:38.000000 femr-0.1.6/native/dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-28 02:31:38.000000 femr-0.1.6/native/dictionary.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-28 02:31:38.000000 femr-0.1.6/native/dictionary_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-28 02:31:38.000000 femr-0.1.6/native/embedding_dot.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-28 02:31:38.000000 femr-0.1.6/native/embedding_dot.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-28 02:31:38.000000 femr-0.1.6/native/exp_mean.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-28 02:31:38.000000 femr-0.1.6/native/exp_mean.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 02:31:38.000000 femr-0.1.6/native/extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-28 02:31:38.000000 femr-0.1.6/native/extension_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-28 02:31:38.000000 femr-0.1.6/native/filesystem_caster.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-28 02:31:38.000000 femr-0.1.6/native/flatmap.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-28 02:31:38.000000 femr-0.1.6/native/gather_scatter.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 02:31:38.000000 femr-0.1.6/native/gather_scatter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 02:31:38.000000 femr-0.1.6/native/jax_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 02:31:38.000000 femr-0.1.6/native/jax_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-28 02:31:38.000000 femr-0.1.6/native/join_csvs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 02:31:38.000000 femr-0.1.6/native/join_csvs.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-28 02:31:38.000000 femr-0.1.6/native/join_csvs_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-04-28 02:31:38.000000 femr-0.1.6/native/local_attention.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-28 02:31:38.000000 femr-0.1.6/native/local_attention.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 02:31:38.000000 femr-0.1.6/native/malloc_trim.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 02:31:38.000000 femr-0.1.6/native/metrics_extension.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 02:31:38.000000 femr-0.1.6/native/metrics_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-28 02:31:38.000000 femr-0.1.6/native/npy.hh
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 02:31:38.000000 femr-0.1.6/native/parse_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 02:31:38.000000 femr-0.1.6/native/parse_utils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-28 02:31:38.000000 femr-0.1.6/native/prepare_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-28 02:31:38.000000 femr-0.1.6/native/prepare_notes_for_tokenization.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-28 02:31:38.000000 femr-0.1.6/native/register_iterable.hh
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 02:31:38.000000 femr-0.1.6/native/simple_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-28 02:31:38.000000 femr-0.1.6/native/stat_utils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-28 02:31:38.000000 femr-0.1.6/native/survival.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-04-28 02:31:38.000000 femr-0.1.6/native/survival_metrics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 02:31:38.000000 femr-0.1.6/native/survival_metrics.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-28 02:31:38.000000 femr-0.1.6/native/survival_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 02:31:38.000000 femr-0.1.6/native/thread_utils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-28 02:31:38.000000 femr-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:31:49.653302 femr-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-28 02:31:38.000000 femr-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.617301 femr-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.637301 femr-0.1.6/src/femr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.641301 femr-0.1.6/src/femr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/datasets/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/datasets/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.641301 femr-0.1.6/src/femr/etl_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/etl_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/etl_pipelines/omop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/etl_pipelines/sickkids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/etl_pipelines/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/etl_pipelines/stanford.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.641301 femr-0.1.6/src/femr/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/extension/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/extension/datasets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/extension/jax.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.641301 femr-0.1.6/src/femr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/extractors/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/extractors/omop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.645301 femr-0.1.6/src/femr/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/featurizers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/featurizers/featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/featurizers/featurizers_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.645301 femr-0.1.6/src/femr/labelers/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/labelers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/labelers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/labelers/omop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/labelers/omop_inpatient_admissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/labelers/omop_lab_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.645301 femr-0.1.6/src/femr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.645301 femr-0.1.6/src/femr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/models/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/models/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/models/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.645301 femr-0.1.6/src/femr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/transforms/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/transforms/sickkids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-28 02:31:38.000000 femr-0.1.6/src/femr/transforms/stanford.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.641301 femr-0.1.6/src/femr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 02:31:49.000000 femr-0.1.6/src/femr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.649301 femr-0.1.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.649301 femr-0.1.6/tests/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-28 02:31:38.000000 femr-0.1.6/tests/featurizers/test_OnlineStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-04-28 02:31:38.000000 femr-0.1.6/tests/featurizers/test_featurizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.649301 femr-0.1.6/tests/labelers/
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_CodeLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_InpatientAdmissionLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_LabValueLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_LabeledPatients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_NLabelerPerPatient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_OpioidOverdoseLabeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-04-28 02:31:38.000000 femr-0.1.6/tests/labelers/test_TimeHorizonEventLabeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 02:31:38.000000 femr-0.1.6/tests/test_csvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-28 02:31:38.000000 femr-0.1.6/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-28 02:31:38.000000 femr-0.1.6/tests/test_jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-28 02:31:38.000000 femr-0.1.6/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-28 02:31:38.000000 femr-0.1.6/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-28 02:31:38.000000 femr-0.1.6/tests/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.621301 femr-0.1.6/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.649301 femr-0.1.6/tools/omop/
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-28 02:31:38.000000 femr-0.1.6/tools/omop/normalize_visit_detail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.649301 femr-0.1.6/tools/stanford/
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-28 02:31:38.000000 femr-0.1.6/tools/stanford/download_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-28 02:31:38.000000 femr-0.1.6/tools/stanford/flowsheet_cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:31:49.653302 femr-0.1.6/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/1_run_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/2_train_baseline_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/3_run_text_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/4_train_clmbr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/Simple FEMR Format.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-28 02:31:38.000000 femr-0.1.6/tutorials/mimic_etl_tutorial.py
```

### Comparing `femr-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `femr-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `femr-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/.github/workflows/build.yaml` & `femr-0.1.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/.github/workflows/tests.yaml` & `femr-0.1.6/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/.mypy.ini` & `femr-0.1.6/.mypy.ini`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/.pre-commit-config.yaml` & `femr-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/LICENSE` & `femr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/PKG-INFO` & `femr-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Framework for Electronic Medical Records. A python package for building models using EHR data.
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: models
 License-File: LICENSE
```

### Comparing `femr-0.1.5/README.md` & `femr-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/.bazelrc` & `femr-0.1.6/native/.bazelrc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/BUILD` & `femr-0.1.6/native/BUILD`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/WORKSPACE` & `femr-0.1.6/native/WORKSPACE`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/backupbazelrc` & `femr-0.1.6/native/backupbazelrc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/civil_day_caster.hh` & `femr-0.1.6/native/civil_day_caster.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/clmbr_dictionary.hh` & `femr-0.1.6/native/clmbr_dictionary.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/compute_statistics.cc` & `femr-0.1.6/native/compute_statistics.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/constdb.cc` & `femr-0.1.6/native/constdb.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/constdb.hh` & `femr-0.1.6/native/constdb.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/convert_dictionary_formats.cc` & `femr-0.1.6/native/convert_dictionary_formats.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/count_codes_and_values.cc` & `femr-0.1.6/native/count_codes_and_values.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/count_codes_and_values_test.cc` & `femr-0.1.6/native/count_codes_and_values_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/create_dictionary.cc` & `femr-0.1.6/native/create_dictionary.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/create_survival_dictionary.cc` & `femr-0.1.6/native/create_survival_dictionary.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/csv.cc` & `femr-0.1.6/native/csv.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/csv.hh` & `femr-0.1.6/native/csv.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/csv_test.cc` & `femr-0.1.6/native/csv_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/database.cc` & `femr-0.1.6/native/database.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/database.hh` & `femr-0.1.6/native/database.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/database_test.cc` & `femr-0.1.6/native/database_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/database_test_helper.cc` & `femr-0.1.6/native/database_test_helper.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/dataloader_extension.cc` & `femr-0.1.6/native/dataloader_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/datasets_extension.cc` & `femr-0.1.6/native/datasets_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/dictionary.cc` & `femr-0.1.6/native/dictionary.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/dictionary.hh` & `femr-0.1.6/native/dictionary.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/dictionary_test.cc` & `femr-0.1.6/native/dictionary_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/embedding_dot.cu` & `femr-0.1.6/native/embedding_dot.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/embedding_dot.hh` & `femr-0.1.6/native/embedding_dot.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/exp_mean.cu` & `femr-0.1.6/native/exp_mean.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/extension_test.py` & `femr-0.1.6/native/extension_test.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/filesystem_caster.hh` & `femr-0.1.6/native/filesystem_caster.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/flatmap.hh` & `femr-0.1.6/native/flatmap.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/gather_scatter.cu` & `femr-0.1.6/native/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/jax_extension.cc` & `femr-0.1.6/native/jax_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/join_csvs.cc` & `femr-0.1.6/native/join_csvs.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/join_csvs.hh` & `femr-0.1.6/native/join_csvs.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/join_csvs_test.cc` & `femr-0.1.6/native/join_csvs_test.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/local_attention.cu` & `femr-0.1.6/native/local_attention.cu`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/local_attention.hh` & `femr-0.1.6/native/local_attention.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/metrics_extension.cc` & `femr-0.1.6/native/metrics_extension.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/npy.hh` & `femr-0.1.6/native/npy.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/parse_utils.hh` & `femr-0.1.6/native/parse_utils.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/prepare_all.sh` & `femr-0.1.6/native/prepare_all.sh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/prepare_notes_for_tokenization.cc` & `femr-0.1.6/native/prepare_notes_for_tokenization.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/register_iterable.hh` & `femr-0.1.6/native/register_iterable.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/stat_utils.hh` & `femr-0.1.6/native/stat_utils.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/survival.hh` & `femr-0.1.6/native/survival.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/survival_metrics.cc` & `femr-0.1.6/native/survival_metrics.cc`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/survival_metrics.hh` & `femr-0.1.6/native/survival_metrics.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/native/survival_test.cc` & `femr-0.1.6/native/survival_test.cc`

 * *Files 1% similar despite different names*

```diff
@@ -18,26 +18,25 @@
     SurvivalCalculator calculator;
     calculator.preprocess_patient(example_patient, [](uint32_t code) {std::vector<uint32_t> result; result.push_back(code); return result;});
 
     auto res = calculator.get_times_for_event(0);
     EXPECT_EQ(res.first, 600);
     std::vector<std::pair<uint32_t, uint32_t>> expected = {{200, 10}, {400, 20}, {600, 30}};
     EXPECT_EQ(res.second, expected);
-    
+
     res = calculator.get_times_for_event(200);
     EXPECT_EQ(res.first, 400);
     expected = {{200, 20}, {400, 30}};
     EXPECT_EQ(res.second, expected);
 
     calculator.preprocess_patient(example_patient, [](uint32_t code) {std::vector<uint32_t> result; result.push_back(code); return result;}, 500);
 
     res = calculator.get_times_for_event(0);
     EXPECT_EQ(res.first, 500);
     expected = {{200, 10}, {400, 20}};
     EXPECT_EQ(res.second, expected);
-    
+
     res = calculator.get_times_for_event(200);
     EXPECT_EQ(res.first, 300);
     expected = {{200, 20}};
     EXPECT_EQ(res.second, expected);
 }
-
```

### Comparing `femr-0.1.5/native/thread_utils.hh` & `femr-0.1.6/native/thread_utils.hh`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/pyproject.toml` & `femr-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "tqdm >= 4.60.0",
     "zstandard >= 0.18",
     "icecream == 2.1.3",
     "nptyping == 2.4.1",
     "msgpack >= 1.0.5",
 ]
 requires-python=">3.9"
-version = "0.1.5"
+version = "0.1.6"
 
 [project.scripts]
 
 etl_stanford_omop = "femr.etl_pipelines.stanford:etl_starr_omop_program"
 etl_generic_omop = "femr.etl_pipelines.omop:etl_generic_omop_program"
 etl_simple_femr = "femr.etl_pipelines.simple:etl_simple_femr_program"
 etl_sickkids_omop = "femr.etl_pipelines.sickkids:etl_sk_omop_program"
```

### Comparing `femr-0.1.5/setup.py` & `femr-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,21 @@
                 extra_args.extend(["--macos_minimum_os", source_env["MACOSX_DEPLOYMENT_TARGET"]])
 
             if not can_build_simple(sourcedir=ext.sourcedir, env=env, bazel_extra_args=bazel_extra_args):
                 bazel_extra_args.extend(["--noworkspace_rc", "--bazelrc=backupbazelrc"])
                 assert can_build_simple(
                     sourcedir=ext.sourcedir, env=env, bazel_extra_args=bazel_extra_args
                 ), "Cannot build C++ extension"
+            
+            subprocess.run(
+                args=["bazel", "clean", "--expunge"],
+                cwd=ext.sourcedir,
+                env=env,
+                check=True,
+            )
 
             subprocess.run(
                 args=["bazel"] + bazel_extra_args + ["build", "-c", "opt", ext.target] + extra_args,
                 cwd=ext.sourcedir,
                 env=env,
                 check=True,
             )
```

### Comparing `femr-0.1.5/src/femr/__init__.py` & `femr-0.1.6/src/femr/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/datasets/__init__.py` & `femr-0.1.6/src/femr/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/datasets/fileio.py` & `femr-0.1.6/src/femr/datasets/fileio.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/datasets/types.py` & `femr-0.1.6/src/femr/datasets/types.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/etl_pipelines/omop.py` & `femr-0.1.6/src/femr/etl_pipelines/omop.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/etl_pipelines/sickkids.py` & `femr-0.1.6/src/femr/etl_pipelines/sickkids.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/etl_pipelines/simple.py` & `femr-0.1.6/src/femr/etl_pipelines/simple.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/etl_pipelines/stanford.py` & `femr-0.1.6/src/femr/etl_pipelines/stanford.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/extension/datasets.pyi` & `femr-0.1.6/src/femr/extension/datasets.pyi`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/extractors/csv.py` & `femr-0.1.6/src/femr/extractors/csv.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/extractors/omop.py` & `femr-0.1.6/src/femr/extractors/omop.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/featurizers/__init__.py` & `femr-0.1.6/src/femr/featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/featurizers/core.py` & `femr-0.1.6/src/femr/featurizers/core.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/featurizers/featurizers.py` & `femr-0.1.6/src/femr/featurizers/featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/featurizers/featurizers_notes.py` & `femr-0.1.6/src/femr/featurizers/featurizers_notes.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/jax.py` & `femr-0.1.6/src/femr/jax.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/labelers/core.py` & `femr-0.1.6/src/femr/labelers/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,17 +552,17 @@
         return n_labels
 
     def get_labeler_type(self) -> LabelType:
         return self.labeler.get_labeler_type()
 
 
 def compute_random_num(seed: int, num_1: int, num_2: int):
-    network_num_1 = struct.pack("!I", num_1)
-    network_num_2 = struct.pack("!I", num_2)
-    network_seed = struct.pack("!I", seed)
+    network_num_1 = struct.pack("!q", num_1)
+    network_num_2 = struct.pack("!q", num_2)
+    network_seed = struct.pack("!q", seed)
 
     to_hash = network_seed + network_num_1 + network_num_2
 
     hash_object = hashlib.sha256()
     hash_object.update(to_hash)
     hash_value = hash_object.digest()
```

### Comparing `femr-0.1.5/src/femr/labelers/omop.py` & `femr-0.1.6/src/femr/labelers/omop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Labeling functions for OMOP data."""
 from __future__ import annotations
 
 import datetime
+import warnings
 from abc import abstractmethod
 from collections import deque
 from typing import Any, Callable, List, Optional, Set, Tuple
 
 from .. import Event, Patient
 from ..extension import datasets as extension_datasets
 from .core import Label, Labeler, LabelType, TimeHorizon, TimeHorizonEventLabeler
@@ -109,15 +110,15 @@
     codes: Set[str] = set()
     for omop_concept_code in omop_concept_codes:
         try:
             codes.update(
                 _get_all_children(ontology, omop_concept_code) if is_ontology_expansion else {omop_concept_code}
             )
         except IndexError:
-            raise ValueError(f"OMOP Concept Code {omop_concept_code} not found in ontology.")
+            warnings.warn(f"OMOP Concept Code {omop_concept_code} not found in ontology.")
     return codes
 
 
 # TODO - move this into the ontology class
 def _get_all_children(ontology: extension_datasets.Ontology, code: str) -> Set[str]:
     children_code_set = set([code])
     parent_deque = deque([code])
```

### Comparing `femr-0.1.5/src/femr/labelers/omop_inpatient_admissions.py` & `femr-0.1.6/src/femr/labelers/omop_inpatient_admissions.py`

 * *Files 19% similar despite different names*

```diff
@@ -105,17 +105,25 @@
         for admission_time, __ in get_inpatient_admission_discharge_times(patient, self.ontology):
             times.append(admission_time)
         return times
 
     def get_prediction_times(self, patient: Patient) -> List[datetime.datetime]:
         """Return end of admission as prediction timm."""
         times: List[datetime.datetime] = []
-        for __, discharge_time in get_inpatient_admission_discharge_times(patient, self.ontology):
+        prev_discharge_date: datetime.date = datetime.date(1900, 1, 1)
+
+        for admission_time, discharge_time in get_inpatient_admission_discharge_times(patient, self.ontology):
             prediction_time: datetime.datetime = self.prediction_time_adjustment_func(discharge_time)
+
+            # Ignore patients who are readmitted the same day they were discharged b/c of data leakage
+            if admission_time.date() <= prev_discharge_date:
+                continue
+
             times.append(prediction_time)
+            prev_discharge_date = discharge_time.date()
         times = sorted(list(set(times)))
         return times
 
     def get_time_horizon(self) -> TimeHorizon:
         return self.time_horizon
 
 
@@ -139,19 +147,36 @@
         prediction_time_adjustment_func: Callable = move_datetime_to_end_of_day,
     ):
         self.ontology: extension_datasets.Ontology = ontology
         self.long_time: datetime.timedelta = long_time
         self.prediction_time_adjustment_func = prediction_time_adjustment_func
 
     def label(self, patient: Patient) -> List[Label]:
-        """Label all admissions with admission length > `self.long_time`"""
+        """
+        Label all admissions with admission length > `self.long_time`
+        Exclude admission if time of discharge or death < prediction time
+        """
         labels: List[Label] = []
         for admission_time, discharge_time in get_inpatient_admission_discharge_times(patient, self.ontology):
             is_long_admission: bool = (discharge_time - admission_time) >= self.long_time
             prediction_time: datetime.datetime = self.prediction_time_adjustment_func(admission_time)
+
+            # exclude if discharge or death occurred before prediction time
+            death_concepts: Set[str] = map_omop_concept_codes_to_femr_codes(self.ontology, get_death_concepts())
+            death_times: List[datetime.datetime] = []
+            for e in patient.events:
+                if e.code in death_concepts:
+                    death_times.append(e.start)
+
+            if prediction_time > discharge_time:
+                continue
+
+            if death_times and prediction_time > min(death_times):
+                continue
+
             labels.append(Label(prediction_time, is_long_admission))
         return labels
 
     def get_labeler_type(self) -> LabelType:
         return "boolean"
 
 
@@ -181,7 +206,50 @@
     def get_outcome_times(self, patient: Patient) -> List[datetime.datetime]:
         """Return time of any event with a code in `self.outcome_codes`."""
         times: List[datetime.datetime] = []
         for e in patient.events:
             if e.code in self.outcome_codes:
                 times.append(e.start)
         return times
+
+    def label(self, patient: Patient) -> List[Label]:
+        """
+        Label all inpatient mortality with prediction_time <= death_time <= discharge
+        Exclude admission if time of discharge or death < prediction time
+        """
+        visits: List[Event] = self.get_visit_events(patient)
+        prediction_start_times: List[datetime.datetime] = [
+            self.visit_start_adjust_func(visit.start) for visit in visits
+        ]
+        prediction_end_times: List[datetime.datetime] = [self.visit_end_adjust_func(visit.end) for visit in visits]
+        outcome_times: List[datetime.datetime] = self.get_outcome_times(patient)
+        death_time = min(outcome_times) if outcome_times else None
+        results: List[Label] = []
+
+        # For each visit, check if there is an outcome which occurs within the (start, end) of the visit
+        for prediction_start, prediction_end in zip(prediction_start_times, prediction_end_times):
+            # exclude if prediction time > discharge time
+            if prediction_start >= prediction_end:
+                continue
+
+            # exclude if deathtime > discharge time
+            if death_time is not None and prediction_start > death_time:
+                continue
+
+            # TRUE if an event occurs within the visit
+            is_outcome_occurs_in_time_horizon: bool = (
+                death_time is not None
+                and (
+                    # outcome occurs after visit starts
+                    prediction_start
+                    <= death_time
+                )
+                and (
+                    # outcome occurs before visit ends
+                    death_time
+                    <= prediction_end
+                )
+            )
+
+            results.append(Label(time=prediction_start, value=is_outcome_occurs_in_time_horizon))
+
+        return results
```

### Comparing `femr-0.1.5/src/femr/labelers/omop_lab_values.py` & `femr-0.1.6/src/femr/labelers/omop_lab_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 class ThrombocytopeniaLabValueLabeler(InpatientLabValueLabeler):
     """lab-based definition for thrombocytopenia based on platelet count (10^9/L).
     Thresholds: mild (<150), moderate(<100), severe(<50), and reference range."""
 
     original_omop_concept_codes = [
         "LOINC/LP393218-5",
         "LOINC/LG32892-8",
+        "LOINC/777-3",
     ]
 
     def value_to_label(self, raw_value: str, unit: Optional[str]) -> str:
         if raw_value.lower() in ["normal", "adequate"]:
             return "normal"
         value = float(raw_value)
         if value < 50:
@@ -158,14 +159,16 @@
     """lab-based definition for hyperkalemia using blood potassium concentration (mmol/L).
     Thresholds: mild(>5.5),moderate(>6),severe(>7), and abnormal range."""
 
     original_omop_concept_codes = [
         "LOINC/LG7931-1",
         "LOINC/LP386618-5",
         "LOINC/LG10990-6",
+        "LOINC/6298-4",
+        "LOINC/2823-3",
     ]
 
     def value_to_label(self, raw_value: str, unit: Optional[str]) -> str:
         if raw_value.lower() in ["normal", "adequate"]:
             return "normal"
         value = float(raw_value)
         if unit is not None:
@@ -198,14 +201,16 @@
 class HypoglycemiaLabValueLabeler(InpatientLabValueLabeler):
     """lab-based definition for hypoglycemia using blood glucose concentration (mmol/L).
     Thresholds: mild(<3), moderate(<3.5), severe(<=3.9), and abnormal range."""
 
     original_omop_concept_codes = [
         "SNOMED/33747003",
         "LOINC/LP416145-3",
+        "LOINC/14749-6",
+        "LOINC/15074-8",
     ]
 
     def value_to_label(self, raw_value: str, unit: Optional[str]) -> str:
         if raw_value.lower() in ["normal", "adequate"]:
             return "normal"
         value = float(raw_value)
         if unit is not None:
@@ -231,17 +236,15 @@
         return "normal"
 
 
 class HyponatremiaLabValueLabeler(InpatientLabValueLabeler):
     """lab-based definition for hyponatremia based on blood sodium concentration (mmol/L).
     Thresholds: mild (<=135),moderate(<130),severe(<125), and abnormal range."""
 
-    original_omop_concept_codes = [
-        "LOINC/LG11363-5",
-    ]
+    original_omop_concept_codes = ["LOINC/LG11363-5", "LOINC/2951-2", "LOINC/2947-0"]
 
     def value_to_label(self, raw_value: str, unit: Optional[str]) -> str:
         if raw_value.lower() in ["normal", "adequate"]:
             return "normal"
         value = float(raw_value)
         if value < 125:
             return "severe"
@@ -272,14 +275,16 @@
                 # NOTE: This weird *10 / 100 is how Lawrence did it
                 value = value * 10
             elif unit.startswith("mg/dl"):
                 # mg / dL (divide by 1000 to get g/dL)
                 # Original OMOP concept ID: 8840
                 # NOTE: This weird *10 / 100 is how Lawrence did it
                 value = value / 100
+            elif unit.startswith("g/l"):
+                value = value
             else:
                 raise ValueError(f"Unknown unit: {unit}")
         else:
             raise ValueError(f"Unknown unit: {unit}")
         if value < 70:
             return "severe"
         elif value < 110:
```

### Comparing `femr-0.1.5/src/femr/models/dataloader.py` & `femr-0.1.6/src/femr/models/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import argparse
 import datetime
 import logging
+import math
 import os
 import pickle
 import queue
 import random
 import threading
 from typing import Any, List, Optional, Tuple, TypeVar
 
 import jax
-import math
 import msgpack
 import numpy as np
 
 import femr.datasets
 import femr.extension.dataloader
 
 T = TypeVar("T")
@@ -169,28 +169,40 @@
     parser.add_argument(
         "--clmbr_survival_dictionary_path", type=str, help="The survival clmbr dictionary if running that task"
     )
     parser.add_argument("--labeled_patients_path", type=str, help="The labeled patients")
     parser.add_argument(
         "--is_hierarchical", default=False, action="store_true", help="Whether to use hierarchical embeddings"
     )
+    parser.add_argument("--seed", default=97, type=int, help="The random seed used for data splitting")
     parser.add_argument(
-        "--seed", default=97, type=int, help="The random seed used for data splitting"
+        "--val_start",
+        default=70,
+        type=int,
+        help="The start of the validation split (and thus end of the train split)",
     )
     parser.add_argument(
-        "--val_start", default=70, type=int, help="The start of the validation split (and thus end of the train split)",
+        "--test_start",
+        default=85,
+        type=int,
+        help="The start of the test split (and thus end of the val split)",
     )
     parser.add_argument(
-        "--test_start", default=85, type=int, help="The start of the test split (and thus end of the val split)",
+        "--batch_size",
+        default=int(1 << 14),
+        type=int,
+        help="The batch size (in events). Must be a power of two",
     )
+    parser.add_argument("--note_embedding_data", default=None, type=str, help="Note embedding data when using notes")
     parser.add_argument(
-        "--batch_size", default=int(1 << 14), type=int, help="The batch size (in events). Must be a power of two",
+        "--limit_to_patients_file",
+        default=None,
+        type=str,
+        help="A file containing the only patient_ids to allow in batches",
     )
-    parser.add_argument("--note_embedding_data", default=None, type=str, help="Note embedding data when using notes")
-    parser.add_argument("--limit_to_patients_file", default=None, type=str, help="A file containing the only patient_ids to allow in batches")
     parser.add_argument("--limit_before_date", default=None, type=str, help="Limit the batches to before a given date")
 
     args = parser.parse_args()
 
     os.mkdir(args.directory)
 
     logFormatter = logging.Formatter("%(asctime)s [%(threadName)-12.12s] [%(levelname)-5.5s]  %(message)s")
@@ -282,15 +294,14 @@
             ids_to_limit = [int(a) for a in f]
         task["patient_ids"] = ids_to_limit
 
     if args.limit_before_date:
         limit_date = datetime.date.fromisoformat(args.limit_before_date)
         task["limit_date"] = limit_date.isoformat()
 
-    
     max_size = math.log2(args.batch_size)
     assert int(max_size) == max_size, "Batch size must be a power of two"
     max_size = int(max_size)
 
     loader_config: Any = {
         "transformer": {
             "vocab_size": args.transformer_vocab_size,
```

### Comparing `femr-0.1.5/src/femr/models/scripts.py` & `femr-0.1.6/src/femr/models/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,20 +60,20 @@
     parser.add_argument("--clmbr_survival_dim", type=int)
     parser.add_argument("--num_batch_threads", type=int)
     parser.add_argument("--start_from_checkpoint", type=str)
     parser.add_argument("--freeze_weights", default=False, action="store_true")
     parser.add_argument("--token_dropout", type=float, default=0)
     parser.add_argument("--internal_dropout", type=float, default=0)
     parser.add_argument("--weight_decay", type=float, default=0)
-    parser.add_argument("--max_iter", type=float, default=None)
-    parser.add_argument("--hidden_size", type=float, default=768, help="Transformer hidden size")
-    parser.add_argument("--intermediate_size", type=float, default=3072, help="Transformer intermediate layer size")
-    parser.add_argument("--n_heads", type=float, default=12, help="Transformer # of heads")
-    parser.add_argument("--n_layers", type=float, default=6, help="Transformer # of layers")
-    parser.add_argument("--attention_width", type=float, default=512, help="Transformer attention width.")
+    parser.add_argument("--max_iter", type=int, default=None)
+    parser.add_argument("--hidden_size", type=int, default=768, help="Transformer hidden size")
+    parser.add_argument("--intermediate_size", type=int, default=3072, help="Transformer intermediate layer size")
+    parser.add_argument("--n_heads", type=int, default=12, help="Transformer # of heads")
+    parser.add_argument("--n_layers", type=int, default=6, help="Transformer # of layers")
+    parser.add_argument("--attention_width", type=int, default=512, help="Transformer attention width.")
 
     parser.add_argument(
         "--early_stopping_window_steps",
         type=int,
         default=None,
         help="If we don't see a decrease in dev loss in this many steps, stop training. A reasonable value is 15000.",
     )
```

### Comparing `femr-0.1.5/src/femr/models/transformer.py` & `femr-0.1.6/src/femr/models/transformer.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/transforms/__init__.py` & `femr-0.1.6/src/femr/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/transforms/notes.py` & `femr-0.1.6/src/femr/transforms/notes.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/transforms/sickkids.py` & `femr-0.1.6/src/femr/transforms/sickkids.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr/transforms/stanford.py` & `femr-0.1.6/src/femr/transforms/stanford.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr.egg-info/PKG-INFO` & `femr-0.1.6/src/femr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Framework for Electronic Medical Records. A python package for building models using EHR data.
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: models
 License-File: LICENSE
```

### Comparing `femr-0.1.5/src/femr.egg-info/SOURCES.txt` & `femr-0.1.6/src/femr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/src/femr.egg-info/entry_points.txt` & `femr-0.1.6/src/femr.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/featurizers/test_OnlineStatistics.py` & `femr-0.1.6/tests/featurizers/test_OnlineStatistics.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/featurizers/test_featurizers.py` & `femr-0.1.6/tests/featurizers/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/labelers/test_CodeLabelers.py` & `femr-0.1.6/tests/labelers/test_CodeLabelers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/labelers/test_InpatientAdmissionLabelers.py` & `femr-0.1.6/tests/labelers/test_InpatientAdmissionLabelers.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,49 +308,39 @@
             return ["DEATH_CHILD"]
         return []
 
 
 def test_mortality(tmp_path: pathlib.Path):
     ontology = DummyMortalityOntology()
     labeler = InpatientMortalityLabeler(ontology)  # type: ignore
-    events_with_labels: EventsWithLabels = [
-        # fmt: off
-        #
-        # test different outcome codes
-        (event((2001, 1, 1), "Visit/IP", end=datetime.datetime(2001, 1, 11), omop_table='visit_occurrence'), True),  # admission
-        (event((2001, 1, 10), "Death Type/OMOP generated"), "skip"),  # event
-        (event((2002, 1, 1), "Visit/IP", end=datetime.datetime(2002, 1, 11), omop_table='visit_occurrence'), True),  # admission
-        (event((2002, 1, 10), "DEATH_CHILD"), "skip"),  # event
-        (event((2003, 1, 1), "Visit/IP", end=datetime.datetime(2003, 1, 11), omop_table='visit_occurrence'), True),  # admission
-        (event((2003, 1, 10), "Condition Type/OMOP4822053"), "skip"),  # event
-        #
-        # not outcome
-        (event((2004, 1, 1), "Visit/IP", end=datetime.datetime(2004, 1, 10), omop_table='visit_occurrence'), False),  # admission
-        (event((2004, 1, 9), 0), "skip"),
-        #
-        # outcome outside of visit
-        (event((2005, 1, 30), "Visit/IP", end=datetime.datetime(2005, 2, 10), omop_table='visit_occurrence'), False),  # admission
-        (event((2005, 2, 10, 1), "Death Type/OMOP generated"), "skip"),
-        (event((2006, 1, 30), "Visit/IP", end=datetime.datetime(2006, 2, 10), omop_table='visit_occurrence'), False),  # admission
-        (event((2006, 1, 29, 1), "Death Type/OMOP generated"), "skip"),
-        #
-        # NOTE: No censoring since we have the end of the admission
-        (event((2006, 1, 2), "Visit/IP", end=datetime.datetime(2006, 5, 10), omop_table='visit_occurrence'), False),
-        # fmt: on
-    ]
-    assert labeler.outcome_codes == {"Condition Type/OMOP4822053", "Death Type/OMOP generated", "DEATH_CHILD"}
-    true_prediction_times: List[datetime.datetime] = [
-        move_datetime_to_end_of_day(x[0].start) for x in events_with_labels if isinstance(x[1], bool) or x[1] is None
-    ]
-    run_test_for_labeler(
-        labeler,
-        events_with_labels,
-        true_prediction_times=true_prediction_times,
-        help_text="test_mortality",
-    )
+    for outcome_code in ["Death Type/OMOP generated", "DEATH_CHILD", "Condition Type/OMOP4822053"]:
+        events_with_labels: EventsWithLabels = [
+            # fmt: off
+            #
+            # test different outcome codes
+            (event((2000, 1, 1), "Visit/IP", end=datetime.datetime(2000, 1, 1), omop_table='visit_occurrence'), "skip"),  # admission
+            (event((2001, 1, 1), "Visit/IP", end=datetime.datetime(2001, 1, 11), omop_table='visit_occurrence'), False),  # admission
+            (event((2002, 1, 1), "Visit/IP", end=datetime.datetime(2002, 1, 11), omop_table='visit_occurrence'), True),  # admission
+            (event((2002, 1, 10), outcome_code), "skip"),  # event
+            (event((2003, 1, 1), "Visit/IP", end=datetime.datetime(2003, 1, 11), omop_table='visit_occurrence'), "skip"),
+            # admission
+            # fmt: on
+        ]
+        assert labeler.outcome_codes == {"Condition Type/OMOP4822053", "Death Type/OMOP generated", "DEATH_CHILD"}
+        true_prediction_times: List[datetime.datetime] = [
+            move_datetime_to_end_of_day(x[0].start)
+            for x in events_with_labels
+            if isinstance(x[1], bool) or x[1] is None
+        ]
+        run_test_for_labeler(
+            labeler,
+            events_with_labels,
+            true_prediction_times=true_prediction_times,
+            help_text="test_mortality",
+        )
 
 
 #############################################
 #############################################
 #
 # Long Length of Stay Labeler
 #
```

### Comparing `femr-0.1.5/tests/labelers/test_LabValueLabelers.py` & `femr-0.1.6/tests/labelers/test_LabValueLabelers.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             return ["child_1"]
         elif parent_code == self.new_codes[1]:
             return ["child_2"]
         return []
 
 
 def test_thrombocytopenia(tmp_path: pathlib.Path):
-    outcome_codes = {"child_1", "child_1_1", "LOINC/LP393218-5", "LOINC/LG32892-8", "child_2"}
+    outcome_codes = {"child_1", "child_1_1", "LOINC/LP393218-5", "LOINC/LG32892-8", "child_2", "LOINC/777-3"}
     labeler = _create_specific_labvalue_labeler(
         ThrombocytopeniaLabValueLabeler,
         "severe",
         outcome_codes,
     )
 
     # Test value parsing
@@ -340,15 +340,24 @@
         [(130, "g/L"), (145.123, "g/L")],
         [(200, "g/L"), (400.1, "g/L")],
         "test_thrombocytopenia",
     )
 
 
 def test_hyperkalemia(tmp_path: pathlib.Path):
-    outcome_codes = {"child_1_1", "child_2", "child_1", "LOINC/LP386618-5", "LOINC/LG10990-6", "LOINC/LG7931-1"}
+    outcome_codes = {
+        "child_1_1",
+        "child_2",
+        "child_1",
+        "LOINC/LP386618-5",
+        "LOINC/LG10990-6",
+        "LOINC/LG7931-1",
+        "LOINC/6298-4",
+        "LOINC/2823-3",
+    }
     labeler = _create_specific_labvalue_labeler(
         HyperkalemiaLabValueLabeler,
         "severe",
         outcome_codes,
     )
 
     # Test value parsing
@@ -363,15 +372,23 @@
         [(5.6, "mEq/L"), (5.99, "mmol/L")],
         [(0, "mEq/L"), (4 * 18, "mg/dL")],
         "test_hyperkalemia",
     )
 
 
 def test_hypoglycemia(tmp_path: pathlib.Path):
-    outcome_codes = {"child_2", "child_1_1", "SNOMED/33747003", "LOINC/LP416145-3", "child_1"}
+    outcome_codes = {
+        "child_2",
+        "child_1_1",
+        "SNOMED/33747003",
+        "LOINC/LP416145-3",
+        "child_1",
+        "LOINC/14749-6",
+        "LOINC/15074-8",
+    }
     labeler = _create_specific_labvalue_labeler(
         HypoglycemiaLabValueLabeler,
         "severe",
         outcome_codes,
     )
 
     # Test value parsing
@@ -386,15 +403,15 @@
         [(3.51, "mmol/L"), (3.7, "mmol/L")],
         [(10, "mmol/L"), (3.99 * 18, "mg/dL")],
         "test_hypoglycemia",
     )
 
 
 def test_hyponatremia(tmp_path: pathlib.Path):
-    outcome_codes = {"child_1", "child_1_1", "LOINC/LG11363-5"}
+    outcome_codes = {"child_1", "child_1_1", "child_2", "LOINC/LG11363-5", "LOINC/2951-2", "LOINC/2947-0"}
     labeler = _create_specific_labvalue_labeler(
         HyponatremiaLabValueLabeler,
         "severe",
         outcome_codes,
     )
 
     # Test value parsing
```

### Comparing `femr-0.1.5/tests/labelers/test_LabeledPatients.py` & `femr-0.1.6/tests/labelers/test_LabeledPatients.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/labelers/test_NLabelerPerPatient.py` & `femr-0.1.6/tests/labelers/test_NLabelerPerPatient.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/labelers/test_OpioidOverdoseLabeler.py` & `femr-0.1.6/tests/labelers/test_OpioidOverdoseLabeler.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/labelers/test_TimeHorizonEventLabeler.py` & `femr-0.1.6/tests/labelers/test_TimeHorizonEventLabeler.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/test_csvs.py` & `femr-0.1.6/tests/test_csvs.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/test_datasets.py` & `femr-0.1.6/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/test_jax.py` & `femr-0.1.6/tests/test_jax.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/test_metrics.py` & `femr-0.1.6/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/test_transforms.py` & `femr-0.1.6/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tests/tools.py` & `femr-0.1.6/tests/tools.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tools/omop/normalize_visit_detail.py` & `femr-0.1.6/tools/omop/normalize_visit_detail.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tools/stanford/download_bigquery.py` & `femr-0.1.6/tools/stanford/download_bigquery.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tools/stanford/flowsheet_cleaner.py` & `femr-0.1.6/tools/stanford/flowsheet_cleaner.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb` & `femr-0.1.6/tutorials/0_Fundamental FEMR Schema, Patients And Events.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/1_run_featurizers.py` & `femr-0.1.6/tutorials/1_run_featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/2_train_baseline_models.py` & `femr-0.1.6/tutorials/2_train_baseline_models.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/3_run_text_featurizer.py` & `femr-0.1.6/tutorials/3_run_text_featurizer.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/4_train_clmbr_model.py` & `femr-0.1.6/tutorials/4_train_clmbr_model.py`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/Simple FEMR Format.ipynb` & `femr-0.1.6/tutorials/Simple FEMR Format.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.1.5/tutorials/mimic_etl_tutorial.py` & `femr-0.1.6/tutorials/mimic_etl_tutorial.py`

 * *Files identical despite different names*

