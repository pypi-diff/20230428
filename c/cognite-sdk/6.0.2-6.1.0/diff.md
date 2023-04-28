# Comparing `tmp/cognite_sdk-6.0.2.tar.gz` & `tmp/cognite_sdk-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.0.2.tar", max compression
+gzip compressed data, was "cognite_sdk-6.1.0.tar", max compression
```

## Comparing `cognite_sdk-6.0.2.tar` & `cognite_sdk-6.1.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/LICENSE
--rw-r--r--   0        0        0     3945 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/README.md
--rw-r--r--   0        0        0      503 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54659 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87006 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44656 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49923 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24600 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/config.py
--rw-r--r--   0        0        0    16261 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34160 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33929 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    22565 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    22892 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2109 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/LICENSE
+-rw-r--r--   0        0        0     3945 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/README.md
+-rw-r--r--   0        0        0      503 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87464 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17436 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44656 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49923 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/config.py
+-rw-r--r--   0        0        0    16261 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34160 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14287 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    22565 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    23134 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2109 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.1.0/PKG-INFO
```

### Comparing `cognite_sdk-6.0.2/LICENSE` & `cognite_sdk-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/README.md` & `cognite_sdk-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/annotations.py` & `cognite_sdk-6.1.0/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/assets.py` & `cognite_sdk-6.1.0/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/data_sets.py` & `cognite_sdk-6.1.0/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.1.0/cognite/client/_api/datapoint_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Union,
     cast,
 )
 
 from google.protobuf.message import Message
 from sortedcontainers import SortedDict, SortedList
 
-from cognite.client.data_classes.datapoints import NUMPY_IS_AVAILABLE, Datapoints, DatapointsArray
+from cognite.client.data_classes.datapoints import NUMPY_IS_AVAILABLE, Aggregate, Datapoints, DatapointsArray
 from cognite.client.utils._auxiliary import import_legacy_protobuf, is_unlimited
 from cognite.client.utils._identifier import Identifier
 from cognite.client.utils._text import convert_all_keys_to_snake_case, to_camel_case, to_snake_case
 from cognite.client.utils._time import (
     align_start_and_end_for_granularity,
     granularity_to_ms,
     split_time_range,
@@ -111,19 +111,19 @@
     items: List[CustomDatapoints]
 
 
 @dataclass
 class _DatapointsQuery:
     """Internal representation of a user request for datapoints, previously public (before v5)"""
 
-    start: Union[int, str, datetime, None] = None
-    end: Union[int, str, datetime, None] = None
+    start: int | str | datetime | None = None
+    end: int | str | datetime | None = None
     id: Optional[DatapointsId] = None
     external_id: Optional[DatapointsExternalId] = None
-    aggregates: Union[str, List[str], None] = None
+    aggregates: Aggregate | str | list[Aggregate | str] | None = None
     granularity: Optional[str] = None
     limit: Optional[int] = None
     include_outside_points: bool = False
     ignore_unknown_ids: bool = False
 
     @property
     def is_single_identifier(self) -> bool:
```

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/datapoints.py` & `cognite_sdk-6.1.0/cognite/client/_api/datapoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     _DatapointsQuery,
     _SingleTSQueryBase,
     _SingleTSQueryValidator,
 )
 from cognite.client._api.synthetic_time_series import SyntheticDatapointsAPI
 from cognite.client._api_client import APIClient
 from cognite.client.data_classes.datapoints import (
+    Aggregate,
     Datapoints,
     DatapointsArray,
     DatapointsArrayList,
     DatapointsList,
     LatestDatapointQuery,
 )
 from cognite.client.exceptions import CogniteAPIError, CogniteNotFoundError
@@ -596,24 +597,24 @@
         self._RETRIEVE_LATEST_LIMIT = 100
         self._POST_DPS_OBJECTS_LIMIT = 10_000
         self._GRANULARITY_HOURS_LIMIT = 100_000
 
     def retrieve(
         self,
         *,
-        id: Union[None, int, Dict[str, Any], Sequence[Union[int, Dict[str, Any]]]] = None,
-        external_id: Union[None, str, Dict[str, Any], Sequence[Union[str, Dict[str, Any]]]] = None,
-        start: Union[int, str, datetime, None] = None,
-        end: Union[int, str, datetime, None] = None,
-        aggregates: Union[str, List[str], None] = None,
+        id: None | int | dict[str, Any] | Sequence[int | dict[str, Any]] = None,
+        external_id: None | str | dict[str, Any] | Sequence[str | dict[str, Any]] = None,
+        start: int | str | datetime | None = None,
+        end: int | str | datetime | None = None,
+        aggregates: Aggregate | str | list[Aggregate | str] | None = None,
         granularity: Optional[str] = None,
         limit: Optional[int] = None,
         include_outside_points: bool = False,
         ignore_unknown_ids: bool = False,
-    ) -> Union[None, Datapoints, DatapointsList]:
+    ) -> None | Datapoints | DatapointsList:
         """`Retrieve datapoints for one or more time series. <https://docs.cognite.com/api/v1/#operation/getMultiTimeSeriesDatapoints>`_
 
         **Performance guide**:
             In order to retrieve millions of datapoints as efficiently as possible, here are a few guidelines:
 
             1. For best speed, and significantly lower memory usage, consider using `retrieve_arrays(...)` which uses `numpy.ndarrays` for data storage.
             2. Unlimited queries are fastest as they are trivial to parallelize. Thus, specifying a very large finite `limit`, e.g. 1 million, comes with a performance penalty.
@@ -782,24 +783,24 @@
         elif not dps_lst and ignore_unknown_ids:
             return None
         return dps_lst[0]
 
     def retrieve_arrays(
         self,
         *,
-        id: Union[None, int, Dict[str, Any], Sequence[Union[int, Dict[str, Any]]]] = None,
-        external_id: Union[None, str, Dict[str, Any], Sequence[Union[str, Dict[str, Any]]]] = None,
-        start: Union[int, str, datetime, None] = None,
-        end: Union[int, str, datetime, None] = None,
-        aggregates: Union[str, List[str], None] = None,
+        id: None | int | dict[str, Any] | Sequence[int | dict[str, Any]] = None,
+        external_id: None | str | dict[str, Any] | Sequence[str | dict[str, Any]] = None,
+        start: int | str | datetime | None = None,
+        end: int | str | datetime | None = None,
+        aggregates: Aggregate | str | list[Aggregate | str] | None = None,
         granularity: Optional[str] = None,
         limit: Optional[int] = None,
         include_outside_points: bool = False,
         ignore_unknown_ids: bool = False,
-    ) -> Union[None, DatapointsArray, DatapointsArrayList]:
+    ) -> None | DatapointsArray | DatapointsArrayList:
         """`Retrieve datapoints for one or more time series. <https://docs.cognite.com/api/v1/#operation/getMultiTimeSeriesDatapoints>`_
 
         **Note**: This method requires `numpy` to be installed.
 
         Args:
             start (Union[int, str, datetime, None]): Inclusive start. Default: 1970-01-01 UTC.
             end (Union[int, str, datetime, None]): Exclusive end. Default: "now"
@@ -878,19 +879,19 @@
         elif not dps_lst and ignore_unknown_ids:
             return None
         return dps_lst[0]
 
     def retrieve_dataframe(
         self,
         *,
-        id: Union[None, int, Dict[str, Any], Sequence[Union[int, Dict[str, Any]]]] = None,
-        external_id: Union[None, str, Dict[str, Any], Sequence[Union[str, Dict[str, Any]]]] = None,
-        start: Union[int, str, datetime, None] = None,
-        end: Union[int, str, datetime, None] = None,
-        aggregates: Union[str, List[str], None] = None,
+        id: None | int | dict[str, Any] | Sequence[int | dict[str, Any]] = None,
+        external_id: None | str | dict[str, Any] | Sequence[str | dict[str, Any]] = None,
+        start: int | str | datetime | None = None,
+        end: int | str | datetime | None = None,
+        aggregates: Aggregate | str | list[Aggregate | str] | None = None,
         granularity: Optional[str] = None,
         limit: Optional[int] = None,
         include_outside_points: bool = False,
         ignore_unknown_ids: bool = False,
         uniform_index: bool = False,
         include_aggregate_name: bool = True,
         include_granularity_name: bool = False,
@@ -917,47 +918,58 @@
             column_names ("id" | "external_id"): Use either ids or external ids as column names. Time series missing external id will use id as backup. Default: "external_id"
 
         Returns:
             pandas.DataFrame: A pandas DataFrame containing the requested time series. The ordering of columns is ids first, then external_ids. For time series with multiple aggregates, they will be sorted in alphabetical order ("average" before "max").
 
         Examples:
 
-            Get a pandas dataframe using a single id, and use this id as column name, with no more than 100 datapoints::
+            Get a pandas dataframe using a single id, and use this id as column name, with no more than 100 datapoints:
 
                 >>> from cognite.client import CogniteClient
                 >>> client = CogniteClient()
                 >>> df = client.time_series.data.retrieve_dataframe(
                 ...     id=12345,
                 ...     start="2w-ago",
                 ...     end="now",
                 ...     limit=100,
                 ...     column_names="id")
 
             Get the pandas dataframe with a uniform index (fixed spacing between points) of 1 day, for two time series with
-            individually specified aggregates, from 1990 through 2020::
+            individually specified aggregates, from 1990 through 2020:
 
                 >>> from datetime import datetime, timezone
                 >>> df = client.time_series.data.retrieve_dataframe(
                 ...     id=[
                 ...         {"external_id": "foo", "aggregates": ["discrete_variance"]},
                 ...         {"external_id": "bar", "aggregates": ["total_variation", "continuous_variance"]},
                 ...     ],
                 ...     granularity="1d",
                 ...     start=datetime(1990, 1, 1, tzinfo=timezone.utc),
                 ...     end=datetime(2020, 12, 31, tzinfo=timezone.utc),
                 ...     uniform_index=True)
 
             Get a pandas dataframe containing the 'average' aggregate for two time series using a 30-day granularity,
-            starting Jan 1, 1970 all the way up to present, without having the aggregate name in the column names::
+            starting Jan 1, 1970 all the way up to present, without having the aggregate name in the column names:
 
                 >>> df = client.time_series.data.retrieve_dataframe(
                 ...     external_id=["foo", "bar"],
                 ...     aggregates=["average"],
                 ...     granularity="30d",
                 ...     include_aggregate_name=False)
+
+            Remember that pandas.Timestamp is a subclass of datetime, so you can use Timestamps as start and
+            end arguments:
+
+                >>> import pandas as pd
+                >>> df = client.time_series.data.retrieve_dataframe(
+                ...     external_id="foo",
+                ...     start=pd.Timestamp("2023-01-01"),
+                ...     end=pd.Timestamp("2023-02-01"),
+                ...     )
+
         """
         _, pd = local_import("numpy", "pandas")  # Verify that deps are available or raise CogniteImportError
         if column_names not in {"id", "external_id"}:
             raise ValueError(f"Given parameter {column_names=} must be one of 'id' or 'external_id'")
 
         query = _DatapointsQuery(
             start=start,
@@ -997,15 +1009,15 @@
     def retrieve_dataframe_in_tz(
         self,
         *,
         id: int | Sequence[int] | None = None,
         external_id: str | Sequence[str] | None = None,
         start: datetime,
         end: datetime,
-        aggregates: Sequence[str] | str | None = None,
+        aggregates: Aggregate | str | Sequence[Aggregate | str] | None = None,
         granularity: Optional[str] = None,
         ignore_unknown_ids: bool = False,
         uniform_index: bool = False,
         include_aggregate_name: bool = True,
         include_granularity_name: bool = False,
         column_names: Literal["id", "external_id"] = "external_id",
     ) -> pd.DataFrame:
@@ -1032,15 +1044,15 @@
             DST with an offset from standard time that is not a multiple of 1 hour.
 
         Args:
             id (int | Sequence[int] | None): ID or list of IDs.
             external_id (str | Sequence[str] | None): External ID or list of External IDs.
             start (datetime): Inclusive start, must be time zone aware.
             end (datetime): Exclusive end, must be time zone aware and have the same time zone as start.
-            aggregates (str | list[str] | None): Single aggregate or list of aggregates to retrieve. Default: None (raw datapoints returned)
+            aggregates (Aggregate | str | Sequence[Aggregate | str] | None): Single aggregate or list of aggregates to retrieve. Default: None (raw datapoints returned)
             granularity (str): The granularity to fetch aggregates at, supported are: second, minute, hour, day, week, month, quarter and year. Default: None.
             ignore_unknown_ids (bool): Whether to ignore missing time series rather than raising an exception. Default: False
             uniform_index (bool): If querying aggregates, specifying `uniform_index=True` will return a dataframe with an
                 index with constant spacing between timestamps decided by granularity all the way from `start` to `end` (missing values will be NaNs). Default: False
             include_aggregate_name (bool): Include 'aggregate' in the column name, e.g. `my-ts|average`. Ignored for raw time series. Default: True
             include_granularity_name (bool): Include 'granularity' in the column name, e.g. `my-ts|12h`. Added after 'aggregate' when present. Ignored for raw time series. Default: False
             column_names ("id" | "external_id"): Use either ids or external ids as column names. Time series missing external id will use id as backup. Default: "external_id"
@@ -1112,15 +1124,15 @@
                     uniform_index=uniform_index,
                     include_aggregate_name=include_aggregate_name,
                     include_granularity_name=include_granularity_name,
                     column_names=column_names,
                     limit=None,
                 )
                 .tz_localize("utc")
-                .tz_convert(tz.key)
+                .tz_convert(str(tz))
             )
 
         assert isinstance(granularity, str)  # mypy
 
         if in_timedelta(granularity) / timedelta(hours=1) > self._GRANULARITY_HOURS_LIMIT:
             multiplier, unit = get_granularity_multiplier_and_unit(granularity)
             days = _unit_in_days(unit)
@@ -1128,15 +1140,15 @@
             raise ValueError(f"Granularity above the maximum limit, {limit} {unit}s.")
 
         identifiers = IdentifierSequence.load(id, external_id)
         if not identifiers.are_unique():
             duplicated = find_duplicates(identifiers.as_primitives())
             raise ValueError(f"The following identifiers were not unique: {duplicated}")
 
-        intervals = to_fixed_utc_intervals(start, end, granularity)
+        intervals = to_fixed_utc_intervals(start, end, granularity)  # type: ignore [arg-type]
 
         queries = [
             {**ident_dct, "aggregates": aggregates, **interval}  # type: ignore [arg-type]
             for ident_dct, interval in itertools.product(identifiers.as_dicts(), intervals)
         ]
 
         arrays = self.retrieve_arrays(
@@ -1145,31 +1157,31 @@
             **{identifiers[0].name(): queries},  # type: ignore [arg-type]
         )
         assert isinstance(arrays, DatapointsArrayList)  # mypy
         arrays.concat_duplicate_ids()
         df = (
             arrays.to_pandas(column_names, include_aggregate_name, include_granularity_name)
             .tz_localize("utc")
-            .tz_convert(tz.key)
+            .tz_convert(str(tz))
         )
 
         if uniform_index:
-            freq = to_pandas_freq(granularity, start)
-            start, end = align_large_granularity(start, end, granularity)
+            freq = to_pandas_freq(granularity, start)  # type: ignore [arg-type]
+            start, end = align_large_granularity(start, end, granularity)  # type: ignore [arg-type]
             return df.reindex(pandas_date_range_tz(start, end, freq, inclusive="left"))
 
         return df
 
     def retrieve_latest(
         self,
-        id: Union[int, LatestDatapointQuery, List[Union[int, LatestDatapointQuery]]] = None,
-        external_id: Union[str, LatestDatapointQuery, List[Union[str, LatestDatapointQuery]]] = None,
-        before: Union[None, int, str, datetime] = None,
+        id: int | LatestDatapointQuery | list[int | LatestDatapointQuery] | None = None,
+        external_id: str | LatestDatapointQuery | list[str | LatestDatapointQuery] | None = None,
+        before: None | int | str | datetime = None,
         ignore_unknown_ids: bool = False,
-    ) -> Union[None, Datapoints, DatapointsList]:
+    ) -> Datapoints | DatapointsList | None:
         """`Get the latest datapoint for one or more time series <https://docs.cognite.com/api/v1/#operation/getLatest>`_
 
         Args:
             id (Union[int, LatestDatapointQuery, List[Union[int, LatestDatapointQuery]]]): Id or list of ids.
             external_id (Union[str, LatestDatapointQuery, List[Union[str, LatestDatapointQuery]]]): External id or list of external ids.
             before: (Union[int, str, datetime]): Get latest datapoint before this time. Not used when passing 'LatestDatapointQuery'.
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
@@ -1220,20 +1232,18 @@
             return DatapointsList._load(res, cognite_client=self._cognite_client)
         elif not res and ignore_unknown_ids:
             return None
         return Datapoints._load(res[0], cognite_client=self._cognite_client)
 
     def insert(
         self,
-        datapoints: Union[
-            Datapoints,
-            DatapointsArray,
-            Sequence[Dict[str, Union[int, float, str, datetime]]],
-            Sequence[Tuple[Union[int, float, datetime], Union[int, float, str]]],
-        ],
+        datapoints: Datapoints
+        | DatapointsArray
+        | Sequence[dict[str, int | float | str | datetime]]
+        | Sequence[tuple[int | float | datetime, int | float | str]],
         id: int = None,
         external_id: str = None,
     ) -> None:
         """Insert datapoints into a time series
 
         Timestamps can be represented as milliseconds since epoch or datetime objects.
 
@@ -1290,15 +1300,15 @@
         else:
             dps_to_post = datapoints
 
         post_dps_object["datapoints"] = dps_to_post
         dps_poster = DatapointsPoster(self)
         dps_poster.insert([post_dps_object])
 
-    def insert_multiple(self, datapoints: List[Dict[str, Union[str, int, List, Datapoints, DatapointsArray]]]) -> None:
+    def insert_multiple(self, datapoints: list[dict[str, str | int | list | Datapoints | DatapointsArray]]) -> None:
         """`Insert datapoints into multiple time series <https://docs.cognite.com/api/v1/#operation/postMultiTimeSeriesDatapoints>`_
 
         Args:
             datapoints (List[Dict]): The datapoints you wish to insert along with the ids of the time series. See examples below.
 
         Returns:
             None
@@ -1333,15 +1343,15 @@
             # Extract data inplace for any Datapoints and/or DatapointsArray:
             if isinstance(dps_dct, Mapping) and isinstance(dps_dct["datapoints"], (Datapoints, DatapointsArray)):
                 dps_dct["datapoints"] = DatapointsPoster._extract_raw_data_from_dps_container(dps_dct["datapoints"])
         dps_poster = DatapointsPoster(self)
         dps_poster.insert(datapoints)
 
     def delete_range(
-        self, start: Union[int, str, datetime], end: Union[int, str, datetime], id: int = None, external_id: str = None
+        self, start: int | str | datetime, end: int | str | datetime, id: int = None, external_id: str = None
     ) -> None:
         """Delete a range of datapoints from a time series.
 
         Args:
             start (Union[int, str, datetime]): Inclusive start of delete range
             end (Union[int, str, datetime]): Exclusvie end of delete range
             id (int): Id of time series to delete data from
@@ -1362,15 +1372,15 @@
         end = timestamp_to_ms(end)
         assert end > start, "end must be larger than start"
 
         identifier = Identifier.of_either(id, external_id).as_dict()
         delete_dps_object = {**identifier, "inclusiveBegin": start, "exclusiveEnd": end}
         self._delete_datapoints_ranges([delete_dps_object])
 
-    def delete_ranges(self, ranges: List[Dict[str, Any]]) -> None:
+    def delete_ranges(self, ranges: list[dict[str, Any]]) -> None:
         """`Delete a range of datapoints from multiple time series. <https://docs.cognite.com/api/v1/#operation/deleteDatapoints>`_
 
         Args:
             ranges (List[Dict[str, Any]]): The list of datapoint ids along with time range to delete. See examples below.
 
         Returns:
             None
@@ -1391,15 +1401,15 @@
             valid_range.update(
                 inclusiveBegin=timestamp_to_ms(time_range["start"]),
                 exclusiveEnd=timestamp_to_ms(time_range["end"]),
             )
             valid_ranges.append(valid_range)
         self._delete_datapoints_ranges(valid_ranges)
 
-    def _delete_datapoints_ranges(self, delete_range_objects: List[Dict]) -> None:
+    def _delete_datapoints_ranges(self, delete_range_objects: list[dict]) -> None:
         self._post(url_path=self._RESOURCE_PATH + "/delete", json={"items": delete_range_objects})
 
     def insert_dataframe(self, df: pd.DataFrame, external_id_headers: bool = True, dropna: bool = True) -> None:
         """Insert a dataframe (columns must be unique).
 
         The index of the dataframe must contain the timestamps (pd.DatetimeIndex). The names of the columns specify
         the ids or external ids of the time series to which the datapoints will be written.
@@ -1455,15 +1465,15 @@
 class DatapointsBin:
     def __init__(self, dps_objects_limit: int, dps_limit: int):
         self.dps_objects_limit = dps_objects_limit
         self.dps_limit = dps_limit
         self.current_num_datapoints = 0
         self.dps_object_list: List[dict] = []
 
-    def add(self, dps_object: Dict[str, Any]) -> None:
+    def add(self, dps_object: dict[str, Any]) -> None:
         self.current_num_datapoints += len(dps_object["datapoints"])
         self.dps_object_list.append(dps_object)
 
     def will_fit(self, number_of_dps: int) -> bool:
         will_fit_dps = (self.current_num_datapoints + number_of_dps) <= self.dps_limit
         will_fit_dps_objects = (len(self.dps_object_list) + 1) <= self.dps_objects_limit
         return will_fit_dps and will_fit_dps_objects
@@ -1471,15 +1481,15 @@
 
 class DatapointsPoster:
     def __init__(self, dps_client: DatapointsAPI) -> None:
         self.dps_client = dps_client
         self.limit = self.dps_client._DPS_INSERT_LIMIT
         self.bins: List[DatapointsBin] = []
 
-    def insert(self, dps_object_list: List[Dict[str, Any]]) -> None:
+    def insert(self, dps_object_list: list[dict[str, Any]]) -> None:
         valid_dps_object_list = self._validate_dps_objects(dps_object_list)
         binned_dps_object_lists = self._bin_datapoints(valid_dps_object_list)
         self._insert_datapoints_concurrently(binned_dps_object_lists)
 
     @staticmethod
     def _extract_raw_data_from_dps_container(
         dps: Union[Datapoints, DatapointsArray]
```

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/diagrams.py` & `cognite_sdk-6.1.0/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.1.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/events.py` & `cognite_sdk-6.1.0/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.1.0/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/files.py` & `cognite_sdk-6.1.0/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/functions.py` & `cognite_sdk-6.1.0/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/geospatial.py` & `cognite_sdk-6.1.0/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/iam.py` & `cognite_sdk-6.1.0/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/labels.py` & `cognite_sdk-6.1.0/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/raw.py` & `cognite_sdk-6.1.0/cognite/client/_api/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,16 +317,16 @@
         Fetches rows as they are iterated over, so you keep a limited number of rows in memory.
 
         Args:
             db_name (str): Name of the database
             table_name (str): Name of the table to iterate over rows for
             chunk_size (int, optional): Number of rows to return in each chunk. Defaults to yielding one row a time.
             limit (int, optional): Maximum number of rows to return. Defaults to return all items.
-            min_last_updated_time (int): Rows must have been last updated after this time. ms since epoch.
-            max_last_updated_time (int): Rows must have been last updated before this time. ms since epoch.
+            min_last_updated_time (int): Rows must have been last updated after this time (exclusive). ms since epoch.
+            max_last_updated_time (int): Rows must have been last updated before this time (inclusive). ms since epoch.
             columns (List[str]): List of column keys. Set to `None` for retrieving all, use [] to retrieve only row keys.
         """
         return self._list_generator(
             list_cls=RowList,
             resource_cls=Row,
             resource_path=utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, db_name, table_name),
             chunk_size=chunk_size,
@@ -497,16 +497,16 @@
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> RowList:
         """`List rows in a table. <https://docs.cognite.com/api/v1/#operation/getRows>`_
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
-            min_last_updated_time (int): Rows must have been last updated after this time. ms since epoch.
-            max_last_updated_time (int): Rows must have been last updated before this time. ms since epoch.
+            min_last_updated_time (int): Rows must have been last updated after this time (exclusive). ms since epoch.
+            max_last_updated_time (int): Rows must have been last updated before this time (inclusive). ms since epoch.
             columns (List[str]): List of column keys. Set to `None` for retrieving all, use [] to retrieve only row keys.
             limit (int): The number of rows to retrieve. Defaults to 25. Set to -1, float("inf") or None to return all items.
 
         Returns:
             RowList: The requested rows.
 
         Examples:
```

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/relationships.py` & `cognite_sdk-6.1.0/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/sequences.py` & `cognite_sdk-6.1.0/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.1.0/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/templates.py` & `cognite_sdk-6.1.0/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/three_d.py` & `cognite_sdk-6.1.0/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/time_series.py` & `cognite_sdk-6.1.0/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.1.0/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.1.0/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.1.0/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.1.0/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.1.0/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api/vision.py` & `cognite_sdk-6.1.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_api_client.py` & `cognite_sdk-6.1.0/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_cognite_client.py` & `cognite_sdk-6.1.0/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_http_client.py` & `cognite_sdk-6.1.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.1.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/config.py` & `cognite_sdk-6.1.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/credentials.py` & `cognite_sdk-6.1.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/_base.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/assets.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/datapoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import operator as op
+import typing
 import warnings
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
 from functools import cached_property
 from typing import (
     TYPE_CHECKING,
@@ -36,28 +37,28 @@
 from cognite.client.utils._text import (
     convert_all_keys_to_camel_case,
     convert_all_keys_to_snake_case,
     to_camel_case,
     to_snake_case,
 )
 
-ALL_SORTED_DP_AGGS = sorted(
-    [
-        "average",
-        "continuous_variance",
-        "count",
-        "discrete_variance",
-        "interpolation",
-        "max",
-        "min",
-        "step_interpolation",
-        "sum",
-        "total_variation",
-    ]
-)
+Aggregate = Literal[
+    "average",
+    "continuous_variance",
+    "count",
+    "discrete_variance",
+    "interpolation",
+    "max",
+    "min",
+    "step_interpolation",
+    "sum",
+    "total_variation",
+]
+
+ALL_SORTED_DP_AGGS = sorted(typing.get_args(Aggregate))
 
 try:
     import numpy as np
 
     NUMPY_IS_AVAILABLE = True
 
 except ImportError:  # pragma no cover
```

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/events.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/files.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/functions.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/iam.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/labels.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/raw.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/shared.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/templates.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/exceptions.py` & `cognite_sdk-6.1.0/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/testing.py` & `cognite_sdk-6.1.0/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/__init__.py` & `cognite_sdk-6.1.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.1.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.1.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_graph.py` & `cognite_sdk-6.1.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_identifier.py` & `cognite_sdk-6.1.0/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_logging.py` & `cognite_sdk-6.1.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.1.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.1.0/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.1.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_text.py` & `cognite_sdk-6.1.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_time.py` & `cognite_sdk-6.1.0/cognite/client/utils/_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,22 +539,25 @@
         nonexistent="shift_forward",
         ambiguous=True,
     )
 
 
 def validate_timezone(start: datetime, end: datetime) -> ZoneInfo:
     ZoneInfo = import_zoneinfo()
+    pd = cast(Any, local_import("pandas"))
 
     if missing := [name for name, timestamp in zip(("start", "end"), (start, end)) if not timestamp.tzinfo]:
         names = " and ".join(missing)
         end_sentence = " do not have timezones." if len(missing) >= 2 else " does not have a timezone."
         raise ValueError(f"All times must be time zone aware, {names}{end_sentence}")
 
-    if not isinstance(start.tzinfo, ZoneInfo) or not isinstance(end.tzinfo, ZoneInfo):  # type: ignore [arg-type]
-        raise ValueError("Only ZoneInfo implementation of tzinfo is supported")
+    is_start_valid = isinstance(start, pd.Timestamp) or isinstance(start.tzinfo, ZoneInfo)  # type: ignore [arg-type]
+    is_end_valid = isinstance(end, pd.Timestamp) or isinstance(end.tzinfo, ZoneInfo)  # type: ignore [arg-type]
+    if not is_start_valid or not is_end_valid:
+        raise ValueError("Only pandas.Timestamp or datetime with ZoneInfo implementation of tzinfo are supported.")
 
     if start.tzinfo is not end.tzinfo:
         raise ValueError(f"start and end have different timezones, {start.tzinfo.key!r} and {end.tzinfo.key!r}.")  # type: ignore [union-attr]
 
     return start.tzinfo  # type: ignore [return-value]
```

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_validation.py` & `cognite_sdk-6.1.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.1.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.2/pyproject.toml` & `cognite_sdk-6.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.0.2"
+version = "6.1.0"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
```

### Comparing `cognite_sdk-6.0.2/PKG-INFO` & `cognite_sdk-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.0.2
+Version: 6.1.0
 Summary: Cognite Python SDK
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.0.2 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.0 Summary: Cognite Python
 SDK Author: Erlend Vollset Author-email: erlend.vollset@cognite.com Requires-
 Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
 functions Provides-Extra: geo Provides-Extra: numpy Provides-Extra: pandas
 Provides-Extra: pyodide Provides-Extra: sympy Requires-Dist: backports-zoneinfo
```

