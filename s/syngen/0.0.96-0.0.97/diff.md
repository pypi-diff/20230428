# Comparing `tmp/syngen-0.0.96.tar.gz` & `tmp/syngen-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.96.tar", last modified: Tue Apr 25 15:53:52 2023, max compression
+gzip compressed data, was "syngen-0.0.97.tar", last modified: Fri Apr 28 13:33:01 2023, max compression
```

## Comparing `syngen-0.0.96.tar` & `syngen-0.0.97.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-25 15:52:30.000000 syngen-0.0.96/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-25 15:52:30.000000 syngen-0.0.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-25 15:52:30.000000 syngen-0.0.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-25 15:53:52.656111 syngen-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-25 15:52:30.000000 syngen-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-25 15:52:30.000000 syngen-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-25 15:53:52.660111 syngen-0.0.96/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.632110 syngen-0.0.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.640111 syngen-0.0.96/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10053 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7274 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.648111 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.636110 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.648111 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.648111 syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.652111 syngen-0.0.96/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    30208 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.656111 syngen-0.0.96/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-25 15:52:30.000000 syngen-0.0.96/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:53:52.644111 syngen-0.0.96/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-25 15:53:52.000000 syngen-0.0.96/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.838267 syngen-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-28 13:31:35.000000 syngen-0.0.97/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-28 13:31:35.000000 syngen-0.0.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-28 13:31:35.000000 syngen-0.0.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-28 13:33:01.838267 syngen-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-28 13:31:35.000000 syngen-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-28 13:31:35.000000 syngen-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-28 13:33:01.838267 syngen-0.0.97/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.814267 syngen-0.0.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.818267 syngen-0.0.97/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10053 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7274 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.826267 syngen-0.0.97/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.826267 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.814267 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.826267 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30208 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11543 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.838267 syngen-0.0.97/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.96/LICENSE` & `syngen-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/PKG-INFO` & `syngen-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.96
+Version: 0.0.97
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.96 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.97 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.96/README.md` & `syngen-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/setup.cfg` & `syngen-0.0.97/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/infer.py` & `syngen-0.0.97/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/config/configurations.py` & `syngen-0.0.97/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/convertor/convertor.py` & `syngen-0.0.97/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.0.97/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/__init__.py` & `syngen-0.0.97/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/metrics/utils.py` & `syngen-0.0.97/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.97/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/strategies/strategies.py` & `syngen-0.0.97/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.0.97/src/syngen/ml/train_chain/train_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 import dill
 from scipy.stats import gaussian_kde
 from collections import OrderedDict
 from tensorflow.keras.preprocessing.text import Tokenizer
 
 from syngen.ml.vae import *
 from syngen.ml.data_loaders import DataLoader
-from syngen.ml.utils import slugify_parameters, fetch_dataset
+from syngen.ml.utils import (
+    slugify_parameters,
+    fetch_dataset,
+    check_if_features_assigned
+)
 
 
 class AbstractHandler(ABC):
     @abstractmethod
     def set_next(self, handler):
         pass
 
@@ -162,23 +166,22 @@
 
         logger.debug(
             f"Train model with parameters: epochs={self.epochs}, row_subset={self.row_subset}, "
             f"drop_null={self.drop_null}, batch_size={self.batch_size}")
 
         self.model.prepare_dataset()
 
-        features = fetch_dataset(self.paths["dataset_pickle_path"]).features
-        if len(features) == 0:
-            logger.info("No features to train VAE on")
-            return
         self.model.fit_on_df(
             data,
             epochs=self.epochs,
         )
 
+        if not check_if_features_assigned(self.paths["dataset_pickle_path"]):
+            return
+
         self.model.save_state(self.paths["state_path"])
         logger.info("Finished VAE training")
 
     def handle(self, data: pd.DataFrame, **kwargs):
         self.__fit_model(data)
         return super().handle(data, **kwargs)
```

### Comparing `syngen-0.0.96/src/syngen/ml/utils/utils.py` & `syngen-0.0.97/src/syngen/ml/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dateutil.parser import parse
 import pickle
 from datetime import datetime, timedelta
 
 import pandas as pd
 import numpy as np
 from slugify import slugify
+from loguru import logger
 
 
 def get_date_columns(df: pd.DataFrame, str_columns: List[str]):
     # TODO: extend pattern to more formats
     # pattern = r'\d{2}(\.|/|\-)\d{2}(\.|/|\-)(\d{2}|\d{4})'
     # pattern = r"\s{0,1}\d+[-/\\:]\s{0,1}\d+[-/\\:]\s{0,1}\d+"
 
@@ -172,7 +173,18 @@
     Convert timestamp to datetime
     """
     timestamp = int(timestamp * 1e-9)
     if timestamp < 0:
         return datetime(1970, 1, 1) + timedelta(seconds=timestamp)
     else:
         return datetime.utcfromtimestamp(timestamp)
+
+
+def check_if_features_assigned(dataset_pickle_path: str):
+    """
+    Check if features are assigned in the dataset
+    """
+    features = fetch_dataset(dataset_pickle_path).features
+    if len(features) == 0:
+        logger.info("No features to train VAE on")
+        return False
+    return True
```

### Comparing `syngen-0.0.96/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.97/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/vae/models/dataset.py` & `syngen-0.0.97/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/vae/models/features.py` & `syngen-0.0.97/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/vae/models/model.py` & `syngen-0.0.97/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.97/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import tqdm
 from loguru import logger
 import pandas as pd
 import numpy as np
 
 from syngen.ml.vae.models.model import CVAE
 from syngen.ml.vae.models import Dataset
-from syngen.ml.utils import fetch_dataset
+from syngen.ml.utils import (
+    fetch_dataset,
+    check_if_features_assigned
+)
 
 warnings.filterwarnings("ignore")
 
 BATCH_SIZE_DEFAULT = 32
 
 
 class BaseWrapper(ABC):
@@ -120,20 +123,28 @@
                 metadata=self.metadata,
                 table_name=self.table_name,
                 fk_kde_path=self.fk_kde_path
             )
         elif self.process == "infer":
             self.dataset = fetch_dataset(self.dataset_pickle_path)
 
+    def _save_dataset(self):
+        """
+        Save dataset object on the disk
+        """
+        with open(self.dataset_pickle_path, "wb") as f:
+            f.write(pickle.dumps(self.dataset))
+
     def _pipeline(self):
-        self.dataset.set_metadata()
+        """
+        Launch the pipeline in the dataset
+        """
         self.df = self.dataset.pipeline()
+        self._save_dataset()
 
-        with open(self.dataset_pickle_path, "wb") as f:
-            f.write(pickle.dumps(self.dataset))
 
     def _restore_zero_values(self, df):
         for column in self.dataset.zero_num_column_names:
             if column.endswith("_zero"):
                 # remove _zero to get original column name
                 num_column_name = column[:-5]
                 num_column = df[num_column_name].copy()
@@ -172,24 +183,34 @@
             df[column_name] = df[column_name].fillna(np.nan) if nan_label is None else df[column_name].fillna(nan_label)
         return df
 
     @abstractmethod
     def _init_model(self):
         pass
 
+    def _set_dataset_metadata(self):
+        """
+        Set metadata for the dataset and save it on the disk
+        """
+        self.dataset.set_metadata()
+        self._save_dataset()
+
     def prepare_dataset(self):
         self.__post__init__()
-        self._pipeline()
+        self._set_dataset_metadata()
 
     def fit_on_df(
         self,
         df: pd.DataFrame,
         epochs: int,
         columns_subset: List[str] = None,  # TODO columns_subset does not work
     ):
+        self._pipeline()
+        if not check_if_features_assigned(self.dataset_pickle_path):
+            return
         self._init_model()
 
         if columns_subset is None:
             columns_subset = self.df.columns
         else:
             # if a column is in columns_subset, its null column should also be added if present
             columns_subset += [
@@ -204,15 +225,15 @@
         self.vae = self.model.model
 
         self.optimizer = self._create_optimizer()
         self.loss_metric = self._create_loss()
         self._train(train_dataset, epochs)
 
         self.model.model = self.vae
-        self.fit_sampler(df.dropna())
+        self.fit_sampler(df)
 
     def _train(self, dataset, epochs: int):
         step = self._train_step
 
         self.feature_losses = defaultdict(list)
         loss_grows_num_epochs = 0
         prev_total_loss = float("inf")
```

### Comparing `syngen-0.0.96/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.0.97/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/ml/worker/worker.py` & `syngen-0.0.97/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen/train.py` & `syngen-0.0.97/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.96/src/syngen.egg-info/PKG-INFO` & `syngen-0.0.97/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.96
+Version: 0.0.97
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.96 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.97 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.96/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.97/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

