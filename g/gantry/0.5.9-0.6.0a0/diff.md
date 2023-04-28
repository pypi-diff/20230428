# Comparing `tmp/gantry-0.5.9.tar.gz` & `tmp/gantry-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.5.9.tar", last modified: Mon Mar 13 18:14:59 2023, max compression
+gzip compressed data, was "gantry-0.6.0a0.tar", last modified: Fri Apr 28 20:06:25 2023, max compression
```

## Comparing `gantry-0.5.9.tar` & `gantry-0.6.0a0.tar`

### file list

```diff
@@ -1,146 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.012965 gantry-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-03-13 18:14:48.000000 gantry-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 18:14:48.000000 gantry-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 18:14:59.012965 gantry-0.5.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.000965 gantry-0.5.9/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.000965 gantry-0.5.9/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.000965 gantry-0.5.9/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26153 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/curators/stock_curators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64418 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49786 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.004965 gantry-0.5.9/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-13 18:14:48.000000 gantry-0.5.9/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.000965 gantry-0.5.9/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 18:14:58.000000 gantry-0.5.9/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-13 18:14:58.000000 gantry-0.5.9/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 18:14:58.000000 gantry-0.5.9/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-13 18:14:58.000000 gantry-0.5.9/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-13 18:14:58.000000 gantry-0.5.9/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 18:14:58.000000 gantry-0.5.9/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 18:14:59.012965 gantry-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-13 18:14:48.000000 gantry-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.008965 gantry-0.5.9/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49160 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.012965 gantry-0.5.9/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    72641 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.012965 gantry-0.5.9/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.012965 gantry-0.5.9/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28690 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.012965 gantry-0.5.9/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:59.012965 gantry-0.5.9/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-13 18:14:48.000000 gantry-0.5.9/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.501926 gantry-0.6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-28 20:06:13.000000 gantry-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 20:06:13.000000 gantry-0.6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 20:06:25.501926 gantry-0.6.0a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.461925 gantry-0.6.0a0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.465925 gantry-0.6.0a0/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.465925 gantry-0.6.0a0/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.469925 gantry-0.6.0a0/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.469925 gantry-0.6.0a0/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.473925 gantry-0.6.0a0/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.473925 gantry-0.6.0a0/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.477926 gantry-0.6.0a0/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64417 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.477926 gantry-0.6.0a0/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.481926 gantry-0.6.0a0/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93859 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.481926 gantry-0.6.0a0/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.465925 gantry-0.6.0a0/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:06:25.501926 gantry-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 20:06:13.000000 gantry-0.6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.489926 gantry-0.6.0a0/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.489926 gantry-0.6.0a0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.489926 gantry-0.6.0a0/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.493926 gantry-0.6.0a0/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.493926 gantry-0.6.0a0/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.497926 gantry-0.6.0a0/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72641 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.497926 gantry-0.6.0a0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.497926 gantry-0.6.0a0/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.501926 gantry-0.6.0a0/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.501926 gantry-0.6.0a0/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_validator.py
```

### Comparing `gantry-0.5.9/LICENSE` & `gantry-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/PKG-INFO` & `gantry-0.6.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.5.9
+Version: 0.6.0a0
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.5.9/gantry/__init__.py` & `gantry-0.6.0a0/gantry/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+import os
 from typing import Optional
 
 from gantry.alerts.main import _init as alerts_init
-from gantry.curators.main import _init as curators_init
+from gantry.applications.main import _init as applications_init
+from gantry.applications.main import (
+    archive_application,
+    create_application,
+    delete_application,
+    get_application,
+)
+from gantry.automations.curators.main import _init as curators_init
+from gantry.automations.main import _init as automations_init
 from gantry.dataset.main import _init as dataset_init
 from gantry.logger.main import LOGGING_LEVEL_T
 from gantry.logger.main import _init as logger_init
 from gantry.logger.main import (
     get_client,
     log_file,
     log_from_data_connector,
@@ -29,14 +38,18 @@
     "ping",
     "ready",
     "get_client",
     "setup_logger",
     "compute_feedback_id",
     "JoinKey",
     "_version",
+    "create_application",
+    "get_application",
+    "delete_application",
+    "archive_application",
 ]
 
 
 def init(
     api_key: Optional[str] = None,
     logging_level: Optional[LOGGING_LEVEL_T] = None,
     environment: Optional[str] = None,
@@ -72,12 +85,28 @@
             in the ingestion methods.
         send_in_background (optional, bool): set whether Gantry logging methods should
             run synchronously or not. You can also set this value by setting
             the env variable GANTRY_SEND_IN_BACKGROUND.
             If not provided, it defaults to True unless running in an AWS lambda.
 
     """
+    api_key = _get_api_key(api_key)
     logger_init(api_key, logging_level, environment, send_in_background)
     query_init(api_key)
     alerts_init(api_key)
     curators_init(api_key)
     dataset_init(api_key)
+    applications_init(api_key)
+    automations_init(api_key)
+
+
+def _get_api_key(api_key: Optional[str] = None) -> str:
+    """
+    Get API key from environment if not already supplied. Raise exception if not found.
+    """
+    api_key = api_key or os.environ.get("GANTRY_API_KEY")
+    if api_key is None:
+        raise ValueError(
+            "Please provide an API key to initialize Gantry SDK. API key can be provided"
+            + "as parameter to init methods or by setting env var GANTRY_API_KEY"
+        )
+    return api_key
```

### Comparing `gantry-0.5.9/gantry/alerts/client.py` & `gantry-0.6.0a0/gantry/alerts/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/alerts/globals.py` & `gantry-0.6.0a0/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/alerts/main.py` & `gantry-0.6.0a0/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/api_client.py` & `gantry-0.6.0a0/gantry/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         files=None,
         headers=None,
         timeout=None,
         proxies=None,
         verify=None,
         json=None,
         raise_for_status: bool = False,
+        raw_response: bool = False,
     ):
         """
         If raise_for_status is True, the method will raise GantryRequestException if the response
         status code is >= 400
         """
         url = urljoin(self._host, path)
 
@@ -77,15 +78,15 @@
         logger.debug("Response: [%s]", response.status_code)
         logger.debug(response.text.strip("\n"))  # Remove newlines not to mess up with tracing tools
 
         if raise_for_status and response.status_code >= 400:
             raise GantryRequestException(url, response.status_code, response.text)
 
         try:
-            return response.json()
+            return response.json() if not raw_response else response
         except Exception as e:
             logger.debug(f"Invalid json response: {response.text} [{str(e)}]")
             return {"response": response.status_code, "error": response.status_code}
 
 
 class LocalClient(APIClient):
     """For testing purposes only"""
```

### Comparing `gantry-0.5.9/gantry/cli/application.py` & `gantry-0.6.0a0/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/cli/bucket.py` & `gantry-0.6.0a0/gantry/cli/bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import click
 from click_aliases import ClickAliasedGroup
 
 import gantry
 from gantry.api_client import APIClient
 from gantry.utils import check_response_status
 
+STORAGE_TYPES = ["S3", "GCS"]
+
 
 @click.group(cls=ClickAliasedGroup)
 def bucket():
     """
     Use this to manage your bucket with gantry.
     """
 
@@ -20,18 +22,18 @@
     help="Register your bucket with Gantry.",
 )
 @click.option("--name", type=click.STRING, required=True, help="Bucket name")
 @click.option(
     "--region",
     type=click.STRING,
     required=True,
-    help="Region of your bucket, for GS you can set this to auto",
+    help="Region of your bucket, for GCS buckets you can set this to auto",
 )
 @click.option(
-    "--storage-type", required=True, type=click.Choice(["S3", "GS"], case_sensitive=False)
+    "--storage-type", required=True, type=click.Choice(STORAGE_TYPES, case_sensitive=False)
 )
 @click.option("--secret", default=None, type=click.STRING, help="Secret name")
 def create(name: str, region: str, storage_type: str, secret: Optional[str]):
     gantry.init()
     api_client = gantry.get_client().log_store._api_client
     data = {
         "bucket_name": name,
@@ -65,15 +67,15 @@
 
 @bucket.command(
     aliases=["update-secrete"],
     help="Update bucket secret key.",
 )
 @click.option("--bucket", type=click.STRING, required=True, help="Bucket name")
 @click.option(
-    "--storage-type", required=True, type=click.Choice(["S3", "GS"], case_sensitive=False)
+    "--storage-type", required=True, type=click.Choice(STORAGE_TYPES, case_sensitive=False)
 )
 @click.option("--secret-id", type=click.STRING, default=None, help="Secret id")
 def update_secret(bucket: str, storage_type: str, secret_id: Optional[str]):
     gantry.init()
     api_client = gantry.get_client().log_store._api_client
     bucket_id = _get_bucket_id(api_client, bucket, storage_type.upper())
     data = {}
```

### Comparing `gantry-0.5.9/gantry/cli/data_connector.py` & `gantry-0.6.0a0/gantry/cli/data_connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from typing import Optional
+
 import click
 from click_aliases import ClickAliasedGroup
 
 import gantry
 from gantry.api_client import APIClient
 
 
@@ -21,37 +22,59 @@
 )
 @click.option(
     "--name", type=click.STRING, required=True, help="A unique name of the data connector"
 )
 @click.option(
     "--connection-type",
     type=click.Choice(
-        ["SNOWFLAKE", "BIGQUERY", "S3"],
+        ["SNOWFLAKE", "S3"],
         case_sensitive=False,
     ),
     required=True,
     help="Type of the source data connection",
 )
 @click.option(
-    "--database-name", type=click.STRING, required=True, help="Name of the source database"
+    "--database-name",
+    type=click.STRING,
+    required=False,
+    default="",
+    help="Name of the source database. WARNING: this field is DEPRECATED and will be removed in a "
+    "future release. Please provide database name to 'options' field.",
 )
 @click.option(
     "--secret-name",
     type=click.STRING,
     required=True,
     help="Name of the secret registered with Gantry",
 )
 @click.option(
     "--description", type=click.STRING, required=True, help="Description of the data connector"
 )
 @click.option(
     "--options",
     type=click.STRING,
     required=True,
-    help="JSON string of the options for the data connector",
+    help="""
+JSON string of the options for the data connector.
+
+For SNOWFLAKE connection type, the options should be:
+    {
+        "snowflake_database_name": "string",
+        "snowflake_schema_name": "string",
+        "snowflake_table_name": "string"
+    }
+
+For S3 connection type, the options should be:
+    {
+        "s3_bucket_name": "string",
+        "s3_path_prefix": "string",
+        "s3_filetype": "string",
+    }
+    S3 bucket name is the one provided in the secret you have registered with Gantry.
+""",
 )
 def create(
     name: str,
     connection_type: str,
     database_name: str,
     secret_name: str,
     description: str,
@@ -68,17 +91,16 @@
         "options": json.loads(options),
     }
 
     resp = api_client.request(
         "POST", "/api/v1/data-connectors/sources", json=request_body, raise_for_status=True
     )
 
-    click.secho(
-        f"--> A source data connector has been created.\n {json.dumps(resp['data'], indent=4)}"
-    )
+    click.secho("--> ", nl=False, fg="cyan")
+    click.secho(f"A source data connector has been created.\n {json.dumps(resp['data'], indent=4)}")
 
 
 @data_connector.command(
     aliases=["list"],
     help="List data connectors registered with Gantry.",
 )
 def list():
@@ -191,7 +213,11 @@
     resp = api_client.request(
         "DELETE",
         query,
         raise_for_status=True,
     )
 
     click.secho(f"--> Deleted the pipeline{pipeline_name}:\n {json.dumps(resp['data'], indent=4)}")
+
+
+if __name__ == "__main__":
+    data_connector()
```

### Comparing `gantry-0.5.9/gantry/cli/main.py` & `gantry-0.6.0a0/gantry/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from gantry import _version
 from gantry.cli.application import application
 from gantry.cli.bucket import bucket
 from gantry.cli.data_connector import data_connector
 from gantry.cli.projection import projection
 from gantry.cli.secret import secret
+from gantry.cli.labeling import labeling
 
 
 @click.group()
 @click.option(
     "--loglevel",
     "-l",
     type=click.Choice(["debug", "info", "warning", "error", "critical"], case_sensitive=False),
@@ -37,10 +38,11 @@
 
 
 cli.add_command(projection)
 cli.add_command(application)
 cli.add_command(bucket)
 cli.add_command(data_connector)
 cli.add_command(secret)
+cli.add_command(labeling)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `gantry-0.5.9/gantry/cli/projection.py` & `gantry-0.6.0a0/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/cli/secret.py` & `gantry-0.6.0a0/gantry/cli/secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     help="Create a secret.",
 )
 @click.option("--name", type=click.STRING, required=True, help="Secret name")
 @click.option(
     "--secret-type",
     required=True,
     type=click.Choice(
-        ["AWS", "GCP", "SNOWFLAKE_CONN_STR", "BIGQUERY_CONN_STR"],
+        ["AWS", "GCP", "SNOWFLAKE_CONN_STR"],
         case_sensitive=False,
     ),
 )
 @click.option(
     "--secret-file",
     type=click.STRING,
     required=True,
```

### Comparing `gantry-0.5.9/gantry/curators/__init__.py` & `gantry-0.6.0a0/gantry/automations/curators/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from gantry.curators.main import get_all_curators, get_curator, list_curators
-from gantry.curators.curators import Curator  # noqa: F401
-from gantry.curators.stock_curators import (   # noqa: F401
+from gantry.automations.curators.curators import Curator  # noqa: F401
+from gantry.automations.curators.main import (
+    get_all_curators,
+    get_curator,
+    list_curators,
+)
+from gantry.automations.curators.stock_curators import (  # noqa: F401
     AscendedSortCurator,
     BalancedStratificationCurator,
     BoundedRangeCurator,
     DescendedSortCurator,
     EqualityCurator,
     NewestCurator,
     OldestCurator,
```

### Comparing `gantry-0.5.9/gantry/curators/curators.py` & `gantry-0.6.0a0/gantry/automations/curators/curators.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import logging
 import uuid
 from typing import List, Optional
 
 from typeguard import typechecked
 
 from gantry.api_client import APIClient
-from gantry.curators import globals
-from gantry.curators.models import (
+from gantry.automations.curators import globals
+from gantry.automations.curators.models import (
     CreateCuratorRequest,
     CuratorInfo,
     EnableCuratorRequest,
     UpdateCuratorRequest,
 )
-from gantry.curators.selectors import Selector
+from gantry.automations.curators.selectors import Selector
 from gantry.dataset.gantry_dataset import GantryDataset
 from gantry.dataset.main import get_dataset
 from gantry.exceptions import (
     ClientNotInitialized,
     CuratorNotFoundError,
     GantryRequestException,
 )
@@ -72,15 +72,15 @@
         """
         Get a curator by name. If the curator does not exist, an exception will be raised.
 
         Args:
             name (str): the name of the curator to be retrieved.
 
         Returns:
-            :class:`gantry.curators.Curator`: A Curator object representing the curator
+            :class:`gantry.automations.curators.Curator`: A Curator object representing the curator
             corresponding to the provided name.
         """
         res = self._api_client.request("GET", f"/api/v1/curator/{name}", raise_for_status=True)
         return Curator.from_curator_info(self._api_client, CuratorInfo.parse_obj(res["data"]))
 
     @typechecked
     def delete_curator(
@@ -298,14 +298,44 @@
         return self._selectors
 
     @property
     def enabled(self) -> bool:
         """Enabling or disabling must be done via the `.enable()` or `.disable()` methods"""
         raise NotImplementedError
 
+    def update_curation_start_on(self, start_on: datetime.datetime) -> None:
+        """
+        Update the curation start on time.
+        Args:
+            start_on (datetime.datetime): The new start on time
+        """
+        self._start_on = start_on
+
+    def update_curation_interval(self, curation_interval: datetime.timedelta) -> None:
+        """
+        Update the curation interval.
+        Args:
+            curation_interval (datetime.timedelta): The new curation interval
+        """
+        self._curation_interval = curation_interval
+
+    def update_curation_delay(self, curation_delay: datetime.timedelta) -> None:
+        """
+        Update the curation delay.
+        Args:
+            curation_delay (datetime.timedelta): The new curation delay
+        """
+        self._curation_delay = curation_delay
+
+    def start(self) -> None:
+        """
+        Trigger to create the curator. This function is called from Automation.
+        """
+        self.create()
+
     def create(self, enable=True) -> "Curator":
         """
         Creates the Curator. By default, the Curator is also enabled upon creation.
         Use the `enable` parameter to change this
 
         Once created, the Curator will start curating the dataset according to the
         curation_interval. If curate_past_intervals is set to True, it will curate all
```

### Comparing `gantry-0.5.9/gantry/curators/main.py` & `gantry-0.6.0a0/gantry/automations/curators/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import inspect
 import logging
 import os
 from typing import Optional
 from urllib.parse import urlparse
 
 from gantry.api_client import APIClient
+from gantry.automations.curators import globals
+from gantry.automations.curators.curators import CuratorClient
 from gantry.const import PROD_API_URL
-from gantry.curators import globals
-from gantry.curators.curators import CuratorClient
 from gantry.exceptions import ClientNotInitialized
 
 logger_obj = logging.getLogger(__name__)
 
 
 def _curators_alias(func):
     """Decorator for CuratorClient functions, exposed in main.py"""
-    doc = "Alias for :meth:`gantry.curators.curators.CuratorClient.{}`".format(func.__name__)
+    doc = "Alias for :meth:`gantry.automations.curators.curators.CuratorClient.{}`".format(
+        func.__name__
+    )
     signature = inspect.signature(getattr(CuratorClient, func.__name__))
     orig_doc = inspect.getdoc(getattr(CuratorClient, func.__name__))
 
     if orig_doc:
         doc += "\n\n{}".format(orig_doc)
     signature = signature.replace(parameters=tuple(signature.parameters.values())[1:])
```

### Comparing `gantry-0.5.9/gantry/curators/models.py` & `gantry-0.6.0a0/gantry/automations/curators/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import uuid
 from typing import List, Optional
 
 import dateparser
 from pydantic import BaseModel, validator
 
-from gantry.curators.selectors import Selector
+from gantry.automations.curators.selectors import Selector
 
 
 class CreateCuratorRequest(BaseModel):
     application_name: str
     name: str
     curated_dataset_name: str
     start_on: datetime.datetime
```

### Comparing `gantry-0.5.9/gantry/curators/selectors.py` & `gantry-0.6.0a0/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/curators/stock_curators.py` & `gantry-0.6.0a0/gantry/automations/curators/stock_curators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 from typing import Optional, Union
 
-from gantry.curators.curators import Curator
-from gantry.curators.selectors import (
+from gantry.automations.curators.curators import Curator
+from gantry.automations.curators.selectors import (
     TIME_COLUMN_NAME,
     BoundsFilter,
     DruidDimensionOrderingDirections,
     EqualsFilter,
     OrderedSampler,
     Selector,
     StratificationMode,
```

### Comparing `gantry-0.5.9/gantry/data_generator/data_generator.py` & `gantry-0.6.0a0/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/dataset/client.py` & `gantry-0.6.0a0/gantry/dataset/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,17 @@
             ``List[Dict[str, Any]]``: list of dictionaries with metadata.
         """
         dataset = self.get_dataset(dataset_name)
 
         return dataset.list_versions()
 
     @typechecked
-    def list_datasets(self, include_deleted: bool = False) -> List[Dict[str, Any]]:
+    def list_datasets(
+        self, include_deleted: bool = False, model_node_id: Optional[str] = None
+    ) -> List[Dict[str, Any]]:
         """
         List all datasets. If ``include_deleted`` is set to ``True``, deleted datasets will be
         included in the result list.
 
         Example usage:
 
         .. code-block:: python
@@ -231,15 +233,15 @@
             ``List[Dict[str, Any]]``: List of dictionaries, each representing one
             dataset and associated metadata.
         """
         res = self._api_client.request(
             "GET",
             "/api/v1/datasets",
             raise_for_status=True,
-            params={"include_deleted": include_deleted},
+            params={"include_deleted": include_deleted, "model_node_id": model_node_id},
         )
 
         return [self._prune_dataset_info(dataset_info) for dataset_info in res["data"]]
 
     @typechecked
     def delete_dataset(self, name: str) -> None:
         """
```

### Comparing `gantry-0.5.9/gantry/dataset/constants.py` & `gantry-0.6.0a0/gantry/dataset/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,20 @@
     "Datetime": Value(dtype="timestamp[ns, tz=UTC]", id=None),
     "Unix_Time": Value(dtype="int64", id=None),
     "Json": dict(),
     "Image": Value(dtype="string", id=None),
     "Audio": Value(dtype="string", id=None),
     "Video": Value(dtype="string", id=None),
     "File": Value(dtype="string", id=None),
+    "Chat_Message": Value(dtype="string", id=None),
+    "Array<LLM_Generation_Choice>": Value(dtype="string", id=None),
+    "Array<Chat_Message>": Value(dtype="string", id=None),
     "Array<String>": Sequence(feature=Value(dtype="string", id=None), length=-1, id=None),
     "Array<Float>": Sequence(feature=Value(dtype="float64", id=None), length=-1, id=None),
     "Array<Integer>": Sequence(feature=Value(dtype="int64", id=None), length=-1, id=None),
     "Array<Boolean>": Sequence(feature=Value(dtype="bool", id=None), length=-1, id=None),
     "Array<UUID>": Sequence(feature=Value(dtype="string", id=None), length=-1, id=None),
     "Array<ID>": Sequence(feature=Value(dtype="string", id=None), length=-1, id=None),
-    "Unknown": Value(dtype="null", id=None),
+    "Unknown": Value(dtype="string", id=None),
 }
 
 EMPTY_STR_SHA256 = "47DEQpj8HBSa+/TImW+5JCeuQeRkm5NMpJWZG3hSuFU="
```

### Comparing `gantry-0.5.9/gantry/dataset/gantry_dataset.py` & `gantry-0.6.0a0/gantry/dataset/gantry_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1097,15 +1097,15 @@
             resp = self._api_client.request(
                 "POST",
                 f"/api/v1/datasets/{self._dataset_id}/commits",
                 json={
                     "message": commit_msg,
                     "metadata_s3_file_version": version_id,
                     "parent_commit_id": (
-                        self._get_current_commit()["id"]
+                        self._get_latest_commit()["id"]
                         if parent_commit_id is None
                         else parent_commit_id
                     ),
                     "commit_id": commit_id,
                 },
                 raise_for_status=True,
             )
```

### Comparing `gantry-0.5.9/gantry/dataset/main.py` & `gantry-0.6.0a0/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.0a0/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/exceptions.py` & `gantry-0.6.0a0/gantry/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     Raised when an API request returns an error.
     """
 
     def __init__(self, url: str, status_code: int, response_text: str) -> None:
         if status_code == 404:
             if "/api/v1/ingest/data-connectors" in url:
                 msg = (
-                    "Data connector not found. Ensure the parameters refer to an existing "
+                    "Data connector exception. Ensure the parameters refer to an existing "
                     "data connector you have access to. Details: {}"
                 ).format(response_text)
             else:
                 msg = (
                     "A resource was not found while trying to access ({}). Ensure the parameters "
                     "refer to an existing resource you have access to. Details: {}"
                 ).format(url, response_text)
```

### Comparing `gantry-0.5.9/gantry/logger/constants.py` & `gantry-0.6.0a0/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/logger/consumer.py` & `gantry-0.6.0a0/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/logger/event_builder.py` & `gantry-0.6.0a0/gantry/logger/event_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     inputs: List[dict],
     outputs: Union[List[dict], List[Any]],
     feedbacks: List[dict],
     join_keys: List[str],
     version: Optional[Union[str, int]] = None,
     ignore_inputs: Optional[List[str]] = None,
     tags: Optional[List[Dict[str, str]]] = None,
+    run_id: Optional[str] = None,
 ):
     """Build prediction and feedback events for log_records"""
     events = []
     for idx, timestamp in timestamp_idx:
         event = {}
 
         event.update(
@@ -32,24 +33,26 @@
                 outputs[idx],
                 application,
                 join_keys[idx],
                 version,
                 ignore_inputs,
                 custom_timestamp=timestamp,
                 tags=tags[idx] if tags else None,
+                batch_id=run_id,
             )
         )
 
         feedback_event = _build_feedback_event(
             application,
             join_keys[idx],
             feedbacks[idx],
             version,  # type: ignore
             timestamp,
             tags=tags[idx] if tags else None,
+            batch_id=run_id,
         )
 
         # Build an event with prediction data
         # and feedback data, now that backend
         # supports it.
         event["metadata"].update(feedback_event.pop("metadata"))
         event.update(feedback_event)
```

### Comparing `gantry-0.5.9/gantry/logger/main.py` & `gantry-0.6.0a0/gantry/logger/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             The environment is essentially a tag attached to data. To override
             this value later, you can set an 'env' tag in the tags parameters
             in the ingestion methods.
         send_in_background (optional, bool): set whether Gantry logging methods should
             run synchronously or not. You can also set this value by setting
             the env variable GANTRY_SEND_IN_BACKGROUND.
             If not provided, it defaults to True unless running in an AWS lambda.
-
     """
     (
         api_key,
         logs_location,
         logging_level,
         environment,
         bypass_firehose,
@@ -178,7 +177,22 @@
 
 def get_client():
     return _CLIENT
 
 
 def setup_logger(level: str = "INFO"):
     return Gantry.setup_logger(level)
+
+
+@_client_alias
+def log(*args, **kwargs):
+    return _CLIENT.log(*args, **kwargs)  # type: ignore[union-attr]
+
+
+@_client_alias
+def generate_records(*args, **kwargs):
+    return _CLIENT.generate_records(*args, **kwargs)  # type: ignore[union-attr]
+
+
+@_client_alias
+def _upload_data_as_batch(*args, **kwargs):
+    return _CLIENT._upload_data_as_batch(*args, **kwargs)  # type: ignore[union-attr]
```

### Comparing `gantry-0.5.9/gantry/logger/stores.py` & `gantry-0.6.0a0/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/logger/types.py` & `gantry-0.6.0a0/gantry/logger/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     file_type: UploadFileType
     batch_type: BatchType
     num_events: int
     application: str
     version: Optional[str]
     batch_id: Optional[str] = None
     log_timestamp: Optional[str] = None
+    run_name: Optional[str] = None
+    run_tags: Optional[Dict] = None
     timestamp: Dict[str, DataLinkElement] = field(default_factory=dict)
     inputs: Dict[str, DataLinkElement] = field(default_factory=dict)
     outputs: Dict[str, DataLinkElement] = field(default_factory=dict)
     feedback: Dict[str, DataLinkElement] = field(default_factory=dict)
     tags: Dict[str, DataLinkElement] = field(default_factory=dict)
     feedback_id: Dict[str, DataLinkElement] = field(default_factory=dict)
     feedback_keys: List[str] = field(default_factory=list)
@@ -66,18 +68,18 @@
         additional specifications for the schedule.
 
         For instance, schedule_type of INCREMENTAL_APPEND requires a "watermark_key",
         which is the timestamp column name to use as the watermark to divide the
         tumbling window for each incremental append.
     """
 
-    start_on: Union[datetime.datetime, str]
     frequency: ScheduleFrequency
-    type: ScheduleType
-    options: ScheduleOptions
+    start_on: Optional[Union[datetime.datetime, str]] = None
+    type: Optional[ScheduleType] = None
+    options: Optional[ScheduleOptions] = None
 
 
 @dataclass
 class IngestFromDataConnectorRequest:
     """
     Request body for creating a new ingestion pipeline from a data connector.
     """
```

### Comparing `gantry-0.5.9/gantry/logger/utils.py` & `gantry-0.6.0a0/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/__init__.py` & `gantry-0.6.0a0/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/client.py` & `gantry-0.6.0a0/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/core/dataframe.py` & `gantry-0.6.0a0/gantry/query/core/dataframe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent.futures
 import datetime
 import functools
 import json
 import pprint
 import sys
 from collections import OrderedDict
-from typing import Any, List, NamedTuple, Optional, Union
+from typing import Any, List, NamedTuple, Optional, Set, Union
 
 import pandas as pd
 from cachetools import TTLCache, cached
 from pandas import DataFrame
 from typeguard import typechecked
 
 from gantry.api_client import APIClient
@@ -54,25 +54,28 @@
         env: Optional[str] = None,
         filters: Optional[List[dict]] = None,
         tags: Optional[dict] = None,
     ):
         """
         :meta private: This is to skip constructor in the docs
         """
-        start_time, end_time = GantryQueryFrame.resolve_time_strings(start_time, end_time)
+        self.start_time, self.end_time = GantryQueryFrame.resolve_time_strings(start_time, end_time)
         application_node_id = get_application_node_id(
-            api_client, application, start_time, end_time, version
+            api_client, application, self.start_time, self.end_time, version
         )
         super().__init__(
             api_client,
-            QueryInfo(application_node_id, application, version, env, start_time, end_time),
+            QueryInfo(
+                application_node_id, application, version, env, self.start_time, self.end_time
+            ),
         )
         self.filters = filters or []  # Holds raw dict filters to be used when fetching data
         self.tags = tags  # Holds tags for filtering when fetching data
-
+        self.version = version
+        self.env = env
         self.series = self._build_series()
 
     def create_view(self, name: str) -> None:
         """Create a view from a Gantry Dataframe"""
         # Inline import to avoid circular dependency.
         from gantry.query.main import create_view
 
@@ -565,145 +568,188 @@
         return self._fetch(
             column=self.name,
             query_filters=self.parent_dataframe.filters,
             tags=self.parent_dataframe.tags,
         )
 
     @runs_on("int", "float")
-    def mean(self, num_points: int = 1) -> Union[float, pd.DataFrame]:
+    def mean(
+        self, num_points: int = 1, group_by: Optional[str] = None
+    ) -> Union[float, pd.DataFrame]:
         """
-        Runs on numeric series only.
+        Runs on int and float series only.
         Get the computed average of this GantrySeries, if available
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
+
 
         Returns:
-            Float with mean in case num_points not specified (or num_points=1),
+            Float with mean if num_points=1 and group_by=None (the default values),
             else a pd.DataFrame.
         """
         try:
-            return self._aggregate_query("mean", num_points=num_points)
+            return self._aggregate_query("mean", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine mean")
 
     @runs_on("int", "float")
-    def std(self, num_points: int = 1) -> Union[float, pd.DataFrame]:
+    def std(
+        self, num_points: int = 1, group_by: Optional[str] = None
+    ) -> Union[float, pd.DataFrame]:
         """
-        Runs on numeric series only.
+        Runs on int and float series only.
         Get the standard deviation for this GantrySeries, if available
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
+
 
         Returns:
-            Float with std in case num_points not specified (or num_points=1),
+            Float with std if num_points=1 and group_by=None (the default values),
             else a pd.DataFrame.
         """
         try:
-            return self._aggregate_query("stddev", num_points=num_points)
+            return self._aggregate_query("stddev", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine standard deviation")
 
     @runs_on("int", "float")
     def median(self, num_points: int = 1) -> Union[float, pd.DataFrame]:
         """
         Runs on numeric series only.
         Get the median for this GantrySeries, if available
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
 
         Returns:
-            Float with median in case num_points not specified (or num_points=1),
+            Float with median in case num_points=1 (the default value),
             else a pd.DataFrame.
         """
+        # ToDo: add group_by once linear.app/gantry/issue/ML-729/ is resolved
         try:
             quantiles = self.quantile([0.5], num_points=num_points)
             return quantiles[0.5]
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine median")
 
-    def count(self, num_points: int = 1) -> Union[float, pd.DataFrame]:
+    def count(
+        self, num_points: int = 1, group_by: Optional[str] = None
+    ) -> Union[float, pd.DataFrame]:
         """
         Get the number of available data points for this GantrySeries, if available.
+        Works on all series types.
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
 
         Returns:
-            Float with count in case num_points not specified (or num_points=1),
+            Float with count if num_points=1 and group_by=None (the default values),
             else a pd.DataFrame.
         """
         try:
-            return self._aggregate_query("total", num_points=num_points)
+            return self._aggregate_query("total", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine count")
 
     @runs_on("int", "float", "datetime")
-    def min(self, num_points: int = 1) -> Union[float, datetime.datetime, pd.DataFrame]:
+    def min(
+        self, num_points: int = 1, group_by: Optional[str] = None
+    ) -> Union[float, datetime.datetime, pd.DataFrame]:
         """
-        Runs on numeric and datetime series only.
+        Runs on int, float, and datetime series only.
         Get the minimum for this GantrySeries, if available.
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
+
 
         Returns:
-            Float with min value in case num_points not specified (or num_points=1),
+            Float with min value if num_points=1 and group_by=None (the default values),
             else a pd.DataFrame.
         """
         try:
-            return self._aggregate_query("minimum", num_points=num_points)
+            return self._aggregate_query("minimum", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine min")
 
     @runs_on("int", "float", "datetime")
-    def max(self, num_points: int = 1) -> Union[float, datetime.datetime, pd.DataFrame]:
+    def max(
+        self, num_points: int = 1, group_by: Optional[str] = None
+    ) -> Union[float, datetime.datetime, pd.DataFrame]:
         """
-        Runs on numeric and datetime series only.
+        Runs on int, float, and datetime series only.
         Get the maximum for this GantrySeries, if available.
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
+
 
         Returns:
-            Float with max value in case num_points not specified (or num_points=1),
+            Float with max value if num_points=1 and group_by=None (the default values),
             else a pd.DataFrame.
         """
         try:
-            return self._aggregate_query("maximum", num_points=num_points)
+            return self._aggregate_query("maximum", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine max")
 
     def histogram(self):
         """
+        Runs on bool, int, float and str series only.
         Get histogram of categories for this GantrySeries, if available.
 
         Gets the histogram of percentages from [0, 1] for available data values
         for this GantrySeries.
 
         Returns:
             Dict[str, float] histogram
         """
         try:
             hist_res = self._aggregate_query("category_percents")
             return hist_res
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine histogram")
 
+    @runs_on("bool", "str")
+    def unique(self) -> Set[str]:
+        """
+        Runs on bool and str series only.
+        Get the unique values in this GantrySeries, if available.
+
+        Returns:
+            Set[str] List containing all the unique values that occur in this series.
+        """
+        try:
+            hist_res = self._aggregate_query("category_percents")
+            return set(hist_res.keys())
+        except (AttributeError, ValueError, KeyError):
+            raise QueryError("Invalid query. GantrySeries cannot determine unique values")
+
     @runs_on("int", "float")
     def quantile(self, quantile_vals: List[float] = [0.5]):
         """
+        Runs on int and float series only.
         Get quantiles for this GantrySeries, if available.
 
         Args:
             quantile_vals: list of requested quantiles. Float values in the list should be in the
                 range [0, 1].
         Returns:
             List[floats] of len(quantiles_vals) where the order of the outputs matches the input
@@ -734,15 +780,21 @@
             return pd.DataFrame(cdf_res)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine cdf")
 
     def _dtype(self):
         return self.datatype
 
-    def _aggregate_query(self, attribute, num_points: int = 1, **attribute_kwargs):
+    def _aggregate_query(
+        self,
+        attribute,
+        num_points: int = 1,
+        group_by: Optional[str] = None,
+        **attribute_kwargs,
+    ):
         data = self.query_info.get_base_query_params()
         if num_points <= 0:
             raise ValueError(f"num_points must be an int > 0, but received value of {num_points}")
         data["num_points"] = num_points
         data["queries"] = {
             "query": {
                 "query_type": "feature",
@@ -750,28 +802,48 @@
                 "stat": attribute,
                 "stat_kwargs": {attribute: attribute_kwargs},
                 "feature": self.name,
                 "filters": self.parent_dataframe.filters,
                 "tags": self.parent_dataframe.tags,
             }
         }
+        if group_by is not None:
+            if group_by not in self.parent_dataframe.series:
+                raise ValueError(f"Cannot find column {group_by} in dataframe.")
+            if num_points != 1:
+                raise ValueError(
+                    "Metric computations that specify a group_by feature "
+                    "cannot also specify num_points."
+                )
+            group_by_type = self.parent_dataframe[group_by].datatype  # type: ignore
+            data["queries"]["query"]["group_by"] = [
+                {"feature_name": group_by, "dtype": group_by_type}
+            ]
         resource = "aggregate" if num_points == 1 else "time_series"
         try:
             response = _raw_query_cached_request(
                 self.api_client,
                 json.dumps(data, default=lambda x: x.isoformat()),
                 resource=resource,
             )
             data = response["data"]["query"]
-
-            if num_points == 1:
-                return data[attribute]
+            if group_by is not None:
+                df_result = []
+                for row in data:
+                    result = {}
+                    _temp = row["group"][0]  # type: ignore
+                    result[_temp["feature_name"]] = _temp["value"]  # type: ignore
+                    result[attribute] = row[attribute]
+                    df_result.append(result)
+                return pd.DataFrame(df_result)
             else:
-                return pd.DataFrame(data["points"])
-
+                if num_points == 1:
+                    return data[attribute]
+                else:
+                    return pd.DataFrame(data["points"])
         except GantryException as e:
             raise GantryException("Aggregation query [" + attribute + "] failed: " + str(e))
 
     def _describe(self) -> dict:
         c = self.count()
         table = {
             "series type": self.series_type,
@@ -794,15 +866,17 @@
             )
         if self.dtype == "bool":
             table["True rate"] = self[self == True].count() / c  # type: ignore # noqa
 
         return table
 
     def describe(self) -> pd.DataFrame:
-        """Return basic stats on the series.
+        """
+        Runs on int, float, and bool series only.
+        Return basic stats on the series.
 
         Returns:
             A pandas dataframe with summary information.
 
         """
         stats = self._describe()
         return pd.DataFrame(
@@ -813,62 +887,87 @@
                 *stats.values(),
             ],
             index=["application", "from", "to", *stats.keys()],
             columns=[self.name],
         )
 
     @runs_on("bool")
-    def percent_true(self, dropna: bool = False, num_points: int = 1):
+    def percent_true(
+        self, dropna: bool = False, num_points: int = 1, group_by: Optional[str] = None
+    ):
         """
-        Percent true
+        Runs on boolean series only.
+        Percent true, optionally drop null values.
 
         Args:
             data_node (GantrySeries): GantrySeries which will be calculated
             dropna (bool, defaults to False): if True, first drops NaN values
                 before calculating result.
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
 
         Returns:
-            (pd.DataFrame) pd.DataFrame of shape (num_points, 1) percent true
+            Float with true percentage if num_points=1 and group_by=None (by default),
+                else pd.DataFrame.
         """
-        from gantry.query.metric.main import percent_true
-
-        return percent_true(self, dropna, num_points)
+        _temp = self
+        if dropna:
+            _temp = _temp[_temp.notna()]  # type: ignore
+        try:
+            return _temp._aggregate_query("percent_true", num_points=num_points, group_by=group_by)
+        except (AttributeError, ValueError, KeyError):
+            raise QueryError("Invalid query. GantrySeries cannot determine percent_true")
 
     @runs_on("bool")
-    def percent_false(self, dropna: bool = False, num_points: int = 1):
+    def percent_false(
+        self, dropna: bool = False, num_points: int = 1, group_by: Optional[str] = None
+    ):
         """
-        Percent false
+        Runs on boolean series only.
+        Percent false, optionally drop null values.
 
         Args:
             data_node (GantrySeries): GantrySeries which will be calculated
             dropna (bool, defaults to False): if True, first drops NaN values
                 before calculating result.
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
 
         Returns:
-            (pd.DataFrame) pd.DataFrame of shape (num_points, 1) percent false
+            Float with false percentage if num_points=1 and group_by=None (by default),
+                else pd.DataFrame.
         """
-        from gantry.query.metric.main import percent_false
-
-        return percent_false(self, dropna, num_points)
+        _temp = self
+        if dropna:
+            _temp = _temp[_temp.notna()]  # type: ignore
+        try:
+            return _temp._aggregate_query("percent_false", num_points=num_points, group_by=group_by)
+        except (AttributeError, ValueError, KeyError):
+            raise QueryError("Invalid query. GantrySeries cannot determine percent_false")
 
     @runs_on("bool")
-    def percent_null(self, num_points: int = 1):
+    def percent_null(self, num_points: int = 1, group_by: Optional[str] = None):
         """
-        Percent null/NaN
+        Runs on boolean series only.
+        Percent null/NaN.
 
         Args:
             data_node (GantrySeries): GantrySeries which will be calculated
             dropna (bool, defaults to False): if True, drop rows with NaN
                 values in result.
             num_points (int, defaults to 1): number of points to divide the
                 time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
 
         Returns:
-            (pd.DataFrame) pd.DataFrame of shape (num_points, 1) percent_null
+            Float with null percentage if num_points=1 and group_by=None (by default),
+                else pd.DataFrame.
         """
-        from gantry.query.metric.main import percent_null
-
-        return percent_null(self, num_points=num_points)
+        try:
+            return self._aggregate_query("percent_null", num_points=num_points, group_by=group_by)
+        except (AttributeError, ValueError, KeyError):
+            raise QueryError("Invalid query. GantrySeries cannot determine percent_null.")
```

### Comparing `gantry-0.5.9/gantry/query/core/distance.py` & `gantry-0.6.0a0/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/core/metric.py` & `gantry-0.6.0a0/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/core/queryframe.py` & `gantry-0.6.0a0/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/core/utils.py` & `gantry-0.6.0a0/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/distance/main.py` & `gantry-0.6.0a0/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/globals.py` & `gantry-0.6.0a0/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/main.py` & `gantry-0.6.0a0/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/query/metric/main.py` & `gantry-0.6.0a0/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/serializers.py` & `gantry-0.6.0a0/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry/utils.py` & `gantry-0.6.0a0/gantry/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -301,7 +301,27 @@
     click.secho("SUCCESS", fg="cyan")
 
 
 def read_lines_from_url(url):
     response = requests.get(url, stream=True)
     for line in response.iter_lines():
         yield line.decode("utf-8")
+
+
+def from_isoformat_duration(duration_string: str) -> datetime.timedelta:
+    # Parse the duration string using regular expressions
+    match = re.match(r"^P((\d+)W)?((\d+)D)?T?((\d+)H)?((\d+)M)?((\d+)S)?$", duration_string)
+    if not match:
+        raise ValueError(f"Invalid duration string: {duration_string}")
+
+    # Extract the component values from the match object
+    weeks = int(match.group(2) or 0)
+    days = int(match.group(4) or 0)
+    hours = int(match.group(6) or 0)
+    minutes = int(match.group(8) or 0)
+    seconds = int(match.group(10) or 0)
+
+    # Calculate the total duration in seconds
+    total_seconds = (weeks * 7 + days) * 86400 + hours * 3600 + minutes * 60 + seconds
+
+    # Return a timedelta object representing the duration
+    return datetime.timedelta(seconds=total_seconds)
```

### Comparing `gantry-0.5.9/gantry/validators.py` & `gantry-0.6.0a0/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/gantry.egg-info/PKG-INFO` & `gantry-0.6.0a0/gantry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.5.9
+Version: 0.6.0a0
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.5.9/gantry.egg-info/SOURCES.txt` & `gantry-0.6.0a0/gantry.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,39 @@
 gantry.egg-info/entry_points.txt
 gantry.egg-info/requires.txt
 gantry.egg-info/top_level.txt
 gantry/alerts/__init__.py
 gantry/alerts/client.py
 gantry/alerts/globals.py
 gantry/alerts/main.py
+gantry/applications/__init__.py
+gantry/applications/client.py
+gantry/applications/core.py
+gantry/applications/main.py
+gantry/automations/__init__.py
+gantry/automations/actions.py
+gantry/automations/automations.py
+gantry/automations/globals.py
+gantry/automations/main.py
+gantry/automations/triggers.py
+gantry/automations/curators/__init__.py
+gantry/automations/curators/curators.py
+gantry/automations/curators/globals.py
+gantry/automations/curators/main.py
+gantry/automations/curators/models.py
+gantry/automations/curators/selectors.py
+gantry/automations/curators/stock_curators.py
 gantry/cli/__init__.py
 gantry/cli/application.py
 gantry/cli/bucket.py
 gantry/cli/data_connector.py
+gantry/cli/labeling.py
 gantry/cli/main.py
 gantry/cli/projection.py
 gantry/cli/secret.py
-gantry/curators/__init__.py
-gantry/curators/curators.py
-gantry/curators/globals.py
-gantry/curators/main.py
-gantry/curators/models.py
-gantry/curators/selectors.py
-gantry/curators/stock_curators.py
 gantry/data_generator/__init__.py
 gantry/data_generator/data_generator.py
 gantry/dataset/__init__.py
 gantry/dataset/client.py
 gantry/dataset/constants.py
 gantry/dataset/gantry_dataset.py
 gantry/dataset/main.py
@@ -50,14 +61,15 @@
 gantry/logger/stores.py
 gantry/logger/types.py
 gantry/logger/utils.py
 gantry/query/__init__.py
 gantry/query/client.py
 gantry/query/globals.py
 gantry/query/main.py
+gantry/query/time_window.py
 gantry/query/core/__init__.py
 gantry/query/core/constants.py
 gantry/query/core/dataframe.py
 gantry/query/core/distance.py
 gantry/query/core/metric.py
 gantry/query/core/queryframe.py
 gantry/query/core/utils.py
@@ -74,14 +86,15 @@
 tests/alerts/__init__.py
 tests/alerts/conftest.py
 tests/alerts/test_client.py
 tests/alerts/test_main.py
 tests/cli/__init__.py
 tests/cli/test_bucket.py
 tests/cli/test_data_connector.py
+tests/cli/test_labeling.py
 tests/cli/test_main.py
 tests/cli/test_projection.py
 tests/cli/test_secrets.py
 tests/curator/__init__.py
 tests/curator/conftest.py
 tests/curator/test_curator.py
 tests/curator/test_main.py
```

### Comparing `gantry-0.5.9/setup.py` & `gantry-0.6.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "cachetools~=4.2",
     "click>=7.1.2",
     "click-aliases~=1.0",
     "click-spinner>=0.1.10",
     "requests>=2.22.0",
     "pyyaml>=5.3.1",
     "colorama>=0.4.0",
+    "label-studio-sdk>=0.0.19,<0.0.22",
     "marshmallow>=3.11.1",
     "marshmallow-oneofschema>=3.0.1",
     "monotonic>=1.4",
     "tabulate~=0.8",
     "typing-extensions~=4.0",
     "tqdm~=4.64",
     "halo~=0.0.31",
```

### Comparing `gantry-0.5.9/tests/alerts/test_client.py` & `gantry-0.6.0a0/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/alerts/test_main.py` & `gantry-0.6.0a0/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/cli/test_bucket.py` & `gantry-0.6.0a0/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/cli/test_data_connector.py` & `gantry-0.6.0a0/tests/cli/test_data_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,89 +1,102 @@
 import json
 
 import mock
+import pytest
 import responses
 from click.testing import CliRunner
 from responses import matchers
+
 from gantry.cli.data_connector import (
     create,
     delete,
+    delete_pipeline,
     list,
-    list_pipelines,
     list_pipeline_operations,
-    delete_pipeline,
+    list_pipelines,
 )
 
 UNITTEST_HOST = "http://unittest"
 DATA_CONNECTOR_NAME = "test_data_connector"
 DATA_CONNECTOR_1_ID = "0db220e0-f568-4295-be48-67095fa57f34"
 DATA_CONNECTOR_2_ID = "9e09947e-fb18-4ce3-bd17-7c386a3c9980"
 DATA_CONNECTOR_ENABLED_STATUS_CMD = "enabled"
 DATA_CONNECTOR_ENABLED_STATUS = "True"
 DATABASE_NAME = "test_database"
-CONNECTION_TYPE = "SNOWFLAKE"
+SUPPORTED_CONNECTION_TYPES = ["SNOWFLAKE", "S3"]
 DESCRIPTION = "Data connector to log records from my snowflake database"
 SECRET_NAME = "test_secret"
-OPTIONS = '{"schema_name": "PUBLIC","table_name": "GANTRY_EVENTS"}'
 APP_NAME = "test_app"
 METADATA_ID = "09a26daf-7edb-4e94-aa57-31315ae1a31a"
 PIPELINE_NAME = "test_pipeline"
 PIPELINE_OPERATION_STATUS = "QUEUED"
 PIPELINE_OPERATION_ID = "b4bc71af-37b7-4460-b66c-7ef078949c41"
 PIPELINE_ID = "b4bc71af-37b7-4460-b66c-7ef078949c41"
 PIPELINE_CONSUMER_ID = "3318762f-a684-480c-b418-d5adcdcb5dc6"
 APP_VERSION = "1.0.0"
 
+SNOWFLAKE_OPTIONS = '{"snowflake_schema_name": "PUBLIC","snowflake_table_name": "GANTRY_EVENTS"}'
+S3_OPTIONS = (
+    '{"s3_bucket_name": "test-bucket-name","s3_filetype": "csv","s3_path_prefix": "test-prefix/"}'
+)
+
 
-def test_create_data_connector():
+@pytest.mark.parametrize(
+    ("connection_type", "options"),
+    [
+        ("SNOWFLAKE", SNOWFLAKE_OPTIONS),
+        ("S3", S3_OPTIONS),
+    ],
+)
+def test_create_data_connector(connection_type, options):
     runner = CliRunner()
     cli_args = [
         "--name",
         DATA_CONNECTOR_NAME,
         "--database-name",
         DATABASE_NAME,
         "--connection-type",
-        CONNECTION_TYPE,
+        connection_type,
         "--secret-name",
         SECRET_NAME,
         "--description",
         DESCRIPTION,
         "--options",
-        OPTIONS,
+        options,
     ]
 
     with responses.RequestsMock() as resp:
         resp.add(
             resp.POST,
             f"{UNITTEST_HOST}/api/v1/data-connectors/sources",
             json={
                 "response": "ok",
                 "data": {
-                    "connection_type": CONNECTION_TYPE,
+                    "connection_type": connection_type,
                     "created_at": "2023-01-18T00:18:01.000000",
                     "database_name": DATABASE_NAME,
                     "description": DESCRIPTION,
                     "id": DATA_CONNECTOR_1_ID,
                     "name": DATABASE_NAME,
-                    "options": {"schema_name": "PUBLIC", "table_name": "GANTRY_EVENTS"},
+                    "options": options,
                     "secret_name": SECRET_NAME,
                     "type": "SOURCE",
                     "updated_at": "2023-01-18T00:18:01.000000",
                 },
             },
             headers={"Content-Type": "application/json"},
             match=[
                 matchers.json_params_matcher(
                     {
                         "name": DATA_CONNECTOR_NAME,
                         "database_name": DATABASE_NAME,
-                        "connection_type": CONNECTION_TYPE,
+                        "connection_type": connection_type,
                         "secret_name": SECRET_NAME,
                         "description": DESCRIPTION,
-                        "options": json.loads(OPTIONS),
+                        "options": json.loads(options),
                     }
                 )
             ],
         )
 
         result = runner.invoke(
             create,
@@ -99,57 +112,56 @@
     """
     Tests that invalid connection type throws an error
     """
     runner = CliRunner()
     cli_args = [
         "--name",
         DATA_CONNECTOR_NAME,
-        "--database-name",
-        DATABASE_NAME,
         "--connection-type",
         "NOT_VALID_TYPE",
         "--secret-name",
         SECRET_NAME,
         "--description",
         DESCRIPTION,
         "--options",
-        OPTIONS,
+        S3_OPTIONS,
     ]
 
     result = runner.invoke(
         create,
         cli_args,
         env={"GANTRY_API_KEY": "test", "GANTRY_LOGS_LOCATION": UNITTEST_HOST},
     )
 
     assert result.exit_code == 2
     assert "Error: Invalid value for '--connection-type': 'NOT_VALID_TYPE'" in result.output
 
 
+@pytest.mark.parametrize("connection_type", SUPPORTED_CONNECTION_TYPES)
 @mock.patch("gantry.cli.data_connector.APIClient.request")
-def test_create_data_connector_api_failure(mock_api_client: mock.Mock):
+def test_create_data_connector_api_failure(mock_api_client: mock.Mock, connection_type):
     """
     Tests that invalid connection type throws an error
     """
     mock_api_client.return_value = {"response": "error", "error": "some error"}
 
     runner = CliRunner()
     cli_args = [
         "--name",
         DATA_CONNECTOR_NAME,
         "--database-name",
         DATABASE_NAME,
         "--connection-type",
-        CONNECTION_TYPE,
+        connection_type,
         "--secret-name",
         SECRET_NAME,
         "--description",
         DESCRIPTION,
         "--options",
-        OPTIONS,
+        SNOWFLAKE_OPTIONS,
     ]
 
     result = runner.invoke(
         create,
         cli_args,
         env={"GANTRY_API_KEY": "test", "GANTRY_LOGS_LOCATION": UNITTEST_HOST},
     )
@@ -167,33 +179,33 @@
         resp.add(
             resp.GET,
             f"{UNITTEST_HOST}/api/v1/data-connectors",
             json={
                 "response": "ok",
                 "data": [
                     {
-                        "connection_type": CONNECTION_TYPE,
+                        "connection_type": "SNOWFLAKE",
                         "created_at": "2023-01-18T00:18:01.000000",
                         "database_name": DATABASE_NAME,
                         "description": DESCRIPTION,
                         "id": DATA_CONNECTOR_1_ID,
                         "name": DATABASE_NAME,
-                        "options": {"schema_name": "PUBLIC", "table_name": "GANTRY_EVENTS"},
+                        "options": SNOWFLAKE_OPTIONS,
                         "secret_name": SECRET_NAME,
                         "type": "SOURCE",
                         "updated_at": "2023-01-18T00:18:01.000000",
                     },
                     {
-                        "connection_type": CONNECTION_TYPE,
+                        "connection_type": "S3",
                         "created_at": "2023-01-18T00:18:01.000000",
-                        "database_name": DATABASE_NAME,
+                        "database_name": "",
                         "description": DESCRIPTION,
                         "id": DATA_CONNECTOR_2_ID,
                         "name": DATABASE_NAME,
-                        "options": {"schema_name": "PUBLIC", "table_name": "GANTRY_EVENTS_2"},
+                        "options": S3_OPTIONS,
                         "secret_name": SECRET_NAME,
                         "type": "SOURCE",
                         "updated_at": "2023-01-18T00:18:01.000000",
                     },
                 ],
             },
             headers={"Content-Type": "application/json"},
@@ -206,27 +218,28 @@
 
         assert result.exit_code == 0
         assert "--> A list of registered data connectors" in result.output
         assert DATA_CONNECTOR_1_ID in result.output
         assert DATA_CONNECTOR_2_ID in result.output
 
 
-def test_delete_data_connector():
+@pytest.mark.parametrize("connection_type", SUPPORTED_CONNECTION_TYPES)
+def test_delete_data_connector(connection_type):
     """ """
     runner = CliRunner()
     cli_args = ["--name", DATA_CONNECTOR_NAME]
 
     with responses.RequestsMock() as resp:
         resp.add(
             resp.DELETE,
             f"{UNITTEST_HOST}/api/v1/data-connectors/sources/{DATA_CONNECTOR_NAME}",
             json={
                 "response": "ok",
                 "data": {
-                    "connection_type": CONNECTION_TYPE,
+                    "connection_type": connection_type,
                     "created_at": "2023-01-18T00:18:01.000000",
                     "database_name": DATABASE_NAME,
                     "description": DESCRIPTION,
                     "id": DATA_CONNECTOR_1_ID,
                     "name": DATABASE_NAME,
                     "options": {"schema_name": "PUBLIC", "table_name": "GANTRY_EVENTS"},
                     "secret_name": SECRET_NAME,
```

### Comparing `gantry-0.5.9/tests/cli/test_projection.py` & `gantry-0.6.0a0/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/cli/test_secrets.py` & `gantry-0.6.0a0/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/conftest.py` & `gantry-0.6.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/curator/conftest.py` & `gantry-0.6.0a0/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/curator/test_curator.py` & `gantry-0.6.0a0/tests/curator/test_curator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 
 import pytest
 import responses
 from responses import matchers
 
 from gantry.api_client import APIClient
-from gantry.curators import Curator
-from gantry.curators.curators import CuratorClient
-from gantry.curators.selectors import Selector
+from gantry.automations.curators import Curator
+from gantry.automations.curators.curators import CuratorClient
+from gantry.automations.curators.selectors import Selector
 
 from .conftest import HOST
 
 
 @pytest.fixture
 def test_api_client():
     return APIClient(origin=HOST)
```

### Comparing `gantry-0.5.9/tests/curator/test_main.py` & `gantry-0.6.0a0/tests/curator/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import mock
 import pytest
 
-from gantry.curators import Curator, UniformCurator, globals, main
+from gantry.automations.curators import Curator, UniformCurator, globals, main
 from gantry.exceptions import ClientNotInitialized
 
 
 @pytest.mark.parametrize(
     ["method", "params"],
     [
         ("get_all_curators", {}),
@@ -13,29 +13,29 @@
         ("list_curators", {}),
     ],
 )
 def test_uninit_client_main(method, params):
     """Test all public methods from curator module
     fail if client is not initialized
     """
-    with mock.patch("gantry.curators.globals._CURATOR_CLIENT", None):
+    with mock.patch("gantry.automations.curators.globals._CURATOR_CLIENT", None):
         with pytest.raises(ClientNotInitialized):
             getattr(main, method)(**params)
 
 
 @pytest.mark.parametrize(
     ["curator_type", "params"],
     [
         (Curator, {"name": "test_curator", "application_name": "test-app"}),
         (UniformCurator, {"name": "test_curator", "application_name": "test-app", "limit": 10}),
     ],
 )
 def test_unint_curator(curator_type, params):
     """Test that curator initialization fails if client is not initialized"""
-    with mock.patch("gantry.curators.globals._API_CLIENT", None):
+    with mock.patch("gantry.automations.curators.globals._API_CLIENT", None):
         with pytest.raises(ClientNotInitialized):
             curator_type(**params)
 
 
 @pytest.mark.parametrize("backend", ["", "/some/file", "tcp://other/protocol"])
 def test_global_init_error(backend):
     with mock.patch.dict("os.environ", {"GANTRY_LOGS_LOCATION": backend}):
@@ -84,10 +84,10 @@
     ],
 )
 def test_curator_methods(method, params):
     """Test all public methods from gantry module or gantry.main module
     resolve in the global _CURATOR_CLIENT methods
     """
     m = mock.Mock()
-    with mock.patch("gantry.curators.globals._CURATOR_CLIENT", m):
+    with mock.patch("gantry.automations.curators.globals._CURATOR_CLIENT", m):
         getattr(main, method)(**params)
         getattr(m, method).assert_called_once_with(**params)
```

### Comparing `gantry-0.5.9/tests/curator/test_selectors.py` & `gantry-0.6.0a0/tests/curator/test_selectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import mock
 import pydantic
 import pytest
 
-from gantry.curators import (
+from gantry.automations.curators import (
     AscendedSortCurator,
     BalancedStratificationCurator,
     BoundedRangeCurator,
     Curator,
     DescendedSortCurator,
     EqualityCurator,
     NewestCurator,
     OldestCurator,
     ProportionalStratificationCurator,
     StrictStratificationCurator,
     UniformCurator,
 )
-from gantry.curators.selectors import (
+from gantry.automations.curators.selectors import (
     BoundsFilter,
     ContainsFilter,
     DruidDimensionOrderingDirections,
     EqualsFilter,
     OrderedSampler,
     Selector,
     StratificationMode,
@@ -121,25 +121,25 @@
                 ),
                 limit=10,
                 filters=[BoundsFilter(field="float_field", lower=0.0, upper=1.0)],
             ),
         ),
     ],
 )
-@mock.patch("gantry.curators.globals._API_CLIENT", "fake-api-client")
+@mock.patch("gantry.automations.curators.globals._API_CLIENT", "fake-api-client")
 def test_selectors_preset_curator(curator_class, curator_kwargs, expected_selector):
     curator_kwargs.update(
         {"name": "test_curator_name", "application_name": "test_application_name", "limit": 10}
     )
     curator = curator_class(**curator_kwargs)
 
     assert curator._selectors[0] == expected_selector
 
 
-@mock.patch("gantry.curators.globals._API_CLIENT", "fake-api-client")
+@mock.patch("gantry.automations.curators.globals._API_CLIENT", "fake-api-client")
 def test_curator_properties(test_curator):
     curator = Curator(**test_curator)
 
     assert curator.id == test_curator["id"]
     assert curator.application_name == test_curator["application_name"]
     assert curator.name == test_curator["name"]
     assert curator.curated_dataset_name == test_curator["curated_dataset_name"]
```

### Comparing `gantry-0.5.9/tests/data_generator/test_data_generator.py` & `gantry-0.6.0a0/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/dataset/conftest.py` & `gantry-0.6.0a0/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/dataset/test_client.py` & `gantry-0.6.0a0/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.0a0/tests/dataset/test_gantry_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -671,14 +671,26 @@
     )
     resp.add(
         resp.GET,
         f"{HOST}/fake_presigned_url_2",
         body="test-string",
     )
 
+    # for getting the latest commit
+    if not parent_commit_id:
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/datasets/{DATASET_ID}/commits",
+            json={
+                "response": "ok",
+                "data": [{"id": "4569ef0b-ff96-4110-a606-8d9d54fab382"}],
+            },
+            headers={"Content-Type": "application/json"},
+        )
+
     # for the actual commit creation request
     resp.add(
         resp.POST,
         f"{HOST}/api/v1/datasets/{DATASET_ID}/commits",
         json={
             "data": {
                 "created_at": "Wed, 07 Oct 2022 06:11:02 GMT",
```

### Comparing `gantry-0.5.9/tests/dataset/test_main.py` & `gantry-0.6.0a0/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/logger/test_client.py` & `gantry-0.6.0a0/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/logger/test_consumer.py` & `gantry-0.6.0a0/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/logger/test_event_builder.py` & `gantry-0.6.0a0/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/logger/test_main.py` & `gantry-0.6.0a0/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/logger/test_stores.py` & `gantry-0.6.0a0/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/logger/test_utils.py` & `gantry-0.6.0a0/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/conftest.py` & `gantry-0.6.0a0/tests/query/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -172,14 +172,36 @@
         series_type="prediction",
         parent_dataframe=mock.Mock(api_client=api_client_obj, query_info=query_info_obj),
         id="abc123",
     )
 
 
 @pytest.fixture
+def series_obj_str(api_client_obj, query_info_obj):
+    return dataframe.GantrySeries(
+        name="series_name",
+        datatype="str",
+        series_type="prediction",
+        parent_dataframe=mock.Mock(api_client=api_client_obj, query_info=query_info_obj),
+        id="abc123",
+    )
+
+
+@pytest.fixture
+def series_obj_bool(api_client_obj, query_info_obj):
+    return dataframe.GantrySeries(
+        name="A",
+        datatype="bool",
+        series_type="prediction",
+        parent_dataframe=mock.Mock(api_client=api_client_obj, query_info=query_info_obj),
+        id="abc123",
+    )
+
+
+@pytest.fixture
 def series_obj_factory(api_client_obj, query_info_obj):
     def wrapper(datatype, parent_dataframe=None, name="series_name", count=10):
         series = dataframe.GantrySeries(
             name=name,
             datatype=datatype,
             series_type="prediction",
             parent_dataframe=parent_dataframe
```

### Comparing `gantry-0.5.9/tests/query/core/test_dataframe.py` & `gantry-0.6.0a0/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/core/test_distance.py` & `gantry-0.6.0a0/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/core/test_filters.py` & `gantry-0.6.0a0/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/core/test_metric.py` & `gantry-0.6.0a0/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/core/test_queryframe.py` & `gantry-0.6.0a0/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/core/test_series.py` & `gantry-0.6.0a0/tests/query/core/test_series.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,41 +24,45 @@
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_mean(mock_query, num_points_kwargs, series_obj):
     mock_query.return_value = 0.5
     assert series_obj.mean(**num_points_kwargs) == 0.5
-    mock_query.assert_called_once_with("mean", num_points=num_points_kwargs.get("num_points", 1))
+    mock_query.assert_called_once_with(
+        "mean", num_points=num_points_kwargs.get("num_points", 1), group_by=None
+    )
 
 
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_mean_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.mean()
-    mock_query.assert_called_once_with("mean", num_points=1)
+    mock_query.assert_called_once_with("mean", num_points=1, group_by=None)
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_std(mock_query, num_points_kwargs, series_obj):
     mock_query.return_value = 0.6
     assert series_obj.std(**num_points_kwargs) == 0.6
-    mock_query.assert_called_once_with("stddev", num_points=num_points_kwargs.get("num_points", 1))
+    mock_query.assert_called_once_with(
+        "stddev", num_points=num_points_kwargs.get("num_points", 1), group_by=None
+    )
 
 
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_std_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.std()
-    mock_query.assert_called_once_with("stddev", num_points=1)
+    mock_query.assert_called_once_with("stddev", num_points=1, group_by=None)
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @mock.patch("gantry.query.core.dataframe.GantrySeries.quantile")
 def test_median(mock_query, num_points_kwargs, series_obj):
     mock_query.return_value = {0.5: 0.7}
     assert series_obj.median(**num_points_kwargs) == 0.7
@@ -75,41 +79,45 @@
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_count(mock_query, num_points_kwargs, series_obj):
     mock_query.return_value = 100
     assert series_obj.count(**num_points_kwargs) == 100
-    mock_query.assert_called_once_with("total", num_points=num_points_kwargs.get("num_points", 1))
+    mock_query.assert_called_once_with(
+        "total", num_points=num_points_kwargs.get("num_points", 1), group_by=None
+    )
 
 
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_len(mock_query, series_obj):
     mock_query.return_value = 100
     assert len(series_obj) == 100
-    mock_query.assert_called_once_with("total", num_points=1)
+    mock_query.assert_called_once_with("total", num_points=1, group_by=None)
 
 
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_count_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.count()
-    mock_query.assert_called_once_with("total", num_points=1)
+    mock_query.assert_called_once_with("total", num_points=1, group_by=None)
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @pytest.mark.parametrize("datatype", ["int", "float"])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_min(mock_query, datatype, num_points_kwargs, series_obj_factory):
     series_obj = series_obj_factory(datatype)
     mock_query.return_value = 1
     assert series_obj.min(**num_points_kwargs) == 1
-    mock_query.assert_called_once_with("minimum", num_points=num_points_kwargs.get("num_points", 1))
+    mock_query.assert_called_once_with(
+        "minimum", num_points=num_points_kwargs.get("num_points", 1), group_by=None
+    )
 
 
 @pytest.mark.parametrize("invalid_datatype", ["str", "bool", "category"])
 def test_min_invalid_datatype(invalid_datatype, series_obj_factory):
     with pytest.raises(ValueError):
         series_obj = series_obj_factory(invalid_datatype)
         _ = series_obj.min()
@@ -117,25 +125,27 @@
 
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_min_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.min()
-    mock_query.assert_called_once_with("minimum", num_points=1)
+    mock_query.assert_called_once_with("minimum", num_points=1, group_by=None)
 
 
 @pytest.mark.parametrize("num_points_kwargs", [{}, {"num_points": 1}, {"num_points": 10}])
 @pytest.mark.parametrize("datatype", ["int", "float"])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_max(mock_query, datatype, num_points_kwargs, series_obj_factory):
     series_obj = series_obj_factory(datatype)
     mock_query.return_value = 1000
     assert series_obj.max(**num_points_kwargs) == 1000
-    mock_query.assert_called_once_with("maximum", num_points=num_points_kwargs.get("num_points", 1))
+    mock_query.assert_called_once_with(
+        "maximum", num_points=num_points_kwargs.get("num_points", 1), group_by=None
+    )
 
 
 @pytest.mark.parametrize("invalid_datatype", ["str", "bool", "category"])
 def test_max_invalid_datatype(invalid_datatype, series_obj_factory):
     with pytest.raises(ValueError):
         series_obj = series_obj_factory(invalid_datatype)
         _ = series_obj.max()
@@ -143,15 +153,15 @@
 
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_max_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.max()
-    mock_query.assert_called_once_with("maximum", num_points=1)
+    mock_query.assert_called_once_with("maximum", num_points=1, group_by=None)
 
 
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_histogram(mock_query, series_obj):
     mock_query.return_value = {"a": 10}
     assert series_obj.histogram() == {"a": 10}
     mock_query.assert_called_once_with("category_percents")
@@ -162,14 +172,37 @@
 def test_histogram_error(mock_query, error, series_obj):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj.histogram()
     mock_query.assert_called_once_with("category_percents")
 
 
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_unique(mock_query, series_obj_str):
+    mock_query.return_value = {"a": 10, "b": -10, "c": None}
+    assert series_obj_str.unique() == set(["a", "b", "c"])
+    mock_query.assert_called_once_with("category_percents")
+
+
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_unique_b(mock_query, series_obj_bool):
+    mock_query.return_value = {"t": 10, "f": -10}
+    assert series_obj_bool.unique() == set(["t", "f"])
+    mock_query.assert_called_once_with("category_percents")
+
+
+@pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_unique_error(mock_query, error, series_obj_bool):
+    mock_query.side_effect = error
+    with pytest.raises(QueryError):
+        series_obj_bool.unique()
+    mock_query.assert_called_once_with("category_percents")
+
+
 @pytest.mark.parametrize("vals", [[0.5], [1, 2, 3], []])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_quantile(mock_query, vals, series_obj):
     mock_query.return_value = {1: 10}
     assert series_obj.quantile(vals) == {1.0: 10}
     mock_query.assert_called_once_with("quantiles", quantile_vals=vals)
 
@@ -216,41 +249,82 @@
 
 def test_dtype(series_obj):
     assert series_obj._dtype() == "int"
 
 
 @pytest.mark.parametrize("tags", [{}, {"foo": "bar"}])
 @pytest.mark.parametrize("filters", [[], [{"some": "filter"}]])
+@pytest.mark.parametrize(
+    "group_by_info",
+    [
+        (None, "str"),
+        ("proj_datanode", "intC"),
+        ("feed_datanode", "intB"),
+        ("column-missing-from-schema", None),
+    ],
+)
 @mock.patch("gantry.query.core.dataframe._raw_query_cached_request")
-def test_aggregate_query(mock_query_data, series_obj_factory_with_filters_and_tags, filters, tags):
-    content = json.dumps(
-        {
-            "start_time": "2008-09-03T20:56:35",
-            "end_time": "2008-09-10T23:58:23",
-            "version": "1.2.3",
-            "num_points": 1,
-            "queries": {
-                "query": {
-                    "query_type": "feature",
-                    "model_node_id": "ABCD1234",
-                    "stat": "some-attribute",
-                    "stat_kwargs": {"some-attribute": {"a": 10}},
-                    "feature": "series_name",
-                    "filters": filters,
-                    "tags": tags,
-                }
-            },
+def test_aggregate_query(
+    mock_query_data, series_obj_factory_with_filters_and_tags, filters, tags, group_by_info
+):
+    group_by = group_by_info[0]
+    group_by_type = group_by_info[1]
+    content_dict = {
+        "start_time": "2008-09-03T20:56:35",
+        "end_time": "2008-09-10T23:58:23",
+        "version": "1.2.3",
+        "num_points": 1,
+        "queries": {
+            "query": {
+                "query_type": "feature",
+                "model_node_id": "ABCD1234",
+                "stat": "some-attribute",
+                "stat_kwargs": {"some-attribute": {"a": 10}},
+                "feature": "series_name",
+                "filters": filters,
+                "tags": tags,
+            }
         },
-        default=lambda x: x.isoformat(),
-    )
+    }
+    if group_by is not None:
+        content_dict["queries"]["query"]["group_by"] = [
+            {"feature_name": group_by, "dtype": group_by_type}
+        ]
+        mock_query_data.return_value = {
+            "response": "ok",
+            "data": {
+                "query": [
+                    {
+                        "group": [{"feature_name": group_by, "value": "group_by_unique_val1"}],
+                        "some-attribute": 9,
+                    },
+                    {
+                        "group": [{"feature_name": group_by, "value": "group_by_unique_val2"}],
+                        "some-attribute": 11,
+                    },
+                ]
+            },
+        }
+    else:
+        mock_query_data.return_value = {"response": "ok", "data": {"query": {"some-attribute": 10}}}
+    content = json.dumps(content_dict, default=lambda x: x.isoformat())
+
     series_obj = series_obj_factory_with_filters_and_tags("int", filters=filters, tags=tags)
-    mock_query_data.return_value = {"response": "ok", "data": {"query": {"some-attribute": 10}}}
 
-    assert series_obj._aggregate_query("some-attribute", a=10) == 10
-    mock_query_data.assert_called_with(series_obj.api_client, content, resource="aggregate")
+    if group_by_type is not None:
+        result = series_obj._aggregate_query("some-attribute", a=10, group_by=group_by)
+        mock_query_data.assert_called_with(series_obj.api_client, content, resource="aggregate")
+        if group_by is None:
+            assert result == 10
+        else:
+            assert result["some-attribute"].sum() == 20
+            assert len(result) == 2
+    else:
+        with pytest.raises(ValueError, match=f"Cannot find column {group_by} in dataframe."):
+            result = series_obj._aggregate_query("some-attribute", a=10, group_by=group_by)
 
 
 @pytest.mark.parametrize("num_points", [2, 5, 10])
 @pytest.mark.parametrize("tags", [{}, {"foo": "bar"}])
 @pytest.mark.parametrize("filters", [[], [{"some": "filter"}]])
 @mock.patch("gantry.query.core.dataframe._raw_query_cached_request")
 def test_aggregate_query_num_points(
@@ -749,7 +823,123 @@
 
     # < 20 and < 10 filters
     assert s3.parent_dataframe.filters == [
         {"feature_name": "A", "lower_bound": 20},
         {"feature_name": "A", "upper_bound": 10},
     ]
     assert s3.parent_dataframe.tags == {"foo": "bar"}
+
+
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_percent_null(mock_query, series_obj_bool):
+    mock_query.return_value = 50.0
+    assert series_obj_bool.percent_null() == 50.0
+    mock_query.assert_called_once_with("percent_null", num_points=1, group_by=None)
+
+
+@pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_percent_null_error(mock_query, error, series_obj_bool):
+    mock_query.side_effect = error
+    with pytest.raises(QueryError):
+        series_obj_bool.percent_null()
+    mock_query.assert_called_once_with("percent_null", num_points=1, group_by=None)
+
+
+@mock.patch("gantry.query.core.dataframe.GantrySeries._filter_builder")
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+@mock.patch("gantry.query.core.dataframe.get_application_node_id")
+@mock.patch(
+    "gantry.query.core.queryframe.GantryQueryFrame.metadata",
+    return_value=MULTIPLE_FEATURES_INT_DATA,
+    new_callable=mock.PropertyMock,
+)
+@pytest.mark.parametrize("dropna", [True, False])
+def test_percent_true(
+    metadata,
+    get_application_node_id_mock,
+    mock_query,
+    mock_na,
+    series_obj_bool,
+    dropna,
+    api_client_obj,
+):
+    get_application_node_id_mock.return_value = "12345"
+    df = dataframe.GantryDataFrame(
+        api_client=api_client_obj,
+        application="foobar",
+        version="1.2.3",
+        env="dev",
+        start_time=START_TIME,
+        end_time=END_TIME,
+        filters=[],
+        tags={"foo": "bar"},
+    )
+
+    series_obj_bool.parent_dataframe = df
+
+    filters = dataframe.Filters._from_single_filter({"foo": "bar"}, series_obj_bool)
+    mock_query.return_value = 50.0
+    mock_na.return_value = filters
+    assert series_obj_bool.percent_true(dropna=dropna) == 50.0
+    mock_query.assert_called_once_with("percent_true", num_points=1, group_by=None)
+    if dropna:
+        mock_na.assert_called_once_with("null_value", False)
+
+
+@pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_percent_true_error(mock_query, error, series_obj_bool):
+    mock_query.side_effect = error
+    with pytest.raises(QueryError):
+        series_obj_bool.percent_true()
+    mock_query.assert_called_once_with("percent_true", num_points=1, group_by=None)
+
+
+@mock.patch("gantry.query.core.dataframe.GantrySeries._filter_builder")
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+@mock.patch("gantry.query.core.dataframe.get_application_node_id")
+@mock.patch(
+    "gantry.query.core.queryframe.GantryQueryFrame.metadata",
+    return_value=MULTIPLE_FEATURES_INT_DATA,
+    new_callable=mock.PropertyMock,
+)
+@pytest.mark.parametrize("dropna", [True, False])
+def test_percent_false(
+    metadata,
+    get_application_node_id_mock,
+    mock_query,
+    mock_na,
+    series_obj_bool,
+    dropna,
+    api_client_obj,
+):
+    get_application_node_id_mock.return_value = "12345"
+    df = dataframe.GantryDataFrame(
+        api_client=api_client_obj,
+        application="foobar",
+        version="1.2.3",
+        env="dev",
+        start_time=START_TIME,
+        end_time=END_TIME,
+        filters=[],
+        tags={"foo": "bar"},
+    )
+
+    series_obj_bool.parent_dataframe = df
+
+    filters = dataframe.Filters._from_single_filter({"foo": "bar"}, series_obj_bool)
+    mock_query.return_value = 50.0
+    mock_na.return_value = filters
+    assert series_obj_bool.percent_false(dropna=dropna) == 50.0
+    mock_query.assert_called_once_with("percent_false", num_points=1, group_by=None)
+    if dropna:
+        mock_na.assert_called_once_with("null_value", False)
+
+
+@pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_percent_false_error(mock_query, error, series_obj_bool):
+    mock_query.side_effect = error
+    with pytest.raises(QueryError):
+        series_obj_bool.percent_false()
+    mock_query.assert_called_once_with("percent_false", num_points=1, group_by=None)
```

### Comparing `gantry-0.5.9/tests/query/core/test_utils.py` & `gantry-0.6.0a0/tests/query/core/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     assert empty_df.columns[0] == "A"
     assert empty_df.columns[1] == "B"
     assert empty_df.columns[2] == "C"
     assert empty_df.columns[3] == "D"
     assert empty_df.columns[4] == "E"
     assert empty_df.columns[5] == "F"
 
-    assert list(empty_df.dtypes.iteritems()) == [
+    assert list(empty_df.dtypes.items()) == [
         ("A", np.dtype("int64")),
         ("B", np.dtype("O")),
         ("C", np.dtype("float")),
         ("D", pd.CategoricalDtype(categories=[])),
         ("E", np.dtype("bool")),
         ("F", np.dtype("O")),
     ]
```

### Comparing `gantry-0.5.9/tests/query/distance/test_main.py` & `gantry-0.6.0a0/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/metric/test_main.py` & `gantry-0.6.0a0/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/test_client.py` & `gantry-0.6.0a0/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/query/test_main.py` & `gantry-0.6.0a0/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/test_api_client.py` & `gantry-0.6.0a0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/test_init.py` & `gantry-0.6.0a0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/test_utils.py` & `gantry-0.6.0a0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.5.9/tests/test_validator.py` & `gantry-0.6.0a0/tests/test_validator.py`

 * *Files identical despite different names*

