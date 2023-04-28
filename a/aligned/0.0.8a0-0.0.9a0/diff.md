# Comparing `tmp/aligned-0.0.8a0.tar.gz` & `tmp/aligned-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned-0.0.8a0.tar", max compression
+gzip compressed data, was "aligned-0.0.9a0.tar", max compression
```

## Comparing `aligned-0.0.8a0.tar` & `aligned-0.0.9a0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0    11358 2022-12-23 11:41:36.799725 aligned-0.0.8a0/LICENSE
--rw-r--r--   0        0        0     7889 2022-12-23 11:41:36.799725 aligned-0.0.8a0/README.md
--rw-r--r--   0        0        0     1189 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/__init__.py
--rw-r--r--   0        0        0    14062 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/cli.py
--rw-r--r--   0        0        0      441 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/compiler/constraint_factory.py
--rw-r--r--   0        0        0    19480 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/compiler/feature_factory.py
--rw-r--r--   0        0        0     5781 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/compiler/repo_reader.py
--rw-r--r--   0        0        0    18324 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/compiler/transformation_factory.py
--rw-r--r--   0        0        0      718 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/data_file.py
--rw-r--r--   0        0        0        0 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/data_source/__init__.py
--rw-r--r--   0        0        0     3467 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/data_source/batch_data_source.py
--rw-r--r--   0        0        0     1973 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/data_source/stream_data_source.py
--rw-r--r--   0        0        0     8108 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/enricher.py
--rw-r--r--   0        0        0      278 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/entity_data_source.py
--rw-r--r--   0        0        0      341 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/exceptions.py
--rw-r--r--   0        0        0     6880 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_source.py
--rw-r--r--   0        0        0    16138 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_store.py
--rw-r--r--   0        0        0      298 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_view/__init__.py
--rw-r--r--   0        0        0     4969 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_view/combined_view.py
--rw-r--r--   0        0        0    10029 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_view/feature_view.py
--rw-r--r--   0        0        0      936 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_view/tests/test_brest_cancer.py
--rw-r--r--   0        0        0     1102 2022-12-23 11:41:36.799725 aligned-0.0.8a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
--rw-r--r--   0        0        0     3040 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/feature_view/tests/test_brest_cancer_standard_scaling.py
--rw-r--r--   0        0        0     1231 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/feature_view/tests/test_combined_view.py
--rw-r--r--   0        0        0     1692 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/feature_view/tests/test_hidden_variable.py
--rw-r--r--   0        0        0        0 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/local/__init__.py
--rw-r--r--   0        0        0     5114 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/local/job.py
--rw-r--r--   0        0        0     8666 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/local/source.py
--rw-r--r--   0        0        0     2676 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/model.py
--rw-r--r--   0        0        0     2967 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/online_source.py
--rw-r--r--   0        0        0        0 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/psql/__init__.py
--rw-r--r--   0        0        0     4431 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/psql/data_source.py
--rw-r--r--   0        0        0     9939 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/psql/jobs.py
--rw-r--r--   0        0        0        0 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redis/__init__.py
--rw-r--r--   0        0        0     4344 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redis/config.py
--rw-r--r--   0        0        0     3275 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redis/job.py
--rw-r--r--   0        0        0     2275 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redis/stream.py
--rw-r--r--   0        0        0     4382 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redis/tests/test_redis_job.py
--rw-r--r--   0        0        0        0 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redshift/__init__.py
--rw-r--r--   0        0        0     2660 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redshift/data_source.py
--rw-r--r--   0        0        0     1172 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/redshift/factory.py
--rw-r--r--   0        0        0     8250 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/request/retrival_request.py
--rw-r--r--   0        0        0     1638 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/request/tests/test_feature_request_generation.py
--rw-r--r--   0        0        0    16825 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/retrival_job.py
--rw-r--r--   0        0        0        0 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/s3/__init__.py
--rw-r--r--   0        0        0     5047 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/s3/config.py
--rw-r--r--   0        0        0     1502 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/s3/factory.py
--rw-r--r--   0        0        0     1748 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/s3/storage.py
--rw-r--r--   0        0        0      251 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/codable.py
--rw-r--r--   0        0        0     2356 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/constraints.py
--rw-r--r--   0        0        0     1379 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/derivied_feature.py
--rw-r--r--   0        0        0     3661 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/feature.py
--rw-r--r--   0        0        0     8258 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/feature_view.py
--rw-r--r--   0        0        0     4447 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/repo_definition.py
--rw-r--r--   0        0        0    26873 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/schemas/transformation.py
--rw-r--r--   0        0        0     8595 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/server.py
--rw-r--r--   0        0        0     5086 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/split_strategy.py
--rw-r--r--   0        0        0      223 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/storage.py
--rw-r--r--   0        0        0      682 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/tests/test_cache_enricher.py
--rw-r--r--   0        0        0      545 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/tests/test_cached_parquet.py
--rw-r--r--   0        0        0     2056 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/tests/test_statistic_enricher.py
--rw-r--r--   0        0        0     1795 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/tests/test_std_transformation.py
--rw-r--r--   0        0        0     2371 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/tests/test_train_test_validate_set.py
--rw-r--r--   0        0        0      658 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/tests/test_transformations.py
--rw-r--r--   0        0        0      193 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/validation/interface.py
--rw-r--r--   0        0        0     2290 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/validation/pandera.py
--rw-r--r--   0        0        0      782 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/validation/tests/test_pandera_validator.py
--rw-r--r--   0        0        0     3846 2022-12-23 11:41:36.803725 aligned-0.0.8a0/aligned/worker.py
--rw-r--r--   0        0        0     2502 2022-12-23 11:41:36.807725 aligned-0.0.8a0/pyproject.toml
--rw-r--r--   0        0        0     9950 1970-01-01 00:00:00.000000 aligned-0.0.8a0/setup.py
--rw-r--r--   0        0        0    10304 1970-01-01 00:00:00.000000 aligned-0.0.8a0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-03 20:34:00.544967 aligned-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     8521 2023-01-03 20:34:00.544967 aligned-0.0.9a0/README.md
+-rw-r--r--   0        0        0     1189 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/__init__.py
+-rw-r--r--   0        0        0    14066 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/cli.py
+-rw-r--r--   0        0        0      441 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/constraint_factory.py
+-rw-r--r--   0        0        0    19110 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/feature_factory.py
+-rw-r--r--   0        0        0     5784 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/repo_reader.py
+-rw-r--r--   0        0        0    18324 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/transformation_factory.py
+-rw-r--r--   0        0        0      822 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_file.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/__init__.py
+-rw-r--r--   0        0        0     3467 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/batch_data_source.py
+-rw-r--r--   0        0        0     1973 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/stream_data_source.py
+-rw-r--r--   0        0        0     8108 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/enricher.py
+-rw-r--r--   0        0        0      278 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/entity_data_source.py
+-rw-r--r--   0        0        0      341 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/exceptions.py
+-rw-r--r--   0        0        0     7657 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_source.py
+-rw-r--r--   0        0        0    17949 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_store.py
+-rw-r--r--   0        0        0      298 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/__init__.py
+-rw-r--r--   0        0        0     4969 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/combined_view.py
+-rw-r--r--   0        0        0    10029 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/feature_view.py
+-rw-r--r--   0        0        0      944 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py
+-rw-r--r--   0        0        0     3135 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
+-rw-r--r--   0        0        0     1239 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_combined_view.py
+-rw-r--r--   0        0        0     1692 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_hidden_variable.py
+-rw-r--r--   0        0        0     1074 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py
+-rw-r--r--   0        0        0     1981 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_derived_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/__init__.py
+-rw-r--r--   0        0        0     6962 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/job.py
+-rw-r--r--   0        0        0     8899 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/source.py
+-rw-r--r--   0        0        0     1105 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/tests/test_jobs.py
+-rw-r--r--   0        0        0     3006 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/model.py
+-rw-r--r--   0        0        0     2967 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/online_source.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/__init__.py
+-rw-r--r--   0        0        0     4431 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/data_source.py
+-rw-r--r--   0        0        0    10601 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/jobs.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/__init__.py
+-rw-r--r--   0        0        0     4348 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/config.py
+-rw-r--r--   0        0        0     3288 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/job.py
+-rw-r--r--   0        0        0     2275 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/stream.py
+-rw-r--r--   0        0        0     4402 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/tests/test_redis_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/__init__.py
+-rw-r--r--   0        0        0     2660 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/data_source.py
+-rw-r--r--   0        0        0     1172 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/factory.py
+-rw-r--r--   0        0        0     8250 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/retrival_request.py
+-rw-r--r--   0        0        0     1817 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py
+-rw-r--r--   0        0        0    15322 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/retrival_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/__init__.py
+-rw-r--r--   0        0        0     5715 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/config.py
+-rw-r--r--   0        0        0     1447 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/factory.py
+-rw-r--r--   0        0        0     1846 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/storage.py
+-rw-r--r--   0        0        0      251 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/codable.py
+-rw-r--r--   0        0        0     2356 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/constraints.py
+-rw-r--r--   0        0        0     1379 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/derivied_feature.py
+-rw-r--r--   0        0        0     3663 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature.py
+-rw-r--r--   0        0        0     8217 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature_view.py
+-rw-r--r--   0        0        0      409 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/model.py
+-rw-r--r--   0        0        0     4478 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/repo_definition.py
+-rw-r--r--   0        0        0    37245 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/transformation.py
+-rw-r--r--   0        0        0     8663 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/server.py
+-rw-r--r--   0        0        0     5086 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/split_strategy.py
+-rw-r--r--   0        0        0      196 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/storage.py
+-rw-r--r--   0        0        0      682 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cache_enricher.py
+-rw-r--r--   0        0        0      549 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cached_parquet.py
+-rw-r--r--   0        0        0     2056 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py
+-rw-r--r--   0        0        0     2371 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_train_test_validate_set.py
+-rw-r--r--   0        0        0      905 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_transformations.py
+-rw-r--r--   0        0        0      193 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/interface.py
+-rw-r--r--   0        0        0     2392 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/pandera.py
+-rw-r--r--   0        0        0      848 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/tests/test_pandera_validator.py
+-rw-r--r--   0        0        0     3846 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/worker.py
+-rw-r--r--   0        0        0     2553 2023-01-03 20:34:00.552967 aligned-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0    10667 1970-01-01 00:00:00.000000 aligned-0.0.9a0/setup.py
+-rw-r--r--   0        0        0    10982 1970-01-01 00:00:00.000000 aligned-0.0.9a0/PKG-INFO
```

### Comparing `aligned-0.0.8a0/LICENSE` & `aligned-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/README.md` & `aligned-0.0.9a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Aligned
 
-A feature store alignes the offline and online features in a ML system. Therefore making it harder to achive a training-serving skew. However, that is only the beginning.
+Aligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.
+
+Read the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)
+
+Also check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used
+
+⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.
 
 ## Feature Views
 
 Write features as the should be, as data models.
 Then get code completion and typesafety by referencing them in other features.
 
 This makes the features light weight, data source indipendent, and flexible.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aligned-0.0.8a0/aligned/__init__.py` & `aligned-0.0.9a0/aligned/__init__.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/cli.py` & `aligned-0.0.9a0/aligned/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
     feature_store = online_store.offline_store()
 
     results = ProfilingResult(numeric_features={}, categorical_features={})
 
     for feature_view_name in sorted(feature_store.feature_views.keys()):
         click.echo(f'Profiling: {feature_view_name}')
         feature_view = feature_store.feature_view(feature_view_name)
-        data_set: DataFrame = sync(feature_view.all(limit=dataset_size).to_df())
+        data_set: DataFrame = sync(feature_view.all(limit=dataset_size).to_pandas())
 
         all_features: list[Feature] = list(feature_view.view.features) + list(
             feature_view.view.derived_features
         )
         for feature in all_features:
 
             data_slice = data_set[feature.name]
```

### Comparing `aligned-0.0.8a0/aligned/compiler/feature_factory.py` & `aligned-0.0.9a0/aligned/compiler/feature_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     @property
     def depending_on_names(self) -> list[str]:
         if not self.transformation:
             return []
         return [feat._name for feat in self.transformation.using_features if feat._name]
 
     def feature_referance(self) -> FeatureReferance:
-        return FeatureReferance(self.name, self._feature_view, self.dtype, self.transformation is not None)
+        return FeatureReferance(self.name, self._feature_view, self.dtype)
 
     async def feature(self) -> Feature:
         return Feature(
             name=self.name,
             dtype=self.dtype,
             description=self._description,
             tags=None,
@@ -346,21 +346,14 @@
     def __abs__(self) -> Float:
         from aligned.compiler.transformation_factory import AbsoluteFactory
 
         feature = Float()
         feature.transformation = AbsoluteFactory(self)
         return feature
 
-    def standard_scaled(self, timespan: timedelta | None = None, limit: int | None = None) -> Float:
-        from aligned.compiler.transformation_factory import StandardScalingFactory
-
-        feature = Float()
-        feature.transformation = StandardScalingFactory(feature=self, limit=limit, timespan=timespan)
-        return feature
-
     def log1p(self) -> Float:
         from aligned.compiler.transformation_factory import LogTransformFactory
 
         feature = Float()
         feature.transformation = LogTransformFactory(self)
         return feature
```

### Comparing `aligned-0.0.8a0/aligned/compiler/repo_reader.py` & `aligned-0.0.9a0/aligned/compiler/repo_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from importlib import import_module
 from inspect import getmro, isclass
 from pathlib import Path
 from typing import Any
 
 from aligned.enricher import Enricher
-from aligned.model import ModelService
+from aligned.model import Model
 from aligned.online_source import BatchOnlineSource, OnlineSource
 from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoReference
 
 logger = logging.getLogger(__name__)
 
 
 def imports_for(file_path: Path) -> set[str]:
@@ -76,15 +76,15 @@
     """
 
     @staticmethod
     async def definition_from_path(repo_path: Path) -> RepoDefinition:
         repo = RepoDefinition(
             feature_views=set(),
             combined_feature_views=set(),
-            models={},
+            models=set(),
             online_source=BatchOnlineSource(),
             enrichers=[],
         )
 
         feature_view_names: dict[str, str] = {}
 
         for py_file in python_files(repo_path):
@@ -104,17 +104,19 @@
 
             for attribute in dir(module):
                 if attribute in imports:
                     continue
 
                 obj = getattr(module, attribute)
 
-                if isinstance(obj, ModelService):
-                    model_name = obj._name or attribute
-                    repo.models[model_name] = obj.feature_refs
+                if isinstance(obj, Model):
+                    if not obj.name:
+                        obj.name = attribute
+                    repo.models.add(obj.schema())
+
                 elif isinstance(obj, Enricher):
                     repo.enrichers.append(
                         EnricherReference(module=module_path, attribute_name=attribute, enricher=obj)
                     )
                 elif isinstance(obj, OnlineSource):
                     repo.online_source = obj
                 else:
```

### Comparing `aligned-0.0.8a0/aligned/compiler/transformation_factory.py` & `aligned-0.0.9a0/aligned/compiler/transformation_factory.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/data_file.py` & `aligned-0.0.9a0/aligned/data_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import polars as pl
 
 
 class DataFileReference:
     """
     A reference to a data file.
 
     It can therefore be loaded in and writen to.
@@ -17,12 +18,15 @@
 
     async def to_df(self) -> pd.DataFrame:
         await self.read_pandas()
 
     async def to_dask(self) -> pd.DataFrame:
         await self.read_dask()
 
+    async def to_polars(self) -> pl.LazyFrame:
+        raise NotImplementedError()
+
     async def write_pandas(self, df: pd.DataFrame) -> None:
         raise NotImplementedError()
 
     async def write_dask(self, df: pd.DataFrame) -> None:
         raise NotImplementedError()
```

### Comparing `aligned-0.0.8a0/aligned/data_source/batch_data_source.py` & `aligned-0.0.9a0/aligned/data_source/batch_data_source.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/data_source/stream_data_source.py` & `aligned-0.0.9a0/aligned/data_source/stream_data_source.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/enricher.py` & `aligned-0.0.9a0/aligned/enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/feature_source.py` & `aligned-0.0.9a0/aligned/feature_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
-from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
+import polars as pl
 
 from aligned.data_source.batch_data_source import BatchDataSource
-from aligned.request.retrival_request import FeatureRequest, RetrivalRequest
+from aligned.request.retrival_request import FeatureRequest, RequestResult, RetrivalRequest
 from aligned.retrival_job import FactualRetrivalJob
 
-with suppress(ModuleNotFoundError):
-    import dask.dataframe as dd
-
 if TYPE_CHECKING:
     from aligned.retrival_job import RetrivalJob
 
 
 class FeatureSource:
     def features_for(self, facts: dict[str, list], request: FeatureRequest) -> RetrivalJob:
         raise NotImplementedError()
@@ -61,59 +58,74 @@
         }
         source_groupes = {
             self.sources[request.feature_view_name].job_group_key()
             for request in request.needed_requests
             if request.feature_view_name in self.sources
         }
         # The combined views basicly, as they have no direct
-        requests = [
+        combined_requests = [
             request for request in request.needed_requests if request.feature_view_name not in self.sources
         ]
         jobs = [
-            self.source_types[source_group].feature_for(
+            self.source_types[source_group]
+            .feature_for(
                 facts=facts,
                 requests={
                     source: req
                     for source, req in core_requests.items()
                     if source.job_group_key() == source_group
                 },
             )
+            .derive_features(
+                requests=[
+                    req for source, req in core_requests.items() if source.job_group_key() == source_group
+                ]
+            )
             for source_group in source_groupes
         ]
         return CombineFactualJob(
             jobs=jobs,
-            combined_requests=requests,
-        )
+            combined_requests=combined_requests,
+        ).ensure_types(request.needed_requests)
 
     def all_for(self, request: FeatureRequest, limit: int | None = None) -> RetrivalJob:
         if len(request.needed_requests) != 1:
             raise ValueError("Can't use all_for with a request that has subrequests")
         if request.name not in self.sources:
             raise ValueError(
                 (
                     f"Unable to find feature view named '{request.name}'.",
                     'Make sure it is added to the featuer store',
                 )
             )
-        return self.sources[request.name].all_data(request.needed_requests[0], limit)
+        return (
+            self.sources[request.name]
+            .all_data(request.needed_requests[0], limit)
+            .derive_features(request.needed_requests)
+            .ensure_types(request.needed_requests)
+        )
 
     def all_between(self, start_date: datetime, end_date: datetime, request: FeatureRequest) -> RetrivalJob:
         if len(request.needed_requests) != 1:
             raise ValueError("Can't use all_for with a request that has subrequests")
         if request.name not in self.sources:
             raise ValueError(
                 (
                     f"Unable to find feature view named '{request.name}'.",
                     'Make sure it is added to the featuer store',
                 )
             )
-        return self.sources[request.name].all_between_dates(request.needed_requests[0], start_date, end_date)
+        return (
+            self.sources[request.name]
+            .all_between_dates(request.needed_requests[0], start_date, end_date)
+            .derive_features(requests=request.needed_requests)
+            .ensure_types(request.needed_requests)
+        )
 
 
-@dataclass
 class FactualInMemoryJob(FactualRetrivalJob):
     """
     A job using a in mem storage, aka a dict.
 
     This will store the features in the following format:
 
     values = {
@@ -128,18 +140,29 @@
     }
     """
 
     values: dict[str, Any]
     requests: list[RetrivalRequest]
     facts: dict[str, list]
 
+    @property
+    def request_result(self) -> RequestResult:
+        return RequestResult.from_request_list(self.requests)
+
+    def __init__(
+        self, values: dict[str, Any], requests: list[RetrivalRequest], facts: dict[str, list]
+    ) -> None:
+        self.values = values
+        self.requests = requests
+        self.facts = facts
+
     def key(self, request: RetrivalRequest, entity: str, feature_name: str) -> str:
         return f'{request.feature_view_name}:{entity}:{feature_name}'
 
-    async def _to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
 
         columns = set()
         for request in self.requests:
             for feature in request.all_feature_names:
                 columns.add(feature)
 
         result_df = pd.DataFrame(self.facts)
@@ -154,34 +177,31 @@
                 # Fetch one column at a time
                 result_df[feature] = [
                     self.values.get(self.key(request, entity, feature)) for entity in entities
                 ]
 
         return result_df
 
-    async def to_df(self) -> pd.DataFrame:
-        return await self._to_df()
-
-    async def _to_dask(self) -> dd.DataFrame:
-        return await self._to_df()
+    async def to_polars(self) -> pl.LazyFrame:
+        return pl.from_pandas(await self.to_pandas()).lazy()
 
 
 @dataclass
 class InMemoryFeatureSource(FeatureSource, WritableFeatureSource):
 
     values: dict[str, Any]
 
     def features_for(self, facts: dict[str, list], request: FeatureRequest) -> RetrivalJob:
         return FactualInMemoryJob(self.values, request.needed_requests, facts)
 
     def key(self, request: RetrivalRequest, entity: str, feature_name: str) -> str:
         return f'{request.feature_view_name}:{entity}:{feature_name}'
 
     async def write(self, job: RetrivalJob, requests: list[RetrivalRequest]) -> None:
-        data = await job.to_df()
+        data = await job.to_pandas()
 
         for _, row in data.iterrows():
             # Run one query per row
             for request in requests:
                 entity_ids = row[list(request.entity_names)]
                 entity_id = ':'.join([str(entity_id) for entity_id in entity_ids])
                 if not entity_id:
```

### Comparing `aligned-0.0.8a0/aligned/feature_store.py` & `aligned-0.0.9a0/aligned/feature_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     BatchFeatureSource,
     FeatureSource,
     RangeFeatureSource,
     WritableFeatureSource,
 )
 from aligned.feature_view.combined_view import CombinedFeatureView, CompiledCombinedFeatureView
 from aligned.feature_view.feature_view import FeatureView
-from aligned.model import ModelService
+from aligned.model import Model
 from aligned.online_source import BatchOnlineSource
 from aligned.request.retrival_request import FeatureRequest, RetrivalRequest
-from aligned.retrival_job import FilterJob, RetrivalJob
+from aligned.retrival_job import DerivedFeatureJob, FilterJob, RetrivalJob
 from aligned.schemas.feature_view import CompiledFeatureView
+from aligned.schemas.model import Model as ModelSchema
 from aligned.schemas.repo_definition import EnricherReference, RepoDefinition
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class RawStringFeatureRequest:
@@ -55,26 +56,26 @@
 
 
 class FeatureStore:
 
     feature_source: FeatureSource
     feature_views: dict[str, CompiledFeatureView]
     combined_feature_views: dict[str, CompiledCombinedFeatureView]
-    model_requests: dict[str, FeatureRequest]
+    models: dict[str, ModelSchema]
     event_timestamp_column = 'event_timestamp'
 
     @property
     def all_models(self) -> list[str]:
         return list(self.model_requests.keys())
 
     def __init__(
         self,
         feature_views: dict[str, CompiledFeatureView],
         combined_feature_views: dict[str, CompiledCombinedFeatureView],
-        models: dict[str, FeatureRequest],
+        models: dict[str, ModelSchema],
         feature_source: FeatureSource,
     ) -> None:
         self.feature_source = feature_source
         self.combined_feature_views = combined_feature_views
         self.feature_views = feature_views
         self.model_requests = models
 
@@ -118,29 +119,40 @@
         for module, values in grouped_enrichers.items():
             set_module(
                 module, DynamicEnricher({enricher.attribute_name: enricher.enricher for enricher in values})
             )
 
     @staticmethod
     def from_definition(repo: RepoDefinition, feature_source: FeatureSource | None = None) -> 'FeatureStore':
+        """Creates a feature store based on a repo definition
+        A feature source can also be defined if wanted, otherwise will the batch source be used for reads
+
+        ```
+        repo_file: bytes = ...
+        repo_def = RepoDefinition.from_json(repo_file)
+        feature_store = FeatureStore.from_definition(repo_def)
+        ```
+
+        Args:
+            repo (RepoDefinition): The definition to setup
+            feature_source (FeatureSource | None, optional): The source to read from and potentially write to.
+
+        Returns:
+            FeatureStore: A ready to use feature store
+        """
         source = feature_source or repo.online_source.feature_source(repo.feature_views)
         feature_views = {fv.name: fv for fv in repo.feature_views}
         combined_feature_views = {fv.name: fv for fv in repo.combined_feature_views}
 
         FeatureStore.register_enrichers(repo.enrichers)
 
         return FeatureStore(
             feature_views=feature_views,
             combined_feature_views=combined_feature_views,
-            models={
-                name: FeatureStore._requests_for(
-                    RawStringFeatureRequest(model), feature_views, combined_feature_views
-                )
-                for name, model in repo.models.items()
-            },
+            models={model.name: model for model in repo.models},
             feature_source=source,
         )
 
     @staticmethod
     async def from_reference_at_path(
         path: str = '.', reference_file: str = 'feature_store_location.py'
     ) -> 'FeatureStore':
@@ -207,17 +219,26 @@
 
         return FilterJob(
             feature_names,
             self.feature_source.features_for(entities, requests),
         )
 
     def model(self, name: str) -> 'ModelFeatureStore':
-        request = self.model_requests[name]
+        model = self.model_requests[name]
+        request = self.requests_for_model(model)
         return ModelFeatureStore(self.feature_source, request)
 
+    def requests_for_model(self, model: ModelSchema) -> FeatureRequest:
+        feature_referances = {f'{feature.feature_view}:{feature.name}' for feature in model.features}.union(
+            {f'{feature.feature_view}:{feature.name}' for feature in model.targets or set()}
+        )
+        return FeatureStore._requests_for(
+            RawStringFeatureRequest(feature_referances), self.feature_views, self.combined_feature_views
+        )
+
     @staticmethod
     def _requests_for(
         feature_request: RawStringFeatureRequest,
         feature_views: dict[str, CompiledFeatureView],
         combined_feature_views: dict[str, CompiledCombinedFeatureView],
     ) -> FeatureRequest:
         features = feature_request.grouped_features
@@ -277,17 +298,16 @@
         if isinstance(self.feature_source, BatchFeatureSource):
             self.feature_source.sources[compiled_view.name] = compiled_view.batch_data_source
 
     async def add_combined_feature_view(self, feature_view: CombinedFeatureView) -> None:
         compiled_view = await type(feature_view).compile()
         self.combined_feature_views[compiled_view.name] = compiled_view
 
-    def add_model_service(self, service: ModelService) -> None:
-        request = RawStringFeatureRequest(service.feature_refs)
-        self.model_requests[service.name] = self.requests_for(request)
+    def add_model(self, model: Model) -> None:
+        self.models[model.name] = model.schema()
 
     def offline_store(self) -> 'FeatureStore':
         return FeatureStore(
             feature_views=self.feature_views,
             combined_feature_views=self.combined_feature_views,
             models=self.model_requests,
             feature_source=BatchOnlineSource().feature_source(set(self.feature_views.values())),
@@ -367,14 +387,35 @@
             if event_timestamp := request.event_timestamp:
                 features.add(event_timestamp.name)
         return features
 
     async def write(self, values: dict[str, list[Any]]) -> None:
         await self.batch_write(values)
 
+    async def process_input(self, values: dict[str, list[Any]]) -> dict[str, list[Any]]:
+        from pandas import DataFrame
+
+        from aligned.local.job import FileFullJob
+        from aligned.local.source import LiteralReference
+
+        request = self.view.request_all.needed_requests[0]
+        df = DataFrame.from_records(values)
+
+        if request.entity_names - set(df.columns):
+            missing = request.entity_names - set(df.columns)
+            raise ValueError(f'Missing entities: {missing}')
+
+        if request.all_required_feature_names - set(df.columns):
+            missing = request.all_required_feature_names - set(df.columns)
+            df[list(missing)] = None
+        output = await DerivedFeatureJob(
+            FileFullJob(LiteralReference(df), request), requests=[request]
+        ).to_pandas()
+        return output.to_dict('list')
+
     async def batch_write(self, values: dict[str, list[Any]]) -> None:
         if not isinstance(self.source, WritableFeatureSource):
             logger.info('Feature Source is not writable')
             return
 
         from pandas import DataFrame
 
@@ -395,8 +436,11 @@
                 f"""
 Some features is missing.
 Will fill values with None, but it could be a potential problem: {missing}
 """
             )
             df[list(missing)] = None
 
-        await self.source.write(FileFullJob(LiteralReference(df), request, limit=None), [request])
+        await self.source.write(
+            DerivedFeatureJob(FileFullJob(LiteralReference(df), request, limit=None), requests=[request]),
+            [request],
+        )
```

### Comparing `aligned-0.0.8a0/aligned/feature_view/combined_view.py` & `aligned-0.0.9a0/aligned/feature_view/combined_view.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/feature_view/feature_view.py` & `aligned-0.0.9a0/aligned/feature_view/feature_view.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from datetime import datetime
-
 import pytest
 
 from aligned import FeatureStore, FeatureView
 
 
 @pytest.mark.asyncio
-async def test_between_datetime_features(
-    breast_scan_feature_view_with_datetime: FeatureView,
-    breast_scan_with_timestamp_feature_store: FeatureStore,
+async def test_all_features(
+    breast_scan_without_timestamp_feature_store: FeatureStore,
+    breast_scan_feature_viewout_with_datetime: FeatureView,
 ) -> None:
-    feature_view = breast_scan_feature_view_with_datetime
-    store = breast_scan_with_timestamp_feature_store
-    features = await store.feature_view(feature_view.metadata.name).all().to_df()
+    store = breast_scan_without_timestamp_feature_store
+    feature_view = breast_scan_feature_viewout_with_datetime
+
+    features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
-    for feature in type(feature_view).select_all().features_to_include:
+    for feature in type(breast_scan_feature_viewout_with_datetime).select_all().features_to_include:
         assert feature in features.columns
 
-    assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
+    assert not features['is_malignant'].isna().any()
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
-    limit_features = (
-        await store.feature_view(feature_view.metadata.name)
-        .between(
-            start_date=datetime(2020, 1, 5),
-            end_date=datetime(2020, 1, 11),
-        )
-        .to_df()
-    )
+    limit = 10
+    limit_features = await store.feature_view(feature_view.metadata.name).all(limit=limit).to_pandas()
 
-    assert limit_features.shape[0] == 6
-    assert features['mean_fd_worst_for_group'].isna().count() != 0
+    assert limit_features.shape[0] == limit
```

### Comparing `aligned-0.0.8a0/aligned/feature_view/tests/test_combined_view.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_combined_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     entities = {'passenger_id': [1, 2, 3, 4, None], 'scan_id': [842302, 84300903, 843786, None, 842301]}
     result = await combined_feature_store.features_for(
         entities,
         features=[
             'combined:some_feature',
             'combined:other_feature',
         ],
-    ).to_df()
+    ).to_pandas()
 
     assert result.shape == (len(entities['passenger_id']), 4)
     assert result.isna().sum().sum() == 4 + 2
 
 
 @pytest.mark.asyncio
 async def test_combined_view_get_all_features(combined_feature_store: FeatureStore) -> None:
 
     entities = {'passenger_id': [1, 2, 3, 4, None], 'scan_id': [842302, 84300903, 843786, None, 842301]}
-    result = await combined_feature_store.features_for(entities, features=['combined:*']).to_df()
+    result = await combined_feature_store.features_for(entities, features=['combined:*']).to_pandas()
 
     assert result.shape == (len(entities['passenger_id']), 4)
     assert result.isna().sum().sum() == 4 + 2
```

### Comparing `aligned-0.0.8a0/aligned/feature_view/tests/test_hidden_variable.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_hidden_variable.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/local/job.py` & `aligned-0.0.9a0/aligned/local/job.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import TypeVar
 
 import pandas as pd
+import polars as pl
 
-from aligned.data_source.batch_data_source import ColumnFeatureMappable
 from aligned.local.source import DataFileReference
 from aligned.request.retrival_request import RetrivalRequest
-from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob
+from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob, RequestResult
 from aligned.schemas.feature import Feature
 
-try:
-    import dask.dataframe as dd
-except ModuleNotFoundError:
-    import pandas as dd
-
-GenericDataFrame = TypeVar('GenericDataFrame', pd.DataFrame, dd.DataFrame)
-
 
 @dataclass
 class FileFullJob(FullExtractJob):
 
     source: DataFileReference
     request: RetrivalRequest
     limit: int | None = field(default=None)
 
-    def file_transformations(self, df: GenericDataFrame) -> GenericDataFrame:
+    @property
+    def request_result(self) -> RequestResult:
+        return self.request.request_result
+
+    def file_transformations(self, df: pd.DataFrame) -> pd.DataFrame:
+        from aligned.data_source.batch_data_source import ColumnFeatureMappable
+
         entity_names = self.request.entity_names
         all_names = list(self.request.all_required_feature_names.union(entity_names))
 
         request_features = all_names
         if isinstance(self.source, ColumnFeatureMappable):
             request_features = self.source.feature_identifier_for(all_names)
 
@@ -38,32 +36,58 @@
         )
 
         if self.limit and df.shape[0] > self.limit:
             return df.iloc[: self.limit]
         else:
             return df
 
-    async def _to_df(self) -> pd.DataFrame:
+    def file_transform_polars(self, df: pl.LazyFrame) -> pl.LazyFrame:
+        from aligned.data_source.batch_data_source import ColumnFeatureMappable
+
+        entity_names = self.request.entity_names
+        all_names = list(self.request.all_required_feature_names.union(entity_names))
+
+        request_features = all_names
+        if isinstance(self.source, ColumnFeatureMappable):
+            request_features = self.source.feature_identifier_for(all_names)
+        renames = {
+            org_name: wanted_name
+            for org_name, wanted_name in zip(request_features, all_names)
+            if org_name != wanted_name
+        }
+        df = df.rename(mapping=renames)
+
+        if self.limit:
+            return df.limit(self.limit)
+        else:
+            return df
+
+    async def to_pandas(self) -> pd.DataFrame:
         file = await self.source.read_pandas()
         return self.file_transformations(file)
 
-    async def _to_dask(self) -> dd.DataFrame:
-        file = await self.source.read_dask()
-        return self.file_transformations(file)
+    async def to_polars(self) -> pl.LazyFrame:
+        file = await self.source.to_polars()
+        return self.file_transform_polars(file)
 
 
 @dataclass
 class FileDateJob(DateRangeJob):
 
     source: DataFileReference
     request: RetrivalRequest
     start_date: datetime
     end_date: datetime
 
-    def file_transformations(self, df: GenericDataFrame) -> GenericDataFrame:
+    @property
+    def request_result(self) -> RequestResult:
+        return self.request.request_result
+
+    def file_transformations(self, df: pd.DataFrame) -> pd.DataFrame:
+        from aligned.data_source.batch_data_source import ColumnFeatureMappable
 
         entity_names = self.request.entity_names
         all_names = list(self.request.all_required_feature_names.union(entity_names))
 
         request_features = all_names
         if isinstance(self.source, ColumnFeatureMappable):
             request_features = self.source.feature_identifier_for(all_names)
@@ -79,31 +103,54 @@
             df[event_timestamp_column], infer_datetime_format=True, utc=True
         )
 
         start_date_ts = pd.to_datetime(self.start_date, utc=True)
         end_date_ts = pd.to_datetime(self.end_date, utc=True)
         return df.loc[df[event_timestamp_column].between(start_date_ts, end_date_ts)]
 
-    async def _to_df(self) -> pd.DataFrame:
+    def file_transform_polars(self, df: pl.LazyFrame) -> pl.LazyFrame:
+        from aligned.data_source.batch_data_source import ColumnFeatureMappable
+
+        entity_names = self.request.entity_names
+        all_names = list(self.request.all_required_feature_names.union(entity_names))
+
+        request_features = all_names
+        if isinstance(self.source, ColumnFeatureMappable):
+            request_features = self.source.feature_identifier_for(all_names)
+
+        df = df.rename(
+            mapping={org_name: wanted_name for org_name, wanted_name in zip(request_features, all_names)}
+        )
+        event_timestamp_column = self.request.event_timestamp.name
+
+        return df.filter(pl.col(event_timestamp_column).is_between(self.start_date, self.end_date))
+
+    async def to_pandas(self) -> pd.DataFrame:
         file = await self.source.read_pandas()
         return self.file_transformations(file)
 
-    async def _to_dask(self) -> dd.DataFrame:
-        file = await self.source.read_dask()
-        return self.file_transformations(file)
+    async def to_polars(self) -> pl.LazyFrame:
+        file = await self.source.to_polars()
+        return self.file_transform_polars(file)
 
 
 @dataclass
 class FileFactualJob(FactualRetrivalJob):
 
     source: DataFileReference
     requests: list[RetrivalRequest]
     facts: dict[str, list]
 
-    def file_transformations(self, df: GenericDataFrame) -> GenericDataFrame:
+    @property
+    def request_result(self) -> RequestResult:
+        return RequestResult.from_request_list(self.requests)
+
+    def file_transformations(self, df: pd.DataFrame) -> pd.DataFrame:
+        from aligned.data_source.batch_data_source import ColumnFeatureMappable
+
         all_features: set[Feature] = set()
         for request in self.requests:
             all_features.update(request.all_required_features)
 
         result = pd.DataFrame(self.facts)
 
         for request in self.requests:
@@ -129,14 +176,13 @@
             feature_df = feature_df.rename(
                 columns={org_name: wanted_name for org_name, wanted_name in zip(request_features, all_names)},
             )
             result.loc[set_mask, list(all_names)] = feature_df.reset_index(drop=True)
 
         return result
 
-    async def _to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
         file = await self.source.read_pandas()
         return self.file_transformations(file)
 
-    async def _to_dask(self) -> dd.DataFrame:
-        file = await self.source.read_dask()
-        return self.file_transformations(file)
+    async def to_polars(self) -> pl.LazyFrame:
+        return pl.from_pandas(await self.to_pandas())
```

### Comparing `aligned-0.0.8a0/aligned/local/source.py` & `aligned-0.0.9a0/aligned/local/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Literal
 from uuid import uuid4
 
 import pandas as pd
+import polars as pl
 from httpx import HTTPStatusError
 
 from aligned.data_file import DataFileReference
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.enricher import CsvFileEnricher, Enricher, LoadedStatEnricher, StatisticEricher, TimespanSelector
 from aligned.exceptions import UnableToFindFileException
 from aligned.feature_store import FeatureStore
@@ -78,14 +79,17 @@
                 self.path, sep=self.csv_config.seperator, compression=self.csv_config.compression
             )
         except FileNotFoundError:
             raise UnableToFindFileException()
         except HTTPStatusError:
             raise UnableToFindFileException()
 
+    async def to_polars(self) -> pl.LazyFrame:
+        return pl.scan_csv(self.path, sep=self.csv_config.seperator)
+
     async def write_pandas(self, df: pd.DataFrame) -> None:
         df.to_csv(
             self.path,
             sep=self.csv_config.seperator,
             compression=self.csv_config.compression,
             index=self.csv_config.should_write_index,
         )
@@ -270,7 +274,10 @@
     file: pd.DataFrame
 
     def job_group_key(self) -> str:
         return str(uuid4())
 
     async def read_pandas(self) -> pd.DataFrame:
         return self.file
+
+    async def to_polars(self) -> pl.LazyFrame:
+        return pl.from_pandas(self.file).lazy()
```

### Comparing `aligned-0.0.8a0/aligned/model.py` & `aligned-0.0.9a0/aligned/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import logging
+from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from typing import Callable
 
 from pandas import DataFrame
 
 from aligned.compiler.feature_factory import FeatureFactory
 from aligned.entity_data_source import EntityDataSource
-from aligned.request.retrival_request import FeatureRequest, RetrivalRequest
+from aligned.request.retrival_request import FeatureRequest
+from aligned.schemas.feature import FeatureReferance
+from aligned.schemas.model import Model as ModelSchema
 
 logger = logging.getLogger(__name__)
 
 
 class SqlEntityDataSource(EntityDataSource):
 
     url: str
@@ -40,40 +43,46 @@
         return DataFrame.from_records([dict(record) for record in records])
 
     async def last(self, days: int, hours: int, seconds: int) -> DataFrame:
         now = datetime.utcnow()
         return await self.all_in_range(now - timedelta(days=days, hours=hours, seconds=seconds), now)
 
 
-class ModelService:
-    feature_refs: set[str]
-    target_refs: set[str] | None
-
-    _name: str | None
-    entity_source: SqlEntityDataSource | None
-
-    @property
-    def name(self) -> str:
-        if not self._name:
-            raise ValueError('Model name is not set')
-        return self._name
-
-    def __init__(
-        self,
-        features: list[FeatureRequest],
-        targets: list[RetrivalRequest] | list[FeatureFactory] | None = None,
-        name: str | None = None,
-        entity_source: SqlEntityDataSource | None = None,
-    ) -> None:
-        self._name = name
-        self.entity_source = entity_source
-        self.feature_refs = set()
-        self.target_refs = set()
-        for request in features:
-            self.feature_refs.update({f'{request.name}:{feature}' for feature in request.features_to_include})
-        for request in targets or []:
-            if isinstance(targets, FeatureFactory):
-                self.target_refs = {f'{target}' for target in targets}
+@dataclass
+class Model:
+    features: set[FeatureRequest]
+    target: list[FeatureRequest] | FeatureFactory | None = field(default=None)
+    name: str | None = field(default=None)
+
+    def schema(self) -> ModelSchema:
+        if not self.name:
+            raise ValueError(
+                'Missing name for model. You man need to set it manually using the `name` property.'
+            )
+        features: set[FeatureReferance] = set()
+        targets: set[FeatureReferance] = set()
+
+        for request in self.features:
+            features.update(
+                {
+                    FeatureReferance(feature.name, request.name, feature.dtype)
+                    for feature in request.request_result.features
+                }
+            )
+
+        if self.target:
+            if isinstance(self.target, FeatureFactory):
+                targets.add(self.target.feature_referance())
             else:
-                self.target_refs.update(
-                    {f'{request.feature_view_name}:{feature}' for feature in request.all_feature_names}
-                )
+                for request in self.target:
+                    targets.update(
+                        {
+                            FeatureReferance(feature.name, request.name, feature.dtype)
+                            for feature in request.request_result.features
+                        }
+                    )
+
+        return ModelSchema(
+            name=self.name,
+            features=features,
+            targets=targets if targets else None,
+        )
```

### Comparing `aligned-0.0.8a0/aligned/online_source.py` & `aligned-0.0.9a0/aligned/online_source.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/psql/data_source.py` & `aligned-0.0.9a0/aligned/psql/data_source.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/psql/jobs.py` & `aligned-0.0.9a0/aligned/psql/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from abc import abstractproperty
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, TypeVar
 
 import pandas as pd
+import polars as pl
 
 from aligned.psql.data_source import PostgreSQLConfig, PostgreSQLDataSource
-from aligned.request.retrival_request import RetrivalRequest
+from aligned.request.retrival_request import RequestResult, RetrivalRequest
 from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob, RetrivalJob
 from aligned.schemas.feature import FeatureType
 
 logger = logging.getLogger(__name__)
 
 try:
     import dask.dataframe as dd
@@ -31,15 +32,15 @@
     @abstractproperty
     def config(self) -> PostgreSQLConfig:
         pass
 
     def build_request(self) -> SQLQuery:
         raise NotImplementedError()
 
-    async def _to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
         sql_request = self.build_request()
 
         try:
             from sqlalchemy import create_engine
             from sqlalchemy.engine import Engine
 
             engine: Engine = create_engine(self.config.url).execution_options(autocommit=True)
@@ -47,27 +48,30 @@
             engine.dispose()
             return df
         except Exception as error:
             logger.info(sql_request.sql)
             logger.error(error)
             raise error
 
-    async def _to_dask(self) -> dd.DataFrame:
-        df = await self._to_df()
-        return dd.from_pandas(df)
+    async def to_polars(self) -> pl.LazyFrame:
+        return pl.from_pandas(await self.to_pandas())
 
 
 @dataclass
 class FullExtractPsqlJob(PostgreSQLRetrivalJob, FullExtractJob):
 
     source: PostgreSQLDataSource
     request: RetrivalRequest
     limit: int | None = None
 
     @property
+    def request_result(self) -> RequestResult:
+        return RequestResult.from_request(self.request)
+
+    @property
     def config(self) -> PostgreSQLConfig:
         return self.source.config
 
     def build_request(self) -> SQLQuery:
 
         all_features = [
             feature.name for feature in list(self.request.all_required_features.union(self.request.entities))
@@ -94,14 +98,18 @@
 
     source: PostgreSQLDataSource
     start_date: datetime
     end_date: datetime
     request: RetrivalRequest
 
     @property
+    def request_result(self) -> RequestResult:
+        return RequestResult.from_request(self.request)
+
+    @property
     def config(self) -> PostgreSQLConfig:
         return self.source.config
 
     def build_request(self) -> SQLQuery:
 
         if not self.request.event_timestamp:
             raise ValueError('Event timestamp is needed in order to run a data range job')
@@ -124,20 +132,31 @@
             ),
             values={'start_date': self.start_date, 'end_date': self.end_date},
         )
 
 
 @dataclass
 class FactPsqlJob(PostgreSQLRetrivalJob, FactualRetrivalJob):
+    """Fetches features for defined facts within a postgres DB
+
+    It is supported to fetch from different tables, in one request
+    This is hy the `source` property is a dict with sources
+
+    NB: It is expected that the data sources are for the same psql instance
+    """
 
     sources: dict[str, PostgreSQLDataSource]
     requests: list[RetrivalRequest]
     facts: dict[str, list]
 
     @property
+    def request_result(self) -> RequestResult:
+        return RequestResult.from_request_list(self.requests)
+
+    @property
     def config(self) -> PostgreSQLConfig:
         return list(self.sources.values())[0].config
 
     def dtype_to_sql_type(self, dtype: object) -> str:
         if isinstance(dtype, str):
             return dtype
         if dtype == FeatureType('').string:
```

### Comparing `aligned-0.0.8a0/aligned/redis/config.py` & `aligned-0.0.9a0/aligned/redis/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         from aligned.redis.job import FactualRedisJob
 
         return FactualRedisJob(self.config, request.needed_requests, facts)
 
     async def write(self, job: RetrivalJob, requests: list[RetrivalRequest]) -> None:
 
         redis = self.config.redis()
-        data = await job.to_df()
+        data = await job.to_pandas()
 
         async with redis.pipeline(transaction=True) as pipe:
 
             written_count = 0
             # Run one query per row
             for request in requests:
                 entity_ids = (
```

### Comparing `aligned-0.0.8a0/aligned/redis/job.py` & `aligned-0.0.9a0/aligned/redis/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
+import polars as pl
 
 from aligned.redis.config import RedisConfig
 from aligned.request.retrival_request import RetrivalRequest
-from aligned.retrival_job import FactualRetrivalJob
+from aligned.retrival_job import FactualRetrivalJob, RequestResult
 from aligned.schemas.feature import FeatureType
 
-try:
-    import dask.dataframe as dd
-except ModuleNotFoundError:
-    import pandas as dd
-
 
 @dataclass
 class FactualRedisJob(FactualRetrivalJob):
 
     config: RedisConfig
     requests: list[RetrivalRequest]
     facts: dict[str, list]
 
-    async def _to_df(self) -> pd.DataFrame:
+    @property
+    def request_result(self) -> RequestResult:
+        return RequestResult.from_request_list(self.requests)
+
+    async def to_pandas(self) -> pd.DataFrame:
         redis = self.config.redis()
 
         result_df = pd.DataFrame(self.facts)
 
         for request in self.requests:
             for entity in request.entities:
                 if entity.dtype.is_numeric:
@@ -79,12 +79,9 @@
                 else:
                     result_df.loc[set_mask, feature.name] = result_series[result_value_mask].astype(
                         feature.dtype.pandas_type
                     )
 
         return result_df
 
-    async def to_df(self) -> pd.DataFrame:
-        return await self._to_df()
-
-    async def _to_dask(self) -> dd.DataFrame:
-        return await self._to_df()
+    async def to_polars(self) -> pl.LazyFrame:
+        return pl.from_pandas(await self.to_pandas())
```

### Comparing `aligned-0.0.8a0/aligned/redis/stream.py` & `aligned-0.0.9a0/aligned/redis/stream.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/redis/tests/test_redis_job.py` & `aligned-0.0.9a0/aligned/redis/tests/test_redis_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     job = FactualRedisJob(
         RedisConfig.localhost(),
         requests=[retrival_request],
         facts={'id_int': [1.0, 2.0, None, 4.0], 'id_str': ['a', 'b', 'c', None]},
     )
 
-    result = await job.to_df()
+    result = await job.to_pandas()
     redis_mock.assert_called_once()
     assert np.all(redis_mock.call_args[0][0] == ['test:1.0a:x', 'test:2.0b:x'])
     x_result = [int(value) for value in values] + [0, 0]
     assert np.all(result['x'].fillna(0).values == x_result)
 
 
 @pytest.mark.asyncio
@@ -57,15 +57,15 @@
 
     job = FactualRedisJob(
         RedisConfig.localhost(),
         requests=[retrival_request],
         facts={'id_int': ['1', '2', None, '4'], 'id_str': ['a', 'b', 'c', None]},
     )
 
-    result = await job.to_df()
+    result = await job.to_pandas()
     redis_mock.assert_called_once()
     assert np.all(redis_mock.call_args[0][0] == ['test:1.0a:x', 'test:2.0b:x'])
     x_result = [int(value) for value in values] + [0, 0]
     assert np.all(result['x'].fillna(0).values == x_result)
 
 
 @pytest.mark.asyncio
@@ -78,15 +78,15 @@
 
     job = FactualRedisJob(
         RedisConfig.localhost(),
         requests=[retrival_request],
         facts={'id_int': [None, '4'], 'id_str': ['c', None]},
     )
 
-    _ = await job.to_df()
+    _ = await job.to_pandas()
     redis_mock.assert_not_called()
 
 
 @pytest.mark.asyncio
 async def test_no_entities_job(mocker, retrival_request) -> None:  # type: ignore[no-untyped-def]
     values = ['20', '44']
     redis_values: Future = Future()
@@ -96,15 +96,15 @@
 
     job = FactualRedisJob(
         RedisConfig.localhost(),
         requests=[retrival_request],
         facts={'id_int': [], 'id_str': []},
     )
 
-    _ = await job.to_df()
+    _ = await job.to_pandas()
     redis_mock.assert_not_called()
 
 
 @pytest.mark.asyncio
 async def test_factual_redis_job_int_entity(mocker) -> None:  # type: ignore[no-untyped-def]
 
     retrival_request = RetrivalRequest(
@@ -125,12 +125,12 @@
 
     job = FactualRedisJob(
         RedisConfig.localhost(),
         requests=[retrival_request],
         facts={'id_int': [1.0, 2.0, 4.0, None]},
     )
 
-    result = await job.to_df()
+    result = await job.to_pandas()
     redis_mock.assert_called_once()
     assert np.all(redis_mock.call_args[0][0] == ['test:1.0:x', 'test:2.0:x', 'test:4.0:x'])
     x_result = [int(value) for value in values] + [0]
     assert np.all(result['x'].fillna(0).values == x_result)
```

### Comparing `aligned-0.0.8a0/aligned/redshift/data_source.py` & `aligned-0.0.9a0/aligned/redshift/data_source.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/redshift/factory.py` & `aligned-0.0.9a0/aligned/redshift/factory.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/request/retrival_request.py` & `aligned-0.0.9a0/aligned/request/retrival_request.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/request/tests/test_feature_request_generation.py` & `aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,38 +15,39 @@
         'sex',
         'survived',
         'sibsp',
         'cabin',
         'has_siblings',
         'is_male',
         'is_female',
-        'scaled_age',
         'is_mr',
     }
 
     assert not request.needs_event_timestamp
     assert len(request.needed_requests) == 1
 
     retrival_request = request.needed_requests[0]
-    assert retrival_request.all_feature_names == expected_features
+    missing_features = expected_features - retrival_request.all_feature_names
+    assert retrival_request.all_feature_names == expected_features, f'Missing features {missing_features}'
     assert retrival_request.entity_names == {'passenger_id'}
 
     assert len(request.request_result.entities) == 1
     assert len(request.request_result.features) == len(expected_features)
 
 
 @pytest.mark.asyncio
 async def test_fetch_features_request(titanic_feature_view: FeatureView) -> None:
 
     compiled_view = await type(titanic_feature_view).compile()
-    wanted_features = {'cabin', 'scaled_age', 'is_male'}
+    wanted_features = {'cabin', 'is_male'}
     request = compiled_view.request_for(wanted_features)
-    expected_features = {'age', 'sex', 'cabin', 'is_male', 'scaled_age'}
+    expected_features = {'sex', 'cabin', 'is_male'}
     assert not request.needs_event_timestamp
     assert len(request.needed_requests) == 1
 
     retrival_request = request.needed_requests[0]
-    assert retrival_request.all_feature_names == expected_features
+    missing_features = expected_features - retrival_request.all_feature_names
+    assert retrival_request.all_feature_names == expected_features, f'Missing features {missing_features}'
     assert retrival_request.entity_names == {'passenger_id'}
 
     assert len(request.request_result.entities) == 1
     assert len(request.request_result.features) == len(expected_features)
```

### Comparing `aligned-0.0.8a0/aligned/retrival_job.py` & `aligned-0.0.9a0/aligned/retrival_job.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,33 +2,25 @@
 
 import asyncio
 import logging
 from abc import ABC, abstractmethod, abstractproperty
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING
 
 import pandas as pd
+import polars as pl
 
+from aligned.exceptions import UnableToFindFileException
 from aligned.request.retrival_request import RequestResult, RetrivalRequest
-from aligned.schemas.derivied_feature import DerivedFeature
 from aligned.schemas.feature import FeatureType
 from aligned.split_strategy import SplitDataSet, SplitStrategy, TrainTestSet, TrainTestValidateSet
 from aligned.validation.interface import Validator
 
-try:
-    import dask.dataframe as dd
-
-    GenericDataFrame = TypeVar('GenericDataFrame', pd.DataFrame, dd.DataFrame)
-except ModuleNotFoundError:
-    GenericDataFrame = pd.DataFrame  # type: ignore
-
-from aligned.exceptions import UnableToFindFileException
-
 if TYPE_CHECKING:
     from aligned.local.source import DataFileReference
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -49,121 +41,148 @@
 
 class RetrivalJob(ABC):
     @abstractproperty
     def request_result(self) -> RequestResult:
         pass
 
     @abstractmethod
-    async def to_df(self) -> pd.DataFrame:
-        pass
+    async def to_pandas(self) -> pd.DataFrame:
+        raise NotImplementedError()
 
     @abstractmethod
-    async def to_dask(self) -> dd.DataFrame:
-        pass
+    async def to_polars(self) -> pl.LazyFrame:
+        raise NotImplementedError()
 
-    @abstractmethod
     def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
-        pass
+        if isinstance(location, str):
+            from aligned.local.source import ParquetFileSource
+
+            return FileCachedJob(ParquetFileSource(location), self)
+        else:
+            return FileCachedJob(location, self)
 
     def test_size(self, test_size: float, target_column: str) -> TrainTestSetJob:
 
         return TrainTestSetJob(job=self, test_size=test_size, target_column=target_column)
 
     def validate(self, validator: Validator) -> ValidationJob:
 
         return ValidationJob(self, validator)
 
+    def derive_features(self, requests: list[RetrivalRequest]) -> RetrivalJob:
+        return DerivedFeatureJob(job=self, requests=requests)
+
+    def ensure_types(self, requests: list[RetrivalRequest]) -> RetrivalJob:
+        return EnsureTypesJob(job=self, requests=requests)
+
 
 @dataclass
 class ValidationJob(RetrivalJob):
 
     job: RetrivalJob
     validator: Validator
 
     @property
     def request_result(self) -> RequestResult:
         return self.job.request_result
 
-    async def to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
         return await self.validator.validate_pandas(
-            list(self.request_result.features), await self.job.to_df()
+            list(self.request_result.features), await self.job.to_pandas()
         )
 
-    async def to_dask(self) -> dd.DataFrame:
+    async def to_polars(self) -> pl.LazyFrame:
         raise NotImplementedError()
 
     def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
         if isinstance(location, str):
             from aligned.local.source import ParquetFileSource
 
             return FileCachedJob(ParquetFileSource(location), self)
         else:
             return FileCachedJob(location, self)
 
 
+@dataclass
 class DerivedFeatureJob(RetrivalJob):
-    @abstractmethod
-    async def compute_derived_features(self, df: GenericDataFrame) -> GenericDataFrame:
-        pass
 
-    @abstractmethod
-    async def ensure_types(self, df: GenericDataFrame) -> GenericDataFrame:
-        pass
+    job: RetrivalJob
+    requests: list[RetrivalRequest]
 
-    @abstractmethod
-    async def _to_df(self) -> pd.DataFrame:
-        pass
+    @property
+    def request_result(self) -> RequestResult:
+        return self.job.request_result
 
-    @abstractmethod
-    async def _to_dask(self) -> dd.DataFrame:
-        pass
+    async def compute_derived_features_polars(self, df: pl.LazyFrame) -> pl.LazyFrame:
+        for request in self.requests:
+            for feature_round in request.derived_features_order():
+                for feature in feature_round:
+                    if feature.depending_on_views - {request.feature_view_name}:
+                        continue
+                    logger.info(f'Computing feature: {feature.name}')
+                    df = await feature.transformation.transform_polars(df, feature.name)
+        return df
 
-    async def to_df(self) -> pd.DataFrame:
-        df = await self._to_df()
-        df = await self.ensure_types(df)
-        return await self.compute_derived_features(df)
-
-    async def to_dask(self) -> dd.DataFrame:
-        df = await self._to_dask()
-        df = await self.ensure_types(df)
-        return await self.compute_derived_features(df)
+    async def compute_derived_features_pandas(self, df: pd.DataFrame) -> pd.DataFrame:
+        for request in self.requests:
+            for feature_round in request.derived_features_order():
+                for feature in feature_round:
+                    if feature.depending_on_views - {request.feature_view_name}:
+                        continue
 
-    def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
-        if isinstance(location, str):
-            from aligned.local.source import ParquetFileSource
+                    logger.info(f'Computing feature: {feature.name}')
+                    df[feature.name] = await feature.transformation.transform_pandas(
+                        df[feature.depending_on_names]
+                    )
+                    if df[feature.name].dtype != feature.dtype.pandas_type:
+                        if feature.dtype.is_numeric:
+                            df[feature.name] = pd.to_numeric(df[feature.name], errors='coerce').astype(
+                                feature.dtype.pandas_type
+                            )
+                        else:
+                            df[feature.name] = df[feature.name].astype(feature.dtype.pandas_type)
+        return df
 
-            return RawFileCachedJob(ParquetFileSource(location), self)
-        else:
-            return RawFileCachedJob(location, self)
+    async def to_pandas(self) -> pd.DataFrame:
+        return await self.compute_derived_features_pandas(await self.job.to_pandas())
+
+    async def to_polars(self) -> pl.LazyFrame:
+        return await self.compute_derived_features_polars(await self.job.to_polars())
 
 
 @dataclass
 class RawFileCachedJob(RetrivalJob):
 
     location: DataFileReference
     job: DerivedFeatureJob
 
     @property
     def request_result(self) -> RequestResult:
         return self.job.request_result
 
-    async def to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
+        from aligned.local.job import FileFullJob
+        from aligned.local.source import LiteralReference
+
         try:
             logger.info('Trying to read cache file')
             df = await self.location.read_pandas()
         except UnableToFindFileException:
             logger.info('Unable to load file, so fetching from source')
-            df = await self.job._to_df()
+            df = await self.job.job.to_pandas()
             logger.info('Writing result to cache')
             await self.location.write_pandas(df)
-        df = await self.job.ensure_types(df)
-        return await self.job.compute_derived_features(df)
+        return (
+            await FileFullJob(LiteralReference(df), request=self.job.requests[0])
+            .derive_features(self.job.requests)
+            .to_pandas()
+        )
 
-    async def to_dask(self) -> dd.DataFrame:
-        raise NotImplementedError()
+    async def to_polars(self) -> pl.LazyFrame:
+        return await self.job.to_polars()
 
     def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
         return self
 
 
 @dataclass
 class FileCachedJob(RetrivalJob):
@@ -171,27 +190,27 @@
     location: DataFileReference
     job: RetrivalJob
 
     @property
     def request_result(self) -> RequestResult:
         return self.job.request_result
 
-    async def to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
         try:
             logger.info('Trying to read cache file')
             df = await self.location.read_pandas()
         except UnableToFindFileException:
             logger.info('Unable to load file, so fetching from source')
-            df = await self.job.to_df()
+            df = await self.job.to_pandas()
             logger.info('Writing result to cache')
             await self.location.write_pandas(df)
         return df
 
-    async def to_dask(self) -> dd.DataFrame:
-        raise NotImplementedError()
+    async def to_polars(self) -> pl.LazyFrame:
+        return await super().to_polars()
 
     def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
         return self
 
 
 @dataclass
 class TrainTestSetJob:
@@ -202,15 +221,15 @@
 
     @property
     def request_result(self) -> RequestResult:
         return self.job.request_result
 
     async def use_df(self) -> TrainTestSet[pd.DataFrame]:
 
-        data = await self.job.to_df()
+        data = await self.job.to_pandas()
 
         features = list({feature.name for feature in self.request_result.features} - {self.target_column})
 
         test_ratio_start = 1 - self.test_size
         return TrainTestSet(
             data=data,
             features=features,
@@ -258,196 +277,157 @@
     strategy: SplitStrategy
 
     @property
     def request_result(self) -> RequestResult:
         return self.job.request_result
 
     async def use_pandas(self) -> SplitDataSet[pd.DataFrame]:
-        data = await self.job.to_df()
+        data = await self.job.to_pandas()
         return self.strategy.split_pandas(data, self.target_column)
 
 
-class SingleSourceRetrivalJob(DerivedFeatureJob):
-    request: RetrivalRequest
-
-    @property
-    def request_result(self) -> RequestResult:
-        return self.request.request_result
-
-    async def compute_derived_features(self, df: GenericDataFrame) -> GenericDataFrame:
-        for feature_round in self.request.derived_features_order():
-            for feature in feature_round:
-                df[feature.name] = await feature.transformation.transform(df[feature.depending_on_names])
-                if df[feature.name].dtype != feature.dtype.pandas_type:
-                    if feature.dtype.is_numeric:
-                        df[feature.name] = pd.to_numeric(df[feature.name], errors='coerce').astype(
-                            feature.dtype.pandas_type
-                        )
-                    else:
-                        df[feature.name] = df[feature.name].astype(feature.dtype.pandas_type)
-        return df
-
-    async def ensure_types(self, df: GenericDataFrame) -> GenericDataFrame:
-        for feature in self.request.all_required_features:
-            mask = ~df[feature.name].isnull()
-
-            with suppress(AttributeError):
-                df[feature.name] = df[feature.name].mask(
-                    ~mask, other=df.loc[mask, feature.name].str.strip('"')
-                )
-
-            if feature.dtype == FeatureType('').datetime:
-                if isinstance(df, pd.DataFrame):
-                    df[feature.name] = pd.to_datetime(df[feature.name], infer_datetime_format=True, utc=True)
-                else:
-                    df[feature.name] = dd.to_datetime(df[feature.name], infer_datetime_format=True, utc=True)
-            elif feature.dtype == FeatureType('').datetime or feature.dtype == FeatureType('').string:
-                continue
-            else:
-
-                if feature.dtype.is_numeric:
-                    df[feature.name] = pd.to_numeric(df[feature.name], errors='coerce').astype(
-                        feature.dtype.pandas_type
-                    )
-                else:
-                    df[feature.name] = df[feature.name].astype(feature.dtype.pandas_type)
-        return df
-
-
-class FullExtractJob(SingleSourceRetrivalJob):
+class FullExtractJob(RetrivalJob):
     limit: int | None
 
 
-class DateRangeJob(SingleSourceRetrivalJob):
+class DateRangeJob(RetrivalJob):
     start_date: datetime
     end_date: datetime
 
 
-class FactualRetrivalJob(DerivedFeatureJob):
+class FactualRetrivalJob(RetrivalJob):
+    facts: dict[str, list]
+
+
+@dataclass
+class EnsureTypesJob(RetrivalJob):
 
+    job: RetrivalJob
     requests: list[RetrivalRequest]
-    facts: dict[str, list]
 
     @property
     def request_result(self) -> RequestResult:
-        return RequestResult.from_request_list(self.requests)
-
-    async def compute_derived_features(self, df: GenericDataFrame) -> GenericDataFrame:
-        combined_views: list[DerivedFeature] = []
-        for request in self.requests:
-            for feature_round in request.derived_features_order():
-                for feature in feature_round:
-                    if feature.depending_on_views - {request.feature_view_name}:
-                        combined_views.append(feature)
-                        continue
-
-                    df[feature.name] = await feature.transformation.transform(df[feature.depending_on_names])
-                    if df[feature.name].dtype != feature.dtype.pandas_type:
-                        if feature.dtype.is_numeric:
-                            df[feature.name] = pd.to_numeric(df[feature.name], errors='coerce').astype(
-                                feature.dtype.pandas_type
-                            )
-                        else:
-                            df[feature.name] = df[feature.name].astype(feature.dtype.pandas_type)
-        return df
+        return self.job.request_result
 
-    async def ensure_types(self, df: GenericDataFrame) -> GenericDataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
+        df = await self.job.to_pandas()
         for request in self.requests:
             for feature in request.all_required_features:
 
-                # try:
-                #     if feature.dtype == FeatureType('').datetime:
-
-                #         if isinstance(df, pd.DataFrame):
-                #             df[feature.name] = pd.to_datetime(
-                #                 df[feature.name], infer_datetime_format=True, utc=True, errors='coerce'
-                #             )
-                #         else:
-                #             df[feature.name] = dd.to_datetime(
-                #                 df[feature.name], infer_datetime_format=True, utc=True
-                #             )
-                #     elif feature.dtype == FeatureType('').string:
-                #         continue
-                #     else:
-                #         if feature.dtype.is_numeric:
-                #             df[feature.name] = pd.to_numeric(df[feature.name], errors='coerce')
-                #         else:
-                #             df[feature.name] = df[feature.name].astype(feature.dtype.pandas_type)
-                # except ValueError as error:
-                #     logger.info(f'Unable to ensure type for {feature.name}, error: {error}')
-                #     continue
-
                 mask = ~df[feature.name].isnull()
 
                 with suppress(AttributeError):
                     df[feature.name] = df[feature.name].mask(
                         ~mask, other=df.loc[mask, feature.name].str.strip('"')
                     )
 
                 if feature.dtype == FeatureType('').datetime:
-                    if isinstance(df, pd.DataFrame):
-                        df[feature.name] = pd.to_datetime(
-                            df[feature.name], infer_datetime_format=True, utc=True
-                        )
-                    else:
-                        df[feature.name] = dd.to_datetime(
-                            df[feature.name], infer_datetime_format=True, utc=True
-                        )
+                    df[feature.name] = pd.to_datetime(df[feature.name], infer_datetime_format=True, utc=True)
                 elif feature.dtype == FeatureType('').datetime or feature.dtype == FeatureType('').string:
                     continue
                 else:
 
                     if feature.dtype.is_numeric:
                         df[feature.name] = pd.to_numeric(df[feature.name], errors='coerce').astype(
                             feature.dtype.pandas_type
                         )
                     else:
                         df[feature.name] = df[feature.name].astype(feature.dtype.pandas_type)
         return df
 
+    async def to_polars(self) -> pl.LazyFrame:
+        return await self.job.to_polars()
+
 
 @dataclass
 class CombineFactualJob(RetrivalJob):
+    """Computes features that depend on different retrical jobs
+
+    The `job` therefore take in a list of jobs that output some data,
+    and a `combined_requests` which defines the features depending on the data
+
+    one example would be the following
+
+    class SomeView(FeatureView):
+        metadata = FeatureViewMetadata(
+            name="some_view",
+            batch_source=FileSource.csv_at("data.csv")
+        )
+        id = Entity(Int32())
+        a = Int32()
+
+    class OtherView(FeatureView):
+        metadata = FeatureViewMetadata(
+            name="other_view",
+            batch_source=FileSource.parquet_at("other.parquet")
+        )
+        id = Entity(Int32())
+        c = Int32()
+
+    class Combined(CombinedFeatureView):
+        metadata = CombinedMetadata(name="combined")
+
+        some = SomeView()
+        other = OtherView()
+
+        added = some.a + other.c
+    """
 
     jobs: list[RetrivalJob]
     combined_requests: list[RetrivalRequest]
 
     @property
     def request_result(self) -> RequestResult:
         return RequestResult.from_result_list(
             [job.request_result for job in self.jobs]
         ) + RequestResult.from_request_list(self.combined_requests)
 
-    async def combine_data(self, df: GenericDataFrame) -> GenericDataFrame:
+    async def combine_data(self, df: pd.DataFrame) -> pd.DataFrame:
+        for request in self.combined_requests:
+            for feature in request.derived_features:
+                logger.info(f'Computing feature: {feature.name}')
+                df[feature.name] = await feature.transformation.transform_pandas(
+                    df[feature.depending_on_names]
+                )
+        return df
+
+    async def combine_polars_data(self, df: pl.LazyFrame) -> pl.LazyFrame:
         for request in self.combined_requests:
             for feature in request.derived_features:
-                df[feature.name] = await feature.transformation.transform(df[feature.depending_on_names])
+                logger.info(f'Computing feature: {feature.name}')
+                df = await feature.transformation.transform_polars(df, feature.name)
         return df
 
-    async def to_df(self) -> pd.DataFrame:
+    async def to_pandas(self) -> pd.DataFrame:
         job_count = len(self.jobs)
         if job_count > 1:
-            dfs = await asyncio.gather(*[job.to_df() for job in self.jobs])
+            dfs = await asyncio.gather(*[job.to_pandas() for job in self.jobs])
             df = pd.concat(dfs, axis=1)
             combined = await self.combine_data(df)
             return combined.loc[:, ~df.columns.duplicated()].copy()
         elif job_count == 1:
-            df = await self.jobs[0].to_df()
+            df = await self.jobs[0].to_pandas()
             return await self.combine_data(df)
         else:
             raise ValueError(
                 'Have no jobs to fetch. This is probably an internal error.\n'
                 'Please submit an issue, and describe how to reproduce it.\n'
                 'Or maybe even submit a PR'
             )
 
-    async def to_dask(self) -> dd.DataFrame:
-        dfs = await asyncio.gather(*[job.to_dask() for job in self.jobs])
-        df = dd.concat(dfs, axis=1)
-        return await self.combine_data(df)
+    async def to_polars(self) -> pl.LazyFrame:
+        dfs: list[pl.LazyFrame] = await asyncio.gather(*[job.to_polars() for job in self.jobs])
+
+        df = dfs[0]
+
+        for other_df in dfs[1:]:
+            df = df.with_context(other_df).select(pl.all())
+
+        # df = pl.concat(dfs_to_concat, how='horizontal')
+        return await self.combine_polars_data(df)
 
     def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
         return CombineFactualJob([job.cached_at(location) for job in self.jobs], self.combined_requests)
 
 
 @dataclass
 class FilterJob(RetrivalJob):
@@ -455,26 +435,26 @@
     include_features: set[str]
     job: RetrivalJob
 
     @property
     def request_result(self) -> RequestResult:
         return self.job.request_result.filter_features(self.include_features)
 
-    async def to_df(self) -> pd.DataFrame:
-        df = await self.job.to_df()
+    async def to_pandas(self) -> pd.DataFrame:
+        df = await self.job.to_pandas()
         if self.include_features:
             total_list = list({ent.name for ent in self.request_result.entities}.union(self.include_features))
             return df[total_list]
         else:
             return df
 
-    async def to_dask(self) -> dd.DataFrame:
-        df = await self.job.to_dask()
+    async def to_polars(self) -> pl.LazyFrame:
+        df = await self.job.to_polars()
         if self.include_features:
             total_list = list({ent.name for ent in self.request_result.entities}.union(self.include_features))
-            return df[total_list]
+            return df.select(total_list)
         else:
             return df
 
     def cached_at(self, location: DataFileReference | str) -> RetrivalJob:
 
         return FilterJob(self.include_features, self.job.cached_at(location))
```

### Comparing `aligned-0.0.8a0/aligned/s3/config.py` & `aligned-0.0.9a0/aligned/s3/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from dataclasses import dataclass
+from datetime import datetime
 from io import BytesIO
 
 import pandas as pd
-from aioaws.s3 import S3Config
 from httpx import HTTPStatusError
 
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.exceptions import UnableToFindFileException
+from aligned.local.job import FileDateJob, FileFullJob
 from aligned.local.source import CsvConfig, DataFileReference, ParquetConfig, StorageFileReference
+from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalRequest
 from aligned.s3.storage import AwsS3Storage
 from aligned.schemas.codable import Codable
 from aligned.storage import Storage
 
+try:
+    from aioaws.s3 import S3Config
+except ModuleNotFoundError:
+
+    class S3Config:  # type: ignore[no-redef]
+        pass
+
 
 @dataclass
 class AwsS3Config(Codable):
 
     access_token_env: str
     secret_token_env: str
     bucket_env: str
@@ -117,18 +126,31 @@
         except FileNotFoundError:
             raise UnableToFindFileException()
         except HTTPStatusError:
             raise UnableToFindFileException()
 
     async def write_pandas(self, df: pd.DataFrame) -> None:
         buffer = BytesIO()
-        df.to_csv(buffer, sep=self.csv_config.seperator, index=self.csv_config.should_write_index, compression=self.csv_config.compression)
+        df.to_csv(
+            buffer,
+            sep=self.csv_config.seperator,
+            index=self.csv_config.should_write_index,
+            compression=self.csv_config.compression,
+        )
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
 
+    def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
+        return FileFullJob(self, request=request, limit=limit)
+
+    def all_between_dates(
+        self, request: RetrivalRequest, start_date: datetime, end_date: datetime
+    ) -> DateRangeJob:
+        return FileDateJob(self, request, start_date, end_date)
+
 
 @dataclass
 class AwsS3ParquetDataSource(BatchDataSource, DataFileReference, ColumnFeatureMappable):
 
     config: AwsS3Config
     path: str
     mapping_keys: dict[str, str]  # = field(default_factory=dict)
```

### Comparing `aligned-0.0.8a0/aligned/s3/factory.py` & `aligned-0.0.9a0/aligned/s3/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from datetime import datetime
 
-from aligned.job_factory import JobFactory
 from aligned.local.job import FileDateJob, FileFactualJob, FileFullJob
 from aligned.request.retrival_request import RetrivalRequest
 from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob
 from aligned.s3.config import AwsS3CsvDataSource
 
 
-class AwsS3JobFactory(JobFactory):
+class AwsS3JobFactory:
 
     source = AwsS3CsvDataSource
 
     def all_data(
         self, source: AwsS3CsvDataSource, request: RetrivalRequest, limit: int | None
     ) -> FullExtractJob:
         return FileFullJob(source, request, limit)
```

### Comparing `aligned-0.0.8a0/aligned/s3/storage.py` & `aligned-0.0.9a0/aligned/s3/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING
 
-from aioaws.s3 import S3Client
+try:
+    from aioaws.s3 import S3Client
+except ModuleNotFoundError:
+
+    class S3Client:  # type: ignore[no-redef]
+        pass
+
 
 from aligned.storage import Storage
 
 if TYPE_CHECKING:
     from aligned.s3.config import AwsS3Config
```

### Comparing `aligned-0.0.8a0/aligned/schemas/constraints.py` & `aligned-0.0.9a0/aligned/schemas/constraints.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/schemas/derivied_feature.py` & `aligned-0.0.9a0/aligned/schemas/derivied_feature.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/schemas/feature.py` & `aligned-0.0.9a0/aligned/schemas/feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,11 +139,11 @@
 
 
 @dataclass
 class FeatureReferance(Codable):
     name: str
     feature_view: str
     dtype: FeatureType
-    is_derived: bool
+    # is_derived: bool
 
     def __hash__(self) -> int:
         return hash(self.name)
```

### Comparing `aligned-0.0.8a0/aligned/schemas/feature_view.py` & `aligned-0.0.9a0/aligned/schemas/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,30 +57,31 @@
         def dependent_features_for(
             feature: DerivedFeature,
         ) -> tuple[set[Feature], set[Feature]]:
             core_features = set()
             intermediate_features = set()
 
             for dep_ref in feature.depending_on:
-                if dep_ref.is_derived:
-                    dep_features = [feat for feat in self.derived_features if feat.name == dep_ref.name]
-                    if not dep_features:
-                        raise ValueError(
-                            'Unable to find the referenced feature. This is most likely a bug in the systemd'
-                        )
-                    dep_feature = dep_features[0]
-                    intermediate_features.add(dep_feature)
-                    core, intermediate = dependent_features_for(dep_feature)
-                    features.update(core)
-                    intermediate_features.update(intermediate)
-                else:
-                    dep_feature = [
-                        feat for feat in self.features.union(self.entities) if feat.name == dep_ref.name
-                    ][0]
-                    core_features.add(dep_feature)
+                dep_feature = [
+                    feat for feat in self.features.union(self.entities) if feat.name == dep_ref.name
+                ]
+                if len(dep_feature) == 1:
+                    core_features.add(dep_feature[0])
+                    continue
+
+                dep_features = [feat for feat in self.derived_features if feat.name == dep_ref.name]
+                if not dep_features:
+                    raise ValueError(
+                        'Unable to find the referenced feature. This is most likely a bug in the systemd'
+                    )
+                dep_feature = dep_features[0]
+                intermediate_features.add(dep_feature)
+                core, intermediate = dependent_features_for(dep_feature)
+                features.update(core)
+                intermediate_features.update(intermediate)
 
             return core_features, intermediate_features
 
         for dep_feature in derived_features.copy():
             core, intermediate = dependent_features_for(dep_feature)
             features.update(core)
             derived_features.update(intermediate)
```

### Comparing `aligned-0.0.8a0/aligned/schemas/repo_definition.py` & `aligned-0.0.9a0/aligned/schemas/repo_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from aligned.enricher import Enricher
 from aligned.online_source import OnlineSource
 from aligned.schemas.codable import Codable
 from aligned.schemas.feature_view import CompiledCombinedFeatureView, CompiledFeatureView
+from aligned.schemas.model import Model
 
 if TYPE_CHECKING:
     from fastapi import FastAPI
 
     from aligned.local.source import StorageFileReference
 
 
@@ -74,15 +75,15 @@
 @dataclass
 class RepoDefinition(Codable):
 
     online_source: OnlineSource
 
     feature_views: set[CompiledFeatureView] = field(default_factory=set)
     combined_feature_views: set[CompiledCombinedFeatureView] = field(default_factory=set)
-    models: dict[str, set[str]] = field(default_factory=dict)
+    models: set[Model] = field(default_factory=dict)
     enrichers: list[EnricherReference] = field(default_factory=list)
 
     @staticmethod
     async def from_file(file: StorageFileReference) -> RepoDefinition:
         repo = await file.read()
         return RepoDefinition.from_json(repo)
```

### Comparing `aligned-0.0.8a0/aligned/server.py` & `aligned-0.0.9a0/aligned/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,21 +90,22 @@
                 *[feature_store.feature_view(view_name).write(feature_values) for view_name in view_names]
             )
 
     @staticmethod
     def feature_view_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
         @app.post(f'/feature-views/{name}/all')
         async def all(limit: int | None = None) -> dict:
-            df = await feature_store.feature_view(name).all(limit=limit).to_df()
+            df = await feature_store.feature_view(name).all(limit=limit).to_pandas()
             df.replace(nan, value=None, inplace=True)
             return df.to_dict('list')
 
     @staticmethod
     def model_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
-        feature_request = feature_store.model_requests[name]
+        model = feature_store.model_requests[name]
+        feature_request = feature_store.requests_for_model(model)
 
         entities: set[Feature] = set()
         for request in feature_request.needed_requests:
             entities.update(request.entities)
 
         required_features = entities.copy()
         for request in feature_request.needed_requests:
@@ -147,15 +148,15 @@
                 entity_values['event_timestamp'] = [
                     datetime.fromtimestamp(value)
                     if isinstance(value, (float, int))
                     else datetime.fromisoformat(value)
                     for value in entity_values['event_timestamp']
                 ]
 
-            df = await feature_store.model(name).features_for(entity_values).to_df()
+            df = await feature_store.model(name).features_for(entity_values).to_pandas()
             orient = 'values'
             body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
             return Response(content=f'{{{body}}}', media_type='application/json')
 
     @staticmethod
     def app(feature_store: FeatureStore) -> FastAPI:
         from asgi_correlation_id import CorrelationIdMiddleware
@@ -203,15 +204,15 @@
             )
 
         @app.post('/features')
         async def features(payload: APIFeatureRequest) -> dict:
             df = await feature_store.features_for(
                 payload.entities,
                 features=payload.features,
-            ).to_df()
+            ).to_pandas()
             orient = 'values'
             body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
             return Response(content=f'{{{body}}}', media_type='application/json')
 
         return app
 
     @staticmethod
```

### Comparing `aligned-0.0.8a0/aligned/split_strategy.py` & `aligned-0.0.9a0/aligned/split_strategy.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/tests/test_cache_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_cache_enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/tests/test_cached_parquet.py` & `aligned-0.0.9a0/aligned/tests/test_cached_parquet.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from aligned import FeatureStore, FileSource
 
 
 @pytest.mark.asyncio
 async def test_cached_at(titanic_feature_store: FeatureStore) -> None:
     file_source = FileSource.parquet_at('test_data/titanic.parquet')
     data_set = (
-        await titanic_feature_store.feature_view('titanic_parquet').all().cached_at(file_source).to_df()
+        await titanic_feature_store.feature_view('titanic_parquet').all().cached_at(file_source).to_pandas()
     )
     cached = await file_source.read_pandas()
 
     assert cached.shape[0] == data_set.shape[0]
     assert (set(cached.columns).intersection(set(data_set.columns)) - set(cached.columns)) == set()
```

### Comparing `aligned-0.0.8a0/aligned/tests/test_statistic_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/tests/test_train_test_validate_set.py` & `aligned-0.0.9a0/aligned/tests/test_train_test_validate_set.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/aligned/tests/test_transformations.py` & `aligned-0.0.9a0/aligned/tests/test_transformations.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,27 @@
 
 
 @pytest.mark.asyncio
 async def test_transformations() -> None:
     supported = SupportedTransformations.shared()
 
     for transformation in supported.types.values():
-        await transformation.run_transformation_test()
+        await transformation.run_transformation_test_pandas()
+
+
+@pytest.mark.asyncio
+async def test_polars_transformation() -> None:
+    supported = SupportedTransformations.shared()
+
+    for transformation in supported.types.values():
+        await transformation.run_transformation_test_polars()
 
 
 @pytest.mark.asyncio
 async def test_transformations_in_feture_view(alot_of_transforation_feature_store: FeatureStore) -> None:
     store = alot_of_transforation_feature_store
 
     amount = 100
 
-    data = await store.feature_view('titanic').all(limit=amount).to_df()
+    data = await store.feature_view('titanic').all(limit=amount).to_pandas()
 
     assert data.shape[0] == amount
```

### Comparing `aligned-0.0.8a0/aligned/validation/pandera.py` & `aligned-0.0.9a0/aligned/validation/pandera.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,10 +50,13 @@
         except SchemaError as error:
             # Will only return one error at a time, so will remove
             # errors and then run it recrusive
 
             if error.failure_cases.shape[0] == df.shape[0]:
                 raise ValueError('Validation is removing all the data.')
 
+            if error.failure_cases['index'].iloc[0] is None:
+                raise ValueError(error)
+
             return await self.validate_pandas(
                 features, df.loc[df.index.delete(error.failure_cases['index'])].reset_index()
             )
```

### Comparing `aligned-0.0.8a0/aligned/validation/tests/test_pandera_validator.py` & `aligned-0.0.9a0/aligned/validation/tests/test_pandera_validator.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 from aligned import FeatureStore
 from aligned.validation.pandera import PanderaValidator
 
 
 @pytest.mark.asyncio
 async def test_validate_valid_feature_view(titanic_feature_store: FeatureStore) -> None:
-    original = await titanic_feature_store.feature_view('titanic').all(limit=5).to_df()
+    original = await titanic_feature_store.feature_view('titanic').all(limit=5).to_pandas()
     validated_df = (
-        await titanic_feature_store.feature_view('titanic').all(limit=5).validate(PanderaValidator()).to_df()
+        await titanic_feature_store.feature_view('titanic')
+        .all(limit=5)
+        .validate(PanderaValidator())
+        .to_pandas()
     )
 
     assert original.shape == validated_df.shape
 
 
 @pytest.mark.asyncio
 async def test_validate_invalid_feature_view(titanic_feature_store: FeatureStore) -> None:
     validated_df = (
-        await titanic_feature_store.feature_view('titanic').all(limit=20).validate(PanderaValidator()).to_df()
+        await titanic_feature_store.feature_view('titanic')
+        .all(limit=20)
+        .validate(PanderaValidator())
+        .to_pandas()
     )
 
     assert validated_df.shape[0] == 16
```

### Comparing `aligned-0.0.8a0/aligned/worker.py` & `aligned-0.0.9a0/aligned/worker.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.8a0/pyproject.toml` & `aligned-0.0.9a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligned"
-version = "0.0.8a"
+version = "0.0.9a"
 description = "A scalable feature store that makes it easy to align offline and online ML systems"
 authors = ["Mats E. Mollestad <mats@mollestad.no>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/otovo/aladdin"
 repository = "https://github.com/otovo/aladdin"
 keywords = [
@@ -53,14 +53,15 @@
 pyarrow = "^8.0.0"
 Jinja2 = "^3.1.2"
 nest-asyncio = "^1.5.5"
 asgi-correlation-id = { version = "^3.0.0", optional = true }
 dask = {version = "^2022.7.0", extras = ["dataframe"], optional = true}
 pandera = {version = "^0.13.3", optional = true}
 httpx = "^0.23.0"
+polars = { version = "^0.15.6", extras = ["all"] }
 
 [tool.poetry.extras]
 aws = ["aioaws", "databases"]
 psql = ["databases", "asyncpg"]
 redis = ["redis"]
 server = ["asgi-correlation-id", "fastapi", "uvicorn"]
 dask = ["dask"]
```

### Comparing `aligned-0.0.8a0/setup.py` & `aligned-0.0.9a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 packages = \
 ['aligned',
  'aligned.compiler',
  'aligned.data_source',
  'aligned.feature_view',
  'aligned.feature_view.tests',
+ 'aligned.jobs.tests',
  'aligned.local',
+ 'aligned.local.tests',
  'aligned.psql',
  'aligned.redis',
  'aligned.redis.tests',
  'aligned.redshift',
  'aligned.request',
  'aligned.request.tests',
  'aligned.s3',
@@ -27,14 +29,15 @@
 ['Jinja2>=3.1.2,<4.0.0',
  'click>=8.1.3,<9.0.0',
  'dill>=0.3.4,<0.4.0',
  'httpx>=0.23.0,<0.24.0',
  'mashumaro>=3.0.1,<4.0.0',
  'nest-asyncio>=1.5.5,<2.0.0',
  'pandas>=1.3.1,<2.0.0',
+ 'polars[all]>=0.15.6,<0.16.0',
  'pyarrow>=8.0.0,<9.0.0']
 
 extras_require = \
 {'aws': ['aioaws>=0.12,<0.13', 'databases>=0.5.5,<0.6.0'],
  'dask': ['dask[dataframe]>=2022.7.0,<2023.0.0'],
  'pandera': ['pandera>=0.13.3,<0.14.0'],
  'psql': ['databases>=0.5.5,<0.6.0', 'asyncpg>=0.25.0,<0.26.0'],
@@ -44,17 +47,17 @@
             'asgi-correlation-id>=3.0.0,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['aligned = aligned.cli:cli']}
 
 setup_kwargs = {
     'name': 'aligned',
-    'version': '0.0.8a0',
+    'version': '0.0.9a0',
     'description': 'A scalable feature store that makes it easy to align offline and online ML systems',
-    'long_description': '# Aligned\n\nA feature store alignes the offline and online features in a ML system. Therefore making it harder to achive a training-serving skew. However, that is only the beginning.\n\n## Feature Views\n\nWrite features as the should be, as data models.\nThen get code completion and typesafety by referencing them in other features.\n\nThis makes the features light weight, data source indipendent, and flexible.\n\n```python\nclass TitanicPassenger(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="passenger",\n        description="Some features from the titanic dataset",\n        batch_source=FileSource.csv_at("titanic.csv"),\n        stream_source=HttpStreamSource(topic_name="titanic")\n    )\n\n    passenger_id = Entity(dtype=Int32())\n\n    # Input values\n    age = (\n        Float()\n            .description("A float as some have decimals")\n            .is_required()\n            .lower_bound(0)\n            .upper_bound(110)\n    )\n\n    name = String()\n    sex = String().accepted_values(["male", "female"])\n    survived = Bool().description("If the passenger survived")\n    sibsp = Int32().lower_bound(0, is_inclusive=True).description("Number of siblings on titanic")\n    cabin = String()\n\n    # Creates two one hot encoded values\n    is_male, is_female = sex.one_hot_encode([\'male\', \'female\'])\n\n    # Standard scale the age.\n    # This will fit the scaler using a data slice from the batch source\n    # limited to maximum 100 rows. We can also uese a time constraint if wanted\n    scaled_age = age.standard_scaled(limit=100)\n```\n\n## Data sources\n\nAlinged makes handling data sources easy, as you do not have to think about how it is done.\nOnly define where the data is, and we handle the dirty work.\n\n```python\nmy_db = PostgreSQLConfig(env_var="DATABASE_URL")\n\nclass TitanicPassenger(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="passenger",\n        description="Some features from the titanic dataset",\n        batch_source=my_db.table(\n            "passenger",\n            mapping_keys={\n                "Passenger_Id": "passenger_id"\n            }\n        ),\n        stream_source=HttpStreamSource(topic_name="titanic")\n    )\n\n    passenger_id = Entity(dtype=Int32())\n```\n\n### Fast development\n\nMaking iterativ and fast exploration in ML is important. This is why Aligned also makes it super easy to combine, and test multiple sources.\n\n```python\nmy_db = PostgreSQLConfig.localhost()\n\naws_bucket = AwsS3Config(...)\n\nclass SomeFeatures(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="some_features",\n        description="...",\n        batch_source=my_db.table("local_features")\n    )\n\n    # Some features\n    ...\n\nclass AwsFeatures(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="aws",\n        description="...",\n        batch_source=aws_bucket.file_at("path/to/file.parquet")\n    )\n\n    # Some features\n    ...\n```\n\n## Model Service\n\nUsually will you need to combine multiple features for each model.\nThis is where a `ModelService` comes in.\nHere can you define which features should be exposed.\n\n```python\n# Uses the variable name, as the model service name.\n# Can also define a custom name, if wanted.\ntitanic_model = ModelService(\n    features=[\n        TitanicPassenger.select_all(),\n\n        # Select features with code completion\n        LocationFeatures.select(lambda view: [\n            view.distance_to_shore,\n            view.distance_to_closest_boat\n        ]),\n    ]\n)\n```\n\n\n## Data Enrichers\n\nIn manny cases will extra data be needed in order to generate some features.\nWe therefore need some way of enriching the data.\nThis can easily be done with Alinged\'s `DataEnricher`s.\n\n```python\nmy_db = PostgreSQLConfig.localhost()\nredis = RedisConfig.localhost()\n\nuser_location = my_db.data_enricher( # Fetch all user locations\n    sql="SELECT * FROM user_location"\n).cache( # Cache them for one day\n    ttl=timedelta(days=1),\n    cache_key="user_location_cache"\n).lock( # Make sure only one processer fetches the data at a time\n    lock_name="user_location_lock",\n    redis_config=redis\n)\n\n\nasync def distance_to_users(df: DataFrame) -> Series:\n    user_location_df = await user_location.load()\n    ...\n    return distances\n\nclass SomeFeatures(FeatureView):\n\n    metadata = FeatureViewMetadata(...)\n\n    latitude = Float()\n    longitude = Float()\n\n    distance_to_users = Float().transformed(distance_to_users, using_features=[latitude, longitude])\n```\n\n\n## Access Data\n\nYou can easily create a feature store that contains all your feature definitions.\nThis can then be used to genreate data sets, setup an instce to serve features, DAG\'s etc.\n\n```python\nstore = FeatureStore.from_dir(".")\n\n# Select all features from a single feature view\ndf = await store.all_for("passenger", limit=100).to_df()\n```\n\n### Centraliced Feature Store Definition\nYou would often share the features with other coworkers, or split them into different stages, like `staging`, `shadow`, or `production`.\nOne option is therefore to reference the storage you use, and load the `FeatureStore` from there.\n\n```python\naws_bucket = AwsS3Config(...)\nstore = await aws_bucket.file_at("production.json").feature_store()\n\n# This switches from the production online store to the offline store\n# Aka. the batch sources defined on the feature views\nexperimental_store = store.offline_store()\n```\nThis json file can be generated by running `alinged apply`.\n\n### Select multiple feature views\n\n```python\ndf = await store.features_for({\n    "passenger_id": [1, 50, 110]\n}, features=[\n    "passenger:scaled_age",\n    "passenger:is_male",\n    "passenger:sibsp"\n\n    "other_features:distance_to_closest_boat",\n]).to_df()\n```\n\n### Model Service\n\nSelecting features for a model is super simple.\n\n\n```python\ndf = await store.model("titanic_model").features_for({\n    "passenger_id": [1, 50, 110]\n}).to_df()\n```\n\n### Feature View\n\nIf you want to only select features for a specific feature view, then this is also possible.\n\n```python\nprev_30_days = await store.feature_view("match").previous(days=30).to_df()\nsample_of_20 = await store.feature_view("match").all(limit=20).to_df()\n```\n\n## Data quality\nAlinged will make sure all the different features gets formatted as the correct datatype.\nIn addition will aligned also make sure that the returend features aligne with defined constraints.\n\n```python\nclass TitanicPassenger(FeatureView):\n\n    ...\n\n    age = (\n        Float()\n            .is_required()\n            .lower_bound(0)\n            .upper_bound(110)\n    )\n    sibsp = Int32().lower_bound(0, is_inclusive=True)\n```\n\nThen since our feature view have a `is_required` and a `lower_bound`, will the `.validate(...)` command filter out the entites that do not follow that behavior.\n\n```python\nfrom aligned.validation.pandera import PanderaValidator\n\ndf = await store.model("titanic_model").features_for({\n    "passenger_id": [1, 50, 110]\n}).validate(\n    PanderaValidator()  # Validates all features\n).to_df()\n```\n\n## Feature Server\n\nThis expectes that you either run the command in your feature store repo, or have a file with a `RepoReference` instance.\nYou can also setup an online source like Redis, for faster storage.\n\n```python\nredis = RedisConfig.localhost()\n\naws_bucket = AwsS3Config(...)\n\nrepo_files = RepoReference(\n    env_var_name="ENVIRONMENT",\n    repo_paths={\n        "production": aws_bucket.file_at("feature-store/production.json"),\n        "shadow": aws_bucket.file_at("feature-store/shadow.json"),\n        "staging": aws_bucket.file_at("feature-store/staging.json")\n        # else generate the feature store from the current dir\n    }\n)\n\n# Use redis as the online source, if not running localy\nif repo_files.selected != "local":\n    online_source = redis.online_source()\n```\n\nThen run `aligned serve`, and a FastAPI server will start. Here can you push new features, which then transforms and stores the features, or just fetch them.\n',
+    'long_description': '# Aligned\n\nAligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.\n\nRead the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)\n\nAlso check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used\n\n⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.\n\n## Feature Views\n\nWrite features as the should be, as data models.\nThen get code completion and typesafety by referencing them in other features.\n\nThis makes the features light weight, data source indipendent, and flexible.\n\n```python\nclass TitanicPassenger(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="passenger",\n        description="Some features from the titanic dataset",\n        batch_source=FileSource.csv_at("titanic.csv"),\n        stream_source=HttpStreamSource(topic_name="titanic")\n    )\n\n    passenger_id = Entity(dtype=Int32())\n\n    # Input values\n    age = (\n        Float()\n            .description("A float as some have decimals")\n            .is_required()\n            .lower_bound(0)\n            .upper_bound(110)\n    )\n\n    name = String()\n    sex = String().accepted_values(["male", "female"])\n    survived = Bool().description("If the passenger survived")\n    sibsp = Int32().lower_bound(0, is_inclusive=True).description("Number of siblings on titanic")\n    cabin = String()\n\n    # Creates two one hot encoded values\n    is_male, is_female = sex.one_hot_encode([\'male\', \'female\'])\n\n    # Standard scale the age.\n    # This will fit the scaler using a data slice from the batch source\n    # limited to maximum 100 rows. We can also uese a time constraint if wanted\n    scaled_age = age.standard_scaled(limit=100)\n```\n\n## Data sources\n\nAlinged makes handling data sources easy, as you do not have to think about how it is done.\nOnly define where the data is, and we handle the dirty work.\n\n```python\nmy_db = PostgreSQLConfig(env_var="DATABASE_URL")\n\nclass TitanicPassenger(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="passenger",\n        description="Some features from the titanic dataset",\n        batch_source=my_db.table(\n            "passenger",\n            mapping_keys={\n                "Passenger_Id": "passenger_id"\n            }\n        ),\n        stream_source=HttpStreamSource(topic_name="titanic")\n    )\n\n    passenger_id = Entity(dtype=Int32())\n```\n\n### Fast development\n\nMaking iterativ and fast exploration in ML is important. This is why Aligned also makes it super easy to combine, and test multiple sources.\n\n```python\nmy_db = PostgreSQLConfig.localhost()\n\naws_bucket = AwsS3Config(...)\n\nclass SomeFeatures(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="some_features",\n        description="...",\n        batch_source=my_db.table("local_features")\n    )\n\n    # Some features\n    ...\n\nclass AwsFeatures(FeatureView):\n\n    metadata = FeatureViewMetadata(\n        name="aws",\n        description="...",\n        batch_source=aws_bucket.file_at("path/to/file.parquet")\n    )\n\n    # Some features\n    ...\n```\n\n## Model Service\n\nUsually will you need to combine multiple features for each model.\nThis is where a `ModelService` comes in.\nHere can you define which features should be exposed.\n\n```python\n# Uses the variable name, as the model service name.\n# Can also define a custom name, if wanted.\ntitanic_model = ModelService(\n    features=[\n        TitanicPassenger.select_all(),\n\n        # Select features with code completion\n        LocationFeatures.select(lambda view: [\n            view.distance_to_shore,\n            view.distance_to_closest_boat\n        ]),\n    ]\n)\n```\n\n\n## Data Enrichers\n\nIn manny cases will extra data be needed in order to generate some features.\nWe therefore need some way of enriching the data.\nThis can easily be done with Alinged\'s `DataEnricher`s.\n\n```python\nmy_db = PostgreSQLConfig.localhost()\nredis = RedisConfig.localhost()\n\nuser_location = my_db.data_enricher( # Fetch all user locations\n    sql="SELECT * FROM user_location"\n).cache( # Cache them for one day\n    ttl=timedelta(days=1),\n    cache_key="user_location_cache"\n).lock( # Make sure only one processer fetches the data at a time\n    lock_name="user_location_lock",\n    redis_config=redis\n)\n\n\nasync def distance_to_users(df: DataFrame) -> Series:\n    user_location_df = await user_location.load()\n    ...\n    return distances\n\nclass SomeFeatures(FeatureView):\n\n    metadata = FeatureViewMetadata(...)\n\n    latitude = Float()\n    longitude = Float()\n\n    distance_to_users = Float().transformed(distance_to_users, using_features=[latitude, longitude])\n```\n\n\n## Access Data\n\nYou can easily create a feature store that contains all your feature definitions.\nThis can then be used to genreate data sets, setup an instce to serve features, DAG\'s etc.\n\n```python\nstore = FeatureStore.from_dir(".")\n\n# Select all features from a single feature view\ndf = await store.all_for("passenger", limit=100).to_df()\n```\n\n### Centraliced Feature Store Definition\nYou would often share the features with other coworkers, or split them into different stages, like `staging`, `shadow`, or `production`.\nOne option is therefore to reference the storage you use, and load the `FeatureStore` from there.\n\n```python\naws_bucket = AwsS3Config(...)\nstore = await aws_bucket.file_at("production.json").feature_store()\n\n# This switches from the production online store to the offline store\n# Aka. the batch sources defined on the feature views\nexperimental_store = store.offline_store()\n```\nThis json file can be generated by running `alinged apply`.\n\n### Select multiple feature views\n\n```python\ndf = await store.features_for({\n    "passenger_id": [1, 50, 110]\n}, features=[\n    "passenger:scaled_age",\n    "passenger:is_male",\n    "passenger:sibsp"\n\n    "other_features:distance_to_closest_boat",\n]).to_df()\n```\n\n### Model Service\n\nSelecting features for a model is super simple.\n\n\n```python\ndf = await store.model("titanic_model").features_for({\n    "passenger_id": [1, 50, 110]\n}).to_df()\n```\n\n### Feature View\n\nIf you want to only select features for a specific feature view, then this is also possible.\n\n```python\nprev_30_days = await store.feature_view("match").previous(days=30).to_df()\nsample_of_20 = await store.feature_view("match").all(limit=20).to_df()\n```\n\n## Data quality\nAlinged will make sure all the different features gets formatted as the correct datatype.\nIn addition will aligned also make sure that the returend features aligne with defined constraints.\n\n```python\nclass TitanicPassenger(FeatureView):\n\n    ...\n\n    age = (\n        Float()\n            .is_required()\n            .lower_bound(0)\n            .upper_bound(110)\n    )\n    sibsp = Int32().lower_bound(0, is_inclusive=True)\n```\n\nThen since our feature view have a `is_required` and a `lower_bound`, will the `.validate(...)` command filter out the entites that do not follow that behavior.\n\n```python\nfrom aligned.validation.pandera import PanderaValidator\n\ndf = await store.model("titanic_model").features_for({\n    "passenger_id": [1, 50, 110]\n}).validate(\n    PanderaValidator()  # Validates all features\n).to_df()\n```\n\n## Feature Server\n\nThis expectes that you either run the command in your feature store repo, or have a file with a `RepoReference` instance.\nYou can also setup an online source like Redis, for faster storage.\n\n```python\nredis = RedisConfig.localhost()\n\naws_bucket = AwsS3Config(...)\n\nrepo_files = RepoReference(\n    env_var_name="ENVIRONMENT",\n    repo_paths={\n        "production": aws_bucket.file_at("feature-store/production.json"),\n        "shadow": aws_bucket.file_at("feature-store/shadow.json"),\n        "staging": aws_bucket.file_at("feature-store/staging.json")\n        # else generate the feature store from the current dir\n    }\n)\n\n# Use redis as the online source, if not running localy\nif repo_files.selected != "local":\n    online_source = redis.online_source()\n```\n\nThen run `aligned serve`, and a FastAPI server will start. Here can you push new features, which then transforms and stores the features, or just fetch them.\n',
     'author': 'Mats E. Mollestad',
     'author_email': 'mats@mollestad.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/otovo/aladdin',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aligned-0.0.8a0/PKG-INFO` & `aligned-0.0.9a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligned
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: A scalable feature store that makes it easy to align offline and online ML systems
 Home-page: https://github.com/otovo/aladdin
 License: Apache-2.0
 Keywords: python,typed,ml,prediction,feature,store,feature-store,feast,tecton
 Author: Mats E. Mollestad
 Author-email: mats@mollestad.no
 Requires-Python: >=3.10,<4.0
@@ -41,23 +41,30 @@
 Requires-Dist: dill (>=0.3.4,<0.4.0)
 Requires-Dist: fastapi (>=0.77.1,<0.78.0) ; extra == "server"
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: mashumaro (>=3.0.1,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
 Requires-Dist: pandas (>=1.3.1,<2.0.0)
 Requires-Dist: pandera (>=0.13.3,<0.14.0) ; extra == "pandera"
+Requires-Dist: polars[all] (>=0.15.6,<0.16.0)
 Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0) ; extra == "redis"
 Requires-Dist: uvicorn (>=0.17.6,<0.18.0) ; extra == "server"
 Project-URL: Repository, https://github.com/otovo/aladdin
 Description-Content-Type: text/markdown
 
 # Aligned
 
-A feature store alignes the offline and online features in a ML system. Therefore making it harder to achive a training-serving skew. However, that is only the beginning.
+Aligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.
+
+Read the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)
+
+Also check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used
+
+⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.
 
 ## Feature Views
 
 Write features as the should be, as data models.
 Then get code completion and typesafety by referencing them in other features.
 
 This makes the features light weight, data source indipendent, and flexible.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

