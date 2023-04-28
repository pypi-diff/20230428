# Comparing `tmp/ai_transform-0.30.8.tar.gz` & `tmp/ai_transform-0.30.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.8.tar", last modified: Mon Apr 17 02:07:27 2023, max compression
+gzip compressed data, was "ai_transform-0.30.9.tar", last modified: Fri Apr 21 04:29:28 2023, max compression
```

## Comparing `ai_transform-0.30.8.tar` & `ai_transform-0.30.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.613644 ai_transform-0.30.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-17 02:07:07.000000 ai_transform-0.30.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-17 02:07:27.613644 ai_transform-0.30.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-17 02:07:07.000000 ai_transform-0.30.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-17 02:07:07.000000 ai_transform-0.30.8/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.605644 ai_transform-0.30.8/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-17 02:07:27.000000 ai_transform-0.30.8/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-17 02:07:27.000000 ai_transform-0.30.8/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:07:27.000000 ai_transform-0.30.8/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 02:07:27.000000 ai_transform-0.30.8/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 02:07:27.000000 ai_transform-0.30.8/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 02:07:07.000000 ai_transform-0.30.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 02:07:27.613644 ai_transform-0.30.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 02:07:07.000000 ai_transform-0.30.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.609644 ai_transform-0.30.8/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:27.613644 ai_transform-0.30.8/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 02:07:07.000000 ai_transform-0.30.8/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-21 04:29:09.000000 ai_transform-0.30.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 04:29:28.958745 ai_transform-0.30.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-21 04:29:09.000000 ai_transform-0.30.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.950744 ai_transform-0.30.9/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.950744 ai_transform-0.30.9/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.950744 ai_transform-0.30.9/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 04:29:09.000000 ai_transform-0.30.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:29:28.958745 ai_transform-0.30.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-21 04:29:09.000000 ai_transform-0.30.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.8/LICENSE` & `ai_transform-0.30.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/README.md` & `ai_transform-0.30.9/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/__init__.py` & `ai_transform-0.30.9/ai_transform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.30.8"
+__version__ = "0.30.9"
 
 from ai_transform.timer import Timer
 
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.30.8/ai_transform/api/api.py` & `ai_transform-0.30.9/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/api/client.py` & `ai_transform-0.30.9/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/api/helpers.py` & `ai_transform-0.30.9/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/api/wrappers.py` & `ai_transform-0.30.9/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/components/components.py` & `ai_transform-0.30.9/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/config.py` & `ai_transform-0.30.9/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/dataset/dataset.py` & `ai_transform-0.30.9/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/dataset/field.py` & `ai_transform-0.30.9/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/engine/abstract_engine.py` & `ai_transform-0.30.9/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.30.9/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.30.9/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/engine/multipass_engine.py` & `ai_transform-0.30.9/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.30.9/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/engine/stable_engine.py` & `ai_transform-0.30.9/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/logger.py` & `ai_transform-0.30.9/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/operator/abstract_operator.py` & `ai_transform-0.30.9/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/operator/dense_operator.py` & `ai_transform-0.30.9/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/timer.py` & `ai_transform-0.30.9/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/types.py` & `ai_transform-0.30.9/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/utils/document.py` & `ai_transform-0.30.9/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/utils/document_list.py` & `ai_transform-0.30.9/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/utils/example_documents.py` & `ai_transform-0.30.9/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/utils/json_encoder.py` & `ai_transform-0.30.9/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/utils/keyphrase.py` & `ai_transform-0.30.9/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.30.9/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform/workflow/context_manager.py` & `ai_transform-0.30.9/ai_transform/workflow/context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,38 +118,41 @@
             output = self.output
             if self.output_documents is not None:
                 output["documents"] = self.output_documents
         else:
             output = self.output_documents
         return output
 
-    def set_workflow_status(self, status: str):
+    def set_workflow_status(self, status: str, user_errors: str = None):
         result = self.api._set_workflow_status(
             status=status,
             job_id=self.job_id,
             metadata=self.metadata,
             workflow_name=self.workflow_name,
             additional_information=self.additional_information,
             send_email=self.send_email,
             email=self.email,
             worker_number=self.worker_number,
+            user_errors=user_errors,
             output=self._get_output_to_status_obj(),
         )
         logger.debug(format_logging_info(result))
         return result
 
     def __enter__(self):
         if self.operators is not None:
             self._set_field_children_recursively()
         self.set_workflow_status(status=self.IN_PROGRESS)
         return self
 
-    def _handle_workflow_fail(self, exc_type: type, exc_value: BaseException, traceback: Traceback):
+    def _handle_workflow_fail(
+        self, exc_type: type, exc_value: BaseException, traceback: Traceback, user_errors: str = None
+    ):
         logger.exception(exc_value)
-        self.set_workflow_status(status=self.FAILED)
+        self.set_workflow_status(status=self.FAILED, user_errors=user_errors)
         return False
 
     def _handle_workflow_complete(self):
         self.set_workflow_status(status=self.COMPLETE)
         return True
 
     def _calculate_pricing(self):
@@ -180,28 +183,27 @@
             workflow_id=self.job_id,
             step=self.workflow_name,
             worker_number=self.worker_number,
             n_processed_pricing=n_processed_pricing,
         )
 
     def __exit__(self, exc_type: type, exc_value: BaseException, traceback: Traceback):
+        regular_workflow_failed = False
+        user_errors = None
+
         if self.engine is not None:
             regular_workflow_failed = self.engine.success_ratio < self.success_threshold
+
             if regular_workflow_failed:
-                # users should know when regular workflow failed
-                # raise the user facing error
-                UserFacingError(
-                    error_message=WORKFLOW_FAIL_MESSAGE,
-                    client=self.dataset,
-                    job_id=self.job_id,
-                    workflow_name=self.workflow_name,
+                user_errors = WORKFLOW_FAIL_MESSAGE.format(
+                    100 * self.engine.success_ratio, 100 * self.success_threshold
                 )
 
-        if exc_type is not None:
-            return self._handle_workflow_fail(exc_type, exc_value, traceback)
+        if exc_type is not None or regular_workflow_failed:
+            return self._handle_workflow_fail(exc_type, exc_value, traceback, user_errors)
         else:
             n_processed_pricing = self._n_processed_pricing or self._calculate_pricing()
             if n_processed_pricing is not None:
                 self.update_workflow_pricing(n_processed_pricing)
             return self._handle_workflow_complete()
 
     def get_status(self):
```

### Comparing `ai_transform-0.30.8/ai_transform/workflow/helpers.py` & `ai_transform-0.30.9/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.30.9/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/setup.py` & `ai_transform-0.30.9/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/conftest.py` & `ai_transform-0.30.9/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 import random
 import pytest
 import string
 
 from typing import List, Dict, Sequence
 
 from ai_transform.api.client import Client
-from ai_transform.dataset.dataset import Dataset
 from ai_transform.api.helpers import process_token
+
+from ai_transform.dataset.dataset import Dataset
+
 from ai_transform.engine.stable_engine import StableEngine
-from ai_transform.utils.document import Document
-from ai_transform.utils.document_list import DocumentList
+
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.operator.dense_operator import DenseOperator
-from ai_transform.engine.stable_engine import StableEngine
+
+from ai_transform.utils.document import Document
+from ai_transform.utils.document_list import DocumentList
 from ai_transform.utils.example_documents import mock_documents, static_documents, tag_documents
 
 TEST_TOKEN = os.getenv("TEST_TOKEN")
 test_creds = process_token(TEST_TOKEN)
 
 
 @pytest.fixture(scope="session")
@@ -41,78 +44,78 @@
     return dataset_id
 
 
 @pytest.fixture(scope="class")
 def empty_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def full_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(mock_documents(20))
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def mixed_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     documents = mock_documents(10)
     stripped = mock_documents(10)
     for document in stripped:
         document.pop("_chunk_")
     documents += stripped
     dataset.insert_documents(documents)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def static_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(static_documents(20))
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def dense_input_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(static_documents(2))
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def dense_output_dataset1(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def dense_output_dataset2(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="function")
 def test_document() -> Document:
     raw_dict = {"field1": {"field2": 1}, "field3": 3}
@@ -207,15 +210,15 @@
     return StableEngine(dataset=full_dataset, operator=test_paid_operator, refresh=False)
 
 
 @pytest.fixture(scope="function")
 def test_sentiment_workflow_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(mock_documents(20))
     time.sleep(1)
     job_id = str(uuid.uuid4())
     config = dict(
         job_id=job_id,
         authorizationToken=test_client.credentials.token,
         dataset_id=dataset_id,
@@ -225,14 +228,35 @@
     config_bytes = config_string.encode()
     workflow_token = base64.b64encode(config_bytes).decode()
     yield workflow_token
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="function")
+def test_user_facing_error_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(mock_documents(20))
+    time.sleep(1)
+    job_id = str(uuid.uuid4())
+    config = dict(
+        job_id=job_id,
+        dataset_id=dataset_id,
+        authorizationToken=test_client.credentials.token,
+        text_field="sample_1_description_not_in_dataset",
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
 def test_sentiment_workflow_document_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     time.sleep(1)
     job_id = str(uuid.uuid4())
     config = dict(
         job_id=job_id,
         authorizationToken=test_client.credentials.token,
@@ -245,15 +269,15 @@
     yield workflow_token
 
 
 @pytest.fixture(scope="function")
 def test_simple_workflow_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(mock_documents(20))
     time.sleep(1)
     job_id = str(uuid.uuid4())
     config = dict(
         job_id=job_id, authorizationToken=test_client.credentials.token, dataset_id=dataset_id, send_email=True
     )
     config_string = json.dumps(config)
@@ -263,15 +287,15 @@
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="function")
 def test_cluster_workflow_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset((dataset_id), expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(mock_documents(20))
     job_id = str(uuid.uuid4())
     print(job_id)
     config = dict(
         job_id=job_id,
         authorizationToken=test_client.credentials.token,
         dataset_id=dataset_id,
```

### Comparing `ai_transform-0.30.8/tests/core/test_api/test_client.py` & `ai_transform-0.30.9/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_api/test_endpoints.py` & `ai_transform-0.30.9/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.30.9/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_api/test_wrappers.py` & `ai_transform-0.30.9/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.30.9/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_dataset/test_field.py` & `ai_transform-0.30.9/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.30.9/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.30.9/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_engine/test_engine.py` & `ai_transform-0.30.9/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.30.9/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.30.9/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.30.9/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.30.9/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.30.9/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.30.9/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.8/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.30.9/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

