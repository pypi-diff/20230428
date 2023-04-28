# Comparing `tmp/devex_sdk-1.0.1.tar.gz` & `tmp/devex_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devex_sdk-1.0.1.tar", last modified: Thu Apr 20 23:07:02 2023, max compression
+gzip compressed data, was "devex_sdk-1.0.2.tar", last modified: Thu Apr 27 17:30:53 2023, max compression
```

## Comparing `devex_sdk-1.0.1.tar` & `devex_sdk-1.0.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/add.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/bucketization/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/bucketization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/bucketization/bucketization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/circles/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/circles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/circles/circles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk/data_ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Container.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Node.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Pod.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/PodNet.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/eks_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/gz_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/nested_json_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/pandas_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/extras/divide.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/extras/multiply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/feature_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/feature_engine/feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/parity/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/parity/number_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/project_inital_setup/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/console_setup_run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/notebook_setup_run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/project_inital_setup/understanding_eks_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.973944 devex_sdk-1.0.1/devex_sdk/update_cwd/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/update_cwd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/devex_sdk/update_cwd/notebook_setup_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.969944 devex_sdk-1.0.1/devex_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 23:07:02.000000 devex_sdk-1.0.1/devex_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-20 23:06:43.000000 devex_sdk-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:07:02.977944 devex_sdk-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_circles.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_divide.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_eks_bucketization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_gz_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_multiply.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_parity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 23:06:42.000000 devex_sdk-1.0.1/tests/test_update_cwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.779660 devex_sdk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 17:30:53.779660 devex_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.771659 devex_sdk-1.0.2/devex_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.771659 devex_sdk-1.0.2/devex_sdk/bucketization/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/bucketization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/bucketization/bucketization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.771659 devex_sdk-1.0.2/devex_sdk/circles/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/circles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/circles/circles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/data_ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Container.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Pod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/PodNet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/eks_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/gz_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/nested_json_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/pandas_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/spark_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/spark_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/data_ingestion/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/extras/divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/extras/multiply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/feature_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/feature_engine/feature_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/parity/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/parity/number_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.775659 devex_sdk-1.0.2/devex_sdk/project_inital_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/project_inital_setup/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/project_inital_setup/console_setup_run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/project_inital_setup/notebook_setup_run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/project_inital_setup/understanding_eks_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.779660 devex_sdk-1.0.2/devex_sdk/update_cwd/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/update_cwd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/devex_sdk/update_cwd/notebook_setup_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.771659 devex_sdk-1.0.2/devex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 17:30:53.000000 devex_sdk-1.0.2/devex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-27 17:30:53.000000 devex_sdk-1.0.2/devex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:30:53.000000 devex_sdk-1.0.2/devex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:30:53.000000 devex_sdk-1.0.2/devex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 17:30:53.000000 devex_sdk-1.0.2/devex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:30:53.779660 devex_sdk-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:30:53.779660 devex_sdk-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_circles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_eks_bucketization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_gz_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 17:30:37.000000 devex_sdk-1.0.2/tests/test_update_cwd.py
```

### Comparing `devex_sdk-1.0.1/LICENSE.txt` & `devex_sdk-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/PKG-INFO` & `devex_sdk-1.0.2/devex_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: devex_sdk
-Version: 1.0.1
+Name: devex-sdk
+Version: 1.0.2
 Summary: Dish DevEx open source SDK
 Home-page: https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -18,24 +18,26 @@
 ```console
 pip install git+https://github.com/DISHDevEx/dish-devex-sdk.git
 ```
 
 ### __Installing devex_sdk__ from local build (beta testing):
 1. Navigate into the root _devex_sdk_ directory.
 ```console
-$ cd dish-devex-sdk
+cd dish-devex-sdk
 ```
 2. Run the following command to create the wheel file
  
 ```console
-$ python setup.py bdist_wheel
+python setup.py bdist_wheel --version <VERSION_NUMBER>
 ```
+**NOTE**: the ***<VERSION_NUMBER>*** only effects your local build.  You can use any version number you like.  This can be helpful in testing prior to submitting a pull request.  Alternatively, you can eclude the ***--version <VERSION_NUMBER>*** flag and the .whl file name will output as ***devex_sdk-_VERSION_PLACEHOLDER_-py3-none-any.whl***
+
 3. Next, pip install the wheel file by running the following command, note that the _version_ will change depending upon the release:
 ```console
-$ pip install /dist/devex_sdk-(version)-py3-non-any.whl
+pip install /dist/devex_sdk-<VERSION_NUMBER>-py3-none-any.whl
 ```
 ### __Usage__
 
 Once complete, _devex_sdk_ will be available in your Python evironment for use.  Enter your Python environment and import _devex_sdk_ as you would with any other library or package.
 ```console
 >>> import devex_sdk
 ```
```

### Comparing `devex_sdk-1.0.1/README.md` & `devex_sdk-1.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 ```console
 pip install git+https://github.com/DISHDevEx/dish-devex-sdk.git
 ```
 
 ### __Installing devex_sdk__ from local build (beta testing):
 1. Navigate into the root _devex_sdk_ directory.
 ```console
-$ cd dish-devex-sdk
+cd dish-devex-sdk
 ```
 2. Run the following command to create the wheel file
  
 ```console
-$ python setup.py bdist_wheel
+python setup.py bdist_wheel --version <VERSION_NUMBER>
 ```
+**NOTE**: the ***<VERSION_NUMBER>*** only effects your local build.  You can use any version number you like.  This can be helpful in testing prior to submitting a pull request.  Alternatively, you can eclude the ***--version <VERSION_NUMBER>*** flag and the .whl file name will output as ***devex_sdk-_VERSION_PLACEHOLDER_-py3-none-any.whl***
+
 3. Next, pip install the wheel file by running the following command, note that the _version_ will change depending upon the release:
 ```console
-$ pip install /dist/devex_sdk-(version)-py3-non-any.whl
+pip install /dist/devex_sdk-<VERSION_NUMBER>-py3-none-any.whl
 ```
 ### __Usage__
 
 Once complete, _devex_sdk_ will be available in your Python evironment for use.  Enter your Python environment and import _devex_sdk_ as you would with any other library or package.
 ```console
 >>> import devex_sdk
 ```
```

### Comparing `devex_sdk-1.0.1/devex_sdk/__init__.py` & `devex_sdk-1.0.2/devex_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/bucketization/bucketization.py` & `devex_sdk-1.0.2/devex_sdk/bucketization/bucketization.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/circles/circles.py` & `devex_sdk-1.0.2/devex_sdk/circles/circles.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Cluster.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Cluster.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Container.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Container.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Node.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Node.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/Pod.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/Pod.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/PodNet.json` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/PodNet.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/eks_connector.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/eks_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/gz_connector.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/gz_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-"""Process gzip (.gz) files."""
+"""Process gzip (.gz) logs."""
 import gzip
 import json
+from json import JSONDecodeError
+import sys
 import pandas as pd
 import boto3
 
+
 class GzConnector():
     """
     Preprocess EKS logs in a gzip (.gz) file format.
 
     Parameters
     ----------
         bucket : string
             s3 bucket to read.
 
         log_type : {'application', 'controlplane', 'dataplane', 'host', 'performance'}
-            Log-type to ingest.
+            Log-type to process.
 
-        year : string
-            The year from which to ingest logs.
+        year : string, starting with '2023'
+            The year for which to process logs.
+            Example: '2023'
 
-        month : string
-            The month from which to ingest logs.
+        month : string, ['01'-'12']
+            The month for which to process logs.
 
-        day : string
-            The day of the month from which to ingest logs.
+        day : string, ['01'-'31']
+            The day of the month for which to process logs.
 
-        hour : string
-            The hour of day from which to ingest logs.
+        hour : string ['00'-'23']
+            The hour of day for which to process logs.
 
         perf_rec_type : {'node', 'nodefs', 'nodediskio', 'nodenet', 'pod', 'podnet', 'container',
                          'containerfs', 'cluster', 'clusterservice', 'clusternamespace'}
             The performance log record type to filter by.
 
+        cp_log_type : {'kube-scheduler', 'kube-controller-manager', 'kube-apiserver',
+                       'authenticator', 'cloud-controller-manager'}
+            The control plane component for which to process logs.
+
     Methods
     -------
         get_paths(self)
             Get .gz log paths from bucket, filtered by user input of date and hour.
 
         get_objects(self, paths)
             Get objects from paths.
@@ -84,16 +92,16 @@
                 - 'data'
 
         init_host(self, contents)
             Initialize the contents of .gz log file(s) to a dataframe with two columns:
                 - 'log_timestamp'
                 - 'data'
 
-        explode(self, df)
-            Explode nested JSON column in dataframe.
+        normalize(self, df)
+            Normalize nested JSON column in dataframe.
 
         read(self)
             Utilize the methods of GzConnector to read .gz files and convert them to a dataframe.
             If pref_rec_type is provided, dataframe will be filtered by it.
             
         filter_by_columns(self, columns)
             Filter dataframe by column(s).
@@ -103,18 +111,24 @@
                  cp_log_type=None, test=None):
         """
         Construct all the necessary parameters for the GzConnector object.
         """
         self.bucket = bucket
         self.log_type = log_type
         self.misc = misc        # This will later be renamed or removed. Currently not in docstring
-        self.year = year
-        self.month = month
-        self.day = day
-        self.hour = hour
+        if test:
+            self.year = None
+            self.month = None
+            self.day = None
+            self.hour = None
+        else:
+            self.year = int(year)
+            self.month = int(month)
+            self.day = int(day)
+            self.hour = int(hour)
         self.perf_rec_type = perf_rec_type
         self.cp_log_type = cp_log_type
         if cp_log_type:
             self.prefix = f'{misc}/{log_type}/{cp_log_type}/{year}/{month}/{day}/{hour}'
         elif test:
             self.prefix = 'pytest/gz_files'
         else:
@@ -134,15 +148,15 @@
         bucket = self.s3_resource.Bucket('respons-logs')
         paths = []
 
         for i in bucket.objects.filter(Prefix=self.prefix):
             if i.key.endswith('.gz'):
                 paths.append(f'{self.bucket}/{i.key}')
 
-        print('Number of .gz files:', len(paths))
+        print(f'Number of .gz files to process: {len(paths)}')
         return paths
 
     def get_objects(self, paths):
         """
         Get objects from paths.
 
         Parameters
@@ -151,20 +165,27 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             objects : list
                 Objects of .gz log file(s).
         """
+        if len(paths) == 0:
+            print("No paths ending with '.gz' found in S3 given the input parametes.")
+            sys.exit()
+
         objects = []
+
         for path in paths:
             key = path[path.find(self.bucket)+len(self.bucket)+1:]
             obj = self.s3_resource.Object(bucket_name=self.bucket, key=key)
             objects.append(obj)
 
+        print(f'Number of objects from files: {len(objects)}')
+
         return objects
 
     def process_objects(self, objects):
         """
         Process objects from bytes to strings.
 
         Parameters
@@ -173,25 +194,33 @@
                 Ojects of .gz log file(s)
 
         Returns
         -------
             contents : list
                 Content of .gz log file(s) in string format.
         """
+        if len(objects) == 0:
+            print("Error. Cannot process an empty list.")
+            sys.exit()
+
         contents = []
 
         for obj in objects:
             with gzip.GzipFile(fileobj=obj.get()['Body']) as gzfile:
                 content = gzfile.read().decode('utf-8')
                 content = content.split('\n')
                 if '' in content:
                     content.remove('')
                 contents.append(content)
                 gzfile.close()
-
+        
+        if len(contents) == 0:
+            print("Error creating list of object. List is empty.")
+            sys.exit()
+            
         return contents
 
     def init_performance(self, contents):
         """
         Initialize the contents of .gz log file(s) to a dataframe with two columns:
             - 'log_timestamp'
             - 'data'
@@ -204,27 +233,36 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of performance logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+        
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
         for content in contents:
             rows_list = []
             for row in content:
                 idx = row.find(' ')
                 row = [ row[:idx], row[idx:] ]
                 rows_list.append(row)
 
             gz_df = pd.DataFrame(rows_list, columns=['log_timestamp', 'data'])
             df = pd.concat([df, gz_df])
 
         df = df.drop_duplicates().reset_index(drop=True)
-        df['data'] = df.data.apply(json.loads)
+
+        try:
+            df['data'] = df.data.apply(json.loads)
+        except (JSONDecodeError, TypeError):
+            print("Error converting 'data' column to JSON. Dataframe returned without conversion.")
+            return df
 
         return df
 
     def init_application(self, contents):
         """
         Initialize the contents of .gz log file(s) to a dataframe with two columns:
             - 'log_timestamp'
@@ -238,27 +276,36 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of application logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
         for content in contents:
             rows_list = []
             for row in content:
                 idx = row.find(' ')
                 row = [ row[:idx], row[idx:] ]
                 rows_list.append(row)
 
             gz_df = pd.DataFrame(rows_list, columns=['log_timestamp', 'data'])
             df = pd.concat([df, gz_df])
 
         df = df.drop_duplicates().reset_index(drop=True)
-        df['data'] = df.data.apply(json.loads)
+
+        try:
+            df['data'] = df.data.apply(json.loads)
+        except (JSONDecodeError, TypeError):
+            print("Error converting 'data' column to JSON. Dataframe returned without conversion.")
+            return df
 
         return df
 
     def init_cp_scheduler(self, contents):
         """
         Initialize the contents of .gz log file(s) to a dataframe with two columns:
             - 'log_timestamp'
@@ -274,14 +321,18 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of control plane scheduler logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
         for content in contents:
             rows_list = []
             for row in content:
                 row = row.split('      ')
                 rows_list.append(row)
 
@@ -309,14 +360,19 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of control plane kube controller manager logs.
         """
+        
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
         for content in contents:
             rows_list = []
             for row in content:
                 row = row.split('      ')
                 rows_list.append(row)
 
@@ -344,14 +400,18 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of control plane kube api logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+        
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
         row_type1 = []
         row_type2 = []
 
         for content in contents:
 
             for row in content:
@@ -387,14 +447,18 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of control plane authenticator logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+        
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
 
         for content in contents:
             log_timestamps = []
             data = []
 
             for row in content:
@@ -405,14 +469,15 @@
 
             gz_df = pd.DataFrame(columns=['log_timestamp', 'data'])
             gz_df['log_timestamp'] = log_timestamps
             gz_df['data'] = data
 
             df = pd.concat([df, gz_df])
             df = df.drop_duplicates().reset_index(drop=True)
+
         return df
 
     def init_cp_cloud_controller(self, contents):
         """
         Initialize the contents of .gz log file(s) to a dataframe with two columns:
             - 'log_timestamp'
             - 'data'
@@ -423,26 +488,31 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of control plane cloud controller manager logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
 
         for content in contents:
             rows_list = []
 
             for row in content:
                 row = row.split('      ')
                 rows_list.append(row)
 
             gz_df = pd.DataFrame(rows_list, columns=['log_timestamp', 'data'])
             df = pd.concat([df, gz_df])
             df = df.drop_duplicates().reset_index(drop=True)
+
         return df
 
     def init_dataplane(self, contents):
         """
         Initialize the contents of .gz log file(s) to a dataframe with two columns:
             - 'log_timestamp'
             - 'data'
@@ -455,14 +525,18 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of data plane logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
 
         for content in contents:
             rows_list = []
 
             for row in content:
                 idx = row.find(' ')
@@ -491,63 +565,77 @@
                 List of .gz log file path(s).
 
         Returns
         -------
             df : dataframe
                 Pandas dataframe of data plane logs.
         """
+        if len(contents) == 0:
+            print('Error. List of contents is empty. Cannot process an empty list.')
+            sys.exit()
+
         df = pd.DataFrame(columns=['log_timestamp', 'data'])
         for content in contents:
             rows_list = []
             for row in content:
                 idx = row.find(' ')
                 row = [ row[:idx], row[idx:].lstrip() ]
                 rows_list.append(row)
 
             gz_df = pd.DataFrame(rows_list, columns=['log_timestamp', 'data'])
             df = pd.concat([df, gz_df])
 
         df = df.drop_duplicates().reset_index(drop=True)
-        df['data'] = df.data.apply(json.loads)
+
+        try:
+            df['data'] = df.data.apply(json.loads)
+        except (JSONDecodeError, TypeError):
+            print("Error converting 'data' column to JSON. Dataframe returned without conversion.")
+            return df
 
         return df
 
-    def explode(self, df):
+    def normalize(self, df):
         """
-        Explode nested JSON column in dataframe.
+        Normalize nested JSON column in dataframe.
 
         Parameters
         ----------
             df : dataframe
                 Pandas dataframe with a column that has a nested JSON.
 
         Returns
         -------
             df : dataframe
-                Pandas dataframe with nested JSON column expldoded.
+                Pandas dataframe with nested JSON column normalized.
         """
-        print('explode called.')
-        if self.log_type in ['performance', 'application', 'dataplane', 'host']:
-            column = 'data'
-            data_normalized = pd.json_normalize(df[column])
-            df = pd.concat([
-                df[['log_timestamp', 'data']].reset_index(drop=True),
-                data_normalized],
-                axis=1,
-            )
-
-        elif self.log_type == 'controlplane':
-            column = 'message'
-            data_normalized = pd.json_normalize(df[column])
-            df = pd.concat([
-                df[['log_timestamp', 'message_type', 'message_code']].reset_index(drop=True),
-                data_normalized
-                ],
-                axis=1,
-            )
+        try:
+            if self.log_type in ['performance', 'application', 'dataplane', 'host']:
+                column = 'data'
+                data_normalized = pd.json_normalize(df[column])
+                df = pd.concat([
+                    df[['log_timestamp', 'data']].reset_index(drop=True),
+                    data_normalized],
+                    axis=1,
+                )
+
+            elif self.log_type == 'controlplane':
+                column = 'message'
+                data_normalized = pd.json_normalize(df[column])
+                df = pd.concat([
+                    df[['log_timestamp', 'message_type', 'message_code']].reset_index(drop=True),
+                    data_normalized
+                    ],
+                    axis=1,
+                )
+        except Exception as e:
+            print('Error normalizing dataframe. Dataframe returned without normalizing.')
+            print('Please see error below:')
+            print(e)
+            return df
 
         return df
 
     def read(self):
         """
         Utilize the methods of GzConnector to read .gz files and convert them to a dataframe.
 
@@ -557,28 +645,23 @@
         -------
             df : dataframe
                 Pandas dataframe whose nested JSON column is expldoded, filtered by perf_rec_type
                 if it is provided.
         """
         paths = self.get_paths()
         objects = self.get_objects(paths)
-        contents = self.process_objects(objects)
+        contents = self.process_objects(objects) # check for empty
 
         if self.log_type == 'performance':
             df = self.init_performance(contents)
-            df = self.explode(df)
-
-            if self.perf_rec_type:
-                df['Type'] = df['Type'].apply(lambda x: x.lower())
-                df = df[df.Type == self.perf_rec_type.lower()]
+            df = self.normalize(df)
 
         elif self.log_type == 'controlplane':
             if self.cp_log_type == 'kube-scheduler':
                 df = self.init_cp_scheduler(contents)
-                # df = self.explode(df)
 
             elif self.cp_log_type == 'kube-controller-manager':
                 df = self.init_cp_kube_controller(contents)
 
             elif self.cp_log_type == 'kube-apiserver':
                 df = self.init_cp_api(contents)
 
@@ -586,26 +669,34 @@
                 df = self.init_cp_authenticator(contents)
 
             elif self.cp_log_type == 'cloud-controller-manager':
                 df = self.init_cp_cloud_controller(contents)
 
         elif self.log_type == 'application':
             df = self.init_application(contents)
-            df = self.explode(df)
+            df = self.normalize(df)
 
         elif self.log_type == 'dataplane':
             df = self.init_dataplane(contents)
 
         elif self.log_type == 'host':
             df = self.init_host(contents)
-            df = self.explode(df)
+            df = self.normalize(df)
+        
+        if self.perf_rec_type:
+            try:
+                df['Type'] = df['Type'].apply(lambda x: x.lower())
+                df = df[df.Type == self.perf_rec_type.lower()]
+                df = df.dropna(how='all', axis=1)
+            except KeyError:
+                pass
 
         df = df.sort_values('log_timestamp').reset_index(drop=True)
         self.df = df
-
+        
         return self.df
 
     def filter_by_columns(self, columns):
         """
         Filter dataframe by column(s).
 
         Parameters
```

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/nested_json_connector.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/nested_json_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/pandas_data_connector.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/pandas_data_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_config.ini` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/spark_config.ini`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_data_connector.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/spark_data_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/data_ingestion/spark_utils.py` & `devex_sdk-1.0.2/devex_sdk/data_ingestion/spark_utils.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json` & `devex_sdk-1.0.2/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/feature_engine/feature_extractor.py` & `devex_sdk-1.0.2/devex_sdk/feature_engine/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/project_inital_setup/understanding_eks_setup.py` & `devex_sdk-1.0.2/devex_sdk/project_inital_setup/understanding_eks_setup.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk/update_cwd/notebook_setup_path.py` & `devex_sdk-1.0.2/devex_sdk/update_cwd/notebook_setup_path.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/devex_sdk.egg-info/PKG-INFO` & `devex_sdk-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: devex-sdk
-Version: 1.0.1
+Name: devex_sdk
+Version: 1.0.2
 Summary: Dish DevEx open source SDK
 Home-page: https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -18,24 +18,26 @@
 ```console
 pip install git+https://github.com/DISHDevEx/dish-devex-sdk.git
 ```
 
 ### __Installing devex_sdk__ from local build (beta testing):
 1. Navigate into the root _devex_sdk_ directory.
 ```console
-$ cd dish-devex-sdk
+cd dish-devex-sdk
 ```
 2. Run the following command to create the wheel file
  
 ```console
-$ python setup.py bdist_wheel
+python setup.py bdist_wheel --version <VERSION_NUMBER>
 ```
+**NOTE**: the ***<VERSION_NUMBER>*** only effects your local build.  You can use any version number you like.  This can be helpful in testing prior to submitting a pull request.  Alternatively, you can eclude the ***--version <VERSION_NUMBER>*** flag and the .whl file name will output as ***devex_sdk-_VERSION_PLACEHOLDER_-py3-none-any.whl***
+
 3. Next, pip install the wheel file by running the following command, note that the _version_ will change depending upon the release:
 ```console
-$ pip install /dist/devex_sdk-(version)-py3-non-any.whl
+pip install /dist/devex_sdk-<VERSION_NUMBER>-py3-none-any.whl
 ```
 ### __Usage__
 
 Once complete, _devex_sdk_ will be available in your Python evironment for use.  Enter your Python environment and import _devex_sdk_ as you would with any other library or package.
 ```console
 >>> import devex_sdk
 ```
```

### Comparing `devex_sdk-1.0.1/devex_sdk.egg-info/SOURCES.txt` & `devex_sdk-1.0.2/devex_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/tests/test_counts.py` & `devex_sdk-1.0.2/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/tests/test_dataframe_creation.py` & `devex_sdk-1.0.2/tests/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/tests/test_eks_bucketization.py` & `devex_sdk-1.0.2/tests/test_eks_bucketization.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.1/tests/test_gz_connector.py` & `devex_sdk-1.0.2/tests/test_gz_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 def test_init_host(host_contents, init_host_expected_df):
     gzc = GzConnector(bucket='respons-logs', misc=None, log_type='host',
                       year=None, month=None, day=None, hour=None,
                       perf_rec_type=None, cp_log_type=None, test=True)
     actual_result = gzc.init_host(host_contents)
     assert actual_result.equals(init_host_expected_df)
 
-def test_explode(gzc, df_to_explode, exploded_df_expected):
-    actual_result = gzc.explode(df_to_explode)
+def test_normalize(gzc, df_to_explode, exploded_df_expected):
+    actual_result = gzc.normalize(df_to_explode)
     assert actual_result.equals(exploded_df_expected)
 
 def test_read(gzc, df_read_expected):
     actual_result = gzc.read()
     assert actual_result.equals(df_read_expected)
 
 def test_filter_by_column(gzc, df_to_explode, df_filtered_expected):
```

### Comparing `devex_sdk-1.0.1/tests/test_schema.py` & `devex_sdk-1.0.2/tests/test_schema.py`

 * *Files identical despite different names*

